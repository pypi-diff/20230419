# Comparing `tmp/edx-proctoring-4.8.4.tar.gz` & `tmp/edx-proctoring-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-proctoring-4.8.4.tar", last modified: Wed Jan 12 22:08:54 2022, max compression
+gzip compressed data, was "edx-proctoring-4.9.0.tar", last modified: Mon Feb  7 12:43:06 2022, max compression
```

## Comparing `edx-proctoring-4.8.4.tar` & `edx-proctoring-4.9.0.tar`

### file list

```diff
@@ -1,383 +1,383 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.498170 edx-proctoring-4.8.4/
--rw-r--r--   0 runner    (1001) docker     (121)    28405 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35119 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    39094 2022-01-12 22:08:54.498170 edx-proctoring-4.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2927 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.470169 edx-proctoring-4.8.4/edx_proctoring/
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15480 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)   123785 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5394 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.470169 edx-proctoring-4.8.4/edx_proctoring/backends/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4559 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     3808 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/mock.py
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/null.py
--rw-r--r--   0 runner    (1001) docker     (121)    14526 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/rest.py
--rw-r--r--   0 runner    (1001) docker     (121)    15041 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/software_secure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.470169 edx-proctoring-4.8.4/edx_proctoring/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11938 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)    19434 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3655 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/tests/test_review_payload.py
--rw-r--r--   0 runner    (1001) docker     (121)    23066 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/backends/tests/test_software_secure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9727 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/instructor_dashboard_exam_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.470169 edx-proctoring-4.8.4/edx_proctoring/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.462169 edx-proctoring-4.8.4/edx_proctoring/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.470169 edx-proctoring-4.8.4/edx_proctoring/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    13931 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    42698 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    13818 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    42531 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.462169 edx-proctoring-4.8.4/edx_proctoring/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.474169 edx-proctoring-4.8.4/edx_proctoring/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    12871 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    41586 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    12829 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ca/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    41502 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ca/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.462169 edx-proctoring-4.8.4/edx_proctoring/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.474169 edx-proctoring-4.8.4/edx_proctoring/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35799 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35799 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.462169 edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.474169 edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    13214 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    41944 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    13093 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    41898 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.462169 edx-proctoring-4.8.4/edx_proctoring/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.474169 edx-proctoring-4.8.4/edx_proctoring/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36210 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35906 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.462169 edx-proctoring-4.8.4/edx_proctoring/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.474169 edx-proctoring-4.8.4/edx_proctoring/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    34930 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     7979 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.462169 edx-proctoring-4.8.4/edx_proctoring/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.474169 edx-proctoring-4.8.4/edx_proctoring/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    80878 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    93640 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     9570 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    13886 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.462169 edx-proctoring-4.8.4/edx_proctoring/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.474169 edx-proctoring-4.8.4/edx_proctoring/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    43192 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/es_419/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    56988 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/es_419/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    43246 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/es_419/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    57048 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/es_419/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.474169 edx-proctoring-4.8.4/edx_proctoring/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/es_AR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35627 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/es_AR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.478169 edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35895 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35894 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.478169 edx-proctoring-4.8.4/edx_proctoring/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    44534 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    58507 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    44462 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    58437 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.478169 edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    44609 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    58256 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    44601 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    58252 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.478169 edx-proctoring-4.8.4/edx_proctoring/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    13283 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    41960 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    13208 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    41883 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.478169 edx-proctoring-4.8.4/edx_proctoring/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36885 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/id/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36916 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/id/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.478169 edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    41461 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    55990 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    41492 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    56021 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.478169 edx-proctoring-4.8.4/edx_proctoring/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ja_JP/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35978 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ja_JP/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.478169 edx-proctoring-4.8.4/edx_proctoring/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36069 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ka/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ka/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36069 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ka/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.478169 edx-proctoring-4.8.4/edx_proctoring/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35731 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/lv/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35731 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/lv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.482169 edx-proctoring-4.8.4/edx_proctoring/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35608 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/mn/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35737 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.482169 edx-proctoring-4.8.4/edx_proctoring/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36835 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36835 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.482169 edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    42287 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    56442 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    25251 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    48122 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.482169 edx-proctoring-4.8.4/edx_proctoring/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35837 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    35837 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.482169 edx-proctoring-4.8.4/edx_proctoring/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    15496 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    44127 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    15505 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    44216 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.482169 edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    12288 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    41057 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    12381 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    41154 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.482169 edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    14798 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    42523 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    14777 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    42549 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.482169 edx-proctoring-4.8.4/edx_proctoring/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36322 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    36322 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.486169 edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    11440 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    40342 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)    11432 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)    40376 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.486169 edx-proctoring-4.8.4/edx_proctoring/management/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.486169 edx-proctoring-4.8.4/edx_proctoring/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/set_attempt_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/set_is_attempt_active.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.486169 edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/test_set_attempt_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/test_set_is_attempt_active.py
--rw-r--r--   0 runner    (1001) docker     (121)     4551 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/test_update_attempt_status_from_review.py
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/test_update_attempts_for_exam.py
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/update_attempt_status_from_review.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/management/commands/update_attempts_for_exam.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.486169 edx-proctoring-4.8.4/edx_proctoring/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    13980 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0002_proctoredexamstudentattempt_is_status_acknowledged.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0003_auto_20160101_0525.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0004_auto_20160201_0523.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0005_proctoredexam_hide_after_due.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0006_allowed_time_limit_mins.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0007_proctoredexam_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0008_auto_20181116_1551.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0009_proctoredexamreviewpolicy_remove_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0010_update_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0011_allow_multiple_attempts.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0012_proctoredexamstudentattempt_time_remaining_seconds.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0013_proctoredexamsoftwaresecurereview_is_active_attempt.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0014_add_is_resumable_to_proctoredexamstudentattempt.py
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0015_rm_proctoredexamstudentattempt_ips.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0016_nullable_proctoredexamstudentattempt_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0017_rm_proctoredexamstudentattempt_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0018_historicalproctoredexamstudentattempt.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0019_proctoredexamsoftwaresecurereview_encrypted_video_url.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0020_auto_20211028_1915.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0021_auto_20211029_1353.py
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0022_proctoredexamstudentattempt_add_readytoresume_resumed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0023_historicalproctoredexam.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/0024_delete_proctoredexamstudentattempthistory.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30677 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/rules.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.490169 edx-proctoring-4.8.4/edx_proctoring/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/scripts/obscure_user.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      533 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/scripts/version_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     4130 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.490169 edx-proctoring-4.8.4/edx_proctoring/settings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.490169 edx-proctoring-4.8.4/edx_proctoring/static/
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/index.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.490169 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/
--rw-r--r--   0 runner    (1001) docker     (121)     5380 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/clippy.swf
--rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/close-modal-hover.png
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/close-modal.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.490169 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.490169 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/collections/
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/collections/proctored_exam_allowance_collection.js
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/collections/proctored_exam_attempt_grouped_collection.js
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/collections/proctored_exam_collection.js
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/collections/proctored_exam_onboarding_collection.js
--rw-r--r--   0 runner    (1001) docker     (121)     3891 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/dropdown.js
--rw-r--r--   0 runner    (1001) docker     (121)     9561 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/exam_action_handler.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.490169 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/learner_onboarding_model.js
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/proctored_exam_allowance_model.js
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/proctored_exam_attempt_model.js
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/proctored_exam_bulk_allowance_model.js
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/proctored_exam_model.js
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/proctored_app.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.490169 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (121)    60997 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/backbone.js
--rw-r--r--   0 runner    (1001) docker     (121)    30637 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/date.js
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/i18n.js
--rw-r--r--   0 runner    (1001) docker     (121)    95931 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/jquery.js
--rw-r--r--   0 runner    (1001) docker     (121)    47632 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.490169 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/
--rw-r--r--   0 runner    (1001) docker     (121)    14348 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/Backbone.ModalDialog.js
--rw-r--r--   0 runner    (1001) docker     (121)    12066 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_add_bulk_allowance_view.js
--rw-r--r--   0 runner    (1001) docker     (121)     8929 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_allowance_view.js
--rw-r--r--   0 runner    (1001) docker     (121)    13278 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_attempt_view.js
--rw-r--r--   0 runner    (1001) docker     (121)     6439 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_edit_allowance_view.js
--rw-r--r--   0 runner    (1001) docker     (121)     8086 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_info.js
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_instructor_launch.js
--rw-r--r--   0 runner    (1001) docker     (121)    11511 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_onboarding_view.js
--rw-r--r--   0 runner    (1001) docker     (121)    12957 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_view.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.494169 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     3440 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/add-new-bulk-allowance.underscore
--rw-r--r--   0 runner    (1001) docker     (121)     3984 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/course_grouped_allowances.underscore
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/dashboard.underscore
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/edit-allowance.underscore
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/proctored-exam-info.underscore
--rw-r--r--   0 runner    (1001) docker     (121)     6697 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/student-onboarding-status.underscore
--rw-r--r--   0 runner    (1001) docker     (121)    14892 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/student-proctored-exam-attempts-grouped.underscore
--rw-r--r--   0 runner    (1001) docker     (121)    11088 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/statuses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.466169 edx-proctoring-4.8.4/edx_proctoring/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.494169 edx-proctoring-4.8.4/edx_proctoring/templates/common/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/common/waiting_banner.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.494169 edx-proctoring-4.8.4/edx_proctoring/templates/emails/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/emails/proctoring_attempt_satisfactory_email.html
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/emails/proctoring_attempt_submitted_email.html
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/emails/proctoring_attempt_unsatisfactory_email.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.494169 edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/entrance.html
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/error.html
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/ready_to_submit.html
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/rejected.html
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/submitted.html
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/verified.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.494169 edx-proctoring-4.8.4/edx_proctoring/templates/practice_exam/
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/practice_exam/entrance.html
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/practice_exam/error.html
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/practice_exam/submitted.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.494169 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/confirm-decline.html
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/entrance.html
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/error.html
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/error_modal.html
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/error_wrong_browser.html
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/expired.html
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/failed-prerequisites.html
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/id_verification.html
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/inactive_account.html
--rw-r--r--   0 runner    (1001) docker     (121)     7991 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/instructions.html
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/onboarding_error.html
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/pending-prerequisites.html
--rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/proctoring_launch_callback.html
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/proctoring_opt_out_button.html
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/ready_to_resume.html
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/ready_to_start.html
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/ready_to_submit.html
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/rejected.html
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/submitted.html
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/verified.html
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/visit_exam_content.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.498170 edx-proctoring-4.8.4/edx_proctoring/templates/timed_exam/
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/timed_exam/entrance.html
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/timed_exam/expired.html
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/timed_exam/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/timed_exam/ready_to_submit.html
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/templates/timed_exam/submitted.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.498170 edx-proctoring-4.8.4/edx_proctoring/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   145631 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    12024 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_email.py
--rw-r--r--   0 runner    (1001) docker     (121)     2522 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)    20452 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_mfe_views.py
--rw-r--r--   0 runner    (1001) docker     (121)    17666 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    25312 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_reviews.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)    14311 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (121)    67863 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_student_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     6759 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)   240974 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/test_workerconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)    13102 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6092 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    16976 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    86821 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/edx_proctoring/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.470169 edx-proctoring-4.8.4/edx_proctoring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    39094 2022-01-12 22:08:54.000000 edx-proctoring-4.8.4/edx_proctoring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14818 2022-01-12 22:08:54.000000 edx-proctoring-4.8.4/edx_proctoring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 22:08:54.000000 edx-proctoring-4.8.4/edx_proctoring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-01-12 22:08:54.000000 edx-proctoring-4.8.4/edx_proctoring.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 22:08:54.000000 edx-proctoring-4.8.4/edx_proctoring.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-01-12 22:08:54.000000 edx-proctoring-4.8.4/edx_proctoring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-12 22:08:54.000000 edx-proctoring-4.8.4/edx_proctoring.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 22:08:54.498170 edx-proctoring-4.8.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/celery50.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/common_constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/quality.in
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/quality.txt
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (121)     5921 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-01-12 22:08:54.502169 edx-proctoring-4.8.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3291 2022-01-12 22:08:50.000000 edx-proctoring-4.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.628728 edx-proctoring-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    28507 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    35119 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    39158 2022-02-07 12:43:06.628728 edx-proctoring-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2927 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.600728 edx-proctoring-4.9.0/edx_proctoring/
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15480 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)   123785 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5394 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.600728 edx-proctoring-4.9.0/edx_proctoring/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4559 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3808 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/mock.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/null.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14526 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/rest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15041 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/software_secure.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.600728 edx-proctoring-4.9.0/edx_proctoring/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11938 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19434 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3655 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/tests/test_review_payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23066 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/backends/tests/test_software_secure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9727 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/instructor_dashboard_exam_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.600728 edx-proctoring-4.9.0/edx_proctoring/locale/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.600728 edx-proctoring-4.9.0/edx_proctoring/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    13931 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    42698 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13818 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    42531 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.600728 edx-proctoring-4.9.0/edx_proctoring/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    12871 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    41586 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12829 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ca/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    41502 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ca/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.604728 edx-proctoring-4.9.0/edx_proctoring/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35799 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35799 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/cs/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.604728 edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    13214 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    41944 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13093 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    41898 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.604728 edx-proctoring-4.9.0/edx_proctoring/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36210 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35906 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.604728 edx-proctoring-4.9.0/edx_proctoring/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    34930 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     7979 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.604728 edx-proctoring-4.9.0/edx_proctoring/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    80878 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    93640 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)     9570 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    13886 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.604728 edx-proctoring-4.9.0/edx_proctoring/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    43192 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    56988 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    43246 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/es_419/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    57048 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/es_419/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.604728 edx-proctoring-4.9.0/edx_proctoring/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/es_AR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35627 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/es_AR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.604728 edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35895 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35894 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.604728 edx-proctoring-4.9.0/edx_proctoring/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    44570 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    58518 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    44462 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    58437 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.608728 edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    44609 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    58256 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    44601 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    58252 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.608728 edx-proctoring-4.9.0/edx_proctoring/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    13283 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    41960 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    13208 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    41883 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.608728 edx-proctoring-4.9.0/edx_proctoring/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36885 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/id/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36916 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/id/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.608728 edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    41461 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    55990 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    41492 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    56021 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.608728 edx-proctoring-4.9.0/edx_proctoring/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ja_JP/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35978 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ja_JP/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.608728 edx-proctoring-4.9.0/edx_proctoring/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36069 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ka/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ka/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36069 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ka/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.608728 edx-proctoring-4.9.0/edx_proctoring/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35731 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/lv/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35731 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/lv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.608728 edx-proctoring-4.9.0/edx_proctoring/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35608 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/mn/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35737 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.608728 edx-proctoring-4.9.0/edx_proctoring/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     3497 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36835 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)     3497 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36835 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.612728 edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    42287 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    56442 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    25251 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    48122 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.612728 edx-proctoring-4.9.0/edx_proctoring/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35837 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    35837 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.612728 edx-proctoring-4.9.0/edx_proctoring/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    15496 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    44127 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    15505 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    44216 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.612728 edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    12288 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    41057 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    12381 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    41154 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.612728 edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    14798 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    42523 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    14777 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    42549 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.592728 edx-proctoring-4.9.0/edx_proctoring/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.612728 edx-proctoring-4.9.0/edx_proctoring/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36322 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    36322 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.596728 edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.612728 edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    11440 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    40342 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)    11432 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    40376 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.612728 edx-proctoring-4.9.0/edx_proctoring/management/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.612728 edx-proctoring-4.9.0/edx_proctoring/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/set_attempt_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/set_is_attempt_active.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.616728 edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/test_set_attempt_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/test_set_is_attempt_active.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4551 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/test_update_attempt_status_from_review.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/test_update_attempts_for_exam.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/update_attempt_status_from_review.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/management/commands/update_attempts_for_exam.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.616728 edx-proctoring-4.9.0/edx_proctoring/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)    13980 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0002_proctoredexamstudentattempt_is_status_acknowledged.py
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0003_auto_20160101_0525.py
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0004_auto_20160201_0523.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0005_proctoredexam_hide_after_due.py
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0006_allowed_time_limit_mins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0007_proctoredexam_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0008_auto_20181116_1551.py
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0009_proctoredexamreviewpolicy_remove_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0010_update_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0011_allow_multiple_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0012_proctoredexamstudentattempt_time_remaining_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0013_proctoredexamsoftwaresecurereview_is_active_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      672 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0014_add_is_resumable_to_proctoredexamstudentattempt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0015_rm_proctoredexamstudentattempt_ips.py
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0016_nullable_proctoredexamstudentattempt_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0017_rm_proctoredexamstudentattempt_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0018_historicalproctoredexamstudentattempt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0019_proctoredexamsoftwaresecurereview_encrypted_video_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0020_auto_20211028_1915.py
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0021_auto_20211029_1353.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0022_proctoredexamstudentattempt_add_readytoresume_resumed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0023_historicalproctoredexam.py
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/0024_delete_proctoredexamstudentattempthistory.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30677 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.616728 edx-proctoring-4.9.0/edx_proctoring/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/scripts/obscure_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      533 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/scripts/version_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4130 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/services.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.616728 edx-proctoring-4.9.0/edx_proctoring/settings/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.616728 edx-proctoring-4.9.0/edx_proctoring/static/
+-rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/index.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.616728 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/
+-rw-r--r--   0 runner    (1001) docker     (121)     5380 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/clippy.swf
+-rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/close-modal-hover.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/close-modal.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.616728 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.616728 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/collections/
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/collections/proctored_exam_allowance_collection.js
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/collections/proctored_exam_attempt_grouped_collection.js
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/collections/proctored_exam_collection.js
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/collections/proctored_exam_onboarding_collection.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3891 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/dropdown.js
+-rw-r--r--   0 runner    (1001) docker     (121)     9561 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/exam_action_handler.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.620728 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/learner_onboarding_model.js
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/proctored_exam_allowance_model.js
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/proctored_exam_attempt_model.js
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/proctored_exam_bulk_allowance_model.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/proctored_exam_model.js
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/proctored_app.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.620728 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (121)    60997 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/backbone.js
+-rw-r--r--   0 runner    (1001) docker     (121)    30637 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/date.js
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/i18n.js
+-rw-r--r--   0 runner    (1001) docker     (121)    95931 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (121)    47632 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.620728 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/
+-rw-r--r--   0 runner    (1001) docker     (121)    14348 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/Backbone.ModalDialog.js
+-rw-r--r--   0 runner    (1001) docker     (121)    12066 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_add_bulk_allowance_view.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8929 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_allowance_view.js
+-rw-r--r--   0 runner    (1001) docker     (121)    13278 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_attempt_view.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6439 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_edit_allowance_view.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8086 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_info.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_instructor_launch.js
+-rw-r--r--   0 runner    (1001) docker     (121)    11511 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_onboarding_view.js
+-rw-r--r--   0 runner    (1001) docker     (121)    12957 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_view.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.620728 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     3440 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/add-new-bulk-allowance.underscore
+-rw-r--r--   0 runner    (1001) docker     (121)     3984 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/course_grouped_allowances.underscore
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/dashboard.underscore
+-rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/edit-allowance.underscore
+-rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/proctored-exam-info.underscore
+-rw-r--r--   0 runner    (1001) docker     (121)     6697 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/student-onboarding-status.underscore
+-rw-r--r--   0 runner    (1001) docker     (121)    14892 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/student-proctored-exam-attempts-grouped.underscore
+-rw-r--r--   0 runner    (1001) docker     (121)    11088 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/statuses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.596728 edx-proctoring-4.9.0/edx_proctoring/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.620728 edx-proctoring-4.9.0/edx_proctoring/templates/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/common/waiting_banner.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.620728 edx-proctoring-4.9.0/edx_proctoring/templates/emails/
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/emails/proctoring_attempt_satisfactory_email.html
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/emails/proctoring_attempt_submitted_email.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/emails/proctoring_attempt_unsatisfactory_email.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.620728 edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/
+-rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/entrance.html
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/error.html
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/ready_to_submit.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/rejected.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/submitted.html
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/verified.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.620728 edx-proctoring-4.9.0/edx_proctoring/templates/practice_exam/
+-rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/practice_exam/entrance.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/practice_exam/error.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/practice_exam/submitted.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.624728 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/confirm-decline.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/entrance.html
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/error.html
+-rw-r--r--   0 runner    (1001) docker     (121)      941 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/error_modal.html
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/error_wrong_browser.html
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/expired.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/failed-prerequisites.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/footer.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/id_verification.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/inactive_account.html
+-rw-r--r--   0 runner    (1001) docker     (121)     7991 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/onboarding_error.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/pending-prerequisites.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/proctoring_launch_callback.html
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/proctoring_opt_out_button.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/ready_to_resume.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/ready_to_start.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/ready_to_submit.html
+-rw-r--r--   0 runner    (1001) docker     (121)      905 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/rejected.html
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/submitted.html
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/verified.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/visit_exam_content.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.624728 edx-proctoring-4.9.0/edx_proctoring/templates/timed_exam/
+-rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/timed_exam/entrance.html
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/timed_exam/expired.html
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/timed_exam/footer.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/timed_exam/ready_to_submit.html
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/templates/timed_exam/submitted.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.628728 edx-proctoring-4.9.0/edx_proctoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   145631 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12024 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2522 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20452 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_mfe_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17666 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25312 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_reviews.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14311 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67863 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_student_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6759 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)   240974 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/test_workerconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13102 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6092 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16976 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    86821 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/edx_proctoring/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.600728 edx-proctoring-4.9.0/edx_proctoring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    39158 2022-02-07 12:43:06.000000 edx-proctoring-4.9.0/edx_proctoring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14818 2022-02-07 12:43:06.000000 edx-proctoring-4.9.0/edx_proctoring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 12:43:06.000000 edx-proctoring-4.9.0/edx_proctoring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-02-07 12:43:06.000000 edx-proctoring-4.9.0/edx_proctoring.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 12:43:06.000000 edx-proctoring-4.9.0/edx_proctoring.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-02-07 12:43:06.000000 edx-proctoring-4.9.0/edx_proctoring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-02-07 12:43:06.000000 edx-proctoring-4.9.0/edx_proctoring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:43:06.628728 edx-proctoring-4.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/celery50.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/common_constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/quality.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/quality.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5921 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2022-02-07 12:43:06.628728 edx-proctoring-4.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3215 2022-02-07 12:43:04.000000 edx-proctoring-4.9.0/setup.py
```

### Comparing `edx-proctoring-4.8.4/CHANGELOG.rst` & `edx-proctoring-4.9.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[4.9.0] - 2022-01-25
+~~~~~~~~~~~~~~~~~~~~
+* Dropped Django22, 30 and 31
+* Added Support for Django40
+
 [4.8.4] - 2022-01-12
 ~~~~~~~~~~~~~~~~~~~~
 * Return better http status when review callback resulted in the original
   exam no longer being proctored 
 
 [4.8.3] - 2022-01-12
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `edx-proctoring-4.8.4/LICENSE.txt` & `edx-proctoring-4.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/PKG-INFO` & `edx-proctoring-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-proctoring
-Version: 4.8.4
+Version: 4.9.0
 Summary: Proctoring subsystem for Open edX
 Home-page: https://github.com/edx/edx-proctoring
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: edx-proctoring
         ==============
@@ -129,14 +129,19 @@
            This project adheres to Semantic Versioning (https://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ~~~~~~~~~~
         
+        [4.9.0] - 2022-01-25
+        ~~~~~~~~~~~~~~~~~~~~
+        * Dropped Django22, 30 and 31
+        * Added Support for Django40
+        
         [4.8.4] - 2022-01-12
         ~~~~~~~~~~~~~~~~~~~~
         * Return better http status when review callback resulted in the original
           exam no longer being proctored 
         
         [4.8.3] - 2022-01-12
         ~~~~~~~~~~~~~~~~~~~~
@@ -887,15 +892,13 @@
         
         .. _GitHub commit history: https://github.com/edx/edx-proctoring/commits/master
         
 Keywords: Django edx
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edx-proctoring-4.8.4/README.rst` & `edx-proctoring-4.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/admin.py` & `edx-proctoring-4.9.0/edx_proctoring/admin.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/api.py` & `edx-proctoring-4.9.0/edx_proctoring/api.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/apps.py` & `edx-proctoring-4.9.0/edx_proctoring/apps.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/LICENSE.txt` & `edx-proctoring-4.9.0/edx_proctoring/backends/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/__init__.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/backend.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/backend.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/mock.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/mock.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/null.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/null.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/rest.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/rest.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/software_secure.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/software_secure.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/tests/test_backend.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/tests/test_rest.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/tests/test_review_payload.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/tests/test_review_payload.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/backends/tests/test_software_secure.py` & `edx-proctoring-4.9.0/edx_proctoring/backends/tests/test_software_secure.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/callbacks.py` & `edx-proctoring-4.9.0/edx_proctoring/callbacks.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/constants.py` & `edx-proctoring-4.9.0/edx_proctoring/constants.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/exceptions.py` & `edx-proctoring-4.9.0/edx_proctoring/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/handlers.py` & `edx-proctoring-4.9.0/edx_proctoring/handlers.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ar/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ar/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ar/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Karam Hawari <karamhawary71@gmail.com>, 2021
 # Dima Hilal, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Dima Hilal, 2021\n"
 "Language-Team: Arabic (https://www.transifex.com/open-edx/teams/6205/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ar/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ar/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Karam Hawari <karamhawary71@gmail.com>, 2021
 # Dima Hilal, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Dima Hilal, 2021\n"
 "Language-Team: Arabic (https://www.transifex.com/open-edx/teams/6205/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ca/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ca/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ca/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Farhanah Sheets <fsheets@edx.org>, 2018
 # Juanjo Bote <juanjo.botev@ub.edu>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Juanjo Bote <juanjo.botev@ub.edu>, 2021\n"
 "Language-Team: Catalan (https://www.transifex.com/open-edx/teams/6205/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ca\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ca/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ca/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ca/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ca/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # c896ac1a58859742747095a7a9acc41f_ae2eef1 <f3242be5e2827fc993543819c3e74ab4_161414>, 2016
 # Juanjo Bote <juanjo.botev@ub.edu>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Juanjo Bote <juanjo.botev@ub.edu>, 2021\n"
 "Language-Team: Catalan (https://www.transifex.com/open-edx/teams/6205/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ca\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/config.yaml` & `edx-proctoring-4.9.0/edx_proctoring/locale/config.yaml`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/cs/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/cs/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/cs/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Jan Chromý <jan.chromy@gmail.com>, 2017
 # trendspotter <jirka.p@volny.cz>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: trendspotter <jirka.p@volny.cz>, 2021\n"
 "Language-Team: Czech (https://www.transifex.com/open-edx/teams/6205/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: cs\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/cs/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/cs/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Jan Chromý <jan.chromy@gmail.com>, 2017
 # trendspotter <jirka.p@volny.cz>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: trendspotter <jirka.p@volny.cz>, 2021\n"
 "Language-Team: Czech (https://www.transifex.com/open-edx/teams/6205/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: cs\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Agata Kawczynski, 2021
 # Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2021\n"
 "Language-Team: German (Germany) (https://www.transifex.com/open-edx/teams/6205/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de_DE\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/de_DE/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Agata Kawczynski, 2021
 # Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2021\n"
 "Language-Team: German (Germany) (https://www.transifex.com/open-edx/teams/6205/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de_DE\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/el/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/el/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/el/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Eirini Mageiropoulou <eirmageir@yahoo.com>, 2021
 # LOUKAS SKOUROLIAKOS, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: LOUKAS SKOUROLIAKOS, 2021\n"
 "Language-Team: Greek (https://www.transifex.com/open-edx/teams/6205/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: el\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/el/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/el/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/el/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Eirini Mageiropoulou <eirmageir@yahoo.com>, 2021
 # LOUKAS SKOUROLIAKOS, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: LOUKAS SKOUROLIAKOS, 2021\n"
 "Language-Team: Greek (https://www.transifex.com/open-edx/teams/6205/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: el\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/en/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/en/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/eo/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/eo/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/eo/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/eo/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/es_419/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/es_419/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/es_419/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/es_419/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Juan Camilo Montoya Franco <juan.montoya@edunext.co>, 2021
 # Carolina De Mares <carolina.demares@edunext.co>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Carolina De Mares <carolina.demares@edunext.co>, 2021\n"
 "Language-Team: Spanish (Latin America) (https://www.transifex.com/open-edx/teams/6205/es_419/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_419\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/es_419/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/es_419/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/es_419/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/es_419/LC_MESSAGES/djangojs.po`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Juan Camilo Montoya Franco <juan.montoya@edunext.co>, 2021
 # Carolina De Mares <carolina.demares@edunext.co>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Carolina De Mares <carolina.demares@edunext.co>, 2021\n"
 "Language-Team: Spanish (Latin America) (https://www.transifex.com/open-edx/teams/6205/es_419/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_419\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/es_AR/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/es_AR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/es_AR/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/es_AR/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Eliana Moran <eliana_474@hotmail.com>, 2016
 # Aylén <aylen_00@hotmail.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Aylén <aylen_00@hotmail.com>, 2021\n"
 "Language-Team: Spanish (Argentina) (https://www.transifex.com/open-edx/teams/6205/es_AR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_AR\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # Pedro Lonbide <plonbide@gmail.com>, 2016
 # Abel Camacho <abelcama@gmail.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
-"PO-Revision-Date: 2016-12-20 19:52+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
+"PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Abel Camacho <abelcama@gmail.com>, 2021\n"
 "Language-Team: Basque (Spain) (https://www.transifex.com/open-edx/teams/6205/eu_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: eu_ES\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -1317,15 +1317,15 @@
 "                After the due date has passed, you can review the exam, but you cannot change your answers.\n"
 "            "
 msgstr ""
 
 #: utils.py:87
 #, python-brace-format
 msgid "{num_of_hours} hour"
-msgstr " ordu {num_of_hours}"
+msgstr "{num_of_hours} ordu"
 
 #: utils.py:90
 #, python-brace-format
 msgid "{num_of_hours} hours"
 msgstr "{num_of_hours} ordu"
 
 #: utils.py:98 utils.py:108
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/eu_ES/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/eu_ES/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # Pedro Lonbide <plonbide@gmail.com>, 2016
 # Abel Camacho <abelcama@gmail.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
-"PO-Revision-Date: 2016-12-20 19:55+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
+"PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Abel Camacho <abelcama@gmail.com>, 2021\n"
 "Language-Team: Basque (Spain) (https://www.transifex.com/open-edx/teams/6205/eu_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: eu_ES\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -1317,15 +1317,15 @@
 "                After the due date has passed, you can review the exam, but you cannot change your answers.\n"
 "            "
 msgstr ""
 
 #: utils.py:87
 #, python-brace-format
 msgid "{num_of_hours} hour"
-msgstr "{num_of_hours} ordu"
+msgstr " ordu {num_of_hours}"
 
 #: utils.py:90
 #, python-brace-format
 msgid "{num_of_hours} hours"
 msgstr "{num_of_hours} ordu"
 
 #: utils.py:98 utils.py:108
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/fr/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/fr/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1634,14 +1634,17 @@
 
 msgid "Rejected"
 msgstr "Rejeté"
 
 msgid "Resetting Onboarding Exam"
 msgstr "Réinitialisation de l'examen d'intégration"
 
+msgid "Resumed"
+msgstr "Recommencé"
+
 msgid "Retry Verification"
 msgstr "Réessayer la vérification"
 
 msgid "Retry my exam"
 msgstr "Réessayer mon examen"
 
 msgid "Review Policy Exception"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/fr/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Abdessamad Derraz <derraz.abdessamad@gmail.com>, 2021
 # iderr <ibrahim@derraz.fr>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: iderr <ibrahim@derraz.fr>, 2021\n"
 "Language-Team: French (https://www.transifex.com/open-edx/teams/6205/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
@@ -204,15 +204,15 @@
 
 #: models.py:421
 msgid "Ready to Resume"
 msgstr "Prêt à reprendre"
 
 #: models.py:424
 msgid "Resumed"
-msgstr ""
+msgstr "Recommencé"
 
 #: models.py:524
 msgid "Additional Time (minutes)"
 msgstr "Temps additionnel (minutes)"
 
 #: models.py:525
 msgid "Review Policy Exception"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/fr/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/fr/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Abdessamad Derraz <derraz.abdessamad@gmail.com>, 2021
 # iderr <ibrahim@derraz.fr>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: iderr <ibrahim@derraz.fr>, 2021\n"
 "Language-Team: French (https://www.transifex.com/open-edx/teams/6205/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Pierre Mailhot <pierre.mailhot@gmail.com>, 2021
 # David Truong <david.truong@edulib.org>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: David Truong <david.truong@edulib.org>, 2021\n"
 "Language-Team: French (Canada) (https://www.transifex.com/open-edx/teams/6205/fr_CA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr_CA\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/fr_CA/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/fr_CA/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Pierre Mailhot <pierre.mailhot@gmail.com>, 2021
 # David Truong <david.truong@edulib.org>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: David Truong <david.truong@edulib.org>, 2021\n"
 "Language-Team: French (Canada) (https://www.transifex.com/open-edx/teams/6205/fr_CA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr_CA\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/he/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/he/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/he/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # qualityalltext <quality@alltext.co.il>, 2017
 # Hodaya Zada <hodayaz@mse.gov.il>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Hodaya Zada <hodayaz@mse.gov.il>, 2021\n"
 "Language-Team: Hebrew (https://www.transifex.com/open-edx/teams/6205/he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: he\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/he/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/he/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/he/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # qualityalltext <quality@alltext.co.il>, 2017
 # Hodaya Zada <hodayaz@mse.gov.il>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Hodaya Zada <hodayaz@mse.gov.il>, 2021\n"
 "Language-Team: Hebrew (https://www.transifex.com/open-edx/teams/6205/he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: he\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/id/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/id/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/id/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Sari Rahmawati <kusuma.rahmawati@gmail.com>, 2018
 # Aprisa Chrysantina <aprisa.chrysantina@gmail.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Aprisa Chrysantina <aprisa.chrysantina@gmail.com>, 2021\n"
 "Language-Team: Indonesian (https://www.transifex.com/open-edx/teams/6205/id/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: id\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/id/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/id/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/id/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/id/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Sari Rahmawati <kusuma.rahmawati@gmail.com>, 2018
 # Aprisa Chrysantina <aprisa.chrysantina@gmail.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Aprisa Chrysantina <aprisa.chrysantina@gmail.com>, 2021\n"
 "Language-Team: Indonesian (https://www.transifex.com/open-edx/teams/6205/id/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: id\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Mauri Macera, 2021
 # Domenico Casanica <domenico.casanica@sistinf.it>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Domenico Casanica <domenico.casanica@sistinf.it>, 2021\n"
 "Language-Team: Italian (Italy) (https://www.transifex.com/open-edx/teams/6205/it_IT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: it_IT\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/it_IT/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/it_IT/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Mauri Macera, 2021
 # Domenico Casanica <domenico.casanica@sistinf.it>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Domenico Casanica <domenico.casanica@sistinf.it>, 2021\n"
 "Language-Team: Italian (Italy) (https://www.transifex.com/open-edx/teams/6205/it_IT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: it_IT\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ja_JP/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ja_JP/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ja_JP/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ja_JP/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Shoji Kajita <kajita.shoji.5z@kyoto-u.ac.jp>, 2016
 # Kyoto University <edxkyotoux@gmail.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Kyoto University <edxkyotoux@gmail.com>, 2021\n"
 "Language-Team: Japanese (Japan) (https://www.transifex.com/open-edx/teams/6205/ja_JP/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ja_JP\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ka/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ka/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ka/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ka/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Giorgi Goderdzishvili <biggeorgian@gmail.com>, 2017
 # ketevan Kokhreidze <k.kokhreidze@gmail.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: ketevan Kokhreidze <k.kokhreidze@gmail.com>, 2021\n"
 "Language-Team: Georgian (https://www.transifex.com/open-edx/teams/6205/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ka\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ka/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ka/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ka/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ka/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Giorgi Goderdzishvili <biggeorgian@gmail.com>, 2017
 # ketevan Kokhreidze <k.kokhreidze@gmail.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: ketevan Kokhreidze <k.kokhreidze@gmail.com>, 2021\n"
 "Language-Team: Georgian (https://www.transifex.com/open-edx/teams/6205/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ka\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/lv/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/lv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/lv/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/lv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Translators:
 # LTMC Latvijas Tiesnešu mācību centrs <ltmc.training@gmail.com>, 2018
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: LTMC Latvijas Tiesnešu mācību centrs <ltmc.training@gmail.com>, 2018\n"
 "Language-Team: Latvian (https://www.transifex.com/open-edx/teams/6205/lv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lv\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/lv/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/lv/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Translators:
 # LTMC Latvijas Tiesnešu mācību centrs <ltmc.training@gmail.com>, 2018
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: LTMC Latvijas Tiesnešu mācību centrs <ltmc.training@gmail.com>, 2018\n"
 "Language-Team: Latvian (https://www.transifex.com/open-edx/teams/6205/lv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lv\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/mn/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/mn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Munkhtsetseg <moogmonkhoo_n@yahoo.com>, 2016
 # Gerelmaa Byambatsogt <by.gerelmaa@gmail.com>, 2018
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Gerelmaa Byambatsogt <by.gerelmaa@gmail.com>, 2018\n"
 "Language-Team: Mongolian (https://www.transifex.com/open-edx/teams/6205/mn/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: mn\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/mn/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/mn/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Gerelmaa Byambatsogt <by.gerelmaa@gmail.com>, 2018
 # Lodoiravsal Choimaa, 2018
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Lodoiravsal Choimaa, 2018\n"
 "Language-Team: Mongolian (https://www.transifex.com/open-edx/teams/6205/mn/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: mn\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/nb/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/nb/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/nb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Frode Arntsen <frode.arntsen@unit.no>, 2017
 # Joakim S. Johnson, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Joakim S. Johnson, 2021\n"
 "Language-Team: Norwegian Bokmål (https://www.transifex.com/open-edx/teams/6205/nb/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nb\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/nb/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/nb/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Frode Arntsen <frode.arntsen@unit.no>, 2017
 # Joakim S. Johnson, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Joakim S. Johnson, 2021\n"
 "Language-Team: Norwegian Bokmål (https://www.transifex.com/open-edx/teams/6205/nb/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nb\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Filipa Macieira <filipa.macieira@fccn.pt>, 2021
 # Ivo Branco <ivo.branco@fccn.pt>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Ivo Branco <ivo.branco@fccn.pt>, 2021\n"
 "Language-Team: Portuguese (Portugal) (https://www.transifex.com/open-edx/teams/6205/pt_PT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_PT\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/pt_PT/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Ivo Branco <ivo.branco@fccn.pt>, 2021
 # Filipa Macieira <filipa.macieira@fccn.pt>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Filipa Macieira <filipa.macieira@fccn.pt>, 2021\n"
 "Language-Team: Portuguese (Portugal) (https://www.transifex.com/open-edx/teams/6205/pt_PT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_PT\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ro/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ro/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ro/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Lucian Horga <lucian.horga@devtelsoftware.com>, 2020
 # George Turtureanu <contact@didactiv.org>, 2020
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: George Turtureanu <contact@didactiv.org>, 2020\n"
 "Language-Team: Romanian (https://www.transifex.com/open-edx/teams/6205/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ro/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ro/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Lucian Horga <lucian.horga@devtelsoftware.com>, 2020
 # George Turtureanu <contact@didactiv.org>, 2020
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: George Turtureanu <contact@didactiv.org>, 2020\n"
 "Language-Team: Romanian (https://www.transifex.com/open-edx/teams/6205/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ru/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ru/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Weyedide <weyedide@gmail.com>, 2021
 # Anastasija Teresenkova <anastasija_te@inbox.lv>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Anastasija Teresenkova <anastasija_te@inbox.lv>, 2021\n"
 "Language-Team: Russian (https://www.transifex.com/open-edx/teams/6205/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ru/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/ru/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Weyedide <weyedide@gmail.com>, 2021
 # Anastasija Teresenkova <anastasija_te@inbox.lv>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Anastasija Teresenkova <anastasija_te@inbox.lv>, 2021\n"
 "Language-Team: Russian (https://www.transifex.com/open-edx/teams/6205/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # YAHAYA MWAVURIZI <translations_1@camara.ie>, 2017
 # swaleh amin <mkupuofirstnameswaleh@yahoo.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: swaleh amin <mkupuofirstnameswaleh@yahoo.com>, 2021\n"
 "Language-Team: Swahili (Kenya) (https://www.transifex.com/open-edx/teams/6205/sw_KE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sw_KE\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/sw_KE/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/sw_KE/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # YAHAYA MWAVURIZI <translations_1@camara.ie>, 2017
 # swaleh amin <mkupuofirstnameswaleh@yahoo.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: swaleh amin <mkupuofirstnameswaleh@yahoo.com>, 2021\n"
 "Language-Team: Swahili (Kenya) (https://www.transifex.com/open-edx/teams/6205/sw_KE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sw_KE\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Adem Özgür <admozgur@gmail.com>, 2021
 # Ali Işıngör <ali@artistanbul.io>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2021\n"
 "Language-Team: Turkish (Turkey) (https://www.transifex.com/open-edx/teams/6205/tr_TR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: tr_TR\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/tr_TR/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Adem Özgür <admozgur@gmail.com>, 2021
 # Ali Işıngör <ali@artistanbul.io>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2021\n"
 "Language-Team: Turkish (Turkey) (https://www.transifex.com/open-edx/teams/6205/tr_TR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: tr_TR\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/uk/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/uk/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Radmila Segol <geroneja@yahoo.com>, 2021
 # Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021\n"
 "Language-Team: Ukrainian (https://www.transifex.com/open-edx/teams/6205/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: uk\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/uk/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/uk/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Radmila Segol <geroneja@yahoo.com>, 2021
 # Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021\n"
 "Language-Team: Ukrainian (https://www.transifex.com/open-edx/teams/6205/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: uk\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/LC_MESSAGES/django.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/LC_MESSAGES/django.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # ifLab <webmaster@iflab.org>, 2021
 # meelo <bbvy@qq.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:52+0000\n"
 "Last-Translator: meelo <bbvy@qq.com>, 2021\n"
 "Language-Team: Chinese (China) (https://www.transifex.com/open-edx/teams/6205/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/locale/zh_CN/LC_MESSAGES/djangojs.po` & `edx-proctoring-4.9.0/edx_proctoring/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # ifLab <webmaster@iflab.org>, 2021
 # meelo <bbvy@qq.com>, 2021
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-proctoring\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-12-26 18:34+0000\n"
+"POT-Creation-Date: 2022-01-10 21:04+0000\n"
 "PO-Revision-Date: 2016-12-20 19:55+0000\n"
 "Last-Translator: meelo <bbvy@qq.com>, 2021\n"
 "Language-Team: Chinese (China) (https://www.transifex.com/open-edx/teams/6205/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring/management/commands/set_attempt_status.py` & `edx-proctoring-4.9.0/edx_proctoring/management/commands/set_attempt_status.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/management/commands/set_is_attempt_active.py` & `edx-proctoring-4.9.0/edx_proctoring/management/commands/set_is_attempt_active.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/test_set_attempt_status.py` & `edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/test_set_attempt_status.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/test_set_is_attempt_active.py` & `edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/test_set_is_attempt_active.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/test_update_attempt_status_from_review.py` & `edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/test_update_attempt_status_from_review.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/management/commands/tests/test_update_attempts_for_exam.py` & `edx-proctoring-4.9.0/edx_proctoring/management/commands/tests/test_update_attempts_for_exam.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/management/commands/update_attempt_status_from_review.py` & `edx-proctoring-4.9.0/edx_proctoring/management/commands/update_attempt_status_from_review.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/management/commands/update_attempts_for_exam.py` & `edx-proctoring-4.9.0/edx_proctoring/management/commands/update_attempts_for_exam.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0001_initial.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0003_auto_20160101_0525.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0003_auto_20160101_0525.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0006_allowed_time_limit_mins.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0006_allowed_time_limit_mins.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0008_auto_20181116_1551.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0008_auto_20181116_1551.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0010_update_backend.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0010_update_backend.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0013_proctoredexamsoftwaresecurereview_is_active_attempt.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0013_proctoredexamsoftwaresecurereview_is_active_attempt.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0014_add_is_resumable_to_proctoredexamstudentattempt.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0014_add_is_resumable_to_proctoredexamstudentattempt.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0015_rm_proctoredexamstudentattempt_ips.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0015_rm_proctoredexamstudentattempt_ips.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0016_nullable_proctoredexamstudentattempt_name.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0016_nullable_proctoredexamstudentattempt_name.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0017_rm_proctoredexamstudentattempt_name.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0017_rm_proctoredexamstudentattempt_name.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0018_historicalproctoredexamstudentattempt.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0018_historicalproctoredexamstudentattempt.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0020_auto_20211028_1915.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0020_auto_20211028_1915.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0021_auto_20211029_1353.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0021_auto_20211029_1353.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0022_proctoredexamstudentattempt_add_readytoresume_resumed.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0022_proctoredexamstudentattempt_add_readytoresume_resumed.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/migrations/0023_historicalproctoredexam.py` & `edx-proctoring-4.9.0/edx_proctoring/migrations/0023_historicalproctoredexam.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/models.py` & `edx-proctoring-4.9.0/edx_proctoring/models.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/scripts/obscure_user.py` & `edx-proctoring-4.9.0/edx_proctoring/scripts/obscure_user.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/scripts/version_check.py` & `edx-proctoring-4.9.0/edx_proctoring/scripts/version_check.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/serializers.py` & `edx-proctoring-4.9.0/edx_proctoring/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/services.py` & `edx-proctoring-4.9.0/edx_proctoring/services.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/settings/common.py` & `edx-proctoring-4.9.0/edx_proctoring/settings/common.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/settings/production.py` & `edx-proctoring-4.9.0/edx_proctoring/settings/production.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/index.js` & `edx-proctoring-4.9.0/edx_proctoring/static/index.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/clippy.swf` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/clippy.swf`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/close-modal-hover.png` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/close-modal-hover.png`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/close-modal.png` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/close-modal.png`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/collections/proctored_exam_allowance_collection.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/collections/proctored_exam_allowance_collection.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/collections/proctored_exam_attempt_grouped_collection.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/collections/proctored_exam_attempt_grouped_collection.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/collections/proctored_exam_collection.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/collections/proctored_exam_collection.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/collections/proctored_exam_onboarding_collection.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/collections/proctored_exam_onboarding_collection.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/dropdown.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/dropdown.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/exam_action_handler.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/exam_action_handler.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/proctored_exam_allowance_model.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/proctored_exam_allowance_model.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/proctored_exam_attempt_model.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/proctored_exam_attempt_model.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/proctored_exam_bulk_allowance_model.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/proctored_exam_bulk_allowance_model.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/models/proctored_exam_model.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/models/proctored_exam_model.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/proctored_app.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/proctored_app.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/backbone.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/backbone.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/date.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/date.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/jquery.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/jquery.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/vendor/underscore.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/vendor/underscore.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/Backbone.ModalDialog.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/Backbone.ModalDialog.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_add_bulk_allowance_view.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_add_bulk_allowance_view.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_allowance_view.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_allowance_view.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_attempt_view.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_attempt_view.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_edit_allowance_view.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_edit_allowance_view.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_info.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_info.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_instructor_launch.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_instructor_launch.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_onboarding_view.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_onboarding_view.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/js/views/proctored_exam_view.js` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/js/views/proctored_exam_view.js`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/add-new-bulk-allowance.underscore` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/add-new-bulk-allowance.underscore`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/course_grouped_allowances.underscore` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/course_grouped_allowances.underscore`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/edit-allowance.underscore` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/edit-allowance.underscore`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/proctored-exam-info.underscore` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/proctored-exam-info.underscore`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/student-onboarding-status.underscore` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/student-onboarding-status.underscore`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/static/proctoring/templates/student-proctored-exam-attempts-grouped.underscore` & `edx-proctoring-4.9.0/edx_proctoring/static/proctoring/templates/student-proctored-exam-attempts-grouped.underscore`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/statuses.py` & `edx-proctoring-4.9.0/edx_proctoring/statuses.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/emails/proctoring_attempt_satisfactory_email.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/emails/proctoring_attempt_satisfactory_email.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/emails/proctoring_attempt_submitted_email.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/emails/proctoring_attempt_submitted_email.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/emails/proctoring_attempt_unsatisfactory_email.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/emails/proctoring_attempt_unsatisfactory_email.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/entrance.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/entrance.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/rejected.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/rejected.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/submitted.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/submitted.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/onboarding_exam/verified.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/onboarding_exam/verified.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/practice_exam/entrance.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/practice_exam/entrance.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/practice_exam/error.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/practice_exam/error.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/practice_exam/submitted.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/practice_exam/submitted.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/confirm-decline.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/confirm-decline.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/entrance.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/entrance.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/error.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/error.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/error_modal.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/error_modal.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/error_wrong_browser.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/error_wrong_browser.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/failed-prerequisites.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/failed-prerequisites.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/footer.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/footer.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/id_verification.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/id_verification.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/inactive_account.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/inactive_account.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/instructions.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/instructions.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/onboarding_error.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/onboarding_error.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/pending-prerequisites.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/pending-prerequisites.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/proctoring_launch_callback.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/proctoring_launch_callback.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/ready_to_resume.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/ready_to_resume.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/ready_to_start.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/ready_to_start.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/ready_to_submit.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/ready_to_submit.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/rejected.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/rejected.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/submitted.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/submitted.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/verified.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/verified.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/proctored_exam/visit_exam_content.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/proctored_exam/visit_exam_content.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/timed_exam/entrance.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/timed_exam/entrance.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/timed_exam/ready_to_submit.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/timed_exam/ready_to_submit.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/templates/timed_exam/submitted.html` & `edx-proctoring-4.9.0/edx_proctoring/templates/timed_exam/submitted.html`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/__init__.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_api.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_email.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_handlers.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_mfe_views.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_mfe_views.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_models.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_reviews.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_reviews.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_serializer.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_services.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_student_view.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_student_view.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_utils.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_views.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/test_workerconfig.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/test_workerconfig.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/tests/utils.py` & `edx-proctoring-4.9.0/edx_proctoring/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/urls.py` & `edx-proctoring-4.9.0/edx_proctoring/urls.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/utils.py` & `edx-proctoring-4.9.0/edx_proctoring/utils.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring/views.py` & `edx-proctoring-4.9.0/edx_proctoring/views.py`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/edx_proctoring.egg-info/PKG-INFO` & `edx-proctoring-4.9.0/edx_proctoring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-proctoring
-Version: 4.8.4
+Version: 4.9.0
 Summary: Proctoring subsystem for Open edX
 Home-page: https://github.com/edx/edx-proctoring
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: edx-proctoring
         ==============
@@ -129,14 +129,19 @@
            This project adheres to Semantic Versioning (https://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ~~~~~~~~~~
         
+        [4.9.0] - 2022-01-25
+        ~~~~~~~~~~~~~~~~~~~~
+        * Dropped Django22, 30 and 31
+        * Added Support for Django40
+        
         [4.8.4] - 2022-01-12
         ~~~~~~~~~~~~~~~~~~~~
         * Return better http status when review callback resulted in the original
           exam no longer being proctored 
         
         [4.8.3] - 2022-01-12
         ~~~~~~~~~~~~~~~~~~~~
@@ -887,15 +892,13 @@
         
         .. _GitHub commit history: https://github.com/edx/edx-proctoring/commits/master
         
 Keywords: Django edx
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edx-proctoring-4.8.4/edx_proctoring.egg-info/SOURCES.txt` & `edx-proctoring-4.9.0/edx_proctoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/requirements/base.in` & `edx-proctoring-4.9.0/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/requirements/base.txt` & `edx-proctoring-4.9.0/requirements/base.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,29 @@
     # via -r requirements/base.in
 django-model-utils==4.2.0
     # via
     #   -r requirements/base.in
     #   edx-when
 django-simple-history==3.0.0
     # via -r requirements/base.in
-django-waffle==2.2.1
+django-waffle==2.3.0
     # via
     #   -r requirements/base.in
     #   edx-django-utils
     #   edx-drf-extensions
 django-webpack-loader==0.7.0
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
 djangorestframework==3.13.1
     # via
     #   -r requirements/base.in
     #   drf-jwt
     #   edx-drf-extensions
-drf-jwt==1.19.1
+drf-jwt==1.19.2
     # via edx-drf-extensions
 edx-django-utils==4.4.1
     # via
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   edx-when
     #   event-tracking
@@ -89,15 +89,15 @@
     #   -r requirements/base.in
     #   edx-when
 edx-opaque-keys==2.2.2
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-when
-edx-rest-api-client==5.4.1
+edx-rest-api-client==5.5.0
     # via -r requirements/base.in
 edx-when==2.2.2
     # via -r requirements/base.in
 event-tracking==1.1.4
     # via -r requirements/base.in
 fs==2.4.14
     # via xblock
@@ -177,15 +177,15 @@
     # via edx-rest-api-client
 sqlparse==0.4.2
     # via django
 stevedore==3.5.0
     # via
     #   edx-django-utils
     #   edx-opaque-keys
-urllib3==1.26.7
+urllib3==1.26.8
     # via requests
 vine==5.0.0
     # via
     #   amqp
     #   celery
     #   kombu
 wcwidth==0.2.5
```

### Comparing `edx-proctoring-4.8.4/requirements/ci.txt` & `edx-proctoring-4.9.0/requirements/ci.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,11 +40,11 @@
     # via tox
 tox==3.24.5
     # via
     #   -r requirements/ci.in
     #   tox-battery
 tox-battery==0.6.1
     # via -r requirements/ci.in
-urllib3==1.26.7
+urllib3==1.26.8
     # via requests
 virtualenv==20.13.0
     # via tox
```

### Comparing `edx-proctoring-4.8.4/requirements/common_constraints.txt` & `edx-proctoring-4.9.0/requirements/common_constraints.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,7 +21,10 @@
 Django<3.3
 
 # elasticsearch>=7.14.0 includes breaking changes in it which caused issues in discovery upgrade process.
 # elastic search changelog: https://www.elastic.co/guide/en/enterprise-search/master/release-notes-7.14.0.html
 elasticsearch<7.14.0
 
 setuptools<60
+
+# redis 4 client doesn't play nicely with redis 3 server
+redis<4
```

### Comparing `edx-proctoring-4.8.4/requirements/constraints.txt` & `edx-proctoring-4.9.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/requirements/dev.in` & `edx-proctoring-4.9.0/requirements/dev.in`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/requirements/dev.txt` & `edx-proctoring-4.9.0/requirements/dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with python 3.8
 # To update, run:
 #
 #    make upgrade
 #
 asgiref==3.4.1
     # via django
-astroid==2.9.2
+astroid==2.9.3
     # via
     #   pylint
     #   pylint-celery
 chardet==4.0.0
     # via diff-cover
 click==7.1.2
     # via
@@ -57,15 +57,15 @@
     # via astroid
 markupsafe==2.0.1
     # via jinja2
 mccabe==0.6.1
     # via pylint
 packaging==21.3
     # via tox
-path==16.2.0
+path==16.3.0
     # via
     #   edx-i18n-tools
     #   path.py
 path.py==12.5.0
     # via -r requirements/dev.in
 pbr==5.8.0
     # via stevedore
```

### Comparing `edx-proctoring-4.8.4/requirements/quality.txt` & `edx-proctoring-4.9.0/requirements/quality.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with python 3.8
 # To update, run:
 #
 #    make upgrade
 #
 asgiref==3.4.1
     # via django
-astroid==2.9.2
+astroid==2.9.3
     # via
     #   pylint
     #   pylint-celery
 click==7.1.2
     # via
     #   -c requirements/constraints.txt
     #   click-log
```

### Comparing `edx-proctoring-4.8.4/requirements/test.in` & `edx-proctoring-4.9.0/requirements/test.in`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/requirements/test.txt` & `edx-proctoring-4.9.0/requirements/test.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,28 +65,28 @@
     # via -r requirements/base.in
 django-model-utils==4.2.0
     # via
     #   -r requirements/base.in
     #   edx-when
 django-simple-history==3.0.0
     # via -r requirements/base.in
-django-waffle==2.2.1
+django-waffle==2.3.0
     # via
     #   -r requirements/base.in
     #   edx-django-utils
     #   edx-drf-extensions
 django-webpack-loader==0.7.0
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
     # via
     #   -r requirements/base.in
     #   drf-jwt
     #   edx-drf-extensions
-drf-jwt==1.19.1
+drf-jwt==1.19.2
     # via edx-drf-extensions
 edx-django-utils==4.4.1
     # via
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   edx-when
     #   event-tracking
@@ -97,15 +97,15 @@
 edx-i18n-tools==0.8.1
     # via -r requirements/test.in
 edx-opaque-keys==2.2.2
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-when
-edx-rest-api-client==5.4.1
+edx-rest-api-client==5.5.0
     # via -r requirements/base.in
 edx-when==2.2.2
     # via -r requirements/base.in
 event-tracking==1.1.4
     # via -r requirements/base.in
 execnet==1.9.0
     # via pytest-xdist
@@ -142,15 +142,15 @@
     # via -r requirements/test.in
 mypy-extensions==0.4.3
     # via logilab-common
 newrelic==7.2.4.171
     # via edx-django-utils
 packaging==21.3
     # via pytest
-path==16.2.0
+path==16.3.0
     # via edx-i18n-tools
 pbr==5.8.0
     # via stevedore
 pluggy==1.0.0
     # via pytest
 polib==1.1.1
     # via edx-i18n-tools
@@ -221,15 +221,15 @@
     # via
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   httmock
     #   pyjwkest
     #   responses
     #   slumber
-responses==0.16.0
+responses==0.17.0
     # via -r requirements/test.in
 rules==3.1
     # via -r requirements/base.in
 selenium==3.141.0
     # via
     #   -r requirements/test.in
     #   bok-choy
@@ -262,15 +262,15 @@
     # via python-slugify
 toml==0.10.2
     # via pytest
 tomli==2.0.0
     # via coverage
 typing-extensions==4.0.1
     # via logilab-common
-urllib3==1.26.7
+urllib3==1.26.8
     # via
     #   requests
     #   responses
     #   selenium
     # via
     #   amqp
     #   celery
```

### Comparing `edx-proctoring-4.8.4/setup.cfg` & `edx-proctoring-4.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `edx-proctoring-4.8.4/setup.py` & `edx-proctoring-4.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,18 +67,16 @@
     url='https://github.com/edx/edx-proctoring',
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
     ],
     packages=[
         'edx_proctoring',
```

