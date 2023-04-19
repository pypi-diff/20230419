# Comparing `tmp/django-functest-1.5.3.tar.gz` & `tmp/django-functest-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-functest-1.5.3.tar", last modified: Wed Jan  4 10:13:05 2023, max compression
+gzip compressed data, was "django-functest-1.5.4.tar", last modified: Wed Apr 19 16:03:45 2023, max compression
```

## Comparing `django-functest-1.5.3.tar` & `django-functest-1.5.4.tar`

### file list

```diff
@@ -1,121 +1,123 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.185027 django-functest-1.5.3/
--rw-r--r--   0 luke      (1000) luke      (1000)       29 2018-03-20 11:35:06.000000 django-functest-1.5.3/.coveragerc
--rw-r--r--   0 luke      (1000) luke      (1000)      331 2015-12-29 12:29:40.000000 django-functest-1.5.3/.editorconfig
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.169027 django-functest-1.5.3/.github/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.173027 django-functest-1.5.3/.github/workflows/
--rw-r--r--   0 luke      (1000) luke      (1000)     2634 2023-01-04 10:04:42.000000 django-functest-1.5.3/.github/workflows/pythonpackage.yml
--rw-r--r--   0 luke      (1000) luke      (1000)      462 2022-08-20 16:26:04.000000 django-functest-1.5.3/.gitignore
--rw-r--r--   0 luke      (1000) luke      (1000)     1408 2022-12-31 09:04:13.000000 django-functest-1.5.3/.pre-commit-config.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)      145 2021-11-14 21:22:06.000000 django-functest-1.5.3/.readthedocs.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)      245 2016-01-08 16:37:59.000000 django-functest-1.5.3/AUTHORS.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     3506 2022-08-20 16:26:04.000000 django-functest-1.5.3/CONTRIBUTING.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     6442 2023-01-04 10:08:39.000000 django-functest-1.5.3/HISTORY.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1473 2021-01-06 18:46:53.000000 django-functest-1.5.3/LICENSE
--rw-r--r--   0 luke      (1000) luke      (1000)      586 2022-08-22 14:20:44.000000 django-functest-1.5.3/MANIFEST.in
--rw-rw-rw-   0 luke      (1000) luke      (1000)     7147 2023-01-04 10:13:05.185027 django-functest-1.5.3/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     5879 2022-09-30 14:44:23.000000 django-functest-1.5.3/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      634 2023-01-04 10:04:42.000000 django-functest-1.5.3/RELEASE.rst
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.173027 django-functest-1.5.3/django_functest.egg-info/
--rw-rw-rw-   0 luke      (1000) luke      (1000)     7147 2023-01-04 10:13:05.000000 django-functest-1.5.3/django_functest.egg-info/PKG-INFO
--rw-rw-rw-   0 luke      (1000) luke      (1000)     3343 2023-01-04 10:13:05.000000 django-functest-1.5.3/django_functest.egg-info/SOURCES.txt
--rw-rw-rw-   0 luke      (1000) luke      (1000)        1 2023-01-04 10:13:05.000000 django-functest-1.5.3/django_functest.egg-info/dependency_links.txt
--rw-rw-rw-   0 luke      (1000) luke      (1000)        1 2018-05-13 20:09:00.000000 django-functest-1.5.3/django_functest.egg-info/not-zip-safe
--rw-rw-rw-   0 luke      (1000) luke      (1000)       85 2023-01-04 10:13:05.000000 django-functest-1.5.3/django_functest.egg-info/requires.txt
--rw-rw-rw-   0 luke      (1000) luke      (1000)       16 2023-01-04 10:13:05.000000 django-functest-1.5.3/django_functest.egg-info/top_level.txt
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.177027 django-functest-1.5.3/docs/
--rw-r--r--   0 luke      (1000) luke      (1000)     6778 2015-12-29 12:29:40.000000 django-functest-1.5.3/docs/Makefile
--rw-r--r--   0 luke      (1000) luke      (1000)       28 2015-12-29 12:29:40.000000 django-functest-1.5.3/docs/authors.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     9836 2022-09-30 14:44:23.000000 django-functest-1.5.3/docs/common.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     7916 2023-01-04 10:08:50.000000 django-functest-1.5.3/docs/conf.py
--rw-r--r--   0 luke      (1000) luke      (1000)       33 2015-12-29 12:29:40.000000 django-functest-1.5.3/docs/contributing.rst
--rw-r--r--   0 luke      (1000) luke      (1000)       28 2015-12-29 12:29:40.000000 django-functest-1.5.3/docs/history.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      395 2022-09-30 14:44:23.000000 django-functest-1.5.3/docs/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     2649 2022-12-31 09:07:01.000000 django-functest-1.5.3/docs/installation.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     5955 2022-09-01 16:02:55.000000 django-functest-1.5.3/docs/interactive.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     6467 2015-12-29 12:29:40.000000 django-functest-1.5.3/docs/make.bat
--rw-r--r--   0 luke      (1000) luke      (1000)     2569 2022-08-22 14:20:58.000000 django-functest-1.5.3/docs/pytest.rst
--rw-r--r--   0 luke      (1000) luke      (1000)       14 2021-11-14 20:59:12.000000 django-functest-1.5.3/docs/requirements.txt
--rw-r--r--   0 luke      (1000) luke      (1000)     8987 2022-12-31 09:04:13.000000 django-functest-1.5.3/docs/selenium.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     2978 2022-09-30 14:44:23.000000 django-functest-1.5.3/docs/tips.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     6621 2022-09-30 14:44:23.000000 django-functest-1.5.3/docs/usage.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     2057 2022-09-30 14:44:23.000000 django-functest-1.5.3/docs/utils.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      409 2018-05-18 17:34:51.000000 django-functest-1.5.3/docs/webtest.rst
--rwxr-xr--   0 luke      (1000) luke      (1000)      223 2018-03-20 05:53:16.000000 django-functest-1.5.3/download_firefox.sh
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.169027 django-functest-1.5.3/examples/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.177027 django-functest-1.5.3/examples/example_project/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.177027 django-functest-1.5.3/examples/example_project/accounts/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-22 13:54:24.000000 django-functest-1.5.3/examples/example_project/accounts/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)      189 2022-08-22 13:48:00.000000 django-functest-1.5.3/examples/example_project/accounts/admin.py
--rw-r--r--   0 luke      (1000) luke      (1000)      148 2022-08-22 13:41:05.000000 django-functest-1.5.3/examples/example_project/accounts/apps.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.177027 django-functest-1.5.3/examples/example_project/accounts/migrations/
--rw-r--r--   0 luke      (1000) luke      (1000)     4065 2022-08-22 13:50:13.000000 django-functest-1.5.3/examples/example_project/accounts/migrations/0001_initial.py
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-22 13:41:04.000000 django-functest-1.5.3/examples/example_project/accounts/migrations/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)       89 2022-08-22 13:47:22.000000 django-functest-1.5.3/examples/example_project/accounts/models.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.177027 django-functest-1.5.3/examples/example_project/accounts/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-22 13:54:42.000000 django-functest-1.5.3/examples/example_project/accounts/tests/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)      422 2022-08-22 14:19:36.000000 django-functest-1.5.3/examples/example_project/accounts/tests/base.py
--rw-r--r--   0 luke      (1000) luke      (1000)      951 2022-08-22 14:54:12.000000 django-functest-1.5.3/examples/example_project/accounts/tests/factories.py
--rw-r--r--   0 luke      (1000) luke      (1000)      422 2022-09-01 15:59:38.000000 django-functest-1.5.3/examples/example_project/accounts/tests/test_admin.py
--rw-r--r--   0 luke      (1000) luke      (1000)       26 2022-08-22 13:49:35.000000 django-functest-1.5.3/examples/example_project/accounts/views.py
--rw-r--r--   0 luke      (1000) luke      (1000)      471 2022-08-22 13:55:25.000000 django-functest-1.5.3/examples/example_project/conftest.py
--rw-r--r--   0 luke      (1000) luke      (1000)   131072 2022-09-01 15:59:26.000000 django-functest-1.5.3/examples/example_project/db.sqlite3
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.177027 django-functest-1.5.3/examples/example_project/example_project/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-20 20:14:25.000000 django-functest-1.5.3/examples/example_project/example_project/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)      407 2022-08-20 20:14:26.000000 django-functest-1.5.3/examples/example_project/example_project/asgi.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3249 2022-08-22 13:52:58.000000 django-functest-1.5.3/examples/example_project/example_project/settings.py
--rw-r--r--   0 luke      (1000) luke      (1000)      887 2022-08-22 14:19:36.000000 django-functest-1.5.3/examples/example_project/example_project/urls.py
--rw-r--r--   0 luke      (1000) luke      (1000)      407 2022-08-20 20:14:26.000000 django-functest-1.5.3/examples/example_project/example_project/wsgi.py
--rwxr-xr--   0 luke      (1000) luke      (1000)      671 2022-08-22 13:36:41.000000 django-functest-1.5.3/examples/example_project/manage.py
--rw-r--r--   0 luke      (1000) luke      (1000)      116 2022-08-22 13:57:15.000000 django-functest-1.5.3/examples/example_project/pytest.ini
--rw-r--r--   0 luke      (1000) luke      (1000)       62 2022-08-22 14:04:30.000000 django-functest-1.5.3/examples/example_project/requirements.txt
--rw-r--r--   0 luke      (1000) luke      (1000)      297 2022-04-08 19:31:19.000000 django-functest-1.5.3/pyproject.toml
--rw-r--r--   0 luke      (1000) luke      (1000)      275 2022-09-12 13:44:23.000000 django-functest-1.5.3/pytest.ini
--rwxr-xr--   0 luke      (1000) luke      (1000)      484 2023-01-04 10:07:57.000000 django-functest-1.5.3/release.sh
--rw-r--r--   0 luke      (1000) luke      (1000)      138 2022-08-19 16:41:00.000000 django-functest-1.5.3/requirements-dev.txt
--rw-r--r--   0 luke      (1000) luke      (1000)     1562 2023-01-04 10:13:05.185027 django-functest-1.5.3/setup.cfg
--rwxr-xr--   0 luke      (1000) luke      (1000)       38 2023-01-04 10:04:42.000000 django-functest-1.5.3/setup.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.173027 django-functest-1.5.3/src/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.181027 django-functest-1.5.3/src/django_functest/
--rw-r--r--   0 luke      (1000) luke      (1000)      487 2023-01-04 10:08:53.000000 django-functest-1.5.3/src/django_functest/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5590 2022-12-16 13:57:47.000000 django-functest-1.5.3/src/django_functest/base.py
--rw-r--r--   0 luke      (1000) luke      (1000)      222 2022-12-16 13:57:47.000000 django-functest-1.5.3/src/django_functest/exceptions.py
--rw-r--r--   0 luke      (1000) luke      (1000)      312 2022-12-16 13:57:47.000000 django-functest-1.5.3/src/django_functest/files.py
--rw-r--r--   0 luke      (1000) luke      (1000)    29941 2022-12-31 09:04:13.000000 django-functest-1.5.3/src/django_functest/funcselenium.py
--rw-r--r--   0 luke      (1000) luke      (1000)    14186 2022-12-16 13:57:47.000000 django-functest-1.5.3/src/django_functest/funcwebtest.py
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-16 13:57:47.000000 django-functest-1.5.3/src/django_functest/models.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1874 2022-12-31 09:04:13.000000 django-functest-1.5.3/src/django_functest/server.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.173027 django-functest-1.5.3/src/django_functest/templates/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.181027 django-functest-1.5.3/src/django_functest/templates/django_functest/
--rw-r--r--   0 luke      (1000) luke      (1000)      661 2022-12-16 13:57:47.000000 django-functest-1.5.3/src/django_functest/templates/django_functest/base.html
--rw-r--r--   0 luke      (1000) luke      (1000)     1044 2022-12-16 13:57:47.000000 django-functest-1.5.3/src/django_functest/urls.py
--rw-r--r--   0 luke      (1000) luke      (1000)     7043 2022-12-16 13:57:47.000000 django-functest-1.5.3/src/django_functest/utils.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.181027 django-functest-1.5.3/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)      471 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/conftest.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.181027 django-functest-1.5.3/tests/django_functest_tests/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/django_functest_tests/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)       88 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/django_functest_tests/admin.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2440 2022-09-12 13:44:05.000000 django-functest-1.5.3/tests/django_functest_tests/base.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.181027 django-functest-1.5.3/tests/django_functest_tests/migrations/
--rw-r--r--   0 luke      (1000) luke      (1000)     1194 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/django_functest_tests/migrations/0001_initial.py
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/django_functest_tests/migrations/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1081 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/django_functest_tests/models.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2214 2022-09-30 14:44:23.000000 django-functest-1.5.3/tests/django_functest_tests/settings.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.173027 django-functest-1.5.3/tests/django_functest_tests/templates/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-01-04 10:13:05.185027 django-functest-1.5.3/tests/django_functest_tests/templates/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)      623 2022-08-22 13:39:15.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/auto_submit_form.html
--rw-r--r--   0 luke      (1000) luke      (1000)      418 2022-09-21 13:24:07.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/delayed_appearance.html
--rw-r--r--   0 luke      (1000) luke      (1000)     2647 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/edit_thing.html
--rw-r--r--   0 luke      (1000) luke      (1000)      781 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/list_things.html
--rw-r--r--   0 luke      (1000) luke      (1000)      428 2022-12-31 09:04:13.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/long_page.html
--rw-r--r--   0 luke      (1000) luke      (1000)      150 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/new_browser_session_test.html
--rw-r--r--   0 luke      (1000) luke      (1000)     1244 2022-12-31 09:04:13.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/overflowing.html
--rw-r--r--   0 luke      (1000) luke      (1000)     1058 2022-09-01 16:02:55.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/test_misc.html
--rw-r--r--   0 luke      (1000) luke      (1000)       84 2022-08-20 16:26:04.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/thing_cleared.html
--rw-r--r--   0 luke      (1000) luke      (1000)      279 2022-09-20 13:50:46.000000 django-functest-1.5.3/tests/django_functest_tests/templates/tests/with_confirm.html
--rw-r--r--   0 luke      (1000) luke      (1000)    24418 2022-12-31 09:04:13.000000 django-functest-1.5.3/tests/django_functest_tests/test_common.py
--rw-r--r--   0 luke      (1000) luke      (1000)     7488 2022-12-31 09:04:13.000000 django-functest-1.5.3/tests/django_functest_tests/test_selenium.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4652 2022-08-22 12:02:44.000000 django-functest-1.5.3/tests/django_functest_tests/test_utils.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3705 2022-12-31 09:04:13.000000 django-functest-1.5.3/tests/django_functest_tests/urls.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5697 2022-12-31 09:04:13.000000 django-functest-1.5.3/tests/django_functest_tests/views.py
--rw-r--r--   0 luke      (1000) luke      (1000)      949 2023-01-04 10:04:42.000000 django-functest-1.5.3/tox.ini
--rwxr-xr--   0 luke      (1000) luke      (1000)      886 2022-08-20 16:26:04.000000 django-functest-1.5.3/update_migration.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.498431 django-functest-1.5.4/
+-rw-r--r--   0 luke      (1000) luke      (1000)       29 2018-03-20 11:35:06.000000 django-functest-1.5.4/.coveragerc
+-rw-r--r--   0 luke      (1000) luke      (1000)      331 2015-12-29 12:29:40.000000 django-functest-1.5.4/.editorconfig
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.482431 django-functest-1.5.4/.github/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.486431 django-functest-1.5.4/.github/workflows/
+-rw-r--r--   0 luke      (1000) luke      (1000)     2634 2023-01-04 10:04:42.000000 django-functest-1.5.4/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 luke      (1000) luke      (1000)      462 2022-08-20 16:26:04.000000 django-functest-1.5.4/.gitignore
+-rw-r--r--   0 luke      (1000) luke      (1000)     1302 2023-04-19 16:01:22.000000 django-functest-1.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)      145 2023-03-29 14:30:30.000000 django-functest-1.5.4/.readthedocs.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)      245 2016-01-08 16:37:59.000000 django-functest-1.5.4/AUTHORS.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     3506 2022-08-20 16:26:04.000000 django-functest-1.5.4/CONTRIBUTING.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     6526 2023-04-19 16:02:07.000000 django-functest-1.5.4/HISTORY.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1473 2021-01-06 18:46:53.000000 django-functest-1.5.4/LICENSE
+-rw-r--r--   0 luke      (1000) luke      (1000)      586 2022-08-22 14:20:44.000000 django-functest-1.5.4/MANIFEST.in
+-rw-rw-rw-   0 luke      (1000) luke      (1000)     7147 2023-04-19 16:03:45.498431 django-functest-1.5.4/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     5879 2022-09-30 14:44:23.000000 django-functest-1.5.4/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      634 2023-01-04 10:04:42.000000 django-functest-1.5.4/RELEASE.rst
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.486431 django-functest-1.5.4/django_functest.egg-info/
+-rw-rw-rw-   0 luke      (1000) luke      (1000)     7147 2023-04-19 16:03:45.000000 django-functest-1.5.4/django_functest.egg-info/PKG-INFO
+-rw-rw-rw-   0 luke      (1000) luke      (1000)     3427 2023-04-19 16:03:45.000000 django-functest-1.5.4/django_functest.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luke      (1000) luke      (1000)        1 2023-04-19 16:03:45.000000 django-functest-1.5.4/django_functest.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luke      (1000) luke      (1000)        1 2018-05-13 20:09:00.000000 django-functest-1.5.4/django_functest.egg-info/not-zip-safe
+-rw-rw-rw-   0 luke      (1000) luke      (1000)       85 2023-04-19 16:03:45.000000 django-functest-1.5.4/django_functest.egg-info/requires.txt
+-rw-rw-rw-   0 luke      (1000) luke      (1000)       16 2023-04-19 16:03:45.000000 django-functest-1.5.4/django_functest.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.490431 django-functest-1.5.4/docs/
+-rw-r--r--   0 luke      (1000) luke      (1000)     6778 2015-12-29 12:29:40.000000 django-functest-1.5.4/docs/Makefile
+-rw-r--r--   0 luke      (1000) luke      (1000)       28 2015-12-29 12:29:40.000000 django-functest-1.5.4/docs/authors.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     9836 2022-09-30 14:44:23.000000 django-functest-1.5.4/docs/common.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     7916 2023-04-19 16:02:34.000000 django-functest-1.5.4/docs/conf.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       33 2015-12-29 12:29:40.000000 django-functest-1.5.4/docs/contributing.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)       28 2015-12-29 12:29:40.000000 django-functest-1.5.4/docs/history.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      409 2023-04-19 16:01:22.000000 django-functest-1.5.4/docs/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     2649 2022-12-31 09:07:01.000000 django-functest-1.5.4/docs/installation.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     5955 2022-09-01 16:02:55.000000 django-functest-1.5.4/docs/interactive.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     6467 2015-12-29 12:29:40.000000 django-functest-1.5.4/docs/make.bat
+-rw-r--r--   0 luke      (1000) luke      (1000)     2569 2022-08-22 14:20:58.000000 django-functest-1.5.4/docs/pytest.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)       46 2023-03-29 14:31:36.000000 django-functest-1.5.4/docs/requirements.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)     8987 2022-12-31 09:04:13.000000 django-functest-1.5.4/docs/selenium.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1974 2023-04-19 16:01:22.000000 django-functest-1.5.4/docs/shadow_dom.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     3214 2023-01-04 13:41:23.000000 django-functest-1.5.4/docs/tips.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     6621 2022-09-30 14:44:23.000000 django-functest-1.5.4/docs/usage.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     2057 2022-09-30 14:44:23.000000 django-functest-1.5.4/docs/utils.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      409 2018-05-18 17:34:51.000000 django-functest-1.5.4/docs/webtest.rst
+-rwxr-xr--   0 luke      (1000) luke      (1000)      223 2018-03-20 05:53:16.000000 django-functest-1.5.4/download_firefox.sh
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.482431 django-functest-1.5.4/examples/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.490431 django-functest-1.5.4/examples/example_project/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.490431 django-functest-1.5.4/examples/example_project/accounts/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-22 13:54:24.000000 django-functest-1.5.4/examples/example_project/accounts/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      189 2022-08-22 13:48:00.000000 django-functest-1.5.4/examples/example_project/accounts/admin.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      148 2022-08-22 13:41:05.000000 django-functest-1.5.4/examples/example_project/accounts/apps.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.490431 django-functest-1.5.4/examples/example_project/accounts/migrations/
+-rw-r--r--   0 luke      (1000) luke      (1000)     4065 2022-08-22 13:50:13.000000 django-functest-1.5.4/examples/example_project/accounts/migrations/0001_initial.py
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-22 13:41:04.000000 django-functest-1.5.4/examples/example_project/accounts/migrations/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       89 2022-08-22 13:47:22.000000 django-functest-1.5.4/examples/example_project/accounts/models.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.490431 django-functest-1.5.4/examples/example_project/accounts/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-22 13:54:42.000000 django-functest-1.5.4/examples/example_project/accounts/tests/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      422 2022-08-22 14:19:36.000000 django-functest-1.5.4/examples/example_project/accounts/tests/base.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      951 2022-08-22 14:54:12.000000 django-functest-1.5.4/examples/example_project/accounts/tests/factories.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      422 2022-09-01 15:59:38.000000 django-functest-1.5.4/examples/example_project/accounts/tests/test_admin.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       26 2022-08-22 13:49:35.000000 django-functest-1.5.4/examples/example_project/accounts/views.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      471 2022-08-22 13:55:25.000000 django-functest-1.5.4/examples/example_project/conftest.py
+-rw-r--r--   0 luke      (1000) luke      (1000)   131072 2022-09-01 15:59:26.000000 django-functest-1.5.4/examples/example_project/db.sqlite3
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.494431 django-functest-1.5.4/examples/example_project/example_project/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-20 20:14:25.000000 django-functest-1.5.4/examples/example_project/example_project/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      407 2022-08-20 20:14:26.000000 django-functest-1.5.4/examples/example_project/example_project/asgi.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3249 2022-08-22 13:52:58.000000 django-functest-1.5.4/examples/example_project/example_project/settings.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      887 2022-08-22 14:19:36.000000 django-functest-1.5.4/examples/example_project/example_project/urls.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      407 2022-08-20 20:14:26.000000 django-functest-1.5.4/examples/example_project/example_project/wsgi.py
+-rwxr-xr--   0 luke      (1000) luke      (1000)      671 2022-08-22 13:36:41.000000 django-functest-1.5.4/examples/example_project/manage.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      116 2022-08-22 13:57:15.000000 django-functest-1.5.4/examples/example_project/pytest.ini
+-rw-r--r--   0 luke      (1000) luke      (1000)       62 2022-08-22 14:04:30.000000 django-functest-1.5.4/examples/example_project/requirements.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)      328 2023-04-19 16:01:22.000000 django-functest-1.5.4/pyproject.toml
+-rw-r--r--   0 luke      (1000) luke      (1000)      275 2022-09-12 13:44:23.000000 django-functest-1.5.4/pytest.ini
+-rwxr-xr--   0 luke      (1000) luke      (1000)      510 2023-04-19 16:01:22.000000 django-functest-1.5.4/release.sh
+-rw-r--r--   0 luke      (1000) luke      (1000)      138 2022-08-19 16:41:00.000000 django-functest-1.5.4/requirements-dev.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)     1562 2023-04-19 16:03:45.498431 django-functest-1.5.4/setup.cfg
+-rwxr-xr--   0 luke      (1000) luke      (1000)       38 2023-01-04 10:04:42.000000 django-functest-1.5.4/setup.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.482431 django-functest-1.5.4/src/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.494431 django-functest-1.5.4/src/django_functest/
+-rw-r--r--   0 luke      (1000) luke      (1000)      487 2023-04-19 16:02:24.000000 django-functest-1.5.4/src/django_functest/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5590 2022-12-16 13:57:47.000000 django-functest-1.5.4/src/django_functest/base.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      222 2022-12-16 13:57:47.000000 django-functest-1.5.4/src/django_functest/exceptions.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      312 2022-12-16 13:57:47.000000 django-functest-1.5.4/src/django_functest/files.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    30657 2023-04-19 16:01:22.000000 django-functest-1.5.4/src/django_functest/funcselenium.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    14186 2022-12-16 13:57:47.000000 django-functest-1.5.4/src/django_functest/funcwebtest.py
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-16 13:57:47.000000 django-functest-1.5.4/src/django_functest/models.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1874 2022-12-31 09:04:13.000000 django-functest-1.5.4/src/django_functest/server.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.482431 django-functest-1.5.4/src/django_functest/templates/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.494431 django-functest-1.5.4/src/django_functest/templates/django_functest/
+-rw-r--r--   0 luke      (1000) luke      (1000)      661 2022-12-16 13:57:47.000000 django-functest-1.5.4/src/django_functest/templates/django_functest/base.html
+-rw-r--r--   0 luke      (1000) luke      (1000)     1044 2022-12-16 13:57:47.000000 django-functest-1.5.4/src/django_functest/urls.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     7043 2022-12-16 13:57:47.000000 django-functest-1.5.4/src/django_functest/utils.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.494431 django-functest-1.5.4/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)      471 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/conftest.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.494431 django-functest-1.5.4/tests/django_functest_tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/django_functest_tests/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       88 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/django_functest_tests/admin.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2440 2022-09-12 13:44:05.000000 django-functest-1.5.4/tests/django_functest_tests/base.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.498431 django-functest-1.5.4/tests/django_functest_tests/migrations/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1194 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/django_functest_tests/migrations/0001_initial.py
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/django_functest_tests/migrations/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1081 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/django_functest_tests/models.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2214 2022-09-30 14:44:23.000000 django-functest-1.5.4/tests/django_functest_tests/settings.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.486431 django-functest-1.5.4/tests/django_functest_tests/templates/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-19 16:03:45.498431 django-functest-1.5.4/tests/django_functest_tests/templates/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)      623 2022-08-22 13:39:15.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/auto_submit_form.html
+-rw-r--r--   0 luke      (1000) luke      (1000)      418 2022-09-21 13:24:07.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/delayed_appearance.html
+-rw-r--r--   0 luke      (1000) luke      (1000)     2647 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/edit_thing.html
+-rw-r--r--   0 luke      (1000) luke      (1000)      781 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/list_things.html
+-rw-r--r--   0 luke      (1000) luke      (1000)      428 2022-12-31 09:04:13.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/long_page.html
+-rw-r--r--   0 luke      (1000) luke      (1000)      150 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/new_browser_session_test.html
+-rw-r--r--   0 luke      (1000) luke      (1000)     1244 2022-12-31 09:04:13.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/overflowing.html
+-rw-r--r--   0 luke      (1000) luke      (1000)     1058 2022-09-01 16:02:55.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/test_misc.html
+-rw-r--r--   0 luke      (1000) luke      (1000)       84 2022-08-20 16:26:04.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/thing_cleared.html
+-rw-r--r--   0 luke      (1000) luke      (1000)     3435 2023-04-19 16:01:22.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/web_components.html
+-rw-r--r--   0 luke      (1000) luke      (1000)      279 2022-09-20 13:50:46.000000 django-functest-1.5.4/tests/django_functest_tests/templates/tests/with_confirm.html
+-rw-r--r--   0 luke      (1000) luke      (1000)    24418 2022-12-31 09:04:13.000000 django-functest-1.5.4/tests/django_functest_tests/test_common.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     9545 2023-04-19 16:01:22.000000 django-functest-1.5.4/tests/django_functest_tests/test_selenium.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4652 2022-08-22 12:02:44.000000 django-functest-1.5.4/tests/django_functest_tests/test_utils.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1414 2023-04-19 16:01:22.000000 django-functest-1.5.4/tests/django_functest_tests/urls.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5788 2023-04-19 16:01:22.000000 django-functest-1.5.4/tests/django_functest_tests/views.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      949 2023-01-04 10:04:42.000000 django-functest-1.5.4/tox.ini
+-rwxr-xr--   0 luke      (1000) luke      (1000)      886 2022-08-20 16:26:04.000000 django-functest-1.5.4/update_migration.py
```

### Comparing `django-functest-1.5.3/.github/workflows/pythonpackage.yml` & `django-functest-1.5.4/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/.pre-commit-config.yaml` & `django-functest-1.5.4/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -43,11 +43,7 @@
       - id: autopep8
         language_version: python3.9
   - repo: 'https://github.com/psf/black'
     rev: 22.6.0
     hooks:
       - id: black
         language_version: python3.9
-  - repo: https://github.com/mgedmin/check-manifest
-    rev: "0.47"
-    hooks:
-      - id: check-manifest
```

### Comparing `django-functest-1.5.3/CONTRIBUTING.rst` & `django-functest-1.5.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/HISTORY.rst` & `django-functest-1.5.4/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+1.5.4 (2023-04-19)
+++++++++++++++++++
+
+* Added some support for :doc:`shadow_dom`.
+
 1.5.3 (2023-01-04)
 ++++++++++++++++++
 
 * Added a more robust scroll method based on `Element.scrollIntoView
   <https://developer.mozilla.org/en-US/docs/Web/API/Element/scrollIntoView>`_.
   The old method can be used instead by setting ``scroll_method =
   "legacyWindowScrollTo"`` on a test case.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_qua7cgp7_/tmpea8elx8w_TarContainer/0/11.rst", line 224, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_qua7cgp7_/tmpea8elx8w_TarContainer/0/11.rst", line 224, column 0: CDATA terminal not found*

```diff
@@ -1,9 +1,10 @@
-.. :changelog: History ------- 1.5.3 (2023-01-04) ++++++++++++++++++ * Added a
-more robust scroll method based on `Element.scrollIntoView
+.. :changelog: History ------- 1.5.4 (2023-04-19) ++++++++++++++++++ * Added
+some support for :doc:`shadow_dom`. 1.5.3 (2023-01-04) ++++++++++++++++++ *
+Added a more robust scroll method based on `Element.scrollIntoView
 developer.mozilla.org/en-US/docs/Web/API/Element/scrollIntoView>`_. The old
 method can be used instead by setting ``scroll_method =
 "legacyWindowScrollTo"`` on a test case. 1.5.2 (2022-09-21) ++++++++++++++++++
 * Added ``expect_alert`` to :meth:`~django_functest.FuncSeleniumMixin.click`,
 plus :meth:`~django_functest.FuncSeleniumMixin.accept_alert` and :meth:
 `~django_functest.FuncSeleniumMixin.dismiss_alert` * Added ``assertion_passes``
 utility as a convenience for using with :meth:
```

### Comparing `django-functest-1.5.3/LICENSE` & `django-functest-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/MANIFEST.in` & `django-functest-1.5.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/PKG-INFO` & `django-functest-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-functest
-Version: 1.5.3
+Version: 1.5.4
 Summary: Helpers for creating functional tests in Django, with a unified API for WebTest and Selenium tests.
 Home-page: https://github.com/django-functest/django-functest
 Author: Luke Plant
 Author-email: L.Plant.98@cantab.net
 License: BSD
 Keywords: django-functest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-functest-1.5.3/README.rst` & `django-functest-1.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/RELEASE.rst` & `django-functest-1.5.4/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/django_functest.egg-info/PKG-INFO` & `django-functest-1.5.4/django_functest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-functest
-Version: 1.5.3
+Version: 1.5.4
 Summary: Helpers for creating functional tests in Django, with a unified API for WebTest and Selenium tests.
 Home-page: https://github.com/django-functest/django-functest
 Author: Luke Plant
 Author-email: L.Plant.98@cantab.net
 License: BSD
 Keywords: django-functest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-functest-1.5.3/django_functest.egg-info/SOURCES.txt` & `django-functest-1.5.4/django_functest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 docs/index.rst
 docs/installation.rst
 docs/interactive.rst
 docs/make.bat
 docs/pytest.rst
 docs/requirements.txt
 docs/selenium.rst
+docs/shadow_dom.rst
 docs/tips.rst
 docs/usage.rst
 docs/utils.rst
 docs/webtest.rst
 examples/example_project/conftest.py
 examples/example_project/db.sqlite3
 examples/example_project/manage.py
@@ -93,8 +94,9 @@
 tests/django_functest_tests/templates/tests/edit_thing.html
 tests/django_functest_tests/templates/tests/list_things.html
 tests/django_functest_tests/templates/tests/long_page.html
 tests/django_functest_tests/templates/tests/new_browser_session_test.html
 tests/django_functest_tests/templates/tests/overflowing.html
 tests/django_functest_tests/templates/tests/test_misc.html
 tests/django_functest_tests/templates/tests/thing_cleared.html
+tests/django_functest_tests/templates/tests/web_components.html
 tests/django_functest_tests/templates/tests/with_confirm.html
```

### Comparing `django-functest-1.5.3/docs/Makefile` & `django-functest-1.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/docs/common.rst` & `django-functest-1.5.4/docs/common.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/docs/conf.py` & `django-functest-1.5.4/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = "1.5"
 # The full version, including alpha/beta/rc tags.
-release = "1.5.3"
+release = "1.5.4"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `django-functest-1.5.3/docs/installation.rst` & `django-functest-1.5.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/docs/interactive.rst` & `django-functest-1.5.4/docs/interactive.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/docs/make.bat` & `django-functest-1.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/docs/pytest.rst` & `django-functest-1.5.4/docs/pytest.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/docs/selenium.rst` & `django-functest-1.5.4/docs/selenium.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/docs/tips.rst` & `django-functest-1.5.4/docs/tips.rst`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 built in. When this is not sufficient, however, it’s tempting do a bit of::
 
   import time
 
   time.sleep(0.2)  # Should be enough…
 
 
-This works great until you run the test on CI or on a busy machine and it take
+This works great until you run the test on CI or on a busy machine and it takes
 205ms instead of 200ms. You don’t really want to add 10 second delay to be
 **really** sure, so you end with a flaky test suite that fails randomly, and
 life is miserable.
 
 Instead, use :meth:`~django_functest.FuncSeleniumMixin.wait_until` to wait for
 the thing you are expecting. For example, to wait for some text to appear on the
 page::
@@ -36,14 +36,19 @@
 
     self.wait_until(lambda *args: MyModel.objects.filter(text="Updated").exists())
 
 If these fail, they fail with a timeout, which means they wait a long time
 before failing. This is a bit annoying, but it’s usually better than the
 alternative.
 
+Some of the builtin positive assertions automatically insert waits for you — for
+example meth:`~django_functest.FuncCommonApi.assertTextPresent` will
+automatically wait for the specified element (``body`` by default) to be
+present.
+
 
 Use FuncBaseMixin
 -----------------
 
 In the above example, ``FuncBaseMixin`` is not strictly needed at all — it
 provides method definitions which all raise ``NotImplementedError`` — so you
 could remove it. However, it can be very useful for editors that provide code
```

### Comparing `django-functest-1.5.3/docs/usage.rst` & `django-functest-1.5.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/docs/utils.rst` & `django-functest-1.5.4/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/examples/example_project/accounts/migrations/0001_initial.py` & `django-functest-1.5.4/examples/example_project/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/examples/example_project/accounts/tests/factories.py` & `django-functest-1.5.4/examples/example_project/accounts/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/examples/example_project/db.sqlite3` & `django-functest-1.5.4/examples/example_project/db.sqlite3`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/examples/example_project/example_project/settings.py` & `django-functest-1.5.4/examples/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/examples/example_project/example_project/urls.py` & `django-functest-1.5.4/examples/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/examples/example_project/manage.py` & `django-functest-1.5.4/examples/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/setup.cfg` & `django-functest-1.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/src/django_functest/base.py` & `django-functest-1.5.4/src/django_functest/base.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/src/django_functest/funcselenium.py` & `django-functest-1.5.4/src/django_functest/funcselenium.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from django.conf import settings
 from pyquery import PyQuery
 from selenium import webdriver
 from selenium.common.exceptions import NoSuchElementException, NoSuchWindowException, StaleElementReferenceException
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
+from selenium.webdriver.remote.command import Command
 from selenium.webdriver.support.ui import Select, WebDriverWait
 
 from .base import FuncBaseMixin
 from .exceptions import SeleniumCantUseElement
 from .utils import BrowserSessionToken, CommonMixin, NotPassed, get_session_store
 
 try:
@@ -114,26 +115,26 @@
 
     def get_element_attribute(self, css_selector, attribute):
         """
         Returns the value of the attribute of the element matching the css_selector,
         or None if there is no such element or attribute.
         """
         try:
-            element = self._driver.find_element(By.CSS_SELECTOR, css_selector)
+            element = self._find(css_selector=css_selector)
         except NoSuchElementException:
             return None
         return element.get_dom_attribute(attribute)
 
     def get_element_inner_text(self, css_selector):
         """
         Returns the "inner text" (innerText in JS) of the element matching
         the css_selector, or None if there is none.
         """
         try:
-            element = self._driver.find_element(By.CSS_SELECTOR, css_selector)
+            element = self._find(css_selector=css_selector)
         except NoSuchElementException:
             return None
         return element.text
 
     def get_url(self, name, *args, **kwargs):
         """
         Gets the named URL, passing *args and **kwargs to Django's URL 'reverse' function.
@@ -152,15 +153,15 @@
 
     def is_element_present(self, css_selector):
         """
         Returns True if the element specified by the CSS selector is present on the current page,
         False otherwise.
         """
         try:
-            self._driver.find_element(By.CSS_SELECTOR, css_selector)
+            self._find(css_selector)
         except NoSuchElementException:
             return False
         return True
 
     @property
     def is_full_browser_test(self):
         """
@@ -376,15 +377,15 @@
 
     def is_element_displayed(self, css_selector):
         """
         Returns True if the element specified by the CSS selector is both
         present and visible on the page.
         """
         try:
-            elem = self._driver.find_element(By.CSS_SELECTOR, css_selector)
+            elem = self._find(css_selector=css_selector)
         except NoSuchElementException:
             return False
         return elem.is_displayed()
 
     def new_browser_session(self):
         """
         Creates (and switches to) a new session that is separate from previous
@@ -563,16 +564,24 @@
     def _driver(self):
         if self._instance_drivers:
             return self._instance_drivers[0]
         else:
             return self._cls_driver
 
     def _get_finder(self, css_selector=None, xpath=None, text=None, text_parent_id=None):
+        def _find_by_css(driver):
+            css_selectors = [css_selector] if isinstance(css_selector, str) else list(css_selector)
+            first_selector, *remaining_selectors = css_selectors
+            element = driver.find_element(By.CSS_SELECTOR, first_selector)
+            for selector in remaining_selectors:
+                element = _get_shadow_root(element).find_element(By.CSS_SELECTOR, selector)
+            return element
+
         if css_selector is not None:
-            return lambda driver: driver.find_element(By.CSS_SELECTOR, css_selector)
+            return _find_by_css
         if xpath is not None:
             return lambda driver: driver.find_element(By.XPATH, xpath)
         if text is not None:
             if text_parent_id is not None:
                 prefix = f'//*[@id="{text_parent_id}"]'
             else:
                 prefix = ""
@@ -836,7 +845,14 @@
         if not isinstance(possibly_text, str):
             return possibly_text
         text = possibly_text
         # If you send \r\n to Firefox, it enters 2 line breaks (at least on
         # Linux)
         text = text.replace("\r\n", "\n")
         return text
+
+
+def _get_shadow_root(element):
+    # Workaround the fact that `element.shadow_root` throws assertion error for Firefox.
+    # (finding elements still doesn't work at time of writing, but we don't want to wait
+    # for a Selenium release to get this fixed, when a geckodriver release may fix it).
+    return element._execute(Command.GET_SHADOW_ROOT)["value"]
```

### Comparing `django-functest-1.5.3/src/django_functest/funcwebtest.py` & `django-functest-1.5.4/src/django_functest/funcwebtest.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/src/django_functest/server.py` & `django-functest-1.5.4/src/django_functest/server.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/src/django_functest/templates/django_functest/base.html` & `django-functest-1.5.4/src/django_functest/templates/django_functest/base.html`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/src/django_functest/urls.py` & `django-functest-1.5.4/src/django_functest/urls.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/src/django_functest/utils.py` & `django-functest-1.5.4/src/django_functest/utils.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/base.py` & `django-functest-1.5.4/tests/django_functest_tests/base.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/migrations/0001_initial.py` & `django-functest-1.5.4/tests/django_functest_tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/models.py` & `django-functest-1.5.4/tests/django_functest_tests/models.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/settings.py` & `django-functest-1.5.4/tests/django_functest_tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/templates/tests/auto_submit_form.html` & `django-functest-1.5.4/tests/django_functest_tests/templates/tests/auto_submit_form.html`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/templates/tests/edit_thing.html` & `django-functest-1.5.4/tests/django_functest_tests/templates/tests/edit_thing.html`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/templates/tests/list_things.html` & `django-functest-1.5.4/tests/django_functest_tests/templates/tests/list_things.html`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/templates/tests/overflowing.html` & `django-functest-1.5.4/tests/django_functest_tests/templates/tests/overflowing.html`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/templates/tests/test_misc.html` & `django-functest-1.5.4/tests/django_functest_tests/templates/tests/test_misc.html`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/test_common.py` & `django-functest-1.5.4/tests/django_functest_tests/test_common.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/test_utils.py` & `django-functest-1.5.4/tests/django_functest_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/tests/django_functest_tests/views.py` & `django-functest-1.5.4/tests/django_functest_tests/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,7 +209,11 @@
             "item": item,
         },
     )
 
 
 def with_confirm(request):
     return render(request, "tests/with_confirm.html", {})
+
+
+def web_components(request):
+    return render(request, "tests/web_components.html", {})
```

### Comparing `django-functest-1.5.3/tox.ini` & `django-functest-1.5.4/tox.ini`

 * *Files identical despite different names*

### Comparing `django-functest-1.5.3/update_migration.py` & `django-functest-1.5.4/update_migration.py`

 * *Files identical despite different names*

