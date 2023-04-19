# Comparing `tmp/ytmusicapi-1.0.0.tar.gz` & `tmp/ytmusicapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusicapi-1.0.0.tar", last modified: Sat Apr  8 18:29:21 2023, max compression
+gzip compressed data, was "ytmusicapi-1.0.1.tar", last modified: Wed Apr 19 18:52:04 2023, max compression
```

## Comparing `ytmusicapi-1.0.0.tar` & `ytmusicapi-1.0.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/workflows/docsbuild.yml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/docs/source/setup/
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/setup/browser.rst
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/setup/headers_auth.json.example
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/setup/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/setup/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/tests/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/tests/test.cfg.example
--rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/ytmusicapi/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/ytmusicapi/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/auth/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/auth/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/continuations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/de/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/en/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/en/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/es/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/it/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/update_mo.sh
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/update_po.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/ytmusicapi/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/browsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/playlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/ytmusicapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/albums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/browsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/playlists.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/songs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/ytmusicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.450548 ytmusicapi-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.430548 ytmusicapi-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.430548 ytmusicapi-1.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.430548 ytmusicapi-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.github/workflows/docsbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-19 18:52:04.450548 ytmusicapi-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.434548 ytmusicapi-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.434548 ytmusicapi-1.0.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/source/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.434548 ytmusicapi-1.0.1/docs/source/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/source/setup/browser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/source/setup/headers_auth.json.example
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/source/setup/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/source/setup/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:52:04.450548 ytmusicapi-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.434548 ytmusicapi-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/tests/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/tests/test.cfg.example
+-rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.438548 ytmusicapi-1.0.1/ytmusicapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.438548 ytmusicapi-1.0.1/ytmusicapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/auth/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/auth/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/continuations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.438548 ytmusicapi-1.0.1/ytmusicapi/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.422548 ytmusicapi-1.0.1/ytmusicapi/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.438548 ytmusicapi-1.0.1/ytmusicapi/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ar/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.438548 ytmusicapi-1.0.1/ytmusicapi/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/de/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.442548 ytmusicapi-1.0.1/ytmusicapi/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/en/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/en/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.442548 ytmusicapi-1.0.1/ytmusicapi/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/es/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/es/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.442548 ytmusicapi-1.0.1/ytmusicapi/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/fr/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.442548 ytmusicapi-1.0.1/ytmusicapi/locales/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/hi/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.442548 ytmusicapi-1.0.1/ytmusicapi/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/it/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/it/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.442548 ytmusicapi-1.0.1/ytmusicapi/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ja/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.442548 ytmusicapi-1.0.1/ytmusicapi/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ko/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.442548 ytmusicapi-1.0.1/ytmusicapi/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/pt/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.442548 ytmusicapi-1.0.1/ytmusicapi/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ru/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.446548 ytmusicapi-1.0.1/ytmusicapi/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/tr/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/update_mo.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/update_po.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.446548 ytmusicapi-1.0.1/ytmusicapi/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/ur/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.426548 ytmusicapi-1.0.1/ytmusicapi/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.446548 ytmusicapi-1.0.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.430548 ytmusicapi-1.0.1/ytmusicapi/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.446548 ytmusicapi-1.0.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.446548 ytmusicapi-1.0.1/ytmusicapi/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/mixins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/mixins/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/mixins/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/mixins/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/mixins/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/mixins/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/mixins/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/mixins/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.450548 ytmusicapi-1.0.1/ytmusicapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/songs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/parsers/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-19 18:51:52.000000 ytmusicapi-1.0.1/ytmusicapi/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:52:04.438548 ytmusicapi-1.0.1/ytmusicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-19 18:52:04.000000 ytmusicapi-1.0.1/ytmusicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-19 18:52:04.000000 ytmusicapi-1.0.1/ytmusicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:52:04.000000 ytmusicapi-1.0.1/ytmusicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 18:52:04.000000 ytmusicapi-1.0.1/ytmusicapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 18:52:04.000000 ytmusicapi-1.0.1/ytmusicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 18:52:04.000000 ytmusicapi-1.0.1/ytmusicapi.egg-info/top_level.txt
```

### Comparing `ytmusicapi-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ytmusicapi-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `ytmusicapi-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/.github/workflows/coverage.yml` & `ytmusicapi-1.0.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/.github/workflows/pythonpublish.yml` & `ytmusicapi-1.0.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/CONTRIBUTING.rst` & `ytmusicapi-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/LICENSE` & `ytmusicapi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/PKG-INFO` & `ytmusicapi-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.0.0/README.rst` & `ytmusicapi-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/docs/Makefile` & `ytmusicapi-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/docs/make.bat` & `ytmusicapi-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/docs/source/conf.py` & `ytmusicapi-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/docs/source/faq.rst` & `ytmusicapi-1.0.1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/docs/source/index.rst` & `ytmusicapi-1.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/docs/source/reference.rst` & `ytmusicapi-1.0.1/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/docs/source/setup/browser.rst` & `ytmusicapi-1.0.1/docs/source/setup/browser.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/docs/source/usage.rst` & `ytmusicapi-1.0.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/pyproject.toml` & `ytmusicapi-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/tests/README.rst` & `ytmusicapi-1.0.1/tests/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/tests/test.cfg.example` & `ytmusicapi-1.0.1/tests/test.cfg.example`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/tests/test.py` & `ytmusicapi-1.0.1/tests/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,74 @@
-import json
 import configparser
+import json
 import time
 import unittest
+import warnings
 from pathlib import Path
-from requests import Response
 from unittest import mock
 
+from requests import Response
+
 from ytmusicapi.setup import main, setup  # noqa: E402
 from ytmusicapi.ytmusic import YTMusic  # noqa: E402
 
 
 def get_resource(file: str) -> str:
     data_dir = Path(__file__).parent
     return data_dir.joinpath(file).as_posix()
 
 
 config = configparser.RawConfigParser()
-config.read(get_resource('test.cfg'), 'utf-8')
+config.read(get_resource("test.cfg"), "utf-8")
 
 sample_album = "MPREb_4pL8gzRtw1p"  # Eminem - Revival
 sample_video = "hpSrLjc5SMs"  # Oasis - Wonderwall
 sample_playlist = "PL6bPxvf5dW5clc3y9wAoslzqUrmkZ5c-u"  # very large playlist
 
-headers_oauth = get_resource(config['auth']['headers_oauth'])
-headers_browser = get_resource(config['auth']['headers_file'])
+headers_oauth = get_resource(config["auth"]["headers_oauth"])
+headers_browser = get_resource(config["auth"]["headers_file"])
 
 
 class TestYTMusic(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
+        warnings.filterwarnings(action="ignore", message="unclosed", category=ResourceWarning)
         with YTMusic(requests_session=False) as yt:
             assert isinstance(yt, YTMusic)
         cls.yt = YTMusic()
         cls.yt_oauth = YTMusic(headers_oauth)
+        with open(headers_oauth, mode="r", encoding="utf8") as headers:
+            string_headers = headers.read()
+            cls.yt_oauth = YTMusic(string_headers)
         cls.yt_auth = YTMusic(headers_browser)
-        cls.yt_brand = YTMusic(config['auth']['headers'], config['auth']['brand_account'])
-        cls.yt_empty = YTMusic(config['auth']['headers_empty'],
-                               config['auth']['brand_account_empty'])
+        cls.yt_brand = YTMusic(config["auth"]["headers"], config["auth"]["brand_account"])
+        cls.yt_empty = YTMusic(config["auth"]["headers_empty"],
+                               config["auth"]["brand_account_empty"])
 
-    @mock.patch('sys.argv', ["ytmusicapi", "browser", "--file", headers_browser])
+    @mock.patch("sys.argv", ["ytmusicapi", "browser", "--file", headers_browser])
     def test_setup_browser(self):
-        headers = setup(headers_browser, config['auth']['headers_raw'])
+        headers = setup(headers_browser, config["auth"]["headers_raw"])
         self.assertGreaterEqual(len(headers), 2)
-        headers_raw = config['auth']['headers_raw'].split('\n')
-        with mock.patch('builtins.input', side_effect=(headers_raw + [EOFError()])):
+        headers_raw = config["auth"]["headers_raw"].split("\n")
+        with mock.patch("builtins.input", side_effect=(headers_raw + [EOFError()])):
             headers = main()
             self.assertGreaterEqual(len(headers), 2)
 
     # @unittest.skip("Cannot test oauth flow non-interactively")
-    @mock.patch('requests.Response.json')
-    @mock.patch('requests.Session.post')
-    @mock.patch('sys.argv', ["ytmusicapi", "oauth", "--file", headers_oauth])
+    @mock.patch("requests.Response.json")
+    @mock.patch("requests.Session.post")
+    @mock.patch("sys.argv", ["ytmusicapi", "oauth", "--file", headers_oauth])
     def test_setup_oauth(self, session_mock, json_mock):
         session_mock.return_value = Response()
         json_mock.side_effect = [
-            json.loads(config['auth']['oauth_code']),
-            json.loads(config['auth']['oauth_token'])
+            json.loads(config["auth"]["oauth_code"]),
+            json.loads(config["auth"]["oauth_token"]),
         ]
-        with mock.patch('builtins.input', return_value='y'):
+        with mock.patch("builtins.input", return_value="y"):
             main()
             self.assertTrue(Path(headers_oauth).exists())
 
     ###############
     # BROWSING
     ###############
 
@@ -76,131 +82,135 @@
         query = "edm playlist"
         self.assertRaises(Exception, self.yt_auth.search, query, filter="song")
         self.assertRaises(Exception, self.yt_auth.search, query, scope="upload")
         queries = ["taylor swift", "taylor swift blank space", "taylor swift fearless"]
         for q in queries:
             with self.subTest():
                 results = self.yt_brand.search(q)
-                self.assertListEqual(['resultType' in r for r in results], [True] * len(results))
+                self.assertListEqual(["resultType" in r for r in results], [True] * len(results))
                 self.assertGreater(len(results), 10)
                 results = self.yt.search(q)
                 self.assertGreater(len(results), 10)
-        results = self.yt_auth.search('Martin Stig Andersen - Deteriation', ignore_spelling=True)
+        results = self.yt_auth.search("Martin Stig Andersen - Deteriation", ignore_spelling=True)
         self.assertGreater(len(results), 0)
-        results = self.yt_auth.search(query, filter='songs')
-        self.assertListEqual([r['resultType'] for r in results], ['song'] * len(results))
+        results = self.yt_auth.search(query, filter="songs")
+        self.assertListEqual([r["resultType"] for r in results], ["song"] * len(results))
         self.assertGreater(len(results), 10)
-        results = self.yt_auth.search(query, filter='videos')
+        results = self.yt_auth.search(query, filter="videos")
         self.assertGreater(len(results), 10)
-        results = self.yt_auth.search(query, filter='albums', limit=40)
-        self.assertListEqual([r['resultType'] for r in results], ['album'] * len(results))
+        results = self.yt_auth.search(query, filter="albums", limit=40)
+        self.assertListEqual([r["resultType"] for r in results], ["album"] * len(results))
         self.assertGreater(len(results), 20)
-        results = self.yt_auth.search('project-2', filter='artists', ignore_spelling=True)
+        results = self.yt_auth.search("project-2", filter="artists", ignore_spelling=True)
         self.assertGreater(len(results), 0)
-        results = self.yt_auth.search("classical music", filter='playlists')
+        results = self.yt_auth.search("classical music", filter="playlists")
         self.assertGreater(len(results), 5)
-        results = self.yt_auth.search("clasical music", filter='playlists', ignore_spelling=True)
+        results = self.yt_auth.search("clasical music", filter="playlists", ignore_spelling=True)
         self.assertGreater(len(results), 5)
         results = self.yt_auth.search("clasic rock",
-                                      filter='community_playlists',
+                                      filter="community_playlists",
                                       ignore_spelling=True)
         self.assertGreater(len(results), 5)
-        results = self.yt_auth.search("hip hop", filter='featured_playlists')
+        results = self.yt_auth.search("hip hop", filter="featured_playlists")
         self.assertGreater(len(results), 5)
 
     def test_search_uploads(self):
-        self.assertRaises(Exception,
-                          self.yt.search,
-                          'audiomachine',
-                          filter="songs",
-                          scope='uploads',
-                          limit=40)
-        results = self.yt_auth.search('audiomachine', scope='uploads', limit=40)
+        self.assertRaises(
+            Exception,
+            self.yt.search,
+            "audiomachine",
+            filter="songs",
+            scope="uploads",
+            limit=40,
+        )
+        results = self.yt_auth.search("audiomachine", scope="uploads", limit=40)
         self.assertGreater(len(results), 20)
 
     def test_search_library(self):
-        results = self.yt_oauth.search('garrix', scope='library')
+        results = self.yt_oauth.search("garrix", scope="library")
         self.assertGreater(len(results), 5)
-        results = self.yt_auth.search('bergersen', filter='songs', scope='library', limit=40)
+        results = self.yt_auth.search("bergersen", filter="songs", scope="library", limit=40)
         self.assertGreater(len(results), 10)
-        results = self.yt_auth.search('garrix', filter='albums', scope='library', limit=40)
+        results = self.yt_auth.search("garrix", filter="albums", scope="library", limit=40)
         self.assertGreaterEqual(len(results), 4)
-        results = self.yt_auth.search('garrix', filter='artists', scope='library', limit=40)
+        results = self.yt_auth.search("garrix", filter="artists", scope="library", limit=40)
         self.assertGreaterEqual(len(results), 1)
-        results = self.yt_auth.search('garrix', filter='playlists', scope='library')
+        results = self.yt_auth.search("garrix", filter="playlists", scope="library")
         self.assertGreaterEqual(len(results), 1)
 
     def test_get_artist(self):
         results = self.yt.get_artist("MPLAUCmMUZbaYdNH0bEd1PAlAqsA")
         self.assertEqual(len(results), 14)
 
         # test correctness of related artists
-        related = results['related']['results']
+        related = results["related"]["results"]
         self.assertEqual(
             len([
                 x for x in related
                 if set(x.keys()) == {"browseId", "subscribers", "title", "thumbnails"}
-            ]), len(related))
+            ]),
+            len(related),
+        )
 
         results = self.yt.get_artist("UCLZ7tlKC06ResyDmEStSrOw")  # no album year
         self.assertGreaterEqual(len(results), 11)
 
     def test_get_artist_albums(self):
         artist = self.yt.get_artist("UCj5ZiBBqpe0Tg4zfKGHEFuQ")
-        results = self.yt.get_artist_albums(artist['albums']['browseId'],
-                                            artist['albums']['params'])
+        results = self.yt.get_artist_albums(artist["albums"]["browseId"],
+                                            artist["albums"]["params"])
         self.assertGreater(len(results), 0)
 
     def test_get_artist_singles(self):
         artist = self.yt_auth.get_artist("UCAeLFBCQS7FvI8PvBrWvSBg")
-        results = self.yt_auth.get_artist_albums(artist['singles']['browseId'],
-                                                 artist['singles']['params'])
+        results = self.yt_auth.get_artist_albums(artist["singles"]["browseId"],
+                                                 artist["singles"]["params"])
         self.assertGreater(len(results), 0)
 
     def test_get_user(self):
         results = self.yt.get_user("UC44hbeRoCZVVMVg5z0FfIww")
         self.assertEqual(len(results), 3)
 
     def test_get_user_playlists(self):
         results = self.yt.get_user("UCPVhZsC2od1xjGhgEc2NEPQ")
         results = self.yt.get_user_playlists("UCPVhZsC2od1xjGhgEc2NEPQ",
-                                             results['playlists']['params'])
+                                             results["playlists"]["params"])
         self.assertGreater(len(results), 100)
 
     def test_get_album_browse_id(self):
         browse_id = self.yt.get_album_browse_id("OLAK5uy_nMr9h2VlS-2PULNz3M3XVXQj_P3C2bqaY")
         self.assertEqual(browse_id, sample_album)
 
     def test_get_album(self):
         results = self.yt_auth.get_album(sample_album)
         self.assertGreaterEqual(len(results), 9)
-        self.assertTrue(results['tracks'][0]['isExplicit'])
-        self.assertIn('feedbackTokens', results['tracks'][0])
-        self.assertEqual(len(results['other_versions']), 2)
+        self.assertTrue(results["tracks"][0]["isExplicit"])
+        self.assertIn("feedbackTokens", results["tracks"][0])
+        self.assertEqual(len(results["other_versions"]), 2)
         results = self.yt.get_album("MPREb_BQZvl3BFGay")
-        self.assertEqual(len(results['tracks']), 7)
+        self.assertEqual(len(results["tracks"]), 7)
 
     def test_get_song(self):
-        song = self.yt_oauth.get_song(config['uploads']['private_upload_id'])  # private upload
+        song = self.yt_oauth.get_song(config["uploads"]["private_upload_id"])  # private upload
         self.assertEqual(len(song), 5)
         song = self.yt.get_song(sample_video)
-        self.assertGreaterEqual(len(song['streamingData']['adaptiveFormats']), 10)
+        self.assertGreaterEqual(len(song["streamingData"]["adaptiveFormats"]), 10)
 
     def test_get_song_related_content(self):
         song = self.yt_oauth.get_watch_playlist(sample_video)
         song = self.yt_oauth.get_song_related(song["related"])
         self.assertGreaterEqual(len(song), 5)
 
     def test_get_lyrics(self):
         playlist = self.yt.get_watch_playlist(sample_video)
         lyrics_song = self.yt.get_lyrics(playlist["lyrics"])
         self.assertIsNotNone(lyrics_song["lyrics"])
         self.assertIsNotNone(lyrics_song["source"])
 
-        playlist = self.yt.get_watch_playlist(config['uploads']['private_upload_id'])
+        playlist = self.yt.get_watch_playlist(config["uploads"]["private_upload_id"])
         self.assertIsNone(playlist["lyrics"])
         self.assertRaises(Exception, self.yt.get_lyrics, playlist["lyrics"])
 
     def test_get_signatureTimestamp(self):
         signatureTimestamp = self.yt.get_signatureTimestamp()
         self.assertIsNotNone(signatureTimestamp)
 
@@ -238,253 +248,270 @@
         self.assertGreater(len(categories[cat]), 0)
         playlists = self.yt.get_mood_playlists(categories[cat][0]["params"])
         self.assertGreater(len(playlists), 0)
 
     def test_get_charts(self):
         charts = self.yt_oauth.get_charts()
         self.assertEqual(len(charts), 4)
-        charts = self.yt.get_charts(country='US')
+        charts = self.yt.get_charts(country="US")
         self.assertEqual(len(charts), 5)
-        charts = self.yt.get_charts(country='BE')
+        charts = self.yt.get_charts(country="BE")
         self.assertEqual(len(charts), 4)
 
     ###############
     # WATCH
     ###############
 
     def test_get_watch_playlist(self):
         playlist = self.yt_oauth.get_watch_playlist(
-            playlistId="RDAMPLOLAK5uy_l_fKDQGOUsk8kbWsm9s86n4-nZNd2JR8Q", radio=True, limit=90)
-        self.assertGreaterEqual(len(playlist['tracks']), 90)
+            playlistId="RDAMPLOLAK5uy_l_fKDQGOUsk8kbWsm9s86n4-nZNd2JR8Q",
+            radio=True,
+            limit=90,
+        )
+        self.assertGreaterEqual(len(playlist["tracks"]), 90)
         playlist = self.yt_oauth.get_watch_playlist("9mWr4c_ig54", limit=50)
-        self.assertGreater(len(playlist['tracks']), 45)
+        self.assertGreater(len(playlist["tracks"]), 45)
         playlist = self.yt_oauth.get_watch_playlist("UoAf_y9Ok4k")  # private track
-        self.assertGreaterEqual(len(playlist['tracks']), 25)
+        self.assertGreaterEqual(len(playlist["tracks"]), 25)
         playlist = self.yt.get_watch_playlist(
             playlistId="OLAK5uy_lKgoGvlrWhX0EIPavQUXxyPed8Cj38AWc", shuffle=True)
-        self.assertEqual(len(playlist['tracks']), 12)
-        playlist = self.yt_brand.get_watch_playlist(playlistId=config['playlists']['own'],
+        self.assertEqual(len(playlist["tracks"]), 12)
+        playlist = self.yt_brand.get_watch_playlist(playlistId=config["playlists"]["own"],
                                                     shuffle=True)
-        self.assertEqual(len(playlist['tracks']), 4)
+        self.assertEqual(len(playlist["tracks"]), 4)
 
     ################
     # LIBRARY
     ################
 
     def test_get_library_playlists(self):
         playlists = self.yt_oauth.get_library_playlists(50)
         self.assertGreater(len(playlists), 25)
 
         playlists = self.yt_auth.get_library_playlists(None)
-        self.assertGreaterEqual(len(playlists), config.getint('limits', 'library_playlists'))
+        self.assertGreaterEqual(len(playlists), config.getint("limits", "library_playlists"))
 
         playlists = self.yt_empty.get_library_playlists()
         self.assertLessEqual(len(playlists), 1)  # "Episodes saved for later"
 
     def test_get_library_songs(self):
         self.assertRaises(Exception, self.yt_auth.get_library_songs, None, True)
         songs = self.yt_oauth.get_library_songs(100)
         self.assertGreaterEqual(len(songs), 100)
         songs = self.yt_auth.get_library_songs(200, validate_responses=True)
-        self.assertGreaterEqual(len(songs), config.getint('limits', 'library_songs'))
-        songs = self.yt_auth.get_library_songs(order='a_to_z')
+        self.assertGreaterEqual(len(songs), config.getint("limits", "library_songs"))
+        songs = self.yt_auth.get_library_songs(order="a_to_z")
         self.assertGreaterEqual(len(songs), 25)
         songs = self.yt_empty.get_library_songs()
         self.assertEqual(len(songs), 0)
 
     def test_get_library_albums(self):
         albums = self.yt_oauth.get_library_albums(100)
         self.assertGreater(len(albums), 50)
         for album in albums:
-            self.assertIn('playlistId', album)
-        albums = self.yt_brand.get_library_albums(100, order='a_to_z')
+            self.assertIn("playlistId", album)
+        albums = self.yt_brand.get_library_albums(100, order="a_to_z")
         self.assertGreater(len(albums), 50)
-        albums = self.yt_brand.get_library_albums(100, order='z_to_a')
+        albums = self.yt_brand.get_library_albums(100, order="z_to_a")
         self.assertGreater(len(albums), 50)
-        albums = self.yt_brand.get_library_albums(100, order='recently_added')
+        albums = self.yt_brand.get_library_albums(100, order="recently_added")
         self.assertGreater(len(albums), 50)
         albums = self.yt_empty.get_library_albums()
         self.assertEqual(len(albums), 0)
 
     def test_get_library_artists(self):
         artists = self.yt_auth.get_library_artists(50)
         self.assertGreater(len(artists), 40)
-        artists = self.yt_oauth.get_library_artists(order='a_to_z', limit=50)
+        artists = self.yt_oauth.get_library_artists(order="a_to_z", limit=50)
         self.assertGreater(len(artists), 40)
         artists = self.yt_brand.get_library_artists(limit=None)
-        self.assertGreater(len(artists), config.getint('limits', 'library_artists'))
+        self.assertGreater(len(artists), config.getint("limits", "library_artists"))
         artists = self.yt_empty.get_library_artists()
         self.assertEqual(len(artists), 0)
 
     def test_get_library_subscriptions(self):
         artists = self.yt_brand.get_library_subscriptions(50)
         self.assertGreater(len(artists), 40)
-        artists = self.yt_brand.get_library_subscriptions(order='z_to_a')
+        artists = self.yt_brand.get_library_subscriptions(order="z_to_a")
         self.assertGreater(len(artists), 20)
         artists = self.yt_brand.get_library_subscriptions(limit=None)
-        self.assertGreater(len(artists), config.getint('limits', 'library_subscriptions'))
+        self.assertGreater(len(artists), config.getint("limits", "library_subscriptions"))
         artists = self.yt_empty.get_library_subscriptions()
         self.assertEqual(len(artists), 0)
 
     def test_get_liked_songs(self):
         songs = self.yt_brand.get_liked_songs(200)
-        self.assertGreater(len(songs['tracks']), 100)
+        self.assertGreater(len(songs["tracks"]), 100)
         songs = self.yt_empty.get_liked_songs()
-        self.assertEqual(songs['trackCount'], 0)
+        self.assertEqual(songs["trackCount"], 0)
 
     def test_get_history(self):
         songs = self.yt_oauth.get_history()
         self.assertGreater(len(songs), 0)
 
     def test_manipulate_history_items(self):
         song = self.yt_auth.get_song(sample_video)
         response = self.yt_auth.add_history_item(song)
         self.assertEqual(response.status_code, 204)
         songs = self.yt_auth.get_history()
         self.assertGreater(len(songs), 0)
-        response = self.yt_auth.remove_history_items([songs[0]['feedbackToken']])
-        self.assertIn('feedbackResponses', response)
+        response = self.yt_auth.remove_history_items([songs[0]["feedbackToken"]])
+        self.assertIn("feedbackResponses", response)
 
     def test_rate_song(self):
-        response = self.yt_auth.rate_song(sample_video, 'LIKE')
-        self.assertIn('actions', response)
-        response = self.yt_auth.rate_song(sample_video, 'INDIFFERENT')
-        self.assertIn('actions', response)
+        response = self.yt_auth.rate_song(sample_video, "LIKE")
+        self.assertIn("actions", response)
+        response = self.yt_auth.rate_song(sample_video, "INDIFFERENT")
+        self.assertIn("actions", response)
 
     def test_edit_song_library_status(self):
         album = self.yt_brand.get_album(sample_album)
         response = self.yt_brand.edit_song_library_status(
-            album['tracks'][2]['feedbackTokens']['add'])
-        self.assertTrue(response['feedbackResponses'][0]['isProcessed'])
+            album["tracks"][2]["feedbackTokens"]["add"])
+        self.assertTrue(response["feedbackResponses"][0]["isProcessed"])
         response = self.yt_brand.edit_song_library_status(
-            album['tracks'][2]['feedbackTokens']['remove'])
-        self.assertTrue(response['feedbackResponses'][0]['isProcessed'])
+            album["tracks"][2]["feedbackTokens"]["remove"])
+        self.assertTrue(response["feedbackResponses"][0]["isProcessed"])
 
     def test_rate_playlist(self):
-        response = self.yt_auth.rate_playlist('OLAK5uy_l3g4WcHZsEx_QuEDZzWEiyFzZl6pL0xZ4', 'LIKE')
-        self.assertIn('actions', response)
-        response = self.yt_auth.rate_playlist('OLAK5uy_l3g4WcHZsEx_QuEDZzWEiyFzZl6pL0xZ4',
-                                              'INDIFFERENT')
-        self.assertIn('actions', response)
+        response = self.yt_auth.rate_playlist("OLAK5uy_l3g4WcHZsEx_QuEDZzWEiyFzZl6pL0xZ4", "LIKE")
+        self.assertIn("actions", response)
+        response = self.yt_auth.rate_playlist("OLAK5uy_l3g4WcHZsEx_QuEDZzWEiyFzZl6pL0xZ4",
+                                              "INDIFFERENT")
+        self.assertIn("actions", response)
 
     def test_subscribe_artists(self):
-        self.yt_auth.subscribe_artists(['UCUDVBtnOQi4c7E8jebpjc9Q', 'UCiMhD4jzUqG-IgPzUmmytRQ'])
-        self.yt_auth.unsubscribe_artists(['UCUDVBtnOQi4c7E8jebpjc9Q', 'UCiMhD4jzUqG-IgPzUmmytRQ'])
+        self.yt_auth.subscribe_artists(["UCUDVBtnOQi4c7E8jebpjc9Q", "UCiMhD4jzUqG-IgPzUmmytRQ"])
+        self.yt_auth.unsubscribe_artists(["UCUDVBtnOQi4c7E8jebpjc9Q", "UCiMhD4jzUqG-IgPzUmmytRQ"])
 
     ###############
     # PLAYLISTS
     ###############
 
     def test_get_foreign_playlist(self):
         self.assertRaises(Exception, self.yt.get_playlist, "PLABC")
         playlist = self.yt.get_playlist(sample_playlist, limit=300, suggestions_limit=7)
-        self.assertGreater(len(playlist['tracks']), 200)
-        self.assertNotIn('suggestions', playlist)
+        self.assertGreater(len(playlist["tracks"]), 200)
+        self.assertNotIn("suggestions", playlist)
 
         playlist = self.yt.get_playlist("RDCLAK5uy_kpxnNxJpPZjLKbL9WgvrPuErWkUxMP6x4",
                                         limit=None,
                                         related=True)
-        self.assertGreater(len(playlist['tracks']), 100)
-        self.assertEqual(len(playlist['related']), 10)
+        self.assertGreater(len(playlist["tracks"]), 100)
+        self.assertEqual(len(playlist["related"]), 10)
 
     def test_get_owned_playlist(self):
-        playlist = self.yt_brand.get_playlist(config['playlists']['own'],
+        playlist = self.yt_brand.get_playlist(config["playlists"]["own"],
                                               related=True,
                                               suggestions_limit=21)
-        self.assertLess(len(playlist['tracks']), 100)
-        self.assertEqual(len(playlist['suggestions']), 21)
-        self.assertEqual(len(playlist['related']), 10)
+        self.assertLess(len(playlist["tracks"]), 100)
+        self.assertEqual(len(playlist["suggestions"]), 21)
+        self.assertEqual(len(playlist["related"]), 10)
 
     def test_edit_playlist(self):
-        playlist = self.yt_brand.get_playlist(config['playlists']['own'])
-        response = self.yt_brand.edit_playlist(playlist['id'],
-                                               title='',
-                                               description='',
-                                               privacyStatus='PRIVATE',
-                                               moveItem=(playlist['tracks'][1]['setVideoId'],
-                                                         playlist['tracks'][0]['setVideoId']))
-        self.assertEqual(response, 'STATUS_SUCCEEDED', "Playlist edit failed")
-        self.yt_brand.edit_playlist(playlist['id'],
-                                    title=playlist['title'],
-                                    description=playlist['description'],
-                                    privacyStatus=playlist['privacy'],
-                                    moveItem=(playlist['tracks'][0]['setVideoId'],
-                                              playlist['tracks'][1]['setVideoId']))
-        self.assertEqual(response, 'STATUS_SUCCEEDED', "Playlist edit failed")
+        playlist = self.yt_brand.get_playlist(config["playlists"]["own"])
+        response = self.yt_brand.edit_playlist(
+            playlist["id"],
+            title="",
+            description="",
+            privacyStatus="PRIVATE",
+            moveItem=(
+                playlist["tracks"][1]["setVideoId"],
+                playlist["tracks"][0]["setVideoId"],
+            ),
+        )
+        self.assertEqual(response, "STATUS_SUCCEEDED", "Playlist edit failed")
+        self.yt_brand.edit_playlist(
+            playlist["id"],
+            title=playlist["title"],
+            description=playlist["description"],
+            privacyStatus=playlist["privacy"],
+            moveItem=(
+                playlist["tracks"][0]["setVideoId"],
+                playlist["tracks"][1]["setVideoId"],
+            ),
+        )
+        self.assertEqual(response, "STATUS_SUCCEEDED", "Playlist edit failed")
 
     # end to end test adding playlist, adding item, deleting item, deleting playlist
     def test_end2end(self):
         playlistId = self.yt_brand.create_playlist(
             "test",
             "test description",
-            source_playlist="OLAK5uy_lGQfnMNGvYCRdDq9ZLzJV2BJL2aHQsz9Y")
+            source_playlist="OLAK5uy_lGQfnMNGvYCRdDq9ZLzJV2BJL2aHQsz9Y",
+        )
         self.assertEqual(len(playlistId), 34, "Playlist creation failed")
         response = self.yt_brand.add_playlist_items(
-            playlistId, [sample_video, sample_video],
-            source_playlist='OLAK5uy_nvjTE32aFYdFN7HCyMv3cGqD3wqBb4Jow',
-            duplicates=True)
-        self.assertEqual(response["status"], 'STATUS_SUCCEEDED', "Adding playlist item failed")
+            playlistId,
+            [sample_video, sample_video],
+            source_playlist="OLAK5uy_nvjTE32aFYdFN7HCyMv3cGqD3wqBb4Jow",
+            duplicates=True,
+        )
+        self.assertEqual(response["status"], "STATUS_SUCCEEDED", "Adding playlist item failed")
         self.assertGreater(len(response["playlistEditResults"]), 0, "Adding playlist item failed")
         time.sleep(2)
         playlist = self.yt_brand.get_playlist(playlistId, related=True)
-        self.assertEqual(len(playlist['tracks']), 46, "Getting playlist items failed")
-        response = self.yt_brand.remove_playlist_items(playlistId, playlist['tracks'])
-        self.assertEqual(response, 'STATUS_SUCCEEDED', "Playlist item removal failed")
+        self.assertEqual(len(playlist["tracks"]), 46, "Getting playlist items failed")
+        response = self.yt_brand.remove_playlist_items(playlistId, playlist["tracks"])
+        self.assertEqual(response, "STATUS_SUCCEEDED", "Playlist item removal failed")
         response = self.yt_brand.delete_playlist(playlistId)
-        self.assertEqual(response['command']['handlePlaylistDeletionCommand']['playlistId'],
-                         playlistId, "Playlist removal failed")
+        self.assertEqual(
+            response["command"]["handlePlaylistDeletionCommand"]["playlistId"],
+            playlistId,
+            "Playlist removal failed",
+        )
 
     ###############
     # UPLOADS
     ###############
 
     def test_get_library_upload_songs(self):
-        results = self.yt_oauth.get_library_upload_songs(50, order='z_to_a')
+        results = self.yt_oauth.get_library_upload_songs(50, order="z_to_a")
         self.assertGreater(len(results), 25)
 
         results = self.yt_empty.get_library_upload_songs(100)
         self.assertEqual(len(results), 0)
 
     def test_get_library_upload_albums(self):
-        results = self.yt_oauth.get_library_upload_albums(50, order='a_to_z')
+        results = self.yt_oauth.get_library_upload_albums(50, order="a_to_z")
         self.assertGreater(len(results), 40)
 
         albums = self.yt_auth.get_library_upload_albums(None)
-        self.assertGreaterEqual(len(albums), config.getint('limits', 'library_upload_albums'))
+        self.assertGreaterEqual(len(albums), config.getint("limits", "library_upload_albums"))
 
         results = self.yt_empty.get_library_upload_albums(100)
         self.assertEqual(len(results), 0)
 
     def test_get_library_upload_artists(self):
         artists = self.yt_oauth.get_library_upload_artists(None)
-        self.assertGreaterEqual(len(artists), config.getint('limits', 'library_upload_artists'))
+        self.assertGreaterEqual(len(artists), config.getint("limits", "library_upload_artists"))
 
-        results = self.yt_auth.get_library_upload_artists(50, order='recently_added')
+        results = self.yt_auth.get_library_upload_artists(50, order="recently_added")
         self.assertGreaterEqual(len(results), 25)
 
         results = self.yt_empty.get_library_upload_artists(100)
         self.assertEqual(len(results), 0)
 
     def test_upload_song(self):
-        self.assertRaises(Exception, self.yt_auth.upload_song, 'song.wav')
-        self.assertRaises(Exception, self.yt_oauth.upload_song, config['uploads']['file'])
-        response = self.yt_auth.upload_song(get_resource(config['uploads']['file']))
+        self.assertRaises(Exception, self.yt_auth.upload_song, "song.wav")
+        self.assertRaises(Exception, self.yt_oauth.upload_song, config["uploads"]["file"])
+        response = self.yt_auth.upload_song(get_resource(config["uploads"]["file"]))
         self.assertEqual(response.status_code, 409)
 
     @unittest.skip("Do not delete uploads")
     def test_delete_upload_entity(self):
         results = self.yt_oauth.get_library_upload_songs()
-        response = self.yt_oauth.delete_upload_entity(results[0]['entityId'])
-        self.assertEqual(response, 'STATUS_SUCCEEDED')
+        response = self.yt_oauth.delete_upload_entity(results[0]["entityId"])
+        self.assertEqual(response, "STATUS_SUCCEEDED")
 
     def test_get_library_upload_album(self):
-        album = self.yt_oauth.get_library_upload_album(config['uploads']['private_album_id'])
-        self.assertGreater(len(album['tracks']), 0)
+        album = self.yt_oauth.get_library_upload_album(config["uploads"]["private_album_id"])
+        self.assertGreater(len(album["tracks"]), 0)
 
     def test_get_library_upload_artist(self):
-        tracks = self.yt_oauth.get_library_upload_artist(config['uploads']['private_artist_id'],
+        tracks = self.yt_oauth.get_library_upload_artist(config["uploads"]["private_artist_id"],
                                                          100)
         self.assertGreater(len(tracks), 0)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ytmusicapi-1.0.0/ytmusicapi/auth/browser.py` & `ytmusicapi-1.0.1/ytmusicapi/auth/browser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 import os
 import platform
+
+from requests.structures import CaseInsensitiveDict
+
 from ytmusicapi.helpers import *
 
 path = os.path.dirname(os.path.realpath(__file__)) + os.sep
 
 
+def is_browser(headers: CaseInsensitiveDict) -> bool:
+    browser_structure = {"authorization", "cookie"}
+    return browser_structure.issubset(headers.keys())
+
+
 def setup_browser(filepath=None, headers_raw=None):
     contents = []
     if not headers_raw:
         eof = "Ctrl-D" if platform.system() != "Windows" else "'Enter, Ctrl-Z, Enter'"
-        print("Please paste the request headers from Firefox and press " + eof + " to continue:")
+        print(f"Please paste the request headers from Firefox and press {eof} to continue:")
         while True:
             try:
                 line = input()
             except EOFError:
                 break
             contents.append(line)
     else:
-        contents = headers_raw.split('\n')
+        contents = headers_raw.split("\n")
 
     try:
         user_headers = {}
         for content in contents:
-            header = content.split(': ')
+            header = content.split(": ")
             if len(header) == 1 or header[0].startswith(
                     ":"):  # nothing was split or chromium headers
                 continue
-            user_headers[header[0].lower()] = ': '.join(header[1:])
+            user_headers[header[0].lower()] = ": ".join(header[1:])
 
     except Exception as e:
-        raise Exception("Error parsing your input, please try again. Full error: " + str(e))
+        raise Exception(f"Error parsing your input, please try again. Full error: {e}") from e
 
     missing_headers = {"cookie", "x-goog-authuser"} - set(k.lower() for k in user_headers.keys())
     if missing_headers:
         raise Exception(
             "The following entries are missing in your headers: " + ", ".join(missing_headers)
             + ". Please try a different request (such as /browse) and make sure you are logged in."
         )
@@ -44,11 +52,11 @@
             user_headers.pop(key, None)
 
     init_headers = initialize_headers()
     user_headers.update(init_headers)
     headers = user_headers
 
     if filepath is not None:
-        with open(filepath, 'w') as file:
+        with open(filepath, "w") as file:
             json.dump(headers, file, ensure_ascii=True, indent=4, sort_keys=True)
 
     return json.dumps(headers)
```

### Comparing `ytmusicapi-1.0.0/ytmusicapi/auth/oauth.py` & `ytmusicapi-1.0.1/ytmusicapi/auth/oauth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,31 @@
+import json
 import time
 from typing import Dict, Optional
+
 import requests
-import json
+from requests.structures import CaseInsensitiveDict
 
-from ytmusicapi.constants import OAUTH_CLIENT_ID, OAUTH_CLIENT_SECRET, OAUTH_SCOPE, OAUTH_CODE_URL, OAUTH_TOKEN_URL, OAUTH_USER_AGENT
+from ytmusicapi.constants import (OAUTH_CLIENT_ID, OAUTH_CLIENT_SECRET,
+                                  OAUTH_CODE_URL, OAUTH_SCOPE, OAUTH_TOKEN_URL,
+                                  OAUTH_USER_AGENT)
 from ytmusicapi.helpers import initialize_headers
 
 
+def is_oauth(headers: CaseInsensitiveDict) -> bool:
+    oauth_structure = {
+        "access_token",
+        "expires_at",
+        "expires_in",
+        "token_type",
+        "refresh_token",
+    }
+    return oauth_structure.issubset(headers.keys())
+
+
 class YTMusicOAuth:
     """OAuth implementation for YouTube Music based on YouTube TV"""
 
     def __init__(self, session: requests.Session, proxies: Dict = None):
         self._session = session
         if proxies:
             self._session.proxies.update(proxies)
@@ -19,45 +34,48 @@
         data.update({"client_id": OAUTH_CLIENT_ID})
         headers = {"User-Agent": OAUTH_USER_AGENT}
         return self._session.post(url, data, headers=headers)
 
     def get_code(self) -> Dict:
         code_response = self._send_request(OAUTH_CODE_URL, data={"scope": OAUTH_SCOPE})
         response_json = code_response.json()
-        url = f"{response_json['verification_url']}?user_code={response_json['user_code']}"
-        input(f"Go to {url}, finish the login flow and press Enter when done, Ctrl-C to abort")
         return response_json
 
     def get_token_from_code(self, device_code: str) -> Dict:
-        token_response = self._send_request(OAUTH_TOKEN_URL,
-                                            data={
-                                                "client_secret": OAUTH_CLIENT_SECRET,
-                                                "grant_type":
-                                                "http://oauth.net/grant_type/device/1.0",
-                                                "code": device_code
-                                            })
+        token_response = self._send_request(
+            OAUTH_TOKEN_URL,
+            data={
+                "client_secret": OAUTH_CLIENT_SECRET,
+                "grant_type": "http://oauth.net/grant_type/device/1.0",
+                "code": device_code,
+            },
+        )
         return token_response.json()
 
     def refresh_token(self, refresh_token: str) -> Dict:
-        response = self._send_request(OAUTH_TOKEN_URL,
-                                      data={
-                                          "client_secret": OAUTH_CLIENT_SECRET,
-                                          "grant_type": "refresh_token",
-                                          "refresh_token": refresh_token
-                                      })
+        response = self._send_request(
+            OAUTH_TOKEN_URL,
+            data={
+                "client_secret": OAUTH_CLIENT_SECRET,
+                "grant_type": "refresh_token",
+                "refresh_token": refresh_token,
+            },
+        )
         return response.json()
 
     @staticmethod
     def dump_token(token, filepath):
         token["expires_at"] = int(time.time()) + int(token["expires_in"])
         with open(filepath, encoding="utf8", mode="w") as file:
             json.dump(token, file, indent=True)
 
     def setup(self, filepath: Optional[str] = None) -> Dict:
         code = self.get_code()
+        url = f"{code['verification_url']}?user_code={code['user_code']}"
+        input(f"Go to {url}, finish the login flow and press Enter when done, Ctrl-C to abort")
         token = self.get_token_from_code(code["device_code"])
         if filepath:
             self.dump_token(token, filepath)
 
         return token
 
     def load_headers(self, token: Dict, filepath: Optional[str] = None):
```

### Comparing `ytmusicapi-1.0.0/ytmusicapi/constants.py` & `ytmusicapi-1.0.1/ytmusicapi/constants.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/continuations.py` & `ytmusicapi-1.0.1/ytmusicapi/continuations.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/helpers.py` & `ytmusicapi-1.0.1/ytmusicapi/helpers.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/README.rst` & `ytmusicapi-1.0.1/ytmusicapi/locales/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/ar/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/ar/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/base.pot` & `ytmusicapi-1.0.1/ytmusicapi/locales/base.pot`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/de/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/en/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/en/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/es/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/es/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/es/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/fr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/fr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/hi/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/hi/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/it/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/it/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/it/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/ja/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/ja/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/ko/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/ko/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/pt/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/pt/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/ru/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/ru/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/tr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/tr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/ur/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/ur/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot` & `ytmusicapi-1.0.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po` & `ytmusicapi-1.0.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/mixins/_utils.py` & `ytmusicapi-1.0.1/ytmusicapi/mixins/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/mixins/browsing.py` & `ytmusicapi-1.0.1/ytmusicapi/mixins/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/mixins/explore.py` & `ytmusicapi-1.0.1/ytmusicapi/mixins/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/mixins/library.py` & `ytmusicapi-1.0.1/ytmusicapi/mixins/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/mixins/playlists.py` & `ytmusicapi-1.0.1/ytmusicapi/mixins/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/mixins/search.py` & `ytmusicapi-1.0.1/ytmusicapi/mixins/search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/mixins/uploads.py` & `ytmusicapi-1.0.1/ytmusicapi/mixins/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/mixins/watch.py` & `ytmusicapi-1.0.1/ytmusicapi/mixins/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/navigation.py` & `ytmusicapi-1.0.1/ytmusicapi/navigation.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/_utils.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/albums.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/albums.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/browsing.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/explore.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/i18n.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/i18n.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/library.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/playlists.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/search.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/songs.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/songs.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/uploads.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/parsers/watch.py` & `ytmusicapi-1.0.1/ytmusicapi/parsers/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/setup.py` & `ytmusicapi-1.0.1/ytmusicapi/setup.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi/ytmusic.py` & `ytmusicapi-1.0.1/ytmusicapi/ytmusic.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.0.0/ytmusicapi.egg-info/PKG-INFO` & `ytmusicapi-1.0.1/ytmusicapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.0.0/ytmusicapi.egg-info/SOURCES.txt` & `ytmusicapi-1.0.1/ytmusicapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

