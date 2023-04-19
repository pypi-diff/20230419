# Comparing `tmp/garpix_user-3.5.0rc7.tar.gz` & `tmp/garpix_user-3.5.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_user-3.5.0rc7.tar", last modified: Tue Apr 18 20:27:00 2023, max compression
+gzip compressed data, was "garpix_user-3.5.0rc8.tar", last modified: Wed Apr 19 13:52:47 2023, max compression
```

## Comparing `garpix_user-3.5.0rc7.tar` & `garpix_user-3.5.0rc8.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.391217 garpix_user-3.5.0rc7/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-18 20:27:00.390958 garpix_user-3.5.0rc7/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.382817 garpix_user-3.5.0rc7/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4658 2023-04-18 20:25:50.000000 garpix_user-3.5.0rc7/garpix_user/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc7/garpix_user/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9155 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc7/garpix_user/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc7/garpix_user/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.383888 garpix_user-3.5.0rc7/garpix_user/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/admin/referral_type.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.5.0rc7/garpix_user/admin/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/admin/user_session.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc7/garpix_user/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.5.0rc7/garpix_user/exceptions.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.384102 garpix_user-3.5.0rc7/garpix_user/forms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/forms/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      869 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/forms/login.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.380079 garpix_user-3.5.0rc7/garpix_user/locale/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.380125 garpix_user-3.5.0rc7/garpix_user/locale/ru/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.384325 garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6866 2023-04-14 08:29:08.000000 garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9277 2023-04-07 10:32:34.000000 garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.384433 garpix_user-3.5.0rc7/garpix_user/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.384624 garpix_user-3.5.0rc7/garpix_user/mixins/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.385069 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/code_length_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4965 2023-04-18 20:24:54.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/email_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3242 2023-03-07 13:31:03.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/phone_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5436 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/restore_password.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.385402 garpix_user-3.5.0rc7/garpix_user/mixins/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/mixins/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc7/garpix_user/mixins/serializers/password_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.5.0rc7/garpix_user/mixins/serializers/to_lower.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.386035 garpix_user-3.5.0rc7/garpix_user/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc7/garpix_user/models/access_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/models/refferal.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc7/garpix_user/models/refresh_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.5.0rc7/garpix_user/models/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4894 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc7/garpix_user/models/user_session.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.386227 garpix_user-3.5.0rc7/garpix_user/rest/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/rest/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-01 07:20:35.000000 garpix_user-3.5.0rc7/garpix_user/rest/authentication.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.387083 garpix_user-3.5.0rc7/garpix_user/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      769 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.5.0rc7/garpix_user/serializers/auth_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/serializers/email_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1418 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc7/garpix_user/serializers/passwrod_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/serializers/phone_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/serializers/refresh_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.5.0rc7/garpix_user/serializers/registration_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.5.0rc7/garpix_user/serializers/user_session_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-18 20:25:50.000000 garpix_user-3.5.0rc7/garpix_user/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.387310 garpix_user-3.5.0rc7/garpix_user/tasks/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc7/garpix_user/tasks/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.5.0rc7/garpix_user/tasks/delete_unconfirmed_users.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.380861 garpix_user-3.5.0rc7/garpix_user/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.387425 garpix_user-3.5.0rc7/garpix_user/templates/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/templates/garpix_user/send_confirm.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.387643 garpix_user-3.5.0rc7/garpix_user/tests/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.388074 garpix_user-3.5.0rc7/garpix_user/tests/test_api/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.388266 garpix_user-3.5.0rc7/garpix_user/tests/test_api/_trial_temp/
--rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/_trial_temp/_trial_marker
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/_trial_temp/test.log
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_login.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_registration.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_user_session_restore_password.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_views.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.388573 garpix_user-3.5.0rc7/garpix_user/tests/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/utils/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/utils/test_case_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2581 2023-03-07 13:05:56.000000 garpix_user-3.5.0rc7/garpix_user/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.389256 garpix_user-3.5.0rc7/garpix_user/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-03-20 15:00:08.000000 garpix_user-3.5.0rc7/garpix_user/utils/backends.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/utils/current_date.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.5.0rc7/garpix_user/utils/drf_spectacular.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/utils/get_token_from_request.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc7/garpix_user/utils/repluralize.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.390788 garpix_user-3.5.0rc7/garpix_user/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/change_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3993 2023-04-18 20:26:41.000000 garpix_user-3.5.0rc7/garpix_user/views/email_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1401 2023-02-27 12:35:42.000000 garpix_user-3.5.0rc7/garpix_user/views/login_views.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/views/logout_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1610 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/obtain_auth_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc7/garpix_user/views/phone_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/referral_links_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.5.0rc7/garpix_user/views/refresh_token_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/registration_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3210 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc7/garpix_user/views/restore_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/user_session_view.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.383460 garpix_user-3.5.0rc7/garpix_user.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3140 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      283 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-04-18 20:27:00.391256 garpix_user-3.5.0rc7/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.527492 garpix_user-3.5.0rc8/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-19 13:52:47.527192 garpix_user-3.5.0rc8/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.519347 garpix_user-3.5.0rc8/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4658 2023-04-18 20:25:50.000000 garpix_user-3.5.0rc8/garpix_user/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc8/garpix_user/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9155 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc8/garpix_user/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc8/garpix_user/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.520429 garpix_user-3.5.0rc8/garpix_user/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/admin/referral_type.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.5.0rc8/garpix_user/admin/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/admin/user_session.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc8/garpix_user/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.5.0rc8/garpix_user/exceptions.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.520640 garpix_user-3.5.0rc8/garpix_user/forms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/forms/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      869 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/forms/login.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.516691 garpix_user-3.5.0rc8/garpix_user/locale/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.516744 garpix_user-3.5.0rc8/garpix_user/locale/ru/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.520862 garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6866 2023-04-14 08:29:08.000000 garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9277 2023-04-07 10:32:34.000000 garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.520970 garpix_user-3.5.0rc8/garpix_user/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.521171 garpix_user-3.5.0rc8/garpix_user/mixins/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.521606 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/code_length_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5263 2023-04-19 13:51:11.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/email_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3242 2023-03-07 13:31:03.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/phone_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5436 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/restore_password.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.521924 garpix_user-3.5.0rc8/garpix_user/mixins/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/mixins/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc8/garpix_user/mixins/serializers/password_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.5.0rc8/garpix_user/mixins/serializers/to_lower.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.522544 garpix_user-3.5.0rc8/garpix_user/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc8/garpix_user/models/access_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/models/refferal.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc8/garpix_user/models/refresh_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.5.0rc8/garpix_user/models/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4894 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc8/garpix_user/models/user_session.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.522727 garpix_user-3.5.0rc8/garpix_user/rest/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/rest/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-01 07:20:35.000000 garpix_user-3.5.0rc8/garpix_user/rest/authentication.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.523596 garpix_user-3.5.0rc8/garpix_user/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      769 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.5.0rc8/garpix_user/serializers/auth_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/serializers/email_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1418 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc8/garpix_user/serializers/passwrod_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/serializers/phone_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/serializers/refresh_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.5.0rc8/garpix_user/serializers/registration_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.5.0rc8/garpix_user/serializers/user_session_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-19 13:52:41.000000 garpix_user-3.5.0rc8/garpix_user/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.523808 garpix_user-3.5.0rc8/garpix_user/tasks/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc8/garpix_user/tasks/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.5.0rc8/garpix_user/tasks/delete_unconfirmed_users.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.517488 garpix_user-3.5.0rc8/garpix_user/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.523921 garpix_user-3.5.0rc8/garpix_user/templates/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/templates/garpix_user/send_confirm.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.524129 garpix_user-3.5.0rc8/garpix_user/tests/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.524570 garpix_user-3.5.0rc8/garpix_user/tests/test_api/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.524771 garpix_user-3.5.0rc8/garpix_user/tests/test_api/_trial_temp/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/_trial_temp/_trial_marker
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/_trial_temp/test.log
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_login.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_registration.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_user_session_restore_password.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_views.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.525072 garpix_user-3.5.0rc8/garpix_user/tests/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/utils/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/utils/test_case_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2581 2023-03-07 13:05:56.000000 garpix_user-3.5.0rc8/garpix_user/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.525710 garpix_user-3.5.0rc8/garpix_user/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-03-20 15:00:08.000000 garpix_user-3.5.0rc8/garpix_user/utils/backends.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/utils/current_date.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.5.0rc8/garpix_user/utils/drf_spectacular.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/utils/get_token_from_request.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc8/garpix_user/utils/repluralize.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.527016 garpix_user-3.5.0rc8/garpix_user/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/change_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3914 2023-04-19 13:51:11.000000 garpix_user-3.5.0rc8/garpix_user/views/email_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1401 2023-02-27 12:35:42.000000 garpix_user-3.5.0rc8/garpix_user/views/login_views.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/views/logout_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1610 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/obtain_auth_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc8/garpix_user/views/phone_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/referral_links_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.5.0rc8/garpix_user/views/refresh_token_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/registration_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3210 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc8/garpix_user/views/restore_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/user_session_view.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.519997 garpix_user-3.5.0rc8/garpix_user.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3140 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      283 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-04-19 13:52:47.527535 garpix_user-3.5.0rc8/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/setup.py
```

### Comparing `garpix_user-3.5.0rc7/PKG-INFO` & `garpix_user-3.5.0rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_user
-Version: 3.5.0rc7
+Version: 3.5.0rc8
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_user-3.5.0rc7/garpix_user/CHANGELOG.md` & `garpix_user-3.5.0rc8/garpix_user/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/CONTRIBUTING.md` & `garpix_user-3.5.0rc8/garpix_user/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/README.md` & `garpix_user-3.5.0rc8/garpix_user/README.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/README.rst` & `garpix_user-3.5.0rc8/garpix_user/README.rst`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/admin/user.py` & `garpix_user-3.5.0rc8/garpix_user/admin/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/exceptions.py` & `garpix_user-3.5.0rc8/garpix_user/exceptions.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/forms/login.py` & `garpix_user-3.5.0rc8/garpix_user/forms/login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/django.mo` & `garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/django.po` & `garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/code_length_mixin.py` & `garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/code_length_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/email_confirm.py` & `garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/email_confirm.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,23 @@
                                                null=True)
     email_code_send_date = models.DateTimeField(_("Code sent date"), blank=True, null=True)
     new_email = models.EmailField(_("New email"), blank=True, null=True)
 
     def send_email_confirmation_link(self):
         from garpix_notify.models import Notify
         from garpix_user.models import UserSession
+        from django.contrib.auth import get_user_model
+
+        User = get_user_model()
+
         model_type = 'user_session' if isinstance(self, UserSession) else 'user'
         hash = str(
             hashlib.sha512(f'{self.email}+{self.email_confirmation_code}'.encode("utf-8")).hexdigest()).lower()
         Notify.send(settings.EMAIL_LINK_CONFIRMATION_EVENT, {
-            'confirmation_link': reverse('garpix_user:email_confirmation_link', args=[model_type, hash])
+            'confirmation_link': User.confirm_link_redirect_url(model_type, hash)
         }, email=self.new_email)
 
     def send_email_confirmation_code(self, email=None):
         from django.contrib.auth import get_user_model
         from garpix_user.exceptions import UserRegisteredException, WaitException
         from garpix_notify.models import Notify
 
@@ -46,15 +50,15 @@
         if anybody_have_this_email.count() > 0:
             return UserRegisteredException(field='email', extra_data={
                 'field': self._meta.get_field('email').verbose_name.title().lower()})
 
         if settings.GARPIX_USER.get('TIME_LAST_REQUEST', None):
             if self.email_code_send_date and self.email_code_send_date + timedelta(
                     minutes=settings.GARPIX_USER.get('TIME_LAST_REQUEST')) >= datetime.now(
-                        self.email_code_send_date.tzinfo):
+                self.email_code_send_date.tzinfo):
                 return WaitException()
 
         confirmation_code = get_random_string(self.get_confirm_code_length('email'), string.digits)
 
         self.new_email = email or self.email
 
         self.email_confirmation_code = confirmation_code
@@ -90,35 +94,37 @@
         self.email_confirmation_code = None
         self.save()
         return True
 
     @classmethod
     def confirm_email_by_link(cls, hash):
         from garpix_user.exceptions import IncorrectCodeException, NoTimeLeftException
+        from garpix_user.models import UserSession
 
-        users_list = cls.objects.filter(is_email_confirmed=False)
+        _filter_data = {'is_email_confirmed': False} if isinstance(cls, UserSession) else {}
+        users_list = cls.objects.filter(**_filter_data)
 
         for user in users_list:
             if str(hashlib.sha512(
                     f'{user.email}+{user.email_confirmation_code}'.encode("utf-8")).hexdigest()).lower() == hash:
                 time_is_up = (datetime.now(
                     user.email_code_send_date.tzinfo) - user.email_code_send_date).days > settings.GARPIX_USER.get(
                     'CONFIRM_EMAIL_CODE_LIFE_TIME', 6)
                 if time_is_up:
-                    return NoTimeLeftException(field='email_confirmation_code')
+                    return False, NoTimeLeftException(field='email_confirmation_code')
                 user.is_email_confirmed = True
                 user.email = user.new_email or user.email
                 user.email_confirmation_code = None
                 user.save()
-                return True
+                return True, user
 
-        return IncorrectCodeException(field='email_confirmation_code')
+        return False, IncorrectCodeException(field='email_confirmation_code')
 
     def check_email_confirmation(self):
         return self.is_email_confirmed
 
     @classmethod
-    def confirm_link_redirect_url(cls):
-        return '/'
+    def confirm_link_redirect_url(cls, hash, model_type):
+        return reverse('garpix_user:email_confirmation_link', args=[model_type, hash])
 
     class Meta:
         abstract = True
```

### Comparing `garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/phone_confirm.py` & `garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/phone_confirm.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/mixins/models/restore_password.py` & `garpix_user-3.5.0rc8/garpix_user/mixins/models/restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/mixins/serializers/password_mixin.py` & `garpix_user-3.5.0rc8/garpix_user/mixins/serializers/password_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/models/access_token.py` & `garpix_user-3.5.0rc8/garpix_user/models/access_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/models/refferal.py` & `garpix_user-3.5.0rc8/garpix_user/models/refferal.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/models/refresh_token.py` & `garpix_user-3.5.0rc8/garpix_user/models/refresh_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/models/user.py` & `garpix_user-3.5.0rc8/garpix_user/models/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/models/user_session.py` & `garpix_user-3.5.0rc8/garpix_user/models/user_session.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/rest/authentication.py` & `garpix_user-3.5.0rc8/garpix_user/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/serializers/__init__.py` & `garpix_user-3.5.0rc8/garpix_user/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/serializers/auth_token_serializer.py` & `garpix_user-3.5.0rc8/garpix_user/serializers/auth_token_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/serializers/passwrod_serializer.py` & `garpix_user-3.5.0rc8/garpix_user/serializers/passwrod_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/serializers/registration_serializer.py` & `garpix_user-3.5.0rc8/garpix_user/serializers/registration_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/settings.py` & `garpix_user-3.5.0rc8/garpix_user/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/setup.py` & `garpix_user-3.5.0rc8/garpix_user/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.5.0-rc7',
+    version='3.5.0-rc8',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_user-3.5.0rc7/garpix_user/tasks/delete_unconfirmed_users.py` & `garpix_user-3.5.0rc8/garpix_user/tasks/delete_unconfirmed_users.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_login.py` & `garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_registration.py` & `garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_registration.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_user_session_restore_password.py` & `garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_user_session_restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/tests/test_views.py` & `garpix_user-3.5.0rc8/garpix_user/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/tests/utils/settings.py` & `garpix_user-3.5.0rc8/garpix_user/tests/utils/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/tests/utils/test_case_mixin.py` & `garpix_user-3.5.0rc8/garpix_user/tests/utils/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/urls.py` & `garpix_user-3.5.0rc8/garpix_user/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/utils/backends.py` & `garpix_user-3.5.0rc8/garpix_user/utils/backends.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/utils/repluralize.py` & `garpix_user-3.5.0rc8/garpix_user/utils/repluralize.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/__init__.py` & `garpix_user-3.5.0rc8/garpix_user/views/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/change_password_view.py` & `garpix_user-3.5.0rc8/garpix_user/views/change_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/email_confirmation_view.py` & `garpix_user-3.5.0rc8/garpix_user/views/email_confirmation_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,12 +80,11 @@
 
     def get_redirect_url(self, *args, **kwargs):
         User = get_user_model()
         hash = self.kwargs.get('hash', None)
         model_type = self.kwargs.get('model_type', None)
 
         model = UserSession if model_type == 'user_session' else User
-        result = model.confirm_email_by_link(hash)
-        _redirect_url = User.confirm_link_redirect_url()
+        result, user = model.confirm_email_by_link(hash)
         if result is not True:
-            return f"{_redirect_url}?status=error"
-        return f"{_redirect_url}?status=success"
+            return f"/?status=error"
+        return f"/?status=success"
```

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/login_views.py` & `garpix_user-3.5.0rc8/garpix_user/views/login_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/logout_view.py` & `garpix_user-3.5.0rc8/garpix_user/views/logout_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/obtain_auth_token.py` & `garpix_user-3.5.0rc8/garpix_user/views/obtain_auth_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/phone_confirmation_view.py` & `garpix_user-3.5.0rc8/garpix_user/views/phone_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/referral_links_view.py` & `garpix_user-3.5.0rc8/garpix_user/views/referral_links_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/refresh_token_view.py` & `garpix_user-3.5.0rc8/garpix_user/views/refresh_token_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/registration_view.py` & `garpix_user-3.5.0rc8/garpix_user/views/registration_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/restore_password_view.py` & `garpix_user-3.5.0rc8/garpix_user/views/restore_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user/views/user_session_view.py` & `garpix_user-3.5.0rc8/garpix_user/views/user_session_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/garpix_user.egg-info/PKG-INFO` & `garpix_user-3.5.0rc8/garpix_user.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-user
-Version: 3.5.0rc7
+Version: 3.5.0rc8
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_user-3.5.0rc7/garpix_user.egg-info/SOURCES.txt` & `garpix_user-3.5.0rc8/garpix_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc7/setup.py` & `garpix_user-3.5.0rc8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.5.0-rc7',
+    version='3.5.0-rc8',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

