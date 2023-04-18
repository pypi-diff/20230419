# Comparing `tmp/sloth-framework-0.1.1.tar.gz` & `tmp/sloth-framework-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sloth-framework-0.1.1.tar", last modified: Tue Apr 18 21:07:41 2023, max compression
+gzip compressed data, was "sloth-framework-0.1.2.tar", last modified: Tue Apr 18 21:58:27 2023, max compression
```

## Comparing `sloth-framework-0.1.1.tar` & `sloth-framework-0.1.2.tar`

### file list

```diff
@@ -1,450 +1,292 @@
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.341840 sloth-framework-0.1.1/
--rw-r--r--   0 breno      (503) staff       (20)       89 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/MANIFEST.in
--rw-r--r--   0 breno      (503) staff       (20)      680 2023-04-18 21:07:41.341173 sloth-framework-0.1.1/PKG-INFO
--rw-r--r--   0 breno      (503) staff       (20)       38 2023-04-18 21:07:41.342034 sloth-framework-0.1.1/setup.cfg
--rw-r--r--   0 breno      (503) staff       (20)     1149 2023-04-18 21:07:12.000000 sloth-framework-0.1.1/setup.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.561525 sloth-framework-0.1.1/sloth/
--rw-r--r--   0 breno      (503) staff       (20)     6148 2022-09-25 20:28:22.000000 sloth-framework-0.1.1/sloth/.DS_Store
--rw-r--r--   0 breno      (503) staff       (20)       65 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/.dockerignore
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.563742 sloth-framework-0.1.1/sloth/.idea/
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.564667 sloth-framework-0.1.1/sloth/.idea/inspectionProfiles/
--rw-r--r--   0 breno      (503) staff       (20)      174 2022-04-14 14:03:07.000000 sloth-framework-0.1.1/sloth/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 breno      (503) staff       (20)      262 2022-04-14 14:03:07.000000 sloth-framework-0.1.1/sloth/.idea/modules.xml
--rw-r--r--   0 breno      (503) staff       (20)      323 2022-04-14 14:06:53.000000 sloth-framework-0.1.1/sloth/.idea/sloth.iml
--rw-r--r--   0 breno      (503) staff       (20)      137 2022-04-14 14:03:07.000000 sloth-framework-0.1.1/sloth/.idea/workspace.xml
--rw-r--r--   0 breno      (503) staff       (20)      909 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/Dockerfile
--rw-r--r--   0 breno      (503) staff       (20)     4272 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/__init__.py
--rw-r--r--   0 breno      (503) staff       (20)     5608 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/__main__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.567733 sloth-framework-0.1.1/sloth/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     2420 2022-06-14 14:03:53.000000 sloth-framework-0.1.1/sloth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     4432 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     5047 2023-04-18 10:20:44.000000 sloth-framework-0.1.1/sloth/__pycache__/__main__.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.571554 sloth-framework-0.1.1/sloth/actions/
--rw-r--r--   0 breno      (503) staff       (20)    36880 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/actions/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.581902 sloth-framework-0.1.1/sloth/actions/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)    19031 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/actions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    26352 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/actions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1561 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/actions/__pycache__/fields.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1641 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/actions/__pycache__/fields.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     3933 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/actions/__pycache__/inputs.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     3987 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/actions/__pycache__/inputs.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      770 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/actions/fields.py
--rw-r--r--   0 breno      (503) staff       (20)     3189 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/actions/inputs.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.607584 sloth-framework-0.1.1/sloth/api/
--rw-r--r--   0 breno      (503) staff       (20)     2716 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.625616 sloth-framework-0.1.1/sloth/api/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     2062 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2071 2022-09-21 17:02:37.000000 sloth-framework-0.1.1/sloth/api/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     3564 2022-06-14 14:12:38.000000 sloth-framework-0.1.1/sloth/api/__pycache__/actions.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    22582 2023-04-18 17:34:40.000000 sloth-framework-0.1.1/sloth/api/__pycache__/actions.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    13232 2023-04-18 17:34:40.000000 sloth-framework-0.1.1/sloth/api/__pycache__/dashboard.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     9382 2022-06-14 14:12:30.000000 sloth-framework-0.1.1/sloth/api/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    14269 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/api/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1879 2022-06-14 14:12:38.000000 sloth-framework-0.1.1/sloth/api/__pycache__/urls.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1275 2023-04-18 17:34:40.000000 sloth-framework-0.1.1/sloth/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2871 2022-06-14 14:12:38.000000 sloth-framework-0.1.1/sloth/api/__pycache__/views.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     7927 2023-04-18 17:34:40.000000 sloth-framework-0.1.1/sloth/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    18644 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/actions.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.627329 sloth-framework-0.1.1/sloth/api/backends/
--rw-r--r--   0 breno      (503) staff       (20)      567 2021-11-16 15:14:56.000000 sloth-framework-0.1.1/sloth/api/backends/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.632124 sloth-framework-0.1.1/sloth/api/backends/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     1198 2021-11-16 15:15:26.000000 sloth-framework-0.1.1/sloth/api/backends/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    13994 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/dashboard.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.635533 sloth-framework-0.1.1/sloth/api/exceptions/
--rw-r--r--   0 breno      (503) staff       (20)      406 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/exceptions/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.638198 sloth-framework-0.1.1/sloth/api/exceptions/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     1193 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/api/exceptions/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.639999 sloth-framework-0.1.1/sloth/api/management/
--rw-r--r--   0 breno      (503) staff       (20)        0 2021-11-06 08:00:01.000000 sloth-framework-0.1.1/sloth/api/management/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.642720 sloth-framework-0.1.1/sloth/api/management/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)      165 2022-06-14 22:16:06.000000 sloth-framework-0.1.1/sloth/api/management/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      182 2021-11-17 09:16:01.000000 sloth-framework-0.1.1/sloth/api/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.668084 sloth-framework-0.1.1/sloth/api/management/commands/
--rw-r--r--   0 breno      (503) staff       (20)        0 2021-11-06 08:00:10.000000 sloth-framework-0.1.1/sloth/api/management/commands/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.680918 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)      174 2022-06-14 22:16:06.000000 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      191 2021-11-17 09:16:01.000000 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1482 2023-04-18 11:36:37.000000 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/cloud.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1229 2022-06-11 10:00:43.000000 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/query.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      787 2023-04-14 19:27:15.000000 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/reset_passwords.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2078 2023-04-16 13:23:51.000000 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/startserver.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1495 2022-06-14 22:16:06.000000 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/sync.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1794 2023-04-16 11:53:16.000000 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/sync.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      668 2023-04-13 08:38:15.000000 sloth-framework-0.1.1/sloth/api/management/commands/__pycache__/sync_roles.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1251 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/api/management/commands/cloud.py
--rw-r--r--   0 breno      (503) staff       (20)      600 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/management/commands/query.py
--rw-r--r--   0 breno      (503) staff       (20)      366 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/management/commands/reset_passwords.py
--rw-r--r--   0 breno      (503) staff       (20)      345 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/management/commands/selenium.py
--rw-r--r--   0 breno      (503) staff       (20)      542 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/management/commands/send_web_push_notification.py
--rw-r--r--   0 breno      (503) staff       (20)     1382 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/management/commands/startserver.py
--rw-r--r--   0 breno      (503) staff       (20)     1391 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/management/commands/sync.py
--rw-r--r--   0 breno      (503) staff       (20)      279 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/management/commands/sync_roles.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.696040 sloth-framework-0.1.1/sloth/api/migrations/
--rw-r--r--   0 breno      (503) staff       (20)     3069 2021-11-16 15:14:56.000000 sloth-framework-0.1.1/sloth/api/migrations/0001_initial.py
--rw-r--r--   0 breno      (503) staff       (20)     1961 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0002_role_user.py
--rw-r--r--   0 breno      (503) staff       (20)      632 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0003_alter_application_user.py
--rw-r--r--   0 breno      (503) staff       (20)     1330 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0004_task.py
--rw-r--r--   0 breno      (503) staff       (20)      586 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0005_task_stopped_alter_task_message.py
--rw-r--r--   0 breno      (503) staff       (20)     2379 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
--rw-r--r--   0 breno      (503) staff       (20)      638 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
--rw-r--r--   0 breno      (503) staff       (20)      694 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
--rw-r--r--   0 breno      (503) staff       (20)      966 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0009_pushnotification.py
--rw-r--r--   0 breno      (503) staff       (20)      667 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0010_alter_pushnotification_user.py
--rw-r--r--   0 breno      (503) staff       (20)      634 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/migrations/0011_alter_application_client_secret.py
--rw-r--r--   0 breno      (503) staff       (20)     1089 2022-09-25 21:01:42.000000 sloth-framework-0.1.1/sloth/api/migrations/0012_authcode.py
--rw-r--r--   0 breno      (503) staff       (20)      559 2023-02-02 00:42:42.000000 sloth-framework-0.1.1/sloth/api/migrations/0013_task_partial_task_total.py
--rw-r--r--   0 breno      (503) staff       (20)     1325 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/migrations/0014_email.py
--rw-r--r--   0 breno      (503) staff       (20)        0 2021-11-16 15:14:56.000000 sloth-framework-0.1.1/sloth/api/migrations/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.748699 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     2457 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2476 2021-11-16 15:15:19.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1640 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0002_role_user.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1663 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0002_role_user.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      843 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0003_alter_application_user.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      860 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0003_alter_application_user.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1282 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0004_task.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1299 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0004_task.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      733 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0005_task_stopped_alter_task_message.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      750 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0005_task_stopped_alter_task_message.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1460 2022-05-12 12:21:58.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0006_remove_role_scope_type_role_active_alter_role_name_and_more.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1561 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0006_role_active_alter_role_name_alter_role_scope_key_and_more.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1578 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0006_role_active_alter_role_name_alter_role_scope_key_and_more.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      715 2022-05-12 12:35:19.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0007_alter_role_scope_key.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      784 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0007_alter_scope_description_alter_task_error.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      801 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0007_alter_scope_description_alter_task_error.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      791 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0008_alter_application_available_scopes_and_more.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      808 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0008_alter_application_available_scopes_and_more.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1122 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0009_pushnotification.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      914 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0010_alter_pushnotification_user.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      883 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0011_alter_application_client_secret.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      706 2022-09-01 11:30:34.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0011_task_partial_task_total.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1199 2022-09-26 16:01:37.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0012_authcode.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      684 2023-02-02 11:11:34.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0013_task_partial_task_total.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1297 2023-04-18 17:34:40.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/0014_email.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      165 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      182 2021-11-16 15:15:19.000000 sloth-framework-0.1.1/sloth/api/migrations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    11023 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/models.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.536949 sloth-framework-0.1.1/sloth/api/static/
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.793725 sloth-framework-0.1.1/sloth/api/static/css/
--rw-r--r--   0 breno      (503) staff       (20)    58578 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/all.min.css
--rw-r--r--   0 breno      (503) staff       (20)    67289 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/bootstrap-icons.css
--rw-r--r--   0 breno      (503) staff       (20)   155845 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/bootstrap.min.css
--rw-r--r--   0 breno      (503) staff       (20)      909 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/colorpick.min.css
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.809606 sloth-framework-0.1.1/sloth/api/static/css/fonts/
--rw-r--r--   0 breno      (503) staff       (20)   107280 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 breno      (503) staff       (20)   116316 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 breno      (503) staff       (20)   112880 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 breno      (503) staff       (20)   111976 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 breno      (503) staff       (20)    83304 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 breno      (503) staff       (20)    30702 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/icons.svg
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.813259 sloth-framework-0.1.1/sloth/api/static/css/images/
--rw-r--r--   0 breno      (503) staff       (20)     6992 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 breno      (503) staff       (20)     6988 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 breno      (503) staff       (20)    35973 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/jquery-ui.css
--rw-r--r--   0 breno      (503) staff       (20)    14670 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/leaflet.css
--rw-r--r--   0 breno      (503) staff       (20)    16264 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/select2.min.css
--rw-r--r--   0 breno      (503) staff       (20)     8470 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/sloth.css
--rw-r--r--   0 breno      (503) staff       (20)    17867 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/css/trumbowyg.min.css
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.814058 sloth-framework-0.1.1/sloth/api/static/icons/
--rw-r--r--   0 breno      (503) staff       (20)     6148 2022-06-09 17:07:18.000000 sloth-framework-0.1.1/sloth/api/static/icons/.DS_Store
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.818200 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/
--rw-r--r--   0 breno      (503) staff       (20)     6148 2022-06-09 17:34:53.000000 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/.DS_Store
--rw-r--r--   0 breno      (503) staff       (20)   100170 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/fontawesome.min.css
--rw-r--r--   0 breno      (503) staff       (20)  1726692 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/fontawesome.min.js
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.847343 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/
--rw-r--r--   0 breno      (503) staff       (20)   181852 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 breno      (503) staff       (20)   105536 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 breno      (503) staff       (20)    60520 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 breno      (503) staff       (20)    23940 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 breno      (503) staff       (20)    10556 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 breno      (503) staff       (20)     4960 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.870028 sloth-framework-0.1.1/sloth/api/static/icons/materialicons/
--rw-r--r--   0 breno      (503) staff       (20)   174176 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
--rw-r--r--   0 breno      (503) staff       (20)   127220 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0 breno      (503) staff       (20)   155604 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
--rw-r--r--   0 breno      (503) staff       (20)     2152 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/materialicons/materialicons.css
--rw-r--r--   0 breno      (503) staff       (20)   135988 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.933005 sloth-framework-0.1.1/sloth/api/static/images/
--rw-r--r--   0 breno      (503) staff       (20)     6148 2022-09-25 20:28:22.000000 sloth-framework-0.1.1/sloth/api/static/images/.DS_Store
--rw-r--r--   0 breno      (503) staff       (20)    57420 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/click.png
--rw-r--r--   0 breno      (503) staff       (20)    55448 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/hand.png
--rw-r--r--   0 breno      (503) staff       (20)    10276 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/icon.png
--rw-r--r--   0 breno      (503) staff       (20)     2435 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/icon.svg
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.934514 sloth-framework-0.1.1/sloth/api/static/images/images/
--rw-r--r--   0 breno      (503) staff       (20)      706 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/images/badge.png
--rw-r--r--   0 breno      (503) staff       (20)     1862 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/images/icon.png
--rw-r--r--   0 breno      (503) staff       (20)    45136 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/login.jpeg
--rw-r--r--   0 breno      (503) staff       (20)    22817 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/logo.png
--rw-r--r--   0 breno      (503) staff       (20)     3866 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/logo.svg
--rw-r--r--   0 breno      (503) staff       (20)    21495 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/no-image.png
--rw-r--r--   0 breno      (503) staff       (20)    23102 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/sloth.png
--rw-r--r--   0 breno      (503) staff       (20)    13670 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/images/user.png
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.987803 sloth-framework-0.1.1/sloth/api/static/js/
--rw-r--r--   0 breno      (503) staff       (20)    88459 2023-02-12 02:54:27.000000 sloth-framework-0.1.1/sloth/api/static/js/USA.json
--rw-r--r--   0 breno      (503) staff       (20)     3694 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/api/static/js/api.js
--rw-r--r--   0 breno      (503) staff       (20)    78743 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/bootstrap.bundle.min.js
--rwxr-xr-x   0 breno      (503) staff       (20)     4098 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/colorpick.min.js
--rw-r--r--   0 breno      (503) staff       (20)  1022939 2022-12-09 19:31:21.000000 sloth-framework-0.1.1/sloth/api/static/js/echarts.min.js
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.989065 sloth-framework-0.1.1/sloth/api/static/js/i18n/
--rwxr-xr-x   0 breno      (503) staff       (20)      853 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/i18n/pt-BR.js
--rw-r--r--   0 breno      (503) staff       (20)    89501 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 breno      (503) staff       (20)   520714 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/jquery-ui.js
--rw-r--r--   0 breno      (503) staff       (20)     2516 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/jquery.binarytransport.js
--rw-r--r--   0 breno      (503) staff       (20)     8327 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/jquery.mask.min.js
--rw-r--r--   0 breno      (503) staff       (20)    80794 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/jquery.timepicker.js
--rw-r--r--   0 breno      (503) staff       (20)   147555 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/leaflet.js
--rw-r--r--   0 breno      (503) staff       (20)    24103 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/masonry.pkgd.min.js
--rw-r--r--   0 breno      (503) staff       (20)    18453 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/popper.min.js
--rw-r--r--   0 breno      (503) staff       (20)    43994 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/qr-scanner-worker.min.js
--rw-r--r--   0 breno      (503) staff       (20)    15538 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/qr-scanner.min.js
--rw-r--r--   0 breno      (503) staff       (20)    19927 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/qrcode.min.js
--rw-r--r--   0 breno      (503) staff       (20)    73163 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/select2.min.js
--rw-r--r--   0 breno      (503) staff       (20)    15700 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/sloth.js
--rw-r--r--   0 breno      (503) staff       (20)      723 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/sw.js
--rw-r--r--   0 breno      (503) staff       (20)    10702 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/tests.js
--rw-r--r--   0 breno      (503) staff       (20)    28280 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/trumbowyg.min.js
--rw-r--r--   0 breno      (503) staff       (20)     1943 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/static/js/wpn.js
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.990730 sloth-framework-0.1.1/sloth/api/tasks/
--rw-r--r--   0 breno      (503) staff       (20)     2263 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/tasks/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.992173 sloth-framework-0.1.1/sloth/api/tasks/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     2768 2023-04-18 20:55:27.000000 sloth-framework-0.1.1/sloth/api/tasks/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.543802 sloth-framework-0.1.1/sloth/api/templates/
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.999408 sloth-framework-0.1.1/sloth/api/templates/actions/
--rw-r--r--   0 breno      (503) staff       (20)      777 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/actions/execute_query.html
--rw-r--r--   0 breno      (503) staff       (20)      153 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/actions/execute_script.html
--rw-r--r--   0 breno      (503) staff       (20)     1216 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/actions/show_icons.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.001103 sloth-framework-0.1.1/sloth/api/templates/api/
--rw-r--r--   0 breno      (503) staff       (20)     1034 2021-11-16 15:14:56.000000 sloth-framework-0.1.1/sloth/api/templates/api/index.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.021039 sloth-framework-0.1.1/sloth/api/templates/charts/
--rw-r--r--   0 breno      (503) staff       (20)     1551 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/charts/bar.html
--rw-r--r--   0 breno      (503) staff       (20)     3052 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/charts/column.html
--rw-r--r--   0 breno      (503) staff       (20)       47 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/charts/donut.html
--rw-r--r--   0 breno      (503) staff       (20)      283 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/charts/legend.html
--rw-r--r--   0 breno      (503) staff       (20)     1267 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/charts/pie.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.063939 sloth-framework-0.1.1/sloth/api/templates/dashboard/
--rw-r--r--   0 breno      (503) staff       (20)     4237 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/actions.html
--rw-r--r--   0 breno      (503) staff       (20)     1324 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/apps.html
--rw-r--r--   0 breno      (503) staff       (20)     3125 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/base.html
--rw-r--r--   0 breno      (503) staff       (20)     2066 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/bottom.html
--rw-r--r--   0 breno      (503) staff       (20)     1173 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/cards.html
--rw-r--r--   0 breno      (503) staff       (20)      481 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/dashboards.html
--rw-r--r--   0 breno      (503) staff       (20)      120 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/default.html
--rw-r--r--   0 breno      (503) staff       (20)      727 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/footer.html
--rw-r--r--   0 breno      (503) staff       (20)     6998 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/form.html
--rw-r--r--   0 breno      (503) staff       (20)      749 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/grids.html
--rw-r--r--   0 breno      (503) staff       (20)     1665 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/header.html
--rw-r--r--   0 breno      (503) staff       (20)      710 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/links.html
--rw-r--r--   0 breno      (503) staff       (20)      434 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/menu.html
--rw-r--r--   0 breno      (503) staff       (20)      764 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/messages.html
--rw-r--r--   0 breno      (503) staff       (20)     1113 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/modal.html
--rw-r--r--   0 breno      (503) staff       (20)      718 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/plus.html
--rw-r--r--   0 breno      (503) staff       (20)     4026 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/report.html
--rw-r--r--   0 breno      (503) staff       (20)     1287 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/search.html
--rw-r--r--   0 breno      (503) staff       (20)     1367 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/settings.html
--rw-r--r--   0 breno      (503) staff       (20)      757 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/shortcuts.html
--rw-r--r--   0 breno      (503) staff       (20)      838 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/tasks.html
--rw-r--r--   0 breno      (503) staff       (20)      716 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/dashboard/tools.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.066026 sloth-framework-0.1.1/sloth/api/templates/inputs/
--rw-r--r--   0 breno      (503) staff       (20)      701 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/inputs/picker.html
--rw-r--r--   0 breno      (503) staff       (20)     1009 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/inputs/qrcode.html
--rw-r--r--   0 breno      (503) staff       (20)      924 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/inputs/select.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.075657 sloth-framework-0.1.1/sloth/api/templates/queryset/
--rw-r--r--   0 breno      (503) staff       (20)     1685 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/accordion.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.082027 sloth-framework-0.1.1/sloth/api/templates/queryset/actions/
--rw-r--r--   0 breno      (503) staff       (20)      153 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/actions/actions.html
--rw-r--r--   0 breno      (503) staff       (20)      154 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/actions/batch.html
--rw-r--r--   0 breno      (503) staff       (20)      145 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/actions/global.html
--rw-r--r--   0 breno      (503) staff       (20)     4442 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/calendar.html
--rw-r--r--   0 breno      (503) staff       (20)     1823 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/cards.html
--rw-r--r--   0 breno      (503) staff       (20)      190 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/checkbox.html
--rw-r--r--   0 breno      (503) staff       (20)     2332 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/datatable.html
--rw-r--r--   0 breno      (503) staff       (20)     2930 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/filter.html
--rw-r--r--   0 breno      (503) staff       (20)     3013 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/filters.html
--rw-r--r--   0 breno      (503) staff       (20)     8811 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/queryset.html
--rw-r--r--   0 breno      (503) staff       (20)     2297 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/rows.html
--rw-r--r--   0 breno      (503) staff       (20)     1250 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/scroll.html
--rw-r--r--   0 breno      (503) staff       (20)     5097 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/statistics.html
--rw-r--r--   0 breno      (503) staff       (20)     4511 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/queryset/timeline.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.543104 sloth-framework-0.1.1/sloth/api/templates/renderers/
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.085780 sloth-framework-0.1.1/sloth/api/templates/renderers/badges/
--rw-r--r--   0 breno      (503) staff       (20)      165 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/badges/badge.html
--rw-r--r--   0 breno      (503) staff       (20)      385 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/badges/boolean.html
--rw-r--r--   0 breno      (503) staff       (20)      143 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/badges/primary.html
--rw-r--r--   0 breno      (503) staff       (20)      151 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/badges/status.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.086411 sloth-framework-0.1.1/sloth/api/templates/renderers/boolean/
--rw-r--r--   0 breno      (503) staff       (20)      101 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/boolean/thumb.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.088351 sloth-framework-0.1.1/sloth/api/templates/renderers/calendar/
--rw-r--r--   0 breno      (503) staff       (20)     1997 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/calendar/calendar.html
--rw-r--r--   0 breno      (503) staff       (20)       36 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/calendar/events.html
--rw-r--r--   0 breno      (503) staff       (20)      229 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/calendar/legend.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.088964 sloth-framework-0.1.1/sloth/api/templates/renderers/documents/
--rw-r--r--   0 breno      (503) staff       (20)       63 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/documents/document.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.090322 sloth-framework-0.1.1/sloth/api/templates/renderers/images/
--rw-r--r--   0 breno      (503) staff       (20)       62 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/images/banner.html
--rw-r--r--   0 breno      (503) staff       (20)       61 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/images/image.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.092035 sloth-framework-0.1.1/sloth/api/templates/renderers/links/
--rw-r--r--   0 breno      (503) staff       (20)       77 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/links/file.html
--rw-r--r--   0 breno      (503) staff       (20)      146 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/links/url.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.094521 sloth-framework-0.1.1/sloth/api/templates/renderers/maps/
--rw-r--r--   0 breno      (503) staff       (20)      292 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/maps/geolocation.html
--rw-r--r--   0 breno      (503) staff       (20)     4551 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/maps/map.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.103204 sloth-framework-0.1.1/sloth/api/templates/renderers/messages/
--rw-r--r--   0 breno      (503) staff       (20)      113 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/messages/custom.html
--rw-r--r--   0 breno      (503) staff       (20)       78 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/messages/danger.html
--rw-r--r--   0 breno      (503) staff       (20)      126 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/messages/message.html
--rw-r--r--   0 breno      (503) staff       (20)       79 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/messages/primary.html
--rw-r--r--   0 breno      (503) staff       (20)       79 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/messages/success.html
--rw-r--r--   0 breno      (503) staff       (20)       79 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/messages/warning.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.114328 sloth-framework-0.1.1/sloth/api/templates/renderers/photos/
--rw-r--r--   0 breno      (503) staff       (20)      131 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/photos/photo.html
--rw-r--r--   0 breno      (503) staff       (20)      171 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/photos/round.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.128575 sloth-framework-0.1.1/sloth/api/templates/renderers/programing/
--rw-r--r--   0 breno      (503) staff       (20)      764 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/programing/strtable.html
--rw-r--r--   0 breno      (503) staff       (20)      152 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/programing/terminal.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.138414 sloth-framework-0.1.1/sloth/api/templates/renderers/tags/
--rw-r--r--   0 breno      (503) staff       (20)      276 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/tags/primary.html
--rw-r--r--   0 breno      (503) staff       (20)      287 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/tags/tags.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.159224 sloth-framework-0.1.1/sloth/api/templates/renderers/utils/
--rw-r--r--   0 breno      (503) staff       (20)       16 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/utils/formatted.html
--rw-r--r--   0 breno      (503) staff       (20)      214 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/utils/progress.html
--rw-r--r--   0 breno      (503) staff       (20)      323 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/utils/qrcode.html
--rw-r--r--   0 breno      (503) staff       (20)     2000 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/utils/steps.html
--rw-r--r--   0 breno      (503) staff       (20)      601 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/renderers/utils/table.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.161075 sloth-framework-0.1.1/sloth/api/templates/themes/
--rw-r--r--   0 breno      (503) staff       (20)      635 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/themes/dark.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.174763 sloth-framework-0.1.1/sloth/api/templates/valueset/
--rw-r--r--   0 breno      (503) staff       (20)      152 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/valueset/2-column.html
--rw-r--r--   0 breno      (503) staff       (20)      459 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/valueset/field.html
--rw-r--r--   0 breno      (503) staff       (20)     3576 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/api/templates/valueset/fieldset-group.html
--rw-r--r--   0 breno      (503) staff       (20)     3084 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/api/templates/valueset/fieldset-list.html
--rw-r--r--   0 breno      (503) staff       (20)      110 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/valueset/fieldset-tab.html
--rw-r--r--   0 breno      (503) staff       (20)     2980 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/valueset/fieldset.html
--rw-r--r--   0 breno      (503) staff       (20)       47 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/valueset/primitive.html
--rw-r--r--   0 breno      (503) staff       (20)     1025 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/valueset/value.html
--rw-r--r--   0 breno      (503) staff       (20)     5702 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templates/valueset/valueset.html
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.178027 sloth-framework-0.1.1/sloth/api/templatetags/
--rw-r--r--   0 breno      (503) staff       (20)      162 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templatetags/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.186743 sloth-framework-0.1.1/sloth/api/templatetags/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)      335 2023-04-18 17:34:40.000000 sloth-framework-0.1.1/sloth/api/templatetags/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    10005 2023-04-18 17:34:40.000000 sloth-framework-0.1.1/sloth/api/templatetags/__pycache__/tags.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     9110 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/templatetags/tags.py
--rw-r--r--   0 breno      (503) staff       (20)     1361 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/urls.py
--rw-r--r--   0 breno      (503) staff       (20)    11104 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/api/views.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.545030 sloth-framework-0.1.1/sloth/app/
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.191587 sloth-framework-0.1.1/sloth/app/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)      173 2023-04-14 19:27:14.000000 sloth-framework-0.1.1/sloth/app/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2177 2023-04-14 19:27:15.000000 sloth-framework-0.1.1/sloth/app/__pycache__/actions.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    11325 2023-04-14 19:27:15.000000 sloth-framework-0.1.1/sloth/app/__pycache__/dashboard.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      804 2023-04-14 19:27:15.000000 sloth-framework-0.1.1/sloth/app/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     7660 2023-04-14 19:27:15.000000 sloth-framework-0.1.1/sloth/app/__pycache__/views.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.545243 sloth-framework-0.1.1/sloth/app/templatetags/
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.193707 sloth-framework-0.1.1/sloth/app/templatetags/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)      335 2023-04-14 19:27:15.000000 sloth-framework-0.1.1/sloth/app/templatetags/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     9340 2023-04-14 19:27:15.000000 sloth-framework-0.1.1/sloth/app/templatetags/__pycache__/tags.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.198969 sloth-framework-0.1.1/sloth/cloud/
--rw-r--r--   0 breno      (503) staff       (20)        0 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/cloud/__init__.py
--rwxr-xr-x   0 breno      (503) staff       (20)      688 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/cloud/printer.py
--rwxr-xr-x   0 breno      (503) staff       (20)     6116 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/cloud/server.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.200471 sloth-framework-0.1.1/sloth/conf/
--rw-r--r--   0 breno      (503) staff       (20)        0 2023-04-09 08:16:34.000000 sloth-framework-0.1.1/sloth/conf/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.202442 sloth-framework-0.1.1/sloth/conf/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)      174 2023-04-09 08:18:50.000000 sloth-framework-0.1.1/sloth/conf/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2475 2023-04-18 10:17:59.000000 sloth-framework-0.1.1/sloth/conf/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2875 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/conf/settings.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.211306 sloth-framework-0.1.1/sloth/core/
--rw-r--r--   0 breno      (503) staff       (20)        0 2022-09-27 13:29:31.000000 sloth-framework-0.1.1/sloth/core/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.229877 sloth-framework-0.1.1/sloth/core/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)      155 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      174 2022-09-27 15:59:51.000000 sloth-framework-0.1.1/sloth/core/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    15741 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/core/__pycache__/base.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    18022 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/core/__pycache__/base.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    22470 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/core/__pycache__/queryset.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    28835 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/core/__pycache__/queryset.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     8627 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/core/__pycache__/statistics.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    10343 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/core/__pycache__/statistics.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2033 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/core/__pycache__/validation.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2058 2022-09-21 17:02:37.000000 sloth-framework-0.1.1/sloth/core/__pycache__/validation.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    10034 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/core/__pycache__/valueset.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    14221 2023-04-18 17:37:26.000000 sloth-framework-0.1.1/sloth/core/__pycache__/valueset.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     4555 2022-06-14 14:12:38.000000 sloth-framework-0.1.1/sloth/core/__pycache__/views.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     3410 2023-04-14 19:27:15.000000 sloth-framework-0.1.1/sloth/core/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    21312 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/core/base.py
--rw-r--r--   0 breno      (503) staff       (20)    37888 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/core/queryset.py
--rw-r--r--   0 breno      (503) staff       (20)    10195 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/core/statistics.py
--rw-r--r--   0 breno      (503) staff       (20)     2012 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/core/validation.py
--rw-r--r--   0 breno      (503) staff       (20)    20111 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/core/valueset.py
--rw-r--r--   0 breno      (503) staff       (20)        0 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/core/views.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.230574 sloth-framework-0.1.1/sloth/db/
--rw-r--r--   0 breno      (503) staff       (20)      487 2023-04-11 17:54:19.000000 sloth-framework-0.1.1/sloth/db/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.232293 sloth-framework-0.1.1/sloth/db/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     1035 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/db/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      713 2023-04-11 17:54:27.000000 sloth-framework-0.1.1/sloth/db/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.234010 sloth-framework-0.1.1/sloth/db/models/
--rw-r--r--   0 breno      (503) staff       (20)     9656 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/db/models/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.255967 sloth-framework-0.1.1/sloth/db/models/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)    11266 2022-06-14 14:12:30.000000 sloth-framework-0.1.1/sloth/db/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    12806 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/db/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    12390 2021-11-16 14:44:03.000000 sloth-framework-0.1.1/sloth/db/models/__pycache__/base.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     3365 2021-11-16 14:44:30.000000 sloth-framework-0.1.1/sloth/db/models/__pycache__/model.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    14439 2021-11-16 14:02:52.000000 sloth-framework-0.1.1/sloth/db/models/__pycache__/query.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     7433 2021-11-16 14:02:52.000000 sloth-framework-0.1.1/sloth/db/models/__pycache__/statistics.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     6051 2021-11-16 14:11:38.000000 sloth-framework-0.1.1/sloth/db/models/__pycache__/values.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:40.548518 sloth-framework-0.1.1/sloth/exceptions/
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.257376 sloth-framework-0.1.1/sloth/exceptions/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     1189 2023-04-14 19:27:14.000000 sloth-framework-0.1.1/sloth/exceptions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      190 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/requirements.txt
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.259367 sloth-framework-0.1.1/sloth/test/
--rw-r--r--   0 breno      (503) staff       (20)     3185 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/test/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.271435 sloth-framework-0.1.1/sloth/test/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     3555 2023-04-18 20:55:16.000000 sloth-framework-0.1.1/sloth/test/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.274700 sloth-framework-0.1.1/sloth/test/selenium/
--rw-r--r--   0 breno      (503) staff       (20)     4489 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/test/selenium/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.279543 sloth-framework-0.1.1/sloth/test/selenium/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     7028 2023-04-18 20:55:16.000000 sloth-framework-0.1.1/sloth/test/selenium/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     9598 2023-04-18 20:55:16.000000 sloth-framework-0.1.1/sloth/test/selenium/__pycache__/browser.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    10057 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/test/selenium/browser.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.281124 sloth-framework-0.1.1/sloth/utils/
--rw-r--r--   0 breno      (503) staff       (20)     4213 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/utils/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.284354 sloth-framework-0.1.1/sloth/utils/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     3902 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     4115 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/utils/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.297497 sloth-framework-0.1.1/sloth/utils/formatter/
--rw-r--r--   0 breno      (503) staff       (20)     2170 2023-04-18 17:34:26.000000 sloth-framework-0.1.1/sloth/utils/formatter/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.300895 sloth-framework-0.1.1/sloth/utils/formatter/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     2150 2022-06-14 14:12:38.000000 sloth-framework-0.1.1/sloth/utils/formatter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     2243 2023-04-18 17:34:39.000000 sloth-framework-0.1.1/sloth/utils/formatter/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.302054 sloth-framework-0.1.1/sloth/utils/http/
--rw-r--r--   0 breno      (503) staff       (20)     5317 2023-04-18 17:37:03.000000 sloth-framework-0.1.1/sloth/utils/http/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.305354 sloth-framework-0.1.1/sloth/utils/http/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)     5222 2022-06-14 14:12:29.000000 sloth-framework-0.1.1/sloth/utils/http/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)     5670 2023-04-18 17:37:26.000000 sloth-framework-0.1.1/sloth/utils/http/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.318542 sloth-framework-0.1.1/sloth/utils/icons/
--rw-r--r--   0 breno      (503) staff       (20)        0 2021-10-24 14:05:49.000000 sloth-framework-0.1.1/sloth/utils/icons/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.330587 sloth-framework-0.1.1/sloth/utils/icons/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)      162 2022-06-14 14:12:38.000000 sloth-framework-0.1.1/sloth/utils/icons/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)      157 2021-10-24 14:05:51.000000 sloth-framework-0.1.1/sloth/utils/icons/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    20486 2022-06-14 14:12:38.000000 sloth-framework-0.1.1/sloth/utils/icons/__pycache__/bootstrap.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    28423 2021-10-24 17:36:48.000000 sloth-framework-0.1.1/sloth/utils/icons/__pycache__/bootstrap.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    38757 2022-06-14 14:12:39.000000 sloth-framework-0.1.1/sloth/utils/icons/__pycache__/fontawesome.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    52818 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/utils/icons/__pycache__/fontawesome.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    15541 2022-06-14 14:12:38.000000 sloth-framework-0.1.1/sloth/utils/icons/__pycache__/materialicons.cpython-310.pyc
--rw-r--r--   0 breno      (503) staff       (20)    20652 2022-09-21 17:02:39.000000 sloth-framework-0.1.1/sloth/utils/icons/__pycache__/materialicons.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)    28753 2021-10-24 17:36:45.000000 sloth-framework-0.1.1/sloth/utils/icons/bootstrap.py
--rw-r--r--   0 breno      (503) staff       (20)    53105 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/utils/icons/fontawesome.py
--rw-r--r--   0 breno      (503) staff       (20)    20959 2022-09-21 16:56:21.000000 sloth-framework-0.1.1/sloth/utils/icons/materialicons.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.332472 sloth-framework-0.1.1/sloth/utils/log/
--rw-r--r--   0 breno      (503) staff       (20)        0 2022-10-06 09:42:03.000000 sloth-framework-0.1.1/sloth/utils/log/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.334119 sloth-framework-0.1.1/sloth/utils/log/__pycache__/
--rw-r--r--   0 breno      (503) staff       (20)      179 2022-12-21 12:07:30.000000 sloth-framework-0.1.1/sloth/utils/log/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)     1205 2022-12-21 12:07:44.000000 sloth-framework-0.1.1/sloth/utils/log/__pycache__/sql.cpython-38.pyc
--rw-r--r--   0 breno      (503) staff       (20)      965 2022-10-06 09:42:03.000000 sloth-framework-0.1.1/sloth/utils/log/sql.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.339114 sloth-framework-0.1.1/sloth_framework.egg-info/
--rw-r--r--   0 breno      (503) staff       (20)      680 2023-04-18 21:07:40.000000 sloth-framework-0.1.1/sloth_framework.egg-info/PKG-INFO
--rw-r--r--   0 breno      (503) staff       (20)    16412 2023-04-18 21:07:40.000000 sloth-framework-0.1.1/sloth_framework.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (503) staff       (20)        1 2023-04-18 21:07:40.000000 sloth-framework-0.1.1/sloth_framework.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (503) staff       (20)      209 2023-04-18 21:07:40.000000 sloth-framework-0.1.1/sloth_framework.egg-info/requires.txt
--rw-r--r--   0 breno      (503) staff       (20)       13 2023-04-18 21:07:40.000000 sloth-framework-0.1.1/sloth_framework.egg-info/top_level.txt
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.339691 sloth-framework-0.1.1/themes/
--rw-r--r--   0 breno      (503) staff       (20)        0 2023-02-23 16:57:36.000000 sloth-framework-0.1.1/themes/__init__.py
-drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-18 21:07:41.340125 sloth-framework-0.1.1/themes/dsgovbr/
--rw-r--r--   0 breno      (503) staff       (20)        0 2023-02-23 16:57:51.000000 sloth-framework-0.1.1/themes/dsgovbr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.891843 sloth-framework-0.1.2/sloth/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    36880 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/actions/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/actions/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/reset_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/selenium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/send_web_push_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/startserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/sync_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.899843 sloth-framework-0.1.2/sloth/api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0002_role_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0003_alter_application_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0004_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0005_task_stopped_alter_task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0009_pushnotification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0010_alter_pushnotification_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0011_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0012_authcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0013_task_partial_task_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0014_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.887843 sloth-framework-0.1.2/sloth/api/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.899843 sloth-framework-0.1.2/sloth/api/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/colorpick.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.903843 sloth-framework-0.1.2/sloth/api/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.903843 sloth-framework-0.1.2/sloth/api/static/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/sloth.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/trumbowyg.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.887843 sloth-framework-0.1.2/sloth/api/static/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.903843 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/fontawesome.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.907844 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.907844 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/
+-rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/materialicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.911844 sloth-framework-0.1.2/sloth/api/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/click.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/hand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.911844 sloth-framework-0.1.2/sloth/api/static/images/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/images/badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/login.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/sloth.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/user.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/bootstrap.bundle.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/colorpick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/static/js/i18n/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery.binarytransport.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery.mask.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery.timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/leaflet.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/masonry.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/qr-scanner-worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/qr-scanner.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/qrcode.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/sloth.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/trumbowyg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/wpn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.891843 sloth-framework-0.1.2/sloth/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/templates/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/actions/execute_query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/actions/execute_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/actions/show_icons.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/templates/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/templates/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/column.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/donut.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/legend.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/pie.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.919844 sloth-framework-0.1.2/sloth/api/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/apps.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/grids.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/plus.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/shortcuts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.919844 sloth-framework-0.1.2/sloth/api/templates/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/inputs/picker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/inputs/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/inputs/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/accordion.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/queryset/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/actions/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/actions/batch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/actions/global.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/datatable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/filters.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/queryset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/scroll.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/statistics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/timeline.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.891843 sloth-framework-0.1.2/sloth/api/templates/renderers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/status.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/boolean/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/boolean/thumb.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/events.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/legend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/documents/document.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/images/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/images/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/images/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/links/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/links/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/links/url.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/maps/geolocation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/maps/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/photos/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/photos/photo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/photos/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/programing/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/programing/strtable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/programing/terminal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/tags/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/tags/tags.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/formatted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/progress.html
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/steps.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/themes/dark.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/api/templates/valueset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/2-column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/primitive.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/valueset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/api/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templatetags/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/cloud/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/cloud/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37888 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/valueset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/test/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/test/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/test/selenium/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/utils/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/sloth/utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/icons/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/icons/fontawesome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/icons/materialicons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/sloth/utils/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/log/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/sloth_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/top_level.txt
```

### Comparing `sloth-framework-0.1.1/setup.py` & `sloth-framework-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(os.path.join(root_dir, 'sloth/requirements.txt')) as file:
     requirements = file.read().strip().splitlines()
 
 os.chdir(root_dir)
 
 setup(
     name='sloth-framework',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': [],
         'production': [],
     },
     include_package_data=True,
```

### Comparing `sloth-framework-0.1.1/sloth/Dockerfile` & `sloth-framework-0.1.2/sloth/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 RUN apk add firefox-esr
 RUN ln -sfn /usr/bin/firefox-esr /usr/bin/firefox
 RUN wget -q https://github.com/mozilla/geckodriver/releases/download/v0.32.0/geckodriver-v0.32.0-linux32.tar.gz
 RUN tar -xf geckodriver-v0.32.0-linux32.tar.gz
 RUN chmod +x geckodriver
 RUN mv geckodriver /usr/local/bin/
 ENV PYTHONPATH=/var/site-packages
-ADD sloth $PYTHONPATH/sloth
+ADD . $PYTHONPATH/sloth
 
 FROM sloth-base as sloth-src
 ENV PYTHONPATH=/var/site-packages
 ADD . $PYTHONPATH/sloth
 
 FROM minidocks/weasyprint as sloth-weasyprint
 ADD ./cloud/printer.py /opt/printer.py
 EXPOSE 8888
 ENTRYPOINT ["python", "/opt/printer.py"]
 
 FROM sloth-base as sloth
-RUN pip install --no-cache-dir django-sloth
+RUN pip install --no-cache-dir sloth-framework
```

### Comparing `sloth-framework-0.1.1/sloth/__init__.py` & `sloth-framework-0.1.2/sloth/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/__main__.py` & `sloth-framework-0.1.2/sloth/__main__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/actions/__init__.py` & `sloth-framework-0.1.2/sloth/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/actions/fields.py` & `sloth-framework-0.1.2/sloth/actions/fields.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/actions/inputs.py` & `sloth-framework-0.1.2/sloth/actions/inputs.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/__init__.py` & `sloth-framework-0.1.2/sloth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/actions.py` & `sloth-framework-0.1.2/sloth/api/actions.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/backends/__init__.py` & `sloth-framework-0.1.2/sloth/api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/dashboard.py` & `sloth-framework-0.1.2/sloth/api/dashboard.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/management/commands/cloud.py` & `sloth-framework-0.1.2/sloth/api/management/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/management/commands/query.py` & `sloth-framework-0.1.2/sloth/api/management/commands/query.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/management/commands/send_web_push_notification.py` & `sloth-framework-0.1.2/sloth/api/management/commands/send_web_push_notification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/management/commands/startserver.py` & `sloth-framework-0.1.2/sloth/api/management/commands/startserver.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/management/commands/sync.py` & `sloth-framework-0.1.2/sloth/api/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0001_initial.py` & `sloth-framework-0.1.2/sloth/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0002_role_user.py` & `sloth-framework-0.1.2/sloth/api/migrations/0002_role_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0003_alter_application_user.py` & `sloth-framework-0.1.2/sloth/api/migrations/0003_alter_application_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0004_task.py` & `sloth-framework-0.1.2/sloth/api/migrations/0004_task.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0005_task_stopped_alter_task_message.py` & `sloth-framework-0.1.2/sloth/api/migrations/0005_task_stopped_alter_task_message.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py` & `sloth-framework-0.1.2/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py` & `sloth-framework-0.1.2/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py` & `sloth-framework-0.1.2/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0009_pushnotification.py` & `sloth-framework-0.1.2/sloth/api/migrations/0009_pushnotification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0010_alter_pushnotification_user.py` & `sloth-framework-0.1.2/sloth/api/migrations/0010_alter_pushnotification_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0011_alter_application_client_secret.py` & `sloth-framework-0.1.2/sloth/api/migrations/0011_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0012_authcode.py` & `sloth-framework-0.1.2/sloth/api/migrations/0012_authcode.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0013_task_partial_task_total.py` & `sloth-framework-0.1.2/sloth/api/migrations/0013_task_partial_task_total.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/migrations/0014_email.py` & `sloth-framework-0.1.2/sloth/api/migrations/0014_email.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/models.py` & `sloth-framework-0.1.2/sloth/api/models.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/all.min.css` & `sloth-framework-0.1.2/sloth/api/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/bootstrap-icons.css` & `sloth-framework-0.1.2/sloth/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/bootstrap.min.css` & `sloth-framework-0.1.2/sloth/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/colorpick.min.css` & `sloth-framework-0.1.2/sloth/api/static/css/colorpick.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf` & `sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf` & `sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/fonts/bootstrap-icons.woff` & `sloth-framework-0.1.2/sloth/api/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/fonts/bootstrap-icons.woff2` & `sloth-framework-0.1.2/sloth/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/icons.svg` & `sloth-framework-0.1.2/sloth/api/static/css/icons.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/images/ui-icons_444444_256x240.png` & `sloth-framework-0.1.2/sloth/api/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/images/ui-icons_555555_256x240.png` & `sloth-framework-0.1.2/sloth/api/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/jquery-ui.css` & `sloth-framework-0.1.2/sloth/api/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/leaflet.css` & `sloth-framework-0.1.2/sloth/api/static/css/leaflet.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/select2.min.css` & `sloth-framework-0.1.2/sloth/api/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/sloth.css` & `sloth-framework-0.1.2/sloth/api/static/css/sloth.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/css/trumbowyg.min.css` & `sloth-framework-0.1.2/sloth/api/static/css/trumbowyg.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/fontawesome.min.css` & `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/fontawesome.min.js` & `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf` & `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2` & `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf` & `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2` & `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf` & `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2` & `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2` & `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2` & `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/materialicons/materialicons.css` & `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/materialicons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2` & `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/click.png` & `sloth-framework-0.1.2/sloth/api/static/images/click.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/hand.png` & `sloth-framework-0.1.2/sloth/api/static/images/hand.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/icon.png` & `sloth-framework-0.1.2/sloth/api/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/icon.svg` & `sloth-framework-0.1.2/sloth/api/static/images/icon.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/images/badge.png` & `sloth-framework-0.1.2/sloth/api/static/images/images/badge.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/images/icon.png` & `sloth-framework-0.1.2/sloth/api/static/images/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/login.jpeg` & `sloth-framework-0.1.2/sloth/api/static/images/login.jpeg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/logo.png` & `sloth-framework-0.1.2/sloth/api/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/logo.svg` & `sloth-framework-0.1.2/sloth/api/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/no-image.png` & `sloth-framework-0.1.2/sloth/api/static/images/no-image.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/sloth.png` & `sloth-framework-0.1.2/sloth/api/static/images/sloth.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/images/user.png` & `sloth-framework-0.1.2/sloth/api/static/images/user.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/api.js` & `sloth-framework-0.1.2/sloth/api/static/js/api.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/bootstrap.bundle.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/colorpick.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/colorpick.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/i18n/pt-BR.js` & `sloth-framework-0.1.2/sloth/api/static/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/jquery-3.6.0.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/jquery-ui.js` & `sloth-framework-0.1.2/sloth/api/static/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/jquery.binarytransport.js` & `sloth-framework-0.1.2/sloth/api/static/js/jquery.binarytransport.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/jquery.mask.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/jquery.timepicker.js` & `sloth-framework-0.1.2/sloth/api/static/js/jquery.timepicker.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/leaflet.js` & `sloth-framework-0.1.2/sloth/api/static/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/masonry.pkgd.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/popper.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/qr-scanner-worker.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/qr-scanner-worker.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/qr-scanner.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/qr-scanner.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/qrcode.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/select2.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/sloth.js` & `sloth-framework-0.1.2/sloth/api/static/js/sloth.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/sw.js` & `sloth-framework-0.1.2/sloth/api/static/js/sw.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/tests.js` & `sloth-framework-0.1.2/sloth/api/static/js/tests.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/trumbowyg.min.js` & `sloth-framework-0.1.2/sloth/api/static/js/trumbowyg.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/static/js/wpn.js` & `sloth-framework-0.1.2/sloth/api/static/js/wpn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/tasks/__init__.py` & `sloth-framework-0.1.2/sloth/api/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/actions/execute_query.html` & `sloth-framework-0.1.2/sloth/api/templates/actions/execute_query.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/actions/show_icons.html` & `sloth-framework-0.1.2/sloth/api/templates/actions/show_icons.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/api/index.html` & `sloth-framework-0.1.2/sloth/api/templates/api/index.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/charts/bar.html` & `sloth-framework-0.1.2/sloth/api/templates/charts/bar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/charts/column.html` & `sloth-framework-0.1.2/sloth/api/templates/charts/column.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/charts/pie.html` & `sloth-framework-0.1.2/sloth/api/templates/charts/pie.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/actions.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/actions.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/apps.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/apps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/base.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/base.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/bottom.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/bottom.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/cards.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/footer.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/footer.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/form.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/form.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/grids.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/grids.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/header.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/header.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/links.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/links.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/messages.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/messages.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/modal.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/modal.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/plus.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/plus.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/report.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/report.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/search.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/search.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/settings.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/settings.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/shortcuts.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/shortcuts.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/tasks.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/dashboard/tools.html` & `sloth-framework-0.1.2/sloth/api/templates/dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/inputs/picker.html` & `sloth-framework-0.1.2/sloth/api/templates/inputs/picker.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/inputs/qrcode.html` & `sloth-framework-0.1.2/sloth/api/templates/inputs/qrcode.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/inputs/select.html` & `sloth-framework-0.1.2/sloth/api/templates/inputs/select.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/accordion.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/accordion.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/calendar.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/cards.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/datatable.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/datatable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/filter.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/filter.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/filters.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/filters.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/queryset.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/queryset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/rows.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/rows.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/scroll.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/scroll.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/statistics.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/statistics.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/queryset/timeline.html` & `sloth-framework-0.1.2/sloth/api/templates/queryset/timeline.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/renderers/calendar/calendar.html` & `sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/renderers/maps/map.html` & `sloth-framework-0.1.2/sloth/api/templates/renderers/maps/map.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/renderers/programing/strtable.html` & `sloth-framework-0.1.2/sloth/api/templates/renderers/programing/strtable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/renderers/utils/steps.html` & `sloth-framework-0.1.2/sloth/api/templates/renderers/utils/steps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/renderers/utils/table.html` & `sloth-framework-0.1.2/sloth/api/templates/renderers/utils/table.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/themes/dark.html` & `sloth-framework-0.1.2/sloth/api/templates/themes/dark.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/valueset/fieldset-group.html` & `sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-group.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/valueset/fieldset-list.html` & `sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-list.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/valueset/fieldset.html` & `sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/valueset/value.html` & `sloth-framework-0.1.2/sloth/api/templates/valueset/value.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templates/valueset/valueset.html` & `sloth-framework-0.1.2/sloth/api/templates/valueset/valueset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/templatetags/tags.py` & `sloth-framework-0.1.2/sloth/api/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/urls.py` & `sloth-framework-0.1.2/sloth/api/urls.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/api/views.py` & `sloth-framework-0.1.2/sloth/api/views.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/cloud/printer.py` & `sloth-framework-0.1.2/sloth/cloud/printer.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/cloud/server.py` & `sloth-framework-0.1.2/sloth/cloud/server.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/conf/settings.py` & `sloth-framework-0.1.2/sloth/conf/settings.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/core/base.py` & `sloth-framework-0.1.2/sloth/core/base.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/core/queryset.py` & `sloth-framework-0.1.2/sloth/core/queryset.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/core/statistics.py` & `sloth-framework-0.1.2/sloth/core/statistics.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/core/validation.py` & `sloth-framework-0.1.2/sloth/core/validation.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/core/valueset.py` & `sloth-framework-0.1.2/sloth/core/valueset.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/db/models/__init__.py` & `sloth-framework-0.1.2/sloth/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/test/__init__.py` & `sloth-framework-0.1.2/sloth/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/test/selenium/__init__.py` & `sloth-framework-0.1.2/sloth/test/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/test/selenium/browser.py` & `sloth-framework-0.1.2/sloth/test/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/utils/__init__.py` & `sloth-framework-0.1.2/sloth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/utils/formatter/__init__.py` & `sloth-framework-0.1.2/sloth/utils/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/utils/http/__init__.py` & `sloth-framework-0.1.2/sloth/utils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/utils/icons/bootstrap.py` & `sloth-framework-0.1.2/sloth/utils/icons/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/utils/icons/fontawesome.py` & `sloth-framework-0.1.2/sloth/utils/icons/fontawesome.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/utils/icons/materialicons.py` & `sloth-framework-0.1.2/sloth/utils/icons/materialicons.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.1/sloth/utils/log/sql.py` & `sloth-framework-0.1.2/sloth/utils/log/sql.py`

 * *Files identical despite different names*

