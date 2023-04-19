# Comparing `tmp/django-silly-auth-1.0.5.tar.gz` & `tmp/django-silly-auth-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-auth-1.0.5.tar", last modified: Fri Apr 14 16:45:24 2023, max compression
+gzip compressed data, was "django-silly-auth-1.0.6.tar", last modified: Wed Apr 19 17:17:25 2023, max compression
```

## Comparing `django-silly-auth-1.0.5.tar` & `django-silly-auth-1.0.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.5/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1620 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1010 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5631 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/config.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6302 2023-04-11 19:05:08.000000 django-silly-auth-1.0.5/django_silly_auth/forms.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/locale/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10574 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/locale/django.pot
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.897895 django-silly-auth-1.0.5/django_silly_auth/locale/en/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/locale/en/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      337 2023-04-11 19:05:08.000000 django-silly-auth-1.0.5/django_silly_auth/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10588 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.897895 django-silly-auth-1.0.5/django_silly_auth/locale/fr/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10088 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    15857 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/mixins.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6096 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/serializers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_base.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.905895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4478 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/_base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/_single_page.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/_users.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.905895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/account.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/change_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/change_username.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/index.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/login.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/reset_password.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/signup.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.905895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/emails/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/emails/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.905895 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/silly/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/silly/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      497 2023-04-11 19:05:08.000000 django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/django_silly_auth/tests/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/tests/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3790 2023-04-14 16:20:53.000000 django-silly-auth-1.0.5/django_silly_auth/tests/test_api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3971 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/tests/test_classic_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1051 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/tests/test_silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4924 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3254 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/utils.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/django_silly_auth/views/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.5/django_silly_auth/views/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-14 13:53:37.000000 django-silly-auth-1.0.5/django_silly_auth/views/api_custom_login.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      445 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/views/api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6472 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/views/api_views_if_drf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    13683 2023-04-14 16:42:40.000000 django-silly-auth-1.0.5/django_silly_auth/views/classics.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1771 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/views/silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2023-04-14 14:46:10.000000 django-silly-auth-1.0.5/django_silly_auth/views/try_views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-14 16:45:24.901895 django-silly-auth-1.0.5/django_silly_auth.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1620 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2464 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-14 16:45:24.000000 django-silly-auth-1.0.5/django_silly_auth.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-14 16:45:24.909895 django-silly-auth-1.0.5/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2227 2023-04-14 16:45:16.000000 django-silly-auth-1.0.5/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.752260 django-silly-auth-1.0.6/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.6/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1692 2023-04-19 17:17:25.752260 django-silly-auth-1.0.6/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1082 2023-04-19 16:40:47.000000 django-silly-auth-1.0.6/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.740260 django-silly-auth-1.0.6/django_silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-19 16:40:47.000000 django-silly-auth-1.0.6/django_silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5786 2023-04-19 16:59:34.000000 django-silly-auth-1.0.6/django_silly_auth/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6302 2023-04-11 19:05:08.000000 django-silly-auth-1.0.6/django_silly_auth/forms.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.740260 django-silly-auth-1.0.6/django_silly_auth/locale/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10574 2023-04-14 16:42:40.000000 django-silly-auth-1.0.6/django_silly_auth/locale/django.pot
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.736260 django-silly-auth-1.0.6/django_silly_auth/locale/en/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.744260 django-silly-auth-1.0.6/django_silly_auth/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      337 2023-04-11 19:05:08.000000 django-silly-auth-1.0.6/django_silly_auth/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10588 2023-04-14 16:42:40.000000 django-silly-auth-1.0.6/django_silly_auth/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.736260 django-silly-auth-1.0.6/django_silly_auth/locale/fr/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.744260 django-silly-auth-1.0.6/django_silly_auth/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10088 2023-04-14 16:42:40.000000 django-silly-auth-1.0.6/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    15857 2023-04-14 16:42:40.000000 django-silly-auth-1.0.6/django_silly_auth/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/mixins.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6098 2023-04-19 16:40:47.000000 django-silly-auth-1.0.6/django_silly_auth/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.744260 django-silly-auth-1.0.6/django_silly_auth/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.6/django_silly_auth/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.744260 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/_base.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.744260 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/_try/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-14 14:46:10.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/_try/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4478 2023-04-14 14:46:10.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/_try/_base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-14 14:46:10.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/_try/_single_page.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-14 14:46:10.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/_try/_users.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.748260 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/account.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/change_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/change_username.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/index.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/login.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/reset_password.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/signup.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.748260 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/emails/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/emails/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.748260 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/silly/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/silly/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      497 2023-04-11 19:05:08.000000 django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.748260 django-silly-auth-1.0.6/django_silly_auth/tests/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-14 14:46:10.000000 django-silly-auth-1.0.6/django_silly_auth/tests/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3790 2023-04-14 16:20:53.000000 django-silly-auth-1.0.6/django_silly_auth/tests/test_api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3971 2023-04-14 16:42:40.000000 django-silly-auth-1.0.6/django_silly_auth/tests/test_classic_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1051 2023-04-14 16:42:40.000000 django-silly-auth-1.0.6/django_silly_auth/tests/test_silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5294 2023-04-19 16:59:34.000000 django-silly-auth-1.0.6/django_silly_auth/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3254 2023-04-14 14:46:10.000000 django-silly-auth-1.0.6/django_silly_auth/utils.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.752260 django-silly-auth-1.0.6/django_silly_auth/views/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.6/django_silly_auth/views/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3091 2023-04-19 16:40:47.000000 django-silly-auth-1.0.6/django_silly_auth/views/api_custom_login.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      445 2023-04-14 16:42:40.000000 django-silly-auth-1.0.6/django_silly_auth/views/api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6688 2023-04-19 16:59:34.000000 django-silly-auth-1.0.6/django_silly_auth/views/api_views_if_drf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    13683 2023-04-14 16:42:40.000000 django-silly-auth-1.0.6/django_silly_auth/views/classics.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1771 2023-04-14 14:46:10.000000 django-silly-auth-1.0.6/django_silly_auth/views/silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2023-04-14 14:46:10.000000 django-silly-auth-1.0.6/django_silly_auth/views/try_views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-19 17:17:25.740260 django-silly-auth-1.0.6/django_silly_auth.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1692 2023-04-19 17:17:25.000000 django-silly-auth-1.0.6/django_silly_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2464 2023-04-19 17:17:25.000000 django-silly-auth-1.0.6/django_silly_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-19 17:17:25.000000 django-silly-auth-1.0.6/django_silly_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-19 17:17:25.000000 django-silly-auth-1.0.6/django_silly_auth.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-19 17:17:25.000000 django-silly-auth-1.0.6/django_silly_auth.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-19 17:17:25.752260 django-silly-auth-1.0.6/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2227 2023-04-19 16:40:47.000000 django-silly-auth-1.0.6/setup.py
```

### Comparing `django-silly-auth-1.0.5/LICENSE.md` & `django-silly-auth-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/PKG-INFO` & `django-silly-auth-1.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.5
+Version: 1.0.6
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
@@ -39,11 +39,12 @@
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
 ### Changelog
 
+- 1.0.6: login improved: returns 'auth_token', errors are json objects.
 - 1.0.5: test coverage: 75 %
 - 1.0.1: **i18n** fr + en
```

### Comparing `django-silly-auth-1.0.5/README.md` & `django-silly-auth-1.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
 ### Changelog
 
+- 1.0.6: login improved: returns 'auth_token', errors are json objects.
 - 1.0.5: test coverage: 75 %
 - 1.0.1: **i18n** fr + en
```

### Comparing `django-silly-auth-1.0.5/django_silly_auth/config.py` & `django-silly-auth-1.0.6/django_silly_auth/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     # Quick settings
     "AUTO_SET": 'TRY',  # 'CLASSIC', 'SPA', 'TRY', 'SILLY' or 'TEST'
     "DSA_PREFIX": 'auth/',  # only the CLASSIC_INDEX view has a blank prefix, it's the entry point in a classic site.
 
     # Secondary settings
     "SITE_NAME": None,  # str used in templates if provided
     "DELETE_UNCONFIRMED_TIME": 24.0,  # hours after what an unconfirmed account is deleted, O to set off
+    "ALLOW_CHANGE_USERNAME": True,  # allows the change username endpoint
+
 
     # Classic settings
     "USE_CLASSIC": True,
         # redirections
     "USE_CLASSIC_INDEX": True,  # if False, your index route must have the name='classic_index'
     "USE_CLASSIC_ACCOUNT": True,  # if False, your account route must have the name='classic_account'
         # templates settings
@@ -56,14 +58,15 @@
         "silly_auth/emails/confirm_email.txt",
     "EMAIL_RESET_PASSWORD_TEMPLATE":  # email template
         "silly_auth/emails/request_password_reset.txt",
 
     # For development,
     "TRY_TEMPLATES": False,  # for dev only,  opens 2 "_test/" endpoint
     "VERBOSE": False,  # prints to terminal : imports
+    "ALLOW_GET_ALL_USERS": False,  # for DEV ONLY,  opens 'users/all/' endpoint
 }
 
 
 # Overwrite SILLY_AUTH_SETTINGS with datas from settings.SILLY_AUTH
 
 try:
     settings.SILLY_AUTH
```

### Comparing `django-silly-auth-1.0.5/django_silly_auth/forms.py` & `django-silly-auth-1.0.6/django_silly_auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/locale/django.pot` & `django-silly-auth-1.0.6/django_silly_auth/locale/django.pot`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/locale/en/LC_MESSAGES/django.po` & `django-silly-auth-1.0.6/django_silly_auth/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/django.mo` & `django-silly-auth-1.0.6/django_silly_auth/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/locale/fr/LC_MESSAGES/django.po` & `django-silly-auth-1.0.6/django_silly_auth/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/mixins.py` & `django-silly-auth-1.0.6/django_silly_auth/mixins.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/serializers.py` & `django-silly-auth-1.0.6/django_silly_auth/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             if not User.objects.filter(email=credential).exists():
                 credential_errors += [_("Email not found"), ]
         else:
             if not User.objects.filter(username=credential).exists():
                 credential_errors += [_("User not found"), ]
 
         if credential_errors:
-            errors['username'] = credential_errors
+            errors['credential'] = credential_errors
         if password_errors:
             errors['password'] = password_errors
 
         if errors:
             raise serializers.ValidationError(errors)
         return data
```

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_base.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/_try/_base.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/_try/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/account.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/account.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/change_email.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/change_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/change_username.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/change_username.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/login.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/login.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/request_password_reset.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/request_password_reset.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/reset_password.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/reset_password.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/templates/silly_auth/classic/signup.html` & `django-silly-auth-1.0.6/django_silly_auth/templates/silly_auth/classic/signup.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/tests/test_api_views.py` & `django-silly-auth-1.0.6/django_silly_auth/tests/test_api_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/tests/test_classic_views.py` & `django-silly-auth-1.0.6/django_silly_auth/tests/test_classic_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/tests/test_silly_views.py` & `django-silly-auth-1.0.6/django_silly_auth/tests/test_silly_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/urls.py` & `django-silly-auth-1.0.6/django_silly_auth/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,57 +47,71 @@
         ),
         path(
             f'{prefix}password/change/',
             api_views.password_change,
             name='password_change'
         ),
         path(
-            f'{prefix}username/change/',
-            api_views.username_change,
-            name='username_change'
-        ),
-        path(
             f'{prefix}email/request_change/',
             api_views.email_request_change,
             name='email_request_change'
         ),
         ]
 
+    if conf['ALLOW_CHANGE_USERNAME']:
+        urlpatterns += [
+            path(
+                f'{prefix}username/change/',
+                api_views.username_change,
+                name='username_change'
+            ),
+        ]
+
     if conf["ALLOW_DELETE_ME_ENDPOINT"]:
         urlpatterns += [
             path(f'{prefix}users/delete_me/', api_views.users_delete_me, name='users_delete_me'),
         ]
 
     if conf["ALLOW_CREATE_USER_ENDPOINT"]:
         urlpatterns += [path(f'{prefix}users/', api_views.UserView.as_view(), name="users")]
 
     if conf['ALLOW_MY_INFOS_ENDPOINT']:
         urlpatterns += [path(f'{prefix}users/my_infos/', api_views.users_my_infos, name="users_my_infos")]
 
+    if conf["ALLOW_GET_ALL_USERS"]:
+        urlpatterns += [path(f'{prefix}users/all/', api_views.get_users_all, name="get_users_all")]
+
 # Classic routes
 
 if conf["USE_CLASSIC"]:
     urlpatterns += [
         path(f'{prefix}classic_login/', classics.login_view, name='classic_login'),
         path(f'{prefix}classic_logout/', classics.logout_view, name='classic_logout'),
         path(f'{prefix}classic_signup/', classics.signup_view, name='classic_signup'),
-        path(f'{prefix}classic_change_username/', classics.change_username, name='classic_change_username'),
         path(f'{prefix}classic_change_email/', classics.change_email, name='classic_change_email'),
         path(f'{prefix}classic_confirm_email/<token>', classics.confirm_email, name='classic_confirm_email'),
         path(
             f'{prefix}classic_request_resend_confirmation_email/',
             classics.request_resend_account_confirmation_email,
             name='classic_request_resend_confirmation_email'
         ),
         path(
             f'{prefix}classic_reset_password/',
             classics.reset_password,
             name='classic_reset_password_authenticated'
         ),
     ]
+    if conf["ALLOW_CHANGE_USERNAME"]:
+        urlpatterns += [
+            path(
+                f'{prefix}classic_change_username/',
+                classics.change_username,
+                name='classic_change_username'
+            ),
+        ]
     if conf["USE_CLASSIC_INDEX"]:
         urlpatterns += [path('', classics.index, name='classic_index'), ]
     if conf["USE_CLASSIC_ACCOUNT"]:
         urlpatterns += [path(f'{prefix}classic_account/', classics.account, name='classic_account'), ]
 
 # Email Confirmation routes
```

### Comparing `django-silly-auth-1.0.5/django_silly_auth/utils.py` & `django-silly-auth-1.0.6/django_silly_auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/views/api_custom_login.py` & `django-silly-auth-1.0.6/django_silly_auth/views/api_custom_login.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         if match:
             if not user.is_confirmed and not user.is_superuser:
                 msg = _(
                     'Your account has not been confirmed yet. '
                     'Please check your inbox for a confirmation link.')
                 raise ValidationError(msg, code='authorization')
             token, created = Token.objects.get_or_create(user=user)
-            return Response({'token': token.key})
+            return Response({'auth_token': token.key})
         msg = _('Incorrect credentials.')
-        raise ValidationError(msg, code='authorization')
+        raise ValidationError({'authentication': msg}, code='authorization')
 
 
 class LoginWithJWTToken(APIView):
     @transaction.atomic
     def post(self, request, *args, **kwargs):
         serializer = CredentialJWTokenSerializer(data=request.data)
         if serializer.is_valid():
```

### Comparing `django-silly-auth-1.0.5/django_silly_auth/views/api_views_if_drf.py` & `django-silly-auth-1.0.6/django_silly_auth/views/api_views_if_drf.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,21 @@
 
             return Response(msg)
         else:
             msg = serializer.errors
             raise ValidationError({"error": msg}, code='authorization')
 
 
+@api_view(['GET'])
+def get_users_all(request):
+    """!! FOR DEV ONLY !! Get all users"""
+    users = User.objects.all()
+    serializer = GetAllUsersSerializer(users, many=True)
+    return Response(serializer.data)
+
 @transaction.atomic
 @api_view(['POST'])
 @permission_classes([IsAuthenticated])
 def password_change(request):
     """Changes the user's password"""
     serializer = PasswordsSerializer(data=request.data)
     if serializer.is_valid():
```

### Comparing `django-silly-auth-1.0.5/django_silly_auth/views/classics.py` & `django-silly-auth-1.0.6/django_silly_auth/views/classics.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/views/silly_views.py` & `django-silly-auth-1.0.6/django_silly_auth/views/silly_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth/views/try_views.py` & `django-silly-auth-1.0.6/django_silly_auth/views/try_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/django_silly_auth.egg-info/PKG-INFO` & `django-silly-auth-1.0.6/django_silly_auth.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.5
+Version: 1.0.6
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
@@ -39,11 +39,12 @@
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
 ### Changelog
 
+- 1.0.6: login improved: returns 'auth_token', errors are json objects.
 - 1.0.5: test coverage: 75 %
 - 1.0.1: **i18n** fr + en
```

### Comparing `django-silly-auth-1.0.5/django_silly_auth.egg-info/SOURCES.txt` & `django-silly-auth-1.0.6/django_silly_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.5/setup.py` & `django-silly-auth-1.0.6/setup.py`

 * *Files identical despite different names*

