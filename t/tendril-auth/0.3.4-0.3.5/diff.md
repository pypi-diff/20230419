# Comparing `tmp/tendril-auth-0.3.4.tar.gz` & `tmp/tendril-auth-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tendril-auth-0.3.4.tar", last modified: Tue Mar 28 18:08:24 2023, max compression
+gzip compressed data, was "tendril-auth-0.3.5.tar", last modified: Wed Apr 19 18:12:48 2023, max compression
```

## Comparing `tendril-auth-0.3.4.tar` & `tendril-auth-0.3.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3875 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.622493 tendril-auth-0.3.4/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.622493 tendril-auth-0.3.4/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.622493 tendril-auth-0.3.4/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-auth-0.3.4/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.622493 tendril-auth-0.3.4/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.622493 tendril-auth-0.3.4/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3253 2023-03-15 16:03:53.000000 tendril-auth-0.3.4/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.618494 tendril-auth-0.3.4/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.622493 tendril-auth-0.3.4/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.622493 tendril-auth-0.3.4/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.4/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.622493 tendril-auth-0.3.4/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.4/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1075 2023-02-18 10:30:44.000000 tendril-auth-0.3.4/src/tendril/apiserver/routers/authn.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/src/tendril/authn/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:59:41.000000 tendril-auth-0.3.4/src/tendril/authn/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5999 2023-03-15 16:03:53.000000 tendril-auth-0.3.4/src/tendril/authn/auth0.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/src/tendril/authn/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.4/src/tendril/authn/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril-auth-0.3.4/src/tendril/authn/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril-auth-0.3.4/src/tendril/authn/db/mixins.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril-auth-0.3.4/src/tendril/authn/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1155 2023-03-15 16:03:53.000000 tendril-auth-0.3.4/src/tendril/authn/pydantic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2795 2023-03-15 16:03:53.000000 tendril-auth-0.3.4/src/tendril/authn/users.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril-auth-0.3.4/src/tendril/authz/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1508 2023-02-28 00:23:46.000000 tendril-auth-0.3.4/src/tendril/authz/auth0.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril-auth-0.3.4/src/tendril/authz/connector.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril-auth-0.3.4/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril-auth-0.3.4/src/tendril/authz/scopes/common.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1357 2023-02-28 00:59:55.000000 tendril-auth-0.3.4/src/tendril/authz/scopes/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-auth-0.3.4/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2708 2023-03-28 18:07:23.000000 tendril-auth-0.3.4/src/tendril/config/auth.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/src/tendril_auth.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3875 2023-03-28 18:08:24.000000 tendril-auth-0.3.4/src/tendril_auth.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1242 2023-03-28 18:08:24.000000 tendril-auth-0.3.4/src/tendril_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-03-28 18:08:24.000000 tendril-auth-0.3.4/src/tendril_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2023-03-28 18:08:24.000000 tendril-auth-0.3.4/src/tendril_auth.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-03-28 18:08:24.000000 tendril-auth-0.3.4/src/tendril_auth.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:08:24.626492 tendril-auth-0.3.4/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril-auth-0.3.4/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.532154 tendril-auth-0.3.5/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2023-04-19 18:12:48.532154 tendril-auth-0.3.5/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.492155 tendril-auth-0.3.5/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.500155 tendril-auth-0.3.5/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.500155 tendril-auth-0.3.5/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-auth-0.3.5/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.500155 tendril-auth-0.3.5/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.504155 tendril-auth-0.3.5/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-19 18:12:48.536154 tendril-auth-0.3.5/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3253 2023-03-15 16:03:53.000000 tendril-auth-0.3.5/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.468155 tendril-auth-0.3.5/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.504155 tendril-auth-0.3.5/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.504155 tendril-auth-0.3.5/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.5/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.508155 tendril-auth-0.3.5/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.5/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1075 2023-02-18 10:30:44.000000 tendril-auth-0.3.5/src/tendril/apiserver/routers/authn.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.512155 tendril-auth-0.3.5/src/tendril/authn/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:59:41.000000 tendril-auth-0.3.5/src/tendril/authn/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5999 2023-03-15 16:03:53.000000 tendril-auth-0.3.5/src/tendril/authn/auth0.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.516155 tendril-auth-0.3.5/src/tendril/authn/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.5/src/tendril/authn/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril-auth-0.3.5/src/tendril/authn/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril-auth-0.3.5/src/tendril/authn/db/mixins.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril-auth-0.3.5/src/tendril/authn/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1193 2023-04-19 17:58:24.000000 tendril-auth-0.3.5/src/tendril/authn/pydantic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2800 2023-04-19 15:44:25.000000 tendril-auth-0.3.5/src/tendril/authn/users.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.520155 tendril-auth-0.3.5/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril-auth-0.3.5/src/tendril/authz/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1508 2023-02-28 00:23:46.000000 tendril-auth-0.3.5/src/tendril/authz/auth0.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril-auth-0.3.5/src/tendril/authz/connector.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.524155 tendril-auth-0.3.5/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril-auth-0.3.5/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril-auth-0.3.5/src/tendril/authz/scopes/common.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1357 2023-02-28 00:59:55.000000 tendril-auth-0.3.5/src/tendril/authz/scopes/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.524155 tendril-auth-0.3.5/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-auth-0.3.5/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2708 2023-03-28 18:07:23.000000 tendril-auth-0.3.5/src/tendril/config/auth.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.528154 tendril-auth-0.3.5/src/tendril_auth.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2023-04-19 18:12:47.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1242 2023-04-19 18:12:48.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-19 18:12:47.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2023-04-19 18:12:47.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-19 18:12:47.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.532154 tendril-auth-0.3.5/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/tox.ini
```

### Comparing `tendril-auth-0.3.4/.gitignore` & `tendril-auth-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/.readthedocs.yml` & `tendril-auth-0.3.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/.travis.yml` & `tendril-auth-0.3.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/LICENSE` & `tendril-auth-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/PKG-INFO` & `tendril-auth-0.3.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-auth
-Version: 0.3.4
+Version: 0.3.5
 Summary: Authentication and User Management Core for Tendril
 Home-page: https://github.com/tendril-framework/tendril-auth
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-auth.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-auth/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-auth
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-auth.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-auth
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-auth.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-auth
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-auth.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-auth
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-auth.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-auth
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-auth
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-auth.svg
-            :target: https://requires.io/github/tendril-framework/tendril-auth/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-auth.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-auth.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-auth>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-auth`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-auth`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-auth.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-auth
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-auth.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-auth
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-auth.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-auth
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-auth.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-auth
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-auth
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-auth.svg
+    :target: https://requires.io/github/tendril-framework/tendril-auth/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-auth.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-auth.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-auth>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-auth`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-auth`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-auth-0.3.4/README.rst` & `tendril-auth-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/docs/Makefile` & `tendril-auth-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/docs/_static/custom.css` & `tendril-auth-0.3.5/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/docs/_static/favicon.ico` & `tendril-auth-0.3.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/docs/_static/logo.png` & `tendril-auth-0.3.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/docs/_static/logo_packed.png` & `tendril-auth-0.3.5/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/docs/_templates/about.html` & `tendril-auth-0.3.5/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/docs/conf.py` & `tendril-auth-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/docs/index.rst` & `tendril-auth-0.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/docs/installation.rst` & `tendril-auth-0.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/setup.py` & `tendril-auth-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril/apiserver/routers/authn.py` & `tendril-auth-0.3.5/src/tendril/apiserver/routers/authn.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril/authn/auth0.py` & `tendril-auth-0.3.5/src/tendril/authn/auth0.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril/authn/db/controller.py` & `tendril-auth-0.3.5/src/tendril/authn/db/controller.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril/authn/db/model.py` & `tendril-auth-0.3.5/src/tendril/authn/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril/authn/pydantic.py` & `tendril-auth-0.3.5/src/tendril/authn/pydantic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 
 from typing import Union
+from typing import Optional
 
 from pydantic import Field
 from pydantic import HttpUrl
 from pydantic import validator
 from pydantic import create_model
 
 from tendril.utils.pydantic import TendrilTBaseModel
@@ -29,15 +30,15 @@
 
 def UserStubTMixin(inp='puid', out='user'):
     validators = {
         'expand_user_stub':
         validator('puid', pre=True)(_expand_user_stub)
     }
     kwargs = {
-        inp : (UserStubTModel, Field(..., alias=out)),
+        inp: (Optional[UserStubTModel], Field(None, alias=out)),
         '__base__': TendrilTBaseModel,
         '__validators__': validators
     }
     _inner = create_model(
         f'UserStubTModel_{inp}_{out}',
         **kwargs
     )
```

### Comparing `tendril-auth-0.3.4/src/tendril/authn/users.py` & `tendril-auth-0.3.5/src/tendril/authn/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def get_user_profile(user):
     user = preprocess_user(user)
     profile = {}
     profile[provider_name] = get_provider_user_profile(user)
     return profile
 
 
-def expand_user_stub(cls, v):
+def expand_user_stub(v, **kwargs):
     if isinstance(v, str):
         return get_user_stub(v)
     return v
 
 
 def get_user_stub(user):
     user = preprocess_user(user)
```

### Comparing `tendril-auth-0.3.4/src/tendril/authz/auth0.py` & `tendril-auth-0.3.5/src/tendril/authz/auth0.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril/authz/connector.py` & `tendril-auth-0.3.5/src/tendril/authz/connector.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril/authz/scopes/manager.py` & `tendril-auth-0.3.5/src/tendril/authz/scopes/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril/config/__init__.py` & `tendril-auth-0.3.5/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril/config/auth.py` & `tendril-auth-0.3.5/src/tendril/config/auth.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril_auth.egg-info/PKG-INFO` & `tendril-auth-0.3.5/src/tendril_auth.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-auth
-Version: 0.3.4
+Version: 0.3.5
 Summary: Authentication and User Management Core for Tendril
 Home-page: https://github.com/tendril-framework/tendril-auth
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-auth.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-auth/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-auth
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-auth.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-auth
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-auth.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-auth
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-auth.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-auth
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-auth.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-auth
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-auth
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-auth.svg
-            :target: https://requires.io/github/tendril-framework/tendril-auth/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-auth.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-auth.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-auth>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-auth`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-auth`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-auth.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-auth
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-auth.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-auth
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-auth.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-auth
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-auth.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-auth
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-auth
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-auth.svg
+    :target: https://requires.io/github/tendril-framework/tendril-auth/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-auth.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-auth.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-auth>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-auth`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-auth`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-auth-0.3.4/src/tendril_auth.egg-info/SOURCES.txt` & `tendril-auth-0.3.5/src/tendril_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/src/tendril_auth.egg-info/requires.txt` & `tendril-auth-0.3.5/src/tendril_auth.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/tests/coveralls.py` & `tendril-auth-0.3.5/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.4/tox.ini` & `tendril-auth-0.3.5/tox.ini`

 * *Files identical despite different names*

