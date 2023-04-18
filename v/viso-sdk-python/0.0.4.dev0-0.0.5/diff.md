# Comparing `tmp/viso-sdk-python-0.0.4.dev0.tar.gz` & `tmp/viso-sdk-python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viso-sdk-python-0.0.4.dev0.tar", last modified: Wed Apr 12 19:12:42 2023, max compression
+gzip compressed data, was "viso-sdk-python-0.0.5.tar", last modified: Tue Apr 18 22:38:13 2023, max compression
```

## Comparing `viso-sdk-python-0.0.4.dev0.tar` & `viso-sdk-python-0.0.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.110322 viso-sdk-python-0.0.4.dev0/
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-12 13:24:47.000000 viso-sdk-python-0.0.4.dev0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)       45 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     7651 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/COPYING
--rw-r--r--   0 root         (0) root         (0)      173 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-12 19:12:42.110322 viso-sdk-python-0.0.4.dev0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      313 2023-04-12 13:24:36.000000 viso-sdk-python-0.0.4.dev0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.090322 viso-sdk-python-0.0.4.dev0/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7128 2023-04-12 13:25:04.000000 viso-sdk-python-0.0.4.dev0/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.090322 viso-sdk-python-0.0.4.dev0/docs/ext/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/docs/ext/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1407 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/docs/ext/docstrings.py
--rw-r--r--   0 root         (0) root         (0)      816 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/docs/ext/manager_tmpl.j2
--rw-r--r--   0 root         (0) root         (0)      461 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      800 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     1023 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/docs/viso.rst
--rw-r--r--   0 root         (0) root         (0)       31 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)      139 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/requirements-docker.txt
--rw-r--r--   0 root         (0) root         (0)      124 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/requirements-docs.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/requirements-lint.txt
--rw-r--r--   0 root         (0) root         (0)       74 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/requirements-test.txt
--rw-r--r--   0 root         (0) root         (0)      454 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-12 19:12:42.120323 viso-sdk-python-0.0.4.dev0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2527 2023-04-12 18:45:34.000000 viso-sdk-python-0.0.4.dev0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.090322 viso-sdk-python-0.0.4.dev0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      214 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.090322 viso-sdk-python-0.0.4.dev0/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)     3314 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/tests/fixtures/flow.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.090322 viso-sdk-python-0.0.4.dev0/tests/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/tests/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-04-12 13:24:47.000000 viso-sdk-python-0.0.4.dev0/tests/meta/test_ensure_type_hints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.090322 viso-sdk-python-0.0.4.dev0/tests/smoke/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/tests/smoke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-12 13:24:47.000000 viso-sdk-python-0.0.4.dev0/tests/smoke/test_dists.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-04-12 13:24:47.000000 viso-sdk-python-0.0.4.dev0/tests/test_flow.py
--rw-r--r--   0 root         (0) root         (0)     1544 2023-04-12 13:24:47.000000 viso-sdk-python-0.0.4.dev0/tests/test_status.py
--rw-r--r--   0 root         (0) root         (0)     2083 2022-09-30 08:24:28.000000 viso-sdk-python-0.0.4.dev0/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.100322 viso-sdk-python-0.0.4.dev0/viso_sdk/
--rw-r--r--   0 root         (0) root         (0)   128282 2023-04-12 18:46:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/__init__.c
--rw-r--r--   0 root         (0) root         (0)     1131 2023-04-12 13:24:47.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)   139031 2023-04-12 18:46:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/_version.c
--rw-r--r--   0 root         (0) root         (0)      373 2023-04-12 13:24:47.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.100322 viso-sdk-python-0.0.4.dev0/viso_sdk/constants/
--rw-r--r--   0 root         (0) root         (0)   134253 2023-04-12 18:46:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/constants/__init__.c
--rw-r--r--   0 root         (0) root         (0)      278 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/constants/__init__.py
--rw-r--r--   0 root         (0) root         (0)   168423 2023-04-12 18:46:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/constants/constants.c
--rw-r--r--   0 root         (0) root         (0)     2697 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/constants/constants.py
--rw-r--r--   0 root         (0) root         (0)   122038 2023-04-12 18:46:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/constants/modules.c
--rw-r--r--   0 root         (0) root         (0)      244 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/constants/modules.py
--rw-r--r--   0 root         (0) root         (0)   219738 2023-04-12 18:46:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/constants/variables.c
--rw-r--r--   0 root         (0) root         (0)     1502 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/constants/variables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.100322 viso-sdk-python-0.0.4.dev0/viso_sdk/edge/
--rw-r--r--   0 root         (0) root         (0)   108989 2023-04-12 18:46:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/edge/__init__.c
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/edge/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312878 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/edge/common.c
--rw-r--r--   0 root         (0) root         (0)     2435 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/edge/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.100322 viso-sdk-python-0.0.4.dev0/viso_sdk/logging/
--rw-r--r--   0 root         (0) root         (0)   114597 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/logging/__init__.c
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)   275645 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/logging/logger.c
--rw-r--r--   0 root         (0) root         (0)     3434 2023-04-12 18:33:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/logging/logger.py
--rw-r--r--   0 root         (0) root         (0)   356104 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/logging/status_logger.c
--rw-r--r--   0 root         (0) root         (0)     4603 2023-04-11 17:52:25.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/logging/status_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.110322 viso-sdk-python-0.0.4.dev0/viso_sdk/mqtt/
--rw-r--r--   0 root         (0) root         (0)   113135 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/mqtt/__init__.c
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/mqtt/__init__.py
--rw-r--r--   0 root         (0) root         (0)   321219 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/mqtt/mqtt_wrapper.c
--rw-r--r--   0 root         (0) root         (0)     3414 2023-04-12 18:33:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/mqtt/mqtt_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.110322 viso-sdk-python-0.0.4.dev0/viso_sdk/nodered/
--rw-r--r--   0 root         (0) root         (0)   113205 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/nodered/__init__.c
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/nodered/__init__.py
--rw-r--r--   0 root         (0) root         (0)   377549 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/nodered/flow.c
--rw-r--r--   0 root         (0) root         (0)     5613 2023-04-12 18:33:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/nodered/flow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.110322 viso-sdk-python-0.0.4.dev0/viso_sdk/redis/
--rw-r--r--   0 root         (0) root         (0)   113197 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/redis/__init__.c
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)   365685 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/redis/redis_wrapper.c
--rw-r--r--   0 root         (0) root         (0)     4358 2023-04-12 18:33:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/redis/redis_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.110322 viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/
--rw-r--r--   0 root         (0) root         (0)   113212 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/__init__.c
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)   244344 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/custom_font.c
--rw-r--r--   0 root         (0) root         (0)     2861 2023-04-12 18:33:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/custom_font.py
--rw-r--r--   0 root         (0) root         (0)   378258 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/palette.c
--rw-r--r--   0 root         (0) root         (0)     2400 2023-04-06 19:14:45.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/palette.py
--rw-r--r--   0 root         (0) root         (0)   472190 2023-04-12 18:46:52.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/visualization.c
--rw-r--r--   0 root         (0) root         (0)     7621 2023-04-12 18:33:51.000000 viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:12:42.110322 viso-sdk-python-0.0.4.dev0/viso_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-12 19:12:42.000000 viso-sdk-python-0.0.4.dev0/viso_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1959 2023-04-12 19:12:42.000000 viso-sdk-python-0.0.4.dev0/viso_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 19:12:42.000000 viso-sdk-python-0.0.4.dev0/viso_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-04-12 19:12:42.000000 viso-sdk-python-0.0.4.dev0/viso_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-12 19:12:42.000000 viso-sdk-python-0.0.4.dev0/viso_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.026826 viso-sdk-python-0.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-04-18 22:38:13.026826 viso-sdk-python-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.993823 viso-sdk-python-0.0.5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7128 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.994823 viso-sdk-python-0.0.5/docs/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/ext/docstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/ext/manager_tmpl.j2
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/docs/viso.rst
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-docker.txt
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-docs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-lint.txt
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-18 22:38:13.027826 viso-sdk-python-0.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.996823 viso-sdk-python-0.0.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.996823 viso-sdk-python-0.0.5/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/fixtures/flow.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.997823 viso-sdk-python-0.0.5/tests/meta/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/meta/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/meta/test_ensure_type_hints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:12.997823 viso-sdk-python-0.0.5/tests/smoke/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/smoke/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/smoke/test_dists.py
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/test_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tests/test_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.002824 viso-sdk-python-0.0.5/viso_sdk/
+-rw-r--r--   0 root         (0) root         (0)   128282 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138995 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/_version.c
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.007825 viso-sdk-python-0.0.5/viso_sdk/constants/
+-rw-r--r--   0 root         (0) root         (0)   134253 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/constants/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/constants/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   168423 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/constants/constants.c
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/constants/constants.py
+-rw-r--r--   0 root         (0) root         (0)   122038 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/constants/modules.c
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/constants/modules.py
+-rw-r--r--   0 root         (0) root         (0)   219738 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/constants/variables.c
+-rw-rw-rw-   0 root         (0) root         (0)     1502 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/constants/variables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.009825 viso-sdk-python-0.0.5/viso_sdk/edge/
+-rw-r--r--   0 root         (0) root         (0)   108989 2023-04-18 22:38:11.000000 viso-sdk-python-0.0.5/viso_sdk/edge/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/edge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312878 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/edge/common.c
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/edge/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.013825 viso-sdk-python-0.0.5/viso_sdk/logging/
+-rw-r--r--   0 root         (0) root         (0)   114597 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/logging/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   275645 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/logging/logger.c
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/logging/logger.py
+-rw-r--r--   0 root         (0) root         (0)   356104 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/logging/status_logger.c
+-rw-rw-rw-   0 root         (0) root         (0)     4603 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/logging/status_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.015825 viso-sdk-python-0.0.5/viso_sdk/mqtt/
+-rw-r--r--   0 root         (0) root         (0)   113135 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/mqtt/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/mqtt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   353758 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/mqtt/mqtt_wrapper.c
+-rw-rw-rw-   0 root         (0) root         (0)     3802 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/mqtt/mqtt_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.017825 viso-sdk-python-0.0.5/viso_sdk/nodered/
+-rw-r--r--   0 root         (0) root         (0)   113205 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/nodered/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/nodered/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   377549 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/nodered/flow.c
+-rw-rw-rw-   0 root         (0) root         (0)     5613 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/nodered/flow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.019826 viso-sdk-python-0.0.5/viso_sdk/redis/
+-rw-r--r--   0 root         (0) root         (0)   113197 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/redis/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   387846 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/redis/redis_wrapper.c
+-rw-rw-rw-   0 root         (0) root         (0)     4636 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/redis/redis_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.024826 viso-sdk-python-0.0.5/viso_sdk/visualize/
+-rw-r--r--   0 root         (0) root         (0)   113212 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   244344 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/custom_font.c
+-rw-rw-rw-   0 root         (0) root         (0)     2861 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/custom_font.py
+-rw-r--r--   0 root         (0) root         (0)   378258 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/palette.c
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/palette.py
+-rw-r--r--   0 root         (0) root         (0)   472190 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/visualization.c
+-rw-rw-rw-   0 root         (0) root         (0)     7621 2023-04-18 22:37:57.000000 viso-sdk-python-0.0.5/viso_sdk/visualize/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:38:13.026826 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-18 22:38:12.000000 viso-sdk-python-0.0.5/viso_sdk_python.egg-info/top_level.txt
```

### Comparing `viso-sdk-python-0.0.4.dev0/COPYING` & `viso-sdk-python-0.0.5/COPYING`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/PKG-INFO` & `viso-sdk-python-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,15 @@
 Metadata-Version: 2.1
 Name: viso-sdk-python
-Version: 0.0.4.dev0
-Summary: VisoSDK: A SDK in Python for viso containers
+Version: 0.0.5
+Summary: VisoSDK: A Python SDK for use in Viso containers
 Home-page: https://gitlab.com/TopKamera/03_edge/Base/viso-sdk-python-public.git
 Author: support@viso.ai
 Author-email: support@viso.ai
 License: LGPLv3
-Description: # viso-sdk-python
-        
-        **viso-sdk-python** is a utility for [viso.ai](https://viso.ai) containers.
-        
-        ## Installation
-        
-        Use `pip` to install the latest stable version of **viso-sdk-python**:
-        
-        ```shell
-        pip install viso-sdk-python
-        ```
-        
-        
-        ## Build
-        ```shell
-        python3 -m pip install -e .
-        python3 setup.py sdist bdist_wheel
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
@@ -36,7 +17,30 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: AUTHORS
+
+# viso-sdk-python
+
+**viso-sdk-python** is a utility for [viso.ai](https://viso.ai) containers.
+
+## Installation
+
+Use `pip` to install the latest stable version of **viso-sdk-python**:
+
+```shell
+pip install viso-sdk-python
+```
+
+
+## Build
+```shell
+python3 -m pip install -e .
+python3 setup.py sdist bdist_wheel
+```
+
+
```

### Comparing `viso-sdk-python-0.0.4.dev0/docs/Makefile` & `viso-sdk-python-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/docs/conf.py` & `viso-sdk-python-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/docs/ext/docstrings.py` & `viso-sdk-python-0.0.5/docs/ext/docstrings.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/docs/ext/manager_tmpl.j2` & `viso-sdk-python-0.0.5/docs/ext/manager_tmpl.j2`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/docs/make.bat` & `viso-sdk-python-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/docs/viso.rst` & `viso-sdk-python-0.0.5/docs/viso.rst`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/setup.py` & `viso-sdk-python-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="viso-sdk-python",
     cmdclass=get_cmdclass(),
     version=__version__,
-    description="VisoSDK: A SDK in Python for viso containers",
+    description="VisoSDK: A Python SDK for use in Viso containers",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="support@viso.ai",
     author_email="support@viso.ai",
     # choose license
     license="LGPLv3",
     url="https://gitlab.com/TopKamera/03_edge/Base/viso-sdk-python-public.git",
```

### Comparing `viso-sdk-python-0.0.4.dev0/tests/fixtures/flow.json` & `viso-sdk-python-0.0.5/tests/fixtures/flow.json`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/tests/meta/test_ensure_type_hints.py` & `viso-sdk-python-0.0.5/tests/meta/test_ensure_type_hints.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/tests/smoke/test_dists.py` & `viso-sdk-python-0.0.5/tests/smoke/test_dists.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/tests/test_flow.py` & `viso-sdk-python-0.0.5/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/tests/test_status.py` & `viso-sdk-python-0.0.5/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/tox.ini` & `viso-sdk-python-0.0.5/tox.ini`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/__init__.c` & `viso-sdk-python-0.0.5/viso_sdk/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/__init__.py` & `viso-sdk-python-0.0.5/viso_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/_version.c` & `viso-sdk-python-0.0.5/viso_sdk/_version.c`

 * *Files 0% similar despite different names*

```diff
@@ -1289,35 +1289,35 @@
 static const char __pyx_k_now[] = "now";
 static const char __pyx_k_file[] = "__file__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_path[] = "path";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_year[] = "year";
+static const char __pyx_k_0_0_5[] = "0.0.5";
 static const char __pyx_k_LGPL3[] = "LGPL3";
 static const char __pyx_k_email[] = "__email__";
 static const char __pyx_k_title[] = "__title__";
 static const char __pyx_k_author[] = "__author__";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_abspath[] = "abspath";
 static const char __pyx_k_cur_dir[] = "_cur_dir";
 static const char __pyx_k_dirname[] = "dirname";
 static const char __pyx_k_license[] = "__license__";
 static const char __pyx_k_version[] = "__version__";
 static const char __pyx_k_datetime[] = "datetime";
-static const char __pyx_k_0_0_4_dev[] = "0.0.4.dev";
 static const char __pyx_k_copyright[] = "__copyright__";
 static const char __pyx_k_Viso_ai_team[] = "Viso.ai team";
 static const char __pyx_k_Constant_file[] = "\n    Constant file\n";
 static const char __pyx_k_Copyright_2020[] = "Copyright 2020-";
 static const char __pyx_k_viso_sdk_python[] = "viso-sdk-python";
 static const char __pyx_k_s_carlyon_viso_ai[] = "s.carlyon@viso.ai";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_viso_ai_AG_info_viso_ai[] = " viso.ai AG <info@viso.ai>";
-static PyObject *__pyx_kp_u_0_0_4_dev;
+static PyObject *__pyx_kp_u_0_0_5;
 static PyObject *__pyx_kp_u_Copyright_2020;
 static PyObject *__pyx_n_u_LGPL3;
 static PyObject *__pyx_kp_u_Viso_ai_team;
 static PyObject *__pyx_n_s_abspath;
 static PyObject *__pyx_n_s_author;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_copyright;
@@ -1384,15 +1384,15 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_0_0_4_dev, __pyx_k_0_0_4_dev, sizeof(__pyx_k_0_0_4_dev), 0, 1, 0, 0},
+  {&__pyx_kp_u_0_0_5, __pyx_k_0_0_5, sizeof(__pyx_k_0_0_5), 0, 1, 0, 0},
   {&__pyx_kp_u_Copyright_2020, __pyx_k_Copyright_2020, sizeof(__pyx_k_Copyright_2020), 0, 1, 0, 0},
   {&__pyx_n_u_LGPL3, __pyx_k_LGPL3, sizeof(__pyx_k_LGPL3), 0, 1, 0, 1},
   {&__pyx_kp_u_Viso_ai_team, __pyx_k_Viso_ai_team, sizeof(__pyx_k_Viso_ai_team), 0, 1, 0, 0},
   {&__pyx_n_s_abspath, __pyx_k_abspath, sizeof(__pyx_k_abspath), 0, 0, 1, 1},
   {&__pyx_n_s_author, __pyx_k_author, sizeof(__pyx_k_author), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_copyright, __pyx_k_copyright, sizeof(__pyx_k_copyright), 0, 0, 1, 1},
@@ -1870,24 +1870,24 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_license, __pyx_n_u_LGPL3) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
 
   /* "viso_sdk/_version.py":15
  * __email__ = "s.carlyon@viso.ai"
  * __license__ = "LGPL3"
  * __title__ = "viso-sdk-python"             # <<<<<<<<<<<<<<
  * 
- * __version__ = "0.0.4.dev"
+ * __version__ = "0.0.5"
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_title, __pyx_kp_u_viso_sdk_python) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
 
   /* "viso_sdk/_version.py":17
  * __title__ = "viso-sdk-python"
  * 
- * __version__ = "0.0.4.dev"             # <<<<<<<<<<<<<<
+ * __version__ = "0.0.5"             # <<<<<<<<<<<<<<
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_0_4_dev) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_0_5) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
 
   /* "viso_sdk/_version.py":1
  * """             # <<<<<<<<<<<<<<
  *     Constant file
  * """
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
```

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/constants/__init__.c` & `viso-sdk-python-0.0.5/viso_sdk/constants/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/constants/constants.c` & `viso-sdk-python-0.0.5/viso_sdk/constants/constants.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/constants/constants.py` & `viso-sdk-python-0.0.5/viso_sdk/constants/constants.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/constants/modules.c` & `viso-sdk-python-0.0.5/viso_sdk/constants/modules.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/constants/variables.c` & `viso-sdk-python-0.0.5/viso_sdk/constants/variables.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/constants/variables.py` & `viso-sdk-python-0.0.5/viso_sdk/constants/variables.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/edge/__init__.c` & `viso-sdk-python-0.0.5/viso_sdk/edge/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/edge/common.c` & `viso-sdk-python-0.0.5/viso_sdk/edge/common.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/edge/common.py` & `viso-sdk-python-0.0.5/viso_sdk/edge/common.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/logging/__init__.c` & `viso-sdk-python-0.0.5/viso_sdk/logging/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/logging/logger.c` & `viso-sdk-python-0.0.5/viso_sdk/logging/logger.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/logging/logger.py` & `viso-sdk-python-0.0.5/viso_sdk/logging/logger.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/logging/status_logger.c` & `viso-sdk-python-0.0.5/viso_sdk/logging/status_logger.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/logging/status_logger.py` & `viso-sdk-python-0.0.5/viso_sdk/logging/status_logger.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/mqtt/__init__.c` & `viso-sdk-python-0.0.5/viso_sdk/mqtt/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/mqtt/mqtt_wrapper.c` & `viso-sdk-python-0.0.5/viso_sdk/mqtt/mqtt_wrapper.c`

 * *Files 2% similar despite different names*

```diff
@@ -1165,14 +1165,43 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
+/* PyObjectFormatSimple.proto */
+#if CYTHON_COMPILING_IN_PYPY
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#elif PY_MAJOR_VERSION < 3
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyString_CheckExact(s)) ? PyUnicode_FromEncodedObject(s, NULL, "strict") :\
+        PyObject_Format(s, f))
+#elif CYTHON_USE_TYPE_SLOTS
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyLong_CheckExact(s)) ? PyLong_Type.tp_str(s) :\
+        likely(PyFloat_CheckExact(s)) ? PyFloat_Type.tp_str(s) :\
+        PyObject_Format(s, f))
+#else
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* JoinPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1208,43 +1237,14 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
-/* PyObjectFormatSimple.proto */
-#if CYTHON_COMPILING_IN_PYPY
-    #define __Pyx_PyObject_FormatSimple(s, f) (\
-        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
-        PyObject_Format(s, f))
-#elif PY_MAJOR_VERSION < 3
-    #define __Pyx_PyObject_FormatSimple(s, f) (\
-        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
-        likely(PyString_CheckExact(s)) ? PyUnicode_FromEncodedObject(s, NULL, "strict") :\
-        PyObject_Format(s, f))
-#elif CYTHON_USE_TYPE_SLOTS
-    #define __Pyx_PyObject_FormatSimple(s, f) (\
-        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
-        likely(PyLong_CheckExact(s)) ? PyLong_Type.tp_str(s) :\
-        likely(PyFloat_CheckExact(s)) ? PyFloat_Type.tp_str(s) :\
-        PyObject_Format(s, f))
-#else
-    #define __Pyx_PyObject_FormatSimple(s, f) (\
-        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
-        PyObject_Format(s, f))
-#endif
-
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* JoinPyUnicode.proto */
-static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
-                                      Py_UCS4 max_char);
-
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
@@ -1518,18 +1518,20 @@
 
 /* Module declarations from 'viso_sdk.mqtt.mqtt_wrapper' */
 #define __Pyx_MODULE_NAME "viso_sdk.mqtt.mqtt_wrapper"
 extern int __pyx_module_is_main_viso_sdk__mqtt__mqtt_wrapper;
 int __pyx_module_is_main_viso_sdk__mqtt__mqtt_wrapper = 0;
 
 /* Implementation of 'viso_sdk.mqtt.mqtt_wrapper' */
+static PyObject *__pyx_builtin_staticmethod;
 static PyObject *__pyx_builtin_super;
-static const char __pyx_k_[] = ":";
-static const char __pyx_k__2[] = " - ";
-static const char __pyx_k__3[] = "`";
+static const char __pyx_k_[] = "_";
+static const char __pyx_k__2[] = ":";
+static const char __pyx_k__3[] = " - ";
+static const char __pyx_k__4[] = "`";
 static const char __pyx_k_Any[] = "Any";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_err[] = "err";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_run[] = "run";
 static const char __pyx_k_set[] = "set";
@@ -1542,36 +1544,41 @@
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_port[] = "port";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
+static const char __pyx_k_CLOUD[] = "CLOUD";
+static const char __pyx_k_DEBUG[] = "DEBUG";
 static const char __pyx_k_Event[] = "Event";
+static const char __pyx_k_LOCAL[] = "LOCAL";
 static const char __pyx_k_Union[] = "Union";
 static const char __pyx_k_clear[] = "clear";
 static const char __pyx_k_debug[] = "debug";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_sleep[] = "sleep";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_topic[] = "topic";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_Client[] = "Client";
+static const char __pyx_k_PREFIX[] = "PREFIX";
 static const char __pyx_k_Thread[] = "Thread";
 static const char __pyx_k_b_stop[] = "_b_stop";
 static const char __pyx_k_client[] = "_client";
 static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_is_set[] = "is_set";
 static const char __pyx_k_logger[] = "logger";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_connect[] = "connect";
+static const char __pyx_k_node_id[] = "node_id";
 static const char __pyx_k_payload[] = "payload";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_publish[] = "publish";
 static const char __pyx_k_unicode[] = "unicode";
 static const char __pyx_k_verbose[] = "verbose";
 static const char __pyx_k_Optional[] = "Optional";
 static const char __pyx_k_on_topic[] = "`) on topic: `";
@@ -1583,71 +1590,91 @@
 static const char __pyx_k_threading[] = "threading";
 static const char __pyx_k_get_logger[] = "get_logger";
 static const char __pyx_k_loop_start[] = "loop_start";
 static const char __pyx_k_on_connect[] = "on_connect";
 static const char __pyx_k_on_message[] = "on_message";
 static const char __pyx_k_MqttWrapper[] = "MqttWrapper";
 static const char __pyx_k_is_connected[] = "is_connected";
+static const char __pyx_k_staticmethod[] = "staticmethod";
 static const char __pyx_k_MqttWrapper_run[] = "MqttWrapper.run";
 static const char __pyx_k_is_not_callable[] = "' is not callable!";
 static const char __pyx_k_on_mqtt_message[] = "_on_mqtt_message";
 static const char __pyx_k_MqttWrapper_stop[] = "MqttWrapper.stop";
 static const char __pyx_k_paho_mqtt_client[] = "paho.mqtt.client";
 static const char __pyx_k_viso_sdk_logging[] = "viso_sdk.logging";
 static const char __pyx_k_Callback_of_topic[] = "Callback of topic '";
 static const char __pyx_k_on_mqtt_connected[] = "_on_mqtt_connected";
 static const char __pyx_k_MqttWrapper___init[] = "MqttWrapper.__init__";
 static const char __pyx_k_Received_a_message[] = "Received a message(`";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_gen_mqtt_key_cloud[] = "gen_mqtt_key_cloud";
+static const char __pyx_k_gen_mqtt_key_debug[] = "gen_mqtt_key_debug";
+static const char __pyx_k_gen_mqtt_key_local[] = "gen_mqtt_key_local";
+static const char __pyx_k_viso_sdk_constants[] = "viso_sdk.constants";
 static const char __pyx_k_MqttWrapper_connect[] = "MqttWrapper.connect";
 static const char __pyx_k_MqttWrapper_publish[] = "MqttWrapper.publish";
 static const char __pyx_k_Failed_to_connect_to[] = "Failed to connect to ";
 static const char __pyx_k_MQTT_Wrapper_from_viso_ai[] = "\nMQTT Wrapper from viso.ai\n";
 static const char __pyx_k_viso_sdk_mqtt_mqtt_wrapper[] = "viso_sdk.mqtt.mqtt_wrapper";
 static const char __pyx_k_Connected_to_the_MQTT_broker[] = "Connected to the MQTT broker - ";
 static const char __pyx_k_MqttWrapper__on_mqtt_message[] = "MqttWrapper._on_mqtt_message";
 static const char __pyx_k_viso_sdk_mqtt_mqtt_wrapper_py[] = "viso_sdk/mqtt/mqtt_wrapper.py";
 static const char __pyx_k_MqttWrapper__on_mqtt_connected[] = "MqttWrapper._on_mqtt_connected";
+static const char __pyx_k_MqttWrapper_gen_mqtt_key_cloud[] = "MqttWrapper.gen_mqtt_key_cloud";
+static const char __pyx_k_MqttWrapper_gen_mqtt_key_debug[] = "MqttWrapper.gen_mqtt_key_debug";
+static const char __pyx_k_MqttWrapper_gen_mqtt_key_local[] = "MqttWrapper.gen_mqtt_key_local";
 static const char __pyx_k_Represents_a_Viso_MQTT_related_A[] = "Represents a Viso MQTT related API instance\n\n    You can execute your callback function when a message is received from a topic.\n    To do this, use `callbacks` parameter to define callback(s) of topic(s):\n\n    .. highlight:: python\n    .. code-block:: python\n\n        def on_message(msg):\n            # This function is called when a message is arrived on \"my_topic\" topic.\n            print(f\"Message arrived - {msg}\")\n\n        mqtt_client = VisoMQTT(callbacks={\"my_topic\" : on_message, \"topic2\": callback2})\n\n    Args:\n        host(str): Host of the MQTT broker.  Normally 127.0.0.1\n        port(int): Port of the MQTT broker.  Default value is 1883\n        callbacks(dict): Callback dictionary. Contains `topic: callback` pairs.\n        verbose(bool): Use verbose logging or not\n    ";
-static PyObject *__pyx_kp_u_;
+static PyObject *__pyx_n_u_;
 static PyObject *__pyx_kp_u_127_0_0_1;
 static PyObject *__pyx_n_s_Any;
+static PyObject *__pyx_n_s_CLOUD;
 static PyObject *__pyx_kp_u_Callback_of_topic;
 static PyObject *__pyx_n_s_Client;
 static PyObject *__pyx_kp_u_Connected_to_the_MQTT_broker;
+static PyObject *__pyx_n_s_DEBUG;
 static PyObject *__pyx_n_s_Event;
 static PyObject *__pyx_kp_u_Failed_to_connect_to;
+static PyObject *__pyx_n_s_LOCAL;
+static PyObject *__pyx_n_s_MQTT;
 static PyObject *__pyx_n_u_MQTT;
 static PyObject *__pyx_n_s_MqttWrapper;
 static PyObject *__pyx_n_s_MqttWrapper___init;
 static PyObject *__pyx_n_s_MqttWrapper__on_mqtt_connected;
 static PyObject *__pyx_n_s_MqttWrapper__on_mqtt_message;
 static PyObject *__pyx_n_s_MqttWrapper_connect;
+static PyObject *__pyx_n_s_MqttWrapper_gen_mqtt_key_cloud;
+static PyObject *__pyx_n_s_MqttWrapper_gen_mqtt_key_debug;
+static PyObject *__pyx_n_s_MqttWrapper_gen_mqtt_key_local;
 static PyObject *__pyx_n_s_MqttWrapper_publish;
 static PyObject *__pyx_n_s_MqttWrapper_run;
 static PyObject *__pyx_n_s_MqttWrapper_stop;
 static PyObject *__pyx_n_s_Optional;
+static PyObject *__pyx_n_s_PREFIX;
 static PyObject *__pyx_kp_u_Received_a_message;
 static PyObject *__pyx_kp_s_Represents_a_Viso_MQTT_related_A;
 static PyObject *__pyx_n_s_Thread;
 static PyObject *__pyx_n_s_Union;
 static PyObject *__pyx_kp_u__2;
 static PyObject *__pyx_kp_u__3;
+static PyObject *__pyx_kp_u__4;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_b_stop;
 static PyObject *__pyx_n_s_callbacks;
 static PyObject *__pyx_n_s_clear;
 static PyObject *__pyx_n_s_client;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_connect;
 static PyObject *__pyx_n_s_debug;
 static PyObject *__pyx_n_s_decode;
 static PyObject *__pyx_n_s_doc;
 static PyObject *__pyx_n_s_err;
 static PyObject *__pyx_n_s_error;
+static PyObject *__pyx_n_s_gen_mqtt_key_cloud;
+static PyObject *__pyx_n_s_gen_mqtt_key_debug;
+static PyObject *__pyx_n_s_gen_mqtt_key_local;
 static PyObject *__pyx_n_s_get;
 static PyObject *__pyx_n_s_get_logger;
 static PyObject *__pyx_n_s_host;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_info;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_is_connected;
@@ -1657,14 +1684,15 @@
 static PyObject *__pyx_n_s_logger;
 static PyObject *__pyx_n_s_loop_start;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_msg;
 static PyObject *__pyx_n_s_name;
+static PyObject *__pyx_n_s_node_id;
 static PyObject *__pyx_n_s_on_connect;
 static PyObject *__pyx_n_s_on_message;
 static PyObject *__pyx_n_s_on_mqtt_connected;
 static PyObject *__pyx_n_s_on_mqtt_message;
 static PyObject *__pyx_kp_u_on_topic;
 static PyObject *__pyx_n_s_paho_mqtt_client;
 static PyObject *__pyx_n_s_payload;
@@ -1674,54 +1702,65 @@
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_return;
 static PyObject *__pyx_n_s_run;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_set;
 static PyObject *__pyx_n_s_sleep;
 static PyObject *__pyx_n_s_start;
+static PyObject *__pyx_n_s_staticmethod;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_n_s_subscribe;
 static PyObject *__pyx_n_s_super;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_threading;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_topic;
 static PyObject *__pyx_n_s_typing;
 static PyObject *__pyx_n_u_unicode;
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_verbose;
+static PyObject *__pyx_n_s_viso_sdk_constants;
 static PyObject *__pyx_n_s_viso_sdk_logging;
 static PyObject *__pyx_n_s_viso_sdk_mqtt_mqtt_wrapper;
 static PyObject *__pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py;
 static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_host, PyObject *__pyx_v_port, PyObject *__pyx_v_callbacks, PyObject *__pyx_v_verbose); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_2connect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_4run(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_6_on_mqtt_connected(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8_on_mqtt_message(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10publish(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_topic, PyObject *__pyx_v_payload); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12stop(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_2gen_mqtt_key_local(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_4gen_mqtt_key_cloud(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_6gen_mqtt_key_debug(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8connect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10run(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12_on_mqtt_connected(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_14_on_mqtt_message(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_16publish(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_topic, PyObject *__pyx_v_payload); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_18stop(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_1883;
-static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_codeobj__6;
-static PyObject *__pyx_codeobj__9;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
+static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__15;
+static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_tuple__19;
+static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__23;
+static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_codeobj__7;
+static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_codeobj__12;
+static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_codeobj__16;
+static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_codeobj__26;
 /* Late includes */
 
 /* "viso_sdk/mqtt/mqtt_wrapper.py":39
  *     """
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
@@ -2080,15 +2119,15 @@
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_verbose, __pyx_v_verbose) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
 
   /* "viso_sdk/mqtt/mqtt_wrapper.py":56
  *         self._b_stop.clear()
  *         self.verbose = verbose
  *         self.start()             # <<<<<<<<<<<<<<
  * 
- *     def connect(self) -> bool:
+ *     @staticmethod
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -2124,38 +2163,530 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/mqtt/mqtt_wrapper.py":58
- *         self.start()
+/* "viso_sdk/mqtt/mqtt_wrapper.py":59
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_local(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.LOCAL}_{node_id}_{port}"
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3gen_mqtt_key_local(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3gen_mqtt_key_local = {"gen_mqtt_key_local", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3gen_mqtt_key_local, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3gen_mqtt_key_local(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_node_id = 0;
+  PyObject *__pyx_v_port = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen_mqtt_key_local (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node_id,&__pyx_n_s_port,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node_id)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_port)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen_mqtt_key_local", 1, 2, 2, 1); __PYX_ERR(0, 59, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gen_mqtt_key_local") < 0)) __PYX_ERR(0, 59, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_node_id = values[0];
+    __pyx_v_port = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("gen_mqtt_key_local", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 59, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper.gen_mqtt_key_local", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_2gen_mqtt_key_local(__pyx_self, __pyx_v_node_id, __pyx_v_port);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_2gen_mqtt_key_local(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  Py_UCS4 __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("gen_mqtt_key_local", 0);
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":60
+ *     @staticmethod
+ *     def gen_mqtt_key_local(node_id, port):
+ *         return f"{PREFIX.MQTT.LOCAL}_{node_id}_{port}"             # <<<<<<<<<<<<<<
+ * 
+ *     @staticmethod
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 127;
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_PREFIX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_MQTT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_LOCAL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_node_id, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_port, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
+  goto __pyx_L0;
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":59
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_local(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.LOCAL}_{node_id}_{port}"
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper.gen_mqtt_key_local", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "viso_sdk/mqtt/mqtt_wrapper.py":63
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_cloud(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.CLOUD}_{node_id}_{port}"
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5gen_mqtt_key_cloud(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5gen_mqtt_key_cloud = {"gen_mqtt_key_cloud", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5gen_mqtt_key_cloud, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5gen_mqtt_key_cloud(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_node_id = 0;
+  PyObject *__pyx_v_port = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen_mqtt_key_cloud (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node_id,&__pyx_n_s_port,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node_id)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_port)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen_mqtt_key_cloud", 1, 2, 2, 1); __PYX_ERR(0, 63, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gen_mqtt_key_cloud") < 0)) __PYX_ERR(0, 63, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_node_id = values[0];
+    __pyx_v_port = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("gen_mqtt_key_cloud", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 63, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper.gen_mqtt_key_cloud", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_4gen_mqtt_key_cloud(__pyx_self, __pyx_v_node_id, __pyx_v_port);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_4gen_mqtt_key_cloud(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  Py_UCS4 __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("gen_mqtt_key_cloud", 0);
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":64
+ *     @staticmethod
+ *     def gen_mqtt_key_cloud(node_id, port):
+ *         return f"{PREFIX.MQTT.CLOUD}_{node_id}_{port}"             # <<<<<<<<<<<<<<
+ * 
+ *     @staticmethod
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 127;
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_PREFIX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_MQTT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_CLOUD); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_node_id, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_port, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
+  goto __pyx_L0;
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":63
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_cloud(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.CLOUD}_{node_id}_{port}"
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper.gen_mqtt_key_cloud", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "viso_sdk/mqtt/mqtt_wrapper.py":67
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_debug(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7gen_mqtt_key_debug(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7gen_mqtt_key_debug = {"gen_mqtt_key_debug", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7gen_mqtt_key_debug, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7gen_mqtt_key_debug(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_node_id = 0;
+  PyObject *__pyx_v_port = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen_mqtt_key_debug (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node_id,&__pyx_n_s_port,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node_id)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_port)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen_mqtt_key_debug", 1, 2, 2, 1); __PYX_ERR(0, 67, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gen_mqtt_key_debug") < 0)) __PYX_ERR(0, 67, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_node_id = values[0];
+    __pyx_v_port = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("gen_mqtt_key_debug", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 67, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper.gen_mqtt_key_debug", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_6gen_mqtt_key_debug(__pyx_self, __pyx_v_node_id, __pyx_v_port);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_6gen_mqtt_key_debug(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  Py_UCS4 __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("gen_mqtt_key_debug", 0);
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":68
+ *     @staticmethod
+ *     def gen_mqtt_key_debug(node_id, port):
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"             # <<<<<<<<<<<<<<
+ * 
+ *     def connect(self) -> bool:
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 127;
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_PREFIX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_MQTT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_node_id, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_port, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
+  goto __pyx_L0;
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":67
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_debug(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper.gen_mqtt_key_debug", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "viso_sdk/mqtt/mqtt_wrapper.py":70
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
  * 
  *     def connect(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Connect to the target MQTT broker"""
  *         try:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3connect(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_2connect[] = "Connect to the target MQTT broker";
-static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3connect = {"connect", (PyCFunction)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3connect, METH_O, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_2connect};
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3connect(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9connect(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8connect[] = "Connect to the target MQTT broker";
+static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9connect = {"connect", (PyCFunction)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9connect, METH_O, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8connect};
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9connect(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("connect (wrapper)", 0);
-  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_2connect(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8connect(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_2connect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8connect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_v_err = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -2178,15 +2709,15 @@
   PyObject *__pyx_t_21 = NULL;
   PyObject *__pyx_t_22 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("connect", 0);
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":60
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":72
  *     def connect(self) -> bool:
  *         """Connect to the target MQTT broker"""
  *         try:             # <<<<<<<<<<<<<<
  *             self._client.connect(self.host, self.port)
  *         except Exception as err:
  */
   {
@@ -2194,29 +2725,29 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "viso_sdk/mqtt/mqtt_wrapper.py":61
+      /* "viso_sdk/mqtt/mqtt_wrapper.py":73
  *         """Connect to the target MQTT broker"""
  *         try:
  *             self._client.connect(self.host, self.port)             # <<<<<<<<<<<<<<
  *         except Exception as err:
  *             logger.error(f"Failed to connect to {self.host}:{self.port} - {err}")
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 61, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_connect); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 61, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_connect); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_host); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 61, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_host); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_port); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 61, __pyx_L3_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_port); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 73, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -2225,51 +2756,51 @@
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_7};
-        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_7};
-        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       {
-        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 61, __pyx_L3_error)
+        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 73, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (__pyx_t_8) {
           __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_5);
         PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_5);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_7);
         __pyx_t_5 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "viso_sdk/mqtt/mqtt_wrapper.py":60
+      /* "viso_sdk/mqtt/mqtt_wrapper.py":72
  *     def connect(self) -> bool:
  *         """Connect to the target MQTT broker"""
  *         try:             # <<<<<<<<<<<<<<
  *             self._client.connect(self.host, self.port)
  *         except Exception as err:
  */
     }
@@ -2281,88 +2812,88 @@
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":62
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":74
  *         try:
  *             self._client.connect(self.host, self.port)
  *         except Exception as err:             # <<<<<<<<<<<<<<
  *             logger.error(f"Failed to connect to {self.host}:{self.port} - {err}")
  *             return False
  */
     __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_9) {
       __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper.connect", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_10) < 0) __PYX_ERR(0, 62, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_10) < 0) __PYX_ERR(0, 74, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_err = __pyx_t_6;
       /*try:*/ {
 
-        /* "viso_sdk/mqtt/mqtt_wrapper.py":63
+        /* "viso_sdk/mqtt/mqtt_wrapper.py":75
  *             self._client.connect(self.host, self.port)
  *         except Exception as err:
  *             logger.error(f"Failed to connect to {self.host}:{self.port} - {err}")             # <<<<<<<<<<<<<<
  *             return False
  *         self._client.loop_start()
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L14_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_error); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 63, __pyx_L14_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_error); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_5 = PyTuple_New(6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L14_error)
+        __pyx_t_5 = PyTuple_New(6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_5);
         __pyx_t_11 = 0;
         __pyx_t_12 = 127;
         __Pyx_INCREF(__pyx_kp_u_Failed_to_connect_to);
         __pyx_t_11 += 21;
         __Pyx_GIVEREF(__pyx_kp_u_Failed_to_connect_to);
         PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_kp_u_Failed_to_connect_to);
-        __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_host); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 63, __pyx_L14_error)
+        __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_host); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_14 = __Pyx_PyObject_FormatSimple(__pyx_t_13, __pyx_empty_unicode); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 63, __pyx_L14_error)
+        __pyx_t_14 = __Pyx_PyObject_FormatSimple(__pyx_t_13, __pyx_empty_unicode); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         __pyx_t_12 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_14) > __pyx_t_12) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_14) : __pyx_t_12;
         __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_14);
         __Pyx_GIVEREF(__pyx_t_14);
         PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_14);
         __pyx_t_14 = 0;
-        __Pyx_INCREF(__pyx_kp_u_);
+        __Pyx_INCREF(__pyx_kp_u__2);
         __pyx_t_11 += 1;
-        __Pyx_GIVEREF(__pyx_kp_u_);
-        PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u_);
-        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_port); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 63, __pyx_L14_error)
+        __Pyx_GIVEREF(__pyx_kp_u__2);
+        PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u__2);
+        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_port); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_t_14, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 63, __pyx_L14_error)
+        __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_t_14, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_t_12 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) > __pyx_t_12) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) : __pyx_t_12;
         __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_13);
         __Pyx_GIVEREF(__pyx_t_13);
         PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_13);
         __pyx_t_13 = 0;
-        __Pyx_INCREF(__pyx_kp_u__2);
+        __Pyx_INCREF(__pyx_kp_u__3);
         __pyx_t_11 += 3;
-        __Pyx_GIVEREF(__pyx_kp_u__2);
-        PyTuple_SET_ITEM(__pyx_t_5, 4, __pyx_kp_u__2);
-        __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_v_err, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 63, __pyx_L14_error)
+        __Pyx_GIVEREF(__pyx_kp_u__3);
+        PyTuple_SET_ITEM(__pyx_t_5, 4, __pyx_kp_u__3);
+        __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_v_err, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_13);
         __pyx_t_12 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) > __pyx_t_12) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) : __pyx_t_12;
         __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_13);
         __Pyx_GIVEREF(__pyx_t_13);
         PyTuple_SET_ITEM(__pyx_t_5, 5, __pyx_t_13);
         __pyx_t_13 = 0;
-        __pyx_t_13 = __Pyx_PyUnicode_Join(__pyx_t_5, 6, __pyx_t_11, __pyx_t_12); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 63, __pyx_L14_error)
+        __pyx_t_13 = __Pyx_PyUnicode_Join(__pyx_t_5, 6, __pyx_t_11, __pyx_t_12); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -2370,20 +2901,20 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_8, function);
           }
         }
         __pyx_t_7 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_5, __pyx_t_13) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_13);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 63, __pyx_L14_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 75, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "viso_sdk/mqtt/mqtt_wrapper.py":64
+        /* "viso_sdk/mqtt/mqtt_wrapper.py":76
  *         except Exception as err:
  *             logger.error(f"Failed to connect to {self.host}:{self.port} - {err}")
  *             return False             # <<<<<<<<<<<<<<
  *         self._client.loop_start()
  *         return True
  */
         __Pyx_XDECREF(__pyx_r);
@@ -2391,15 +2922,15 @@
         __pyx_r = Py_False;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         goto __pyx_L13_return;
       }
 
-      /* "viso_sdk/mqtt/mqtt_wrapper.py":62
+      /* "viso_sdk/mqtt/mqtt_wrapper.py":74
  *         try:
  *             self._client.connect(self.host, self.port)
  *         except Exception as err:             # <<<<<<<<<<<<<<
  *             logger.error(f"Failed to connect to {self.host}:{self.port} - {err}")
  *             return False
  */
       /*finally:*/ {
@@ -2450,15 +2981,15 @@
           goto __pyx_L6_except_return;
         }
       }
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":60
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":72
  *     def connect(self) -> bool:
  *         """Connect to the target MQTT broker"""
  *         try:             # <<<<<<<<<<<<<<
  *             self._client.connect(self.host, self.port)
  *         except Exception as err:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -2471,57 +3002,57 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
     __pyx_L8_try_end:;
   }
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":65
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":77
  *             logger.error(f"Failed to connect to {self.host}:{self.port} - {err}")
  *             return False
  *         self._client.loop_start()             # <<<<<<<<<<<<<<
  *         return True
  * 
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_loop_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_loop_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_10 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":66
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":78
  *             return False
  *         self._client.loop_start()
  *         return True             # <<<<<<<<<<<<<<
  * 
  *     def run(self) -> None:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(Py_True);
   __pyx_r = Py_True;
   goto __pyx_L0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":58
- *         self.start()
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":70
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
  * 
  *     def connect(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Connect to the target MQTT broker"""
  *         try:
  */
 
   /* function exit code */
@@ -2539,181 +3070,181 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_err);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/mqtt/mqtt_wrapper.py":68
+/* "viso_sdk/mqtt/mqtt_wrapper.py":80
  *         return True
  * 
  *     def run(self) -> None:             # <<<<<<<<<<<<<<
  *         """Main thread loop"""
  *         while not self._b_stop.is_set():
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5run(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_4run[] = "Main thread loop";
-static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5run = {"run", (PyCFunction)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5run, METH_O, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_4run};
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5run(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11run(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10run[] = "Main thread loop";
+static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11run = {"run", (PyCFunction)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11run, METH_O, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10run};
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11run(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("run (wrapper)", 0);
-  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_4run(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10run(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_4run(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10run(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("run", 0);
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":70
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":82
  *     def run(self) -> None:
  *         """Main thread loop"""
  *         while not self._b_stop.is_set():             # <<<<<<<<<<<<<<
  *             # Check MQTT connection and connect if not.
  *             if not self._client.is_connected():
  */
   while (1) {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_b_stop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_b_stop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_is_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_is_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_5 = ((!__pyx_t_4) != 0);
     if (!__pyx_t_5) break;
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":72
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":84
  *         while not self._b_stop.is_set():
  *             # Check MQTT connection and connect if not.
  *             if not self._client.is_connected():             # <<<<<<<<<<<<<<
  *                 self.connect()
  *             time.sleep(1)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_is_connected); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_is_connected); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_4 = ((!__pyx_t_5) != 0);
     if (__pyx_t_4) {
 
-      /* "viso_sdk/mqtt/mqtt_wrapper.py":73
+      /* "viso_sdk/mqtt/mqtt_wrapper.py":85
  *             # Check MQTT connection and connect if not.
  *             if not self._client.is_connected():
  *                 self.connect()             # <<<<<<<<<<<<<<
  *             time.sleep(1)
  * 
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_connect); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_connect); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "viso_sdk/mqtt/mqtt_wrapper.py":72
+      /* "viso_sdk/mqtt/mqtt_wrapper.py":84
  *         while not self._b_stop.is_set():
  *             # Check MQTT connection and connect if not.
  *             if not self._client.is_connected():             # <<<<<<<<<<<<<<
  *                 self.connect()
  *             time.sleep(1)
  */
     }
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":74
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":86
  *             if not self._client.is_connected():
  *                 self.connect()
  *             time.sleep(1)             # <<<<<<<<<<<<<<
  * 
  *     def _on_mqtt_connected(self, *args: Any) -> None:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sleep); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sleep); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_int_1) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_int_1);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":68
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":80
  *         return True
  * 
  *     def run(self) -> None:             # <<<<<<<<<<<<<<
  *         """Main thread loop"""
  *         while not self._b_stop.is_set():
  */
 
@@ -2728,27 +3259,27 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/mqtt/mqtt_wrapper.py":76
+/* "viso_sdk/mqtt/mqtt_wrapper.py":88
  *             time.sleep(1)
  * 
  *     def _on_mqtt_connected(self, *args: Any) -> None:             # <<<<<<<<<<<<<<
  *         """Callback when MQTT is connected"""
  *         logger.info(f"Connected to the MQTT broker - {args}")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7_on_mqtt_connected(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_6_on_mqtt_connected[] = "Callback when MQTT is connected";
-static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7_on_mqtt_connected = {"_on_mqtt_connected", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7_on_mqtt_connected, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_6_on_mqtt_connected};
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7_on_mqtt_connected(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13_on_mqtt_connected(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12_on_mqtt_connected[] = "Callback when MQTT is connected";
+static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13_on_mqtt_connected = {"_on_mqtt_connected", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13_on_mqtt_connected, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12_on_mqtt_connected};
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13_on_mqtt_connected(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_args = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2779,41 +3310,41 @@
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t used_pos_args = (pos_args < 1) ? pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, used_pos_args, "_on_mqtt_connected") < 0)) __PYX_ERR(0, 76, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, used_pos_args, "_on_mqtt_connected") < 0)) __PYX_ERR(0, 88, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) < 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_on_mqtt_connected", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 76, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_on_mqtt_connected", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 88, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
   __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper._on_mqtt_connected", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_6_on_mqtt_connected(__pyx_self, __pyx_v_self, __pyx_v_args);
+  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12_on_mqtt_connected(__pyx_self, __pyx_v_self, __pyx_v_args);
 
   /* function exit code */
   __Pyx_XDECREF(__pyx_v_args);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_6_on_mqtt_connected(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args) {
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12_on_mqtt_connected(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args) {
   PyObject *__pyx_v_topic = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -2823,29 +3354,29 @@
   int __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_on_mqtt_connected", 0);
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":78
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":90
  *     def _on_mqtt_connected(self, *args: Any) -> None:
  *         """Callback when MQTT is connected"""
  *         logger.info(f"Connected to the MQTT broker - {args}")             # <<<<<<<<<<<<<<
  *         if args[-1] == 0:  # Check ResultCode
  *             for topic in self.callbacks.keys():
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_info); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_args, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_args, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Connected_to_the_MQTT_broker, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Connected_to_the_MQTT_broker, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -2853,96 +3384,96 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":79
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":91
  *         """Callback when MQTT is connected"""
  *         logger.info(f"Connected to the MQTT broker - {args}")
  *         if args[-1] == 0:  # Check ResultCode             # <<<<<<<<<<<<<<
  *             for topic in self.callbacks.keys():
  *                 self._client.subscribe(topic=topic)
  */
-  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v_args, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v_args, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":80
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":92
  *         logger.info(f"Connected to the MQTT broker - {args}")
  *         if args[-1] == 0:  # Check ResultCode
  *             for topic in self.callbacks.keys():             # <<<<<<<<<<<<<<
  *                 self._client.subscribe(topic=topic)
  * 
  */
     __pyx_t_6 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_t_1 == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
-      __PYX_ERR(0, 80, __pyx_L1_error)
+      __PYX_ERR(0, 92, __pyx_L1_error)
     }
-    __pyx_t_4 = __Pyx_dict_iterator(__pyx_t_1, 0, __pyx_n_s_keys, (&__pyx_t_7), (&__pyx_t_8)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_dict_iterator(__pyx_t_1, 0, __pyx_n_s_keys, (&__pyx_t_7), (&__pyx_t_8)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
     while (1) {
       __pyx_t_9 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_7, &__pyx_t_6, &__pyx_t_4, NULL, NULL, __pyx_t_8);
       if (unlikely(__pyx_t_9 == 0)) break;
-      if (unlikely(__pyx_t_9 == -1)) __PYX_ERR(0, 80, __pyx_L1_error)
+      if (unlikely(__pyx_t_9 == -1)) __PYX_ERR(0, 92, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_topic, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "viso_sdk/mqtt/mqtt_wrapper.py":81
+      /* "viso_sdk/mqtt/mqtt_wrapper.py":93
  *         if args[-1] == 0:  # Check ResultCode
  *             for topic in self.callbacks.keys():
  *                 self._client.subscribe(topic=topic)             # <<<<<<<<<<<<<<
  * 
  *     def _on_mqtt_message(self, *args: Any) -> None:
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_subscribe); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_subscribe); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_topic, __pyx_v_topic) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_topic, __pyx_v_topic) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":79
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":91
  *         """Callback when MQTT is connected"""
  *         logger.info(f"Connected to the MQTT broker - {args}")
  *         if args[-1] == 0:  # Check ResultCode             # <<<<<<<<<<<<<<
  *             for topic in self.callbacks.keys():
  *                 self._client.subscribe(topic=topic)
  */
   }
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":76
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":88
  *             time.sleep(1)
  * 
  *     def _on_mqtt_connected(self, *args: Any) -> None:             # <<<<<<<<<<<<<<
  *         """Callback when MQTT is connected"""
  *         logger.info(f"Connected to the MQTT broker - {args}")
  */
 
@@ -2959,27 +3490,27 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_topic);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/mqtt/mqtt_wrapper.py":83
+/* "viso_sdk/mqtt/mqtt_wrapper.py":95
  *                 self._client.subscribe(topic=topic)
  * 
  *     def _on_mqtt_message(self, *args: Any) -> None:             # <<<<<<<<<<<<<<
  *         """Callback when a message on subscribed channels is received."""
  *         topic = args[2].topic
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9_on_mqtt_message(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8_on_mqtt_message[] = "Callback when a message on subscribed channels is received.";
-static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9_on_mqtt_message = {"_on_mqtt_message", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9_on_mqtt_message, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8_on_mqtt_message};
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9_on_mqtt_message(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_15_on_mqtt_message(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_14_on_mqtt_message[] = "Callback when a message on subscribed channels is received.";
+static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_15_on_mqtt_message = {"_on_mqtt_message", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_15_on_mqtt_message, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_14_on_mqtt_message};
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_15_on_mqtt_message(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_args = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3010,41 +3541,41 @@
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t used_pos_args = (pos_args < 1) ? pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, used_pos_args, "_on_mqtt_message") < 0)) __PYX_ERR(0, 83, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, used_pos_args, "_on_mqtt_message") < 0)) __PYX_ERR(0, 95, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) < 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_on_mqtt_message", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 83, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_on_mqtt_message", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 95, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
   __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper._on_mqtt_message", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8_on_mqtt_message(__pyx_self, __pyx_v_self, __pyx_v_args);
+  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_14_on_mqtt_message(__pyx_self, __pyx_v_self, __pyx_v_args);
 
   /* function exit code */
   __Pyx_XDECREF(__pyx_v_args);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_8_on_mqtt_message(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args) {
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_14_on_mqtt_message(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args) {
   PyObject *__pyx_v_topic = NULL;
   PyObject *__pyx_v_msg = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -3054,118 +3585,118 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_on_mqtt_message", 0);
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":85
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":97
  *     def _on_mqtt_message(self, *args: Any) -> None:
  *         """Callback when a message on subscribed channels is received."""
  *         topic = args[2].topic             # <<<<<<<<<<<<<<
  *         msg = args[2].payload.decode("utf-8")
  *         if self.verbose:
  */
-  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v_args, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v_args, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_topic); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_topic); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_topic = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":86
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":98
  *         """Callback when a message on subscribed channels is received."""
  *         topic = args[2].topic
  *         msg = args[2].payload.decode("utf-8")             # <<<<<<<<<<<<<<
  *         if self.verbose:
  *             logger.debug(f"Received a message(`{msg}`) on topic: `{topic}`")
  */
-  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v_args, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v_args, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_payload); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_payload); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_msg = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":87
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":99
  *         topic = args[2].topic
  *         msg = args[2].payload.decode("utf-8")
  *         if self.verbose:             # <<<<<<<<<<<<<<
  *             logger.debug(f"Received a message(`{msg}`) on topic: `{topic}`")
  *         if callable(self.callbacks.get(topic)):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_verbose); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_verbose); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_4) {
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":88
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":100
  *         msg = args[2].payload.decode("utf-8")
  *         if self.verbose:
  *             logger.debug(f"Received a message(`{msg}`) on topic: `{topic}`")             # <<<<<<<<<<<<<<
  *         if callable(self.callbacks.get(topic)):
  *             # Call corresponding callback function with the message payload as an argument.
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
     __Pyx_INCREF(__pyx_kp_u_Received_a_message);
     __pyx_t_5 += 20;
     __Pyx_GIVEREF(__pyx_kp_u_Received_a_message);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Received_a_message);
-    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_msg, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_msg, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_on_topic);
     __pyx_t_5 += 14;
     __Pyx_GIVEREF(__pyx_kp_u_on_topic);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_on_topic);
-    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_topic, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_topic, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_7);
     __pyx_t_7 = 0;
-    __Pyx_INCREF(__pyx_kp_u__3);
+    __Pyx_INCREF(__pyx_kp_u__4);
     __pyx_t_5 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__3);
-    PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__3);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__4);
+    PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__4);
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -3173,132 +3704,132 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":87
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":99
  *         topic = args[2].topic
  *         msg = args[2].payload.decode("utf-8")
  *         if self.verbose:             # <<<<<<<<<<<<<<
  *             logger.debug(f"Received a message(`{msg}`) on topic: `{topic}`")
  *         if callable(self.callbacks.get(topic)):
  */
   }
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":89
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":101
  *         if self.verbose:
  *             logger.debug(f"Received a message(`{msg}`) on topic: `{topic}`")
  *         if callable(self.callbacks.get(topic)):             # <<<<<<<<<<<<<<
  *             # Call corresponding callback function with the message payload as an argument.
  *             self.callbacks[topic](msg)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_3, __pyx_v_topic) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_topic);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_4 = __Pyx_PyCallable_Check(__pyx_t_2); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyCallable_Check(__pyx_t_2); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_8 = (__pyx_t_4 != 0);
   if (__pyx_t_8) {
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":91
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":103
  *         if callable(self.callbacks.get(topic)):
  *             # Call corresponding callback function with the message payload as an argument.
  *             self.callbacks[topic](msg)             # <<<<<<<<<<<<<<
  *         else:
  *             logger.error(f"Callback of topic '{topic}' is not callable!")
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 103, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_7, __pyx_v_topic); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_7, __pyx_v_topic); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_7, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_msg);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "viso_sdk/mqtt/mqtt_wrapper.py":89
+    /* "viso_sdk/mqtt/mqtt_wrapper.py":101
  *         if self.verbose:
  *             logger.debug(f"Received a message(`{msg}`) on topic: `{topic}`")
  *         if callable(self.callbacks.get(topic)):             # <<<<<<<<<<<<<<
  *             # Call corresponding callback function with the message payload as an argument.
  *             self.callbacks[topic](msg)
  */
     goto __pyx_L4;
   }
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":93
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":105
  *             self.callbacks[topic](msg)
  *         else:
  *             logger.error(f"Callback of topic '{topic}' is not callable!")             # <<<<<<<<<<<<<<
  * 
  *     def publish(self, topic: str, payload: str) -> None:
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_error); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_error); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
     __Pyx_INCREF(__pyx_kp_u_Callback_of_topic);
     __pyx_t_5 += 19;
     __Pyx_GIVEREF(__pyx_kp_u_Callback_of_topic);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Callback_of_topic);
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_topic, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_topic, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_kp_u_is_not_callable);
     __pyx_t_5 += 18;
     __Pyx_GIVEREF(__pyx_kp_u_is_not_callable);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_is_not_callable);
-    __pyx_t_1 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -3306,22 +3837,22 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L4:;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":83
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":95
  *                 self._client.subscribe(topic=topic)
  * 
  *     def _on_mqtt_message(self, *args: Any) -> None:             # <<<<<<<<<<<<<<
  *         """Callback when a message on subscribed channels is received."""
  *         topic = args[2].topic
  */
 
@@ -3339,27 +3870,27 @@
   __Pyx_XDECREF(__pyx_v_topic);
   __Pyx_XDECREF(__pyx_v_msg);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/mqtt/mqtt_wrapper.py":95
+/* "viso_sdk/mqtt/mqtt_wrapper.py":107
  *             logger.error(f"Callback of topic '{topic}' is not callable!")
  * 
  *     def publish(self, topic: str, payload: str) -> None:             # <<<<<<<<<<<<<<
  *         """Publish a message to a topic"""
  *         self._client.publish(topic=topic, payload=payload)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11publish(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10publish[] = "Publish a message to a topic";
-static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11publish = {"publish", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11publish, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10publish};
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11publish(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_17publish(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_16publish[] = "Publish a message to a topic";
+static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_17publish = {"publish", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_17publish, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_16publish};
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_17publish(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_topic = 0;
   PyObject *__pyx_v_payload = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -3386,92 +3917,92 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_topic)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("publish", 1, 3, 3, 1); __PYX_ERR(0, 95, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("publish", 1, 3, 3, 1); __PYX_ERR(0, 107, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_payload)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("publish", 1, 3, 3, 2); __PYX_ERR(0, 95, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("publish", 1, 3, 3, 2); __PYX_ERR(0, 107, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "publish") < 0)) __PYX_ERR(0, 95, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "publish") < 0)) __PYX_ERR(0, 107, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_topic = ((PyObject*)values[1]);
     __pyx_v_payload = ((PyObject*)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("publish", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 95, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("publish", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 107, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viso_sdk.mqtt.mqtt_wrapper.MqttWrapper.publish", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_topic), (&PyUnicode_Type), 1, "topic", 1))) __PYX_ERR(0, 95, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_payload), (&PyUnicode_Type), 1, "payload", 1))) __PYX_ERR(0, 95, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10publish(__pyx_self, __pyx_v_self, __pyx_v_topic, __pyx_v_payload);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_topic), (&PyUnicode_Type), 1, "topic", 1))) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_payload), (&PyUnicode_Type), 1, "payload", 1))) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_16publish(__pyx_self, __pyx_v_self, __pyx_v_topic, __pyx_v_payload);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_10publish(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_topic, PyObject *__pyx_v_payload) {
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_16publish(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_topic, PyObject *__pyx_v_payload) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("publish", 0);
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":97
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":109
  *     def publish(self, topic: str, payload: str) -> None:
  *         """Publish a message to a topic"""
  *         self._client.publish(topic=topic, payload=payload)             # <<<<<<<<<<<<<<
  * 
  *     def stop(self) -> None:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_client); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_publish); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_publish); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_topic, __pyx_v_topic) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_payload, __pyx_v_payload) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_topic, __pyx_v_topic) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_payload, __pyx_v_payload) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":95
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":107
  *             logger.error(f"Callback of topic '{topic}' is not callable!")
  * 
  *     def publish(self, topic: str, payload: str) -> None:             # <<<<<<<<<<<<<<
  *         """Publish a message to a topic"""
  *         self._client.publish(topic=topic, payload=payload)
  */
 
@@ -3486,76 +4017,76 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/mqtt/mqtt_wrapper.py":99
+/* "viso_sdk/mqtt/mqtt_wrapper.py":111
  *         self._client.publish(topic=topic, payload=payload)
  * 
  *     def stop(self) -> None:             # <<<<<<<<<<<<<<
  *         """Stop this thread"""
  *         self._b_stop.set()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13stop(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12stop[] = "Stop this thread";
-static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13stop = {"stop", (PyCFunction)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13stop, METH_O, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12stop};
-static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13stop(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_19stop(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_18stop[] = "Stop this thread";
+static PyMethodDef __pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_19stop = {"stop", (PyCFunction)__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_19stop, METH_O, __pyx_doc_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_18stop};
+static PyObject *__pyx_pw_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_19stop(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("stop (wrapper)", 0);
-  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12stop(__pyx_self, ((PyObject *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_18stop(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_12stop(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_18stop(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("stop", 0);
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":101
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":113
  *     def stop(self) -> None:
  *         """Stop this thread"""
  *         self._b_stop.set()             # <<<<<<<<<<<<<<
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_b_stop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_b_stop); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":99
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":111
  *         self._client.publish(topic=topic, payload=payload)
  * 
  *     def stop(self) -> None:             # <<<<<<<<<<<<<<
  *         """Stop this thread"""
  *         self._b_stop.set()
  */
 
@@ -3616,50 +4147,62 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
+  {&__pyx_n_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 1},
   {&__pyx_kp_u_127_0_0_1, __pyx_k_127_0_0_1, sizeof(__pyx_k_127_0_0_1), 0, 1, 0, 0},
   {&__pyx_n_s_Any, __pyx_k_Any, sizeof(__pyx_k_Any), 0, 0, 1, 1},
+  {&__pyx_n_s_CLOUD, __pyx_k_CLOUD, sizeof(__pyx_k_CLOUD), 0, 0, 1, 1},
   {&__pyx_kp_u_Callback_of_topic, __pyx_k_Callback_of_topic, sizeof(__pyx_k_Callback_of_topic), 0, 1, 0, 0},
   {&__pyx_n_s_Client, __pyx_k_Client, sizeof(__pyx_k_Client), 0, 0, 1, 1},
   {&__pyx_kp_u_Connected_to_the_MQTT_broker, __pyx_k_Connected_to_the_MQTT_broker, sizeof(__pyx_k_Connected_to_the_MQTT_broker), 0, 1, 0, 0},
+  {&__pyx_n_s_DEBUG, __pyx_k_DEBUG, sizeof(__pyx_k_DEBUG), 0, 0, 1, 1},
   {&__pyx_n_s_Event, __pyx_k_Event, sizeof(__pyx_k_Event), 0, 0, 1, 1},
   {&__pyx_kp_u_Failed_to_connect_to, __pyx_k_Failed_to_connect_to, sizeof(__pyx_k_Failed_to_connect_to), 0, 1, 0, 0},
+  {&__pyx_n_s_LOCAL, __pyx_k_LOCAL, sizeof(__pyx_k_LOCAL), 0, 0, 1, 1},
+  {&__pyx_n_s_MQTT, __pyx_k_MQTT, sizeof(__pyx_k_MQTT), 0, 0, 1, 1},
   {&__pyx_n_u_MQTT, __pyx_k_MQTT, sizeof(__pyx_k_MQTT), 0, 1, 0, 1},
   {&__pyx_n_s_MqttWrapper, __pyx_k_MqttWrapper, sizeof(__pyx_k_MqttWrapper), 0, 0, 1, 1},
   {&__pyx_n_s_MqttWrapper___init, __pyx_k_MqttWrapper___init, sizeof(__pyx_k_MqttWrapper___init), 0, 0, 1, 1},
   {&__pyx_n_s_MqttWrapper__on_mqtt_connected, __pyx_k_MqttWrapper__on_mqtt_connected, sizeof(__pyx_k_MqttWrapper__on_mqtt_connected), 0, 0, 1, 1},
   {&__pyx_n_s_MqttWrapper__on_mqtt_message, __pyx_k_MqttWrapper__on_mqtt_message, sizeof(__pyx_k_MqttWrapper__on_mqtt_message), 0, 0, 1, 1},
   {&__pyx_n_s_MqttWrapper_connect, __pyx_k_MqttWrapper_connect, sizeof(__pyx_k_MqttWrapper_connect), 0, 0, 1, 1},
+  {&__pyx_n_s_MqttWrapper_gen_mqtt_key_cloud, __pyx_k_MqttWrapper_gen_mqtt_key_cloud, sizeof(__pyx_k_MqttWrapper_gen_mqtt_key_cloud), 0, 0, 1, 1},
+  {&__pyx_n_s_MqttWrapper_gen_mqtt_key_debug, __pyx_k_MqttWrapper_gen_mqtt_key_debug, sizeof(__pyx_k_MqttWrapper_gen_mqtt_key_debug), 0, 0, 1, 1},
+  {&__pyx_n_s_MqttWrapper_gen_mqtt_key_local, __pyx_k_MqttWrapper_gen_mqtt_key_local, sizeof(__pyx_k_MqttWrapper_gen_mqtt_key_local), 0, 0, 1, 1},
   {&__pyx_n_s_MqttWrapper_publish, __pyx_k_MqttWrapper_publish, sizeof(__pyx_k_MqttWrapper_publish), 0, 0, 1, 1},
   {&__pyx_n_s_MqttWrapper_run, __pyx_k_MqttWrapper_run, sizeof(__pyx_k_MqttWrapper_run), 0, 0, 1, 1},
   {&__pyx_n_s_MqttWrapper_stop, __pyx_k_MqttWrapper_stop, sizeof(__pyx_k_MqttWrapper_stop), 0, 0, 1, 1},
   {&__pyx_n_s_Optional, __pyx_k_Optional, sizeof(__pyx_k_Optional), 0, 0, 1, 1},
+  {&__pyx_n_s_PREFIX, __pyx_k_PREFIX, sizeof(__pyx_k_PREFIX), 0, 0, 1, 1},
   {&__pyx_kp_u_Received_a_message, __pyx_k_Received_a_message, sizeof(__pyx_k_Received_a_message), 0, 1, 0, 0},
   {&__pyx_kp_s_Represents_a_Viso_MQTT_related_A, __pyx_k_Represents_a_Viso_MQTT_related_A, sizeof(__pyx_k_Represents_a_Viso_MQTT_related_A), 0, 0, 1, 0},
   {&__pyx_n_s_Thread, __pyx_k_Thread, sizeof(__pyx_k_Thread), 0, 0, 1, 1},
   {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
+  {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_b_stop, __pyx_k_b_stop, sizeof(__pyx_k_b_stop), 0, 0, 1, 1},
   {&__pyx_n_s_callbacks, __pyx_k_callbacks, sizeof(__pyx_k_callbacks), 0, 0, 1, 1},
   {&__pyx_n_s_clear, __pyx_k_clear, sizeof(__pyx_k_clear), 0, 0, 1, 1},
   {&__pyx_n_s_client, __pyx_k_client, sizeof(__pyx_k_client), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_connect, __pyx_k_connect, sizeof(__pyx_k_connect), 0, 0, 1, 1},
   {&__pyx_n_s_debug, __pyx_k_debug, sizeof(__pyx_k_debug), 0, 0, 1, 1},
   {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
   {&__pyx_n_s_err, __pyx_k_err, sizeof(__pyx_k_err), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
+  {&__pyx_n_s_gen_mqtt_key_cloud, __pyx_k_gen_mqtt_key_cloud, sizeof(__pyx_k_gen_mqtt_key_cloud), 0, 0, 1, 1},
+  {&__pyx_n_s_gen_mqtt_key_debug, __pyx_k_gen_mqtt_key_debug, sizeof(__pyx_k_gen_mqtt_key_debug), 0, 0, 1, 1},
+  {&__pyx_n_s_gen_mqtt_key_local, __pyx_k_gen_mqtt_key_local, sizeof(__pyx_k_gen_mqtt_key_local), 0, 0, 1, 1},
   {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
   {&__pyx_n_s_get_logger, __pyx_k_get_logger, sizeof(__pyx_k_get_logger), 0, 0, 1, 1},
   {&__pyx_n_s_host, __pyx_k_host, sizeof(__pyx_k_host), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_info, __pyx_k_info, sizeof(__pyx_k_info), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_is_connected, __pyx_k_is_connected, sizeof(__pyx_k_is_connected), 0, 0, 1, 1},
@@ -3669,14 +4212,15 @@
   {&__pyx_n_s_logger, __pyx_k_logger, sizeof(__pyx_k_logger), 0, 0, 1, 1},
   {&__pyx_n_s_loop_start, __pyx_k_loop_start, sizeof(__pyx_k_loop_start), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_msg, __pyx_k_msg, sizeof(__pyx_k_msg), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+  {&__pyx_n_s_node_id, __pyx_k_node_id, sizeof(__pyx_k_node_id), 0, 0, 1, 1},
   {&__pyx_n_s_on_connect, __pyx_k_on_connect, sizeof(__pyx_k_on_connect), 0, 0, 1, 1},
   {&__pyx_n_s_on_message, __pyx_k_on_message, sizeof(__pyx_k_on_message), 0, 0, 1, 1},
   {&__pyx_n_s_on_mqtt_connected, __pyx_k_on_mqtt_connected, sizeof(__pyx_k_on_mqtt_connected), 0, 0, 1, 1},
   {&__pyx_n_s_on_mqtt_message, __pyx_k_on_mqtt_message, sizeof(__pyx_k_on_mqtt_message), 0, 0, 1, 1},
   {&__pyx_kp_u_on_topic, __pyx_k_on_topic, sizeof(__pyx_k_on_topic), 0, 1, 0, 0},
   {&__pyx_n_s_paho_mqtt_client, __pyx_k_paho_mqtt_client, sizeof(__pyx_k_paho_mqtt_client), 0, 0, 1, 1},
   {&__pyx_n_s_payload, __pyx_k_payload, sizeof(__pyx_k_payload), 0, 0, 1, 1},
@@ -3686,31 +4230,34 @@
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {&__pyx_n_s_run, __pyx_k_run, sizeof(__pyx_k_run), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
   {&__pyx_n_s_sleep, __pyx_k_sleep, sizeof(__pyx_k_sleep), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
+  {&__pyx_n_s_staticmethod, __pyx_k_staticmethod, sizeof(__pyx_k_staticmethod), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_n_s_subscribe, __pyx_k_subscribe, sizeof(__pyx_k_subscribe), 0, 0, 1, 1},
   {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_threading, __pyx_k_threading, sizeof(__pyx_k_threading), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_topic, __pyx_k_topic, sizeof(__pyx_k_topic), 0, 0, 1, 1},
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
   {&__pyx_n_u_unicode, __pyx_k_unicode, sizeof(__pyx_k_unicode), 0, 1, 0, 1},
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_verbose, __pyx_k_verbose, sizeof(__pyx_k_verbose), 0, 0, 1, 1},
+  {&__pyx_n_s_viso_sdk_constants, __pyx_k_viso_sdk_constants, sizeof(__pyx_k_viso_sdk_constants), 0, 0, 1, 1},
   {&__pyx_n_s_viso_sdk_logging, __pyx_k_viso_sdk_logging, sizeof(__pyx_k_viso_sdk_logging), 0, 0, 1, 1},
   {&__pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_k_viso_sdk_mqtt_mqtt_wrapper, sizeof(__pyx_k_viso_sdk_mqtt_mqtt_wrapper), 0, 0, 1, 1},
   {&__pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_k_viso_sdk_mqtt_mqtt_wrapper_py, sizeof(__pyx_k_viso_sdk_mqtt_mqtt_wrapper_py), 0, 0, 1, 0},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
+  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 58, __pyx_L1_error)
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 46, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -3720,104 +4267,140 @@
   /* "viso_sdk/mqtt/mqtt_wrapper.py":14
  * 
  * 
  * logger = get_logger("MQTT")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_u_MQTT); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 14, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_u_MQTT); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "viso_sdk/mqtt/mqtt_wrapper.py":39
  *     """
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             host: Optional[str] = "127.0.0.1",
  */
-  __pyx_tuple__5 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_host, __pyx_n_s_port, __pyx_n_s_callbacks, __pyx_n_s_verbose); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_init, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __pyx_tuple__7 = PyTuple_Pack(4, ((PyObject*)__pyx_kp_u_127_0_0_1), ((PyObject *)__pyx_int_1883), ((PyObject *)Py_None), ((PyObject *)Py_True)); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_host, __pyx_n_s_port, __pyx_n_s_callbacks, __pyx_n_s_verbose); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_init, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(4, ((PyObject*)__pyx_kp_u_127_0_0_1), ((PyObject *)__pyx_int_1883), ((PyObject *)Py_None), ((PyObject *)Py_True)); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":58
- *         self.start()
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":59
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_local(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.LOCAL}_{node_id}_{port}"
+ * 
+ */
+  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_s_node_id, __pyx_n_s_port); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_gen_mqtt_key_local, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 59, __pyx_L1_error)
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":63
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_cloud(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.CLOUD}_{node_id}_{port}"
+ * 
+ */
+  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_node_id, __pyx_n_s_port); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_gen_mqtt_key_cloud, 63, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 63, __pyx_L1_error)
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":67
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_debug(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
+ * 
+ */
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_node_id, __pyx_n_s_port); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_gen_mqtt_key_debug, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 67, __pyx_L1_error)
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":70
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
  * 
  *     def connect(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Connect to the target MQTT broker"""
  *         try:
  */
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_err); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_connect, 58, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_err); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_connect, 70, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 70, __pyx_L1_error)
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":68
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":80
  *         return True
  * 
  *     def run(self) -> None:             # <<<<<<<<<<<<<<
  *         """Main thread loop"""
  *         while not self._b_stop.is_set():
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 68, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_run, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_run, 80, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 80, __pyx_L1_error)
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":76
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":88
  *             time.sleep(1)
  * 
  *     def _on_mqtt_connected(self, *args: Any) -> None:             # <<<<<<<<<<<<<<
  *         """Callback when MQTT is connected"""
  *         logger.info(f"Connected to the MQTT broker - {args}")
  */
-  __pyx_tuple__12 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_args, __pyx_n_s_topic); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_on_mqtt_connected, 76, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_args, __pyx_n_s_topic); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_on_mqtt_connected, 88, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 88, __pyx_L1_error)
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":83
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":95
  *                 self._client.subscribe(topic=topic)
  * 
  *     def _on_mqtt_message(self, *args: Any) -> None:             # <<<<<<<<<<<<<<
  *         """Callback when a message on subscribed channels is received."""
  *         topic = args[2].topic
  */
-  __pyx_tuple__14 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_args, __pyx_n_s_topic, __pyx_n_s_msg); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_on_mqtt_message, 83, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_args, __pyx_n_s_topic, __pyx_n_s_msg); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_on_mqtt_message, 95, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 95, __pyx_L1_error)
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":95
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":107
  *             logger.error(f"Callback of topic '{topic}' is not callable!")
  * 
  *     def publish(self, topic: str, payload: str) -> None:             # <<<<<<<<<<<<<<
  *         """Publish a message to a topic"""
  *         self._client.publish(topic=topic, payload=payload)
  */
-  __pyx_tuple__16 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_topic, __pyx_n_s_payload); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_publish, 95, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_topic, __pyx_n_s_payload); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_publish, 107, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 107, __pyx_L1_error)
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":99
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":111
  *         self._client.publish(topic=topic, payload=payload)
  * 
  *     def stop(self) -> None:             # <<<<<<<<<<<<<<
  *         """Stop this thread"""
  *         self._b_stop.set()
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 99, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_stop, 99, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_mqtt_mqtt_wrapper_py, __pyx_n_s_stop, 111, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -4163,15 +4746,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "viso_sdk/mqtt/mqtt_wrapper.py":8
  * import time
  * from typing import Any, Optional, Union
  * from paho.mqtt.client import Client             # <<<<<<<<<<<<<<
  * 
- * 
+ * from viso_sdk.constants import PREFIX
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Client);
   __Pyx_GIVEREF(__pyx_n_s_Client);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Client);
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_paho_mqtt_client, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
@@ -4179,70 +4762,91 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Client); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Client, __pyx_t_2) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":11
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":10
+ * from paho.mqtt.client import Client
  * 
+ * from viso_sdk.constants import PREFIX             # <<<<<<<<<<<<<<
+ * from viso_sdk.logging import get_logger
  * 
+ */
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_n_s_PREFIX);
+  __Pyx_GIVEREF(__pyx_n_s_PREFIX);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PREFIX);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_viso_sdk_constants, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_PREFIX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_PREFIX, __pyx_t_1) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":11
+ * 
+ * from viso_sdk.constants import PREFIX
  * from viso_sdk.logging import get_logger             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_get_logger);
   __Pyx_GIVEREF(__pyx_n_s_get_logger);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_get_logger);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_viso_sdk_logging, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_get_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_get_logger);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_viso_sdk_logging, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_logger, __pyx_t_1) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_get_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_logger, __pyx_t_2) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "viso_sdk/mqtt/mqtt_wrapper.py":14
  * 
  * 
  * logger = get_logger("MQTT")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logger, __pyx_t_1) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logger, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "viso_sdk/mqtt/mqtt_wrapper.py":17
  * 
  * 
  * class MqttWrapper(threading.Thread):             # <<<<<<<<<<<<<<
  *     """Represents a Viso MQTT related API instance
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_threading); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Thread); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_threading); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Thread); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_MqttWrapper, __pyx_n_s_MqttWrapper, (PyObject *) NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_kp_s_Represents_a_Viso_MQTT_related_A); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_MqttWrapper, __pyx_n_s_MqttWrapper, (PyObject *) NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_kp_s_Represents_a_Viso_MQTT_related_A); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
   /* "viso_sdk/mqtt/mqtt_wrapper.py":39
  *     """
  * 
@@ -4331,163 +4935,232 @@
   /* "viso_sdk/mqtt/mqtt_wrapper.py":39
  *     """
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             host: Optional[str] = "127.0.0.1",
  */
-  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_1__init__, 0, __pyx_n_s_MqttWrapper___init, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_1__init__, 0, __pyx_n_s_MqttWrapper___init, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_INCREF(__pyx_t_9);
   PyList_Append(__pyx_t_4, __pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_9);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_9, __pyx_tuple__7);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_9, __pyx_tuple__8);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_9, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_9) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":59
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_local(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.LOCAL}_{node_id}_{port}"
+ * 
+ */
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3gen_mqtt_key_local, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MqttWrapper_gen_mqtt_key_local, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+
   /* "viso_sdk/mqtt/mqtt_wrapper.py":58
  *         self.start()
  * 
+ *     @staticmethod             # <<<<<<<<<<<<<<
+ *     def gen_mqtt_key_local(node_id, port):
+ *         return f"{PREFIX.MQTT.LOCAL}_{node_id}_{port}"
+ */
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_gen_mqtt_key_local, __pyx_t_5) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":63
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_cloud(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.CLOUD}_{node_id}_{port}"
+ * 
+ */
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5gen_mqtt_key_cloud, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MqttWrapper_gen_mqtt_key_cloud, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":62
+ *         return f"{PREFIX.MQTT.LOCAL}_{node_id}_{port}"
+ * 
+ *     @staticmethod             # <<<<<<<<<<<<<<
+ *     def gen_mqtt_key_cloud(node_id, port):
+ *         return f"{PREFIX.MQTT.CLOUD}_{node_id}_{port}"
+ */
+  __pyx_t_9 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_gen_mqtt_key_cloud, __pyx_t_9) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":67
+ * 
+ *     @staticmethod
+ *     def gen_mqtt_key_debug(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
+ * 
+ */
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7gen_mqtt_key_debug, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MqttWrapper_gen_mqtt_key_debug, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":66
+ *         return f"{PREFIX.MQTT.CLOUD}_{node_id}_{port}"
+ * 
+ *     @staticmethod             # <<<<<<<<<<<<<<
+ *     def gen_mqtt_key_debug(node_id, port):
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
+ */
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_gen_mqtt_key_debug, __pyx_t_5) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":70
+ *         return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
+ * 
  *     def connect(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Connect to the target MQTT broker"""
  *         try:
  */
-  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_3connect, 0, __pyx_n_s_MqttWrapper_connect, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_9);
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_connect, __pyx_t_5) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9connect, 0, __pyx_n_s_MqttWrapper_connect, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_9, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_connect, __pyx_t_9) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":68
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":80
  *         return True
  * 
  *     def run(self) -> None:             # <<<<<<<<<<<<<<
  *         """Main thread loop"""
  *         while not self._b_stop.is_set():
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_5run, 0, __pyx_n_s_MqttWrapper_run, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_9, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_run, __pyx_t_9) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11run, 0, __pyx_n_s_MqttWrapper_run, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_9);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_run, __pyx_t_5) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":76
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":88
  *             time.sleep(1)
  * 
  *     def _on_mqtt_connected(self, *args: Any) -> None:             # <<<<<<<<<<<<<<
  *         """Callback when MQTT is connected"""
  *         logger.info(f"Connected to the MQTT broker - {args}")
  */
-  __pyx_t_9 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Any); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_args, __pyx_t_5) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_7_on_mqtt_connected, 0, __pyx_n_s_MqttWrapper__on_mqtt_connected, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_9);
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_Any); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_args, __pyx_t_9) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_on_mqtt_connected, __pyx_t_5) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13_on_mqtt_connected, 0, __pyx_n_s_MqttWrapper__on_mqtt_connected, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_9, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_on_mqtt_connected, __pyx_t_9) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":83
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":95
  *                 self._client.subscribe(topic=topic)
  * 
  *     def _on_mqtt_message(self, *args: Any) -> None:             # <<<<<<<<<<<<<<
  *         """Callback when a message on subscribed channels is received."""
  *         topic = args[2].topic
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_Any); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_args, __pyx_t_9) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_9_on_mqtt_message, 0, __pyx_n_s_MqttWrapper__on_mqtt_message, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_9, __pyx_t_5);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Any); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_args, __pyx_t_5) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_on_mqtt_message, __pyx_t_9) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_15_on_mqtt_message, 0, __pyx_n_s_MqttWrapper__on_mqtt_message, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_9);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_on_mqtt_message, __pyx_t_5) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":95
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":107
  *             logger.error(f"Callback of topic '{topic}' is not callable!")
  * 
  *     def publish(self, topic: str, payload: str) -> None:             # <<<<<<<<<<<<<<
  *         """Publish a message to a topic"""
  *         self._client.publish(topic=topic, payload=payload)
  */
-  __pyx_t_9 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_topic, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_payload, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_11publish, 0, __pyx_n_s_MqttWrapper_publish, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_9);
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_publish, __pyx_t_5) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_topic, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_payload, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_17publish, 0, __pyx_n_s_MqttWrapper_publish, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_9, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_publish, __pyx_t_9) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "viso_sdk/mqtt/mqtt_wrapper.py":99
+  /* "viso_sdk/mqtt/mqtt_wrapper.py":111
  *         self._client.publish(topic=topic, payload=payload)
  * 
  *     def stop(self) -> None:             # <<<<<<<<<<<<<<
  *         """Stop this thread"""
  *         self._b_stop.set()
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_13stop, 0, __pyx_n_s_MqttWrapper_stop, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_9, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_stop, __pyx_t_9) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_return, Py_None) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_4mqtt_12mqtt_wrapper_11MqttWrapper_19stop, 0, __pyx_n_s_MqttWrapper_stop, NULL, __pyx_n_s_viso_sdk_mqtt_mqtt_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_9);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_stop, __pyx_t_5) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "viso_sdk/mqtt/mqtt_wrapper.py":17
  * 
  * 
  * class MqttWrapper(threading.Thread):             # <<<<<<<<<<<<<<
  *     """Represents a Viso MQTT related API instance
  * 
  */
-  __pyx_t_9 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_MqttWrapper, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  if (__Pyx_CyFunction_InitClassCell(__pyx_t_4, __pyx_t_9) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_MqttWrapper, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__Pyx_CyFunction_InitClassCell(__pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MqttWrapper, __pyx_t_9) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MqttWrapper, __pyx_t_5) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "viso_sdk/mqtt/mqtt_wrapper.py":1
  * """             # <<<<<<<<<<<<<<
  * MQTT Wrapper from viso.ai
  * """
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -5020,14 +5693,76 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
+/* JoinPyUnicode */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      CYTHON_UNUSED Py_UCS4 max_char) {
+#if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    PyObject *result_uval;
+    int result_ukind;
+    Py_ssize_t i, char_pos;
+    void *result_udata;
+#if CYTHON_PEP393_ENABLED
+    result_uval = PyUnicode_New(result_ulength, max_char);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
+    result_udata = PyUnicode_DATA(result_uval);
+#else
+    result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = sizeof(Py_UNICODE);
+    result_udata = PyUnicode_AS_UNICODE(result_uval);
+#endif
+    char_pos = 0;
+    for (i=0; i < value_count; i++) {
+        int ukind;
+        Py_ssize_t ulength;
+        void *udata;
+        PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
+        if (unlikely(__Pyx_PyUnicode_READY(uval)))
+            goto bad;
+        ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
+        if (unlikely(!ulength))
+            continue;
+        if (unlikely(char_pos + ulength < 0))
+            goto overflow;
+        ukind = __Pyx_PyUnicode_KIND(uval);
+        udata = __Pyx_PyUnicode_DATA(uval);
+        if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
+            memcpy((char *)result_udata + char_pos * result_ukind, udata, (size_t) (ulength * result_ukind));
+        } else {
+            #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
+            _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
+            #else
+            Py_ssize_t j;
+            for (j=0; j < ulength; j++) {
+                Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
+                __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
+            }
+            #endif
+        }
+        char_pos += ulength;
+    }
+    return result_uval;
+overflow:
+    PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
+bad:
+    Py_DECREF(result_uval);
+    return NULL;
+#else
+    result_ulength++;
+    value_count++;
+    return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
+#endif
+}
+
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -5175,76 +5910,14 @@
     *tb = 0;
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
-/* JoinPyUnicode */
-static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
-                                      CYTHON_UNUSED Py_UCS4 max_char) {
-#if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    PyObject *result_uval;
-    int result_ukind;
-    Py_ssize_t i, char_pos;
-    void *result_udata;
-#if CYTHON_PEP393_ENABLED
-    result_uval = PyUnicode_New(result_ulength, max_char);
-    if (unlikely(!result_uval)) return NULL;
-    result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
-    result_udata = PyUnicode_DATA(result_uval);
-#else
-    result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
-    if (unlikely(!result_uval)) return NULL;
-    result_ukind = sizeof(Py_UNICODE);
-    result_udata = PyUnicode_AS_UNICODE(result_uval);
-#endif
-    char_pos = 0;
-    for (i=0; i < value_count; i++) {
-        int ukind;
-        Py_ssize_t ulength;
-        void *udata;
-        PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
-        if (unlikely(__Pyx_PyUnicode_READY(uval)))
-            goto bad;
-        ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
-        if (unlikely(!ulength))
-            continue;
-        if (unlikely(char_pos + ulength < 0))
-            goto overflow;
-        ukind = __Pyx_PyUnicode_KIND(uval);
-        udata = __Pyx_PyUnicode_DATA(uval);
-        if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
-            memcpy((char *)result_udata + char_pos * result_ukind, udata, (size_t) (ulength * result_ukind));
-        } else {
-            #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
-            _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
-            #else
-            Py_ssize_t j;
-            for (j=0; j < ulength; j++) {
-                Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
-                __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
-            }
-            #endif
-        }
-        char_pos += ulength;
-    }
-    return result_uval;
-overflow:
-    PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
-bad:
-    Py_DECREF(result_uval);
-    return NULL;
-#else
-    result_ulength++;
-    value_count++;
-    return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
-#endif
-}
-
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
```

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/mqtt/mqtt_wrapper.py` & `viso-sdk-python-0.0.5/viso_sdk/mqtt/mqtt_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import threading
 import time
 from typing import Any, Optional, Union
 from paho.mqtt.client import Client
 
-
+from viso_sdk.constants import PREFIX
 from viso_sdk.logging import get_logger
 
 
 logger = get_logger("MQTT")
 
 
 class MqttWrapper(threading.Thread):
@@ -51,14 +51,26 @@
         self._client.on_connect = self._on_mqtt_connected
         self._client.on_message = self._on_mqtt_message
         self._b_stop = threading.Event()
         self._b_stop.clear()
         self.verbose = verbose
         self.start()
 
+    @staticmethod
+    def gen_mqtt_key_local(node_id, port):
+        return f"{PREFIX.MQTT.LOCAL}_{node_id}_{port}"
+
+    @staticmethod
+    def gen_mqtt_key_cloud(node_id, port):
+        return f"{PREFIX.MQTT.CLOUD}_{node_id}_{port}"
+
+    @staticmethod
+    def gen_mqtt_key_debug(node_id, port):
+        return f"{PREFIX.MQTT.DEBUG}_{node_id}_{port}"
+
     def connect(self) -> bool:
         """Connect to the target MQTT broker"""
         try:
             self._client.connect(self.host, self.port)
         except Exception as err:
             logger.error(f"Failed to connect to {self.host}:{self.port} - {err}")
             return False
```

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/nodered/__init__.c` & `viso-sdk-python-0.0.5/viso_sdk/nodered/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/nodered/flow.c` & `viso-sdk-python-0.0.5/viso_sdk/nodered/flow.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/nodered/flow.py` & `viso-sdk-python-0.0.5/viso_sdk/nodered/flow.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/redis/__init__.c` & `viso-sdk-python-0.0.5/viso_sdk/redis/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/redis/redis_wrapper.c` & `viso-sdk-python-0.0.5/viso_sdk/redis/redis_wrapper.c`

 * *Files 1% similar despite different names*

```diff
@@ -1156,14 +1156,43 @@
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
+/* PyObjectFormatSimple.proto */
+#if CYTHON_COMPILING_IN_PYPY
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#elif PY_MAJOR_VERSION < 3
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyString_CheckExact(s)) ? PyUnicode_FromEncodedObject(s, NULL, "strict") :\
+        PyObject_Format(s, f))
+#elif CYTHON_USE_TYPE_SLOTS
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyLong_CheckExact(s)) ? PyLong_Type.tp_str(s) :\
+        likely(PyFloat_CheckExact(s)) ? PyFloat_Type.tp_str(s) :\
+        PyObject_Format(s, f))
+#else
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* JoinPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char);
+
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
@@ -1210,36 +1239,14 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
-/* PyObjectFormatSimple.proto */
-#if CYTHON_COMPILING_IN_PYPY
-    #define __Pyx_PyObject_FormatSimple(s, f) (\
-        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
-        PyObject_Format(s, f))
-#elif PY_MAJOR_VERSION < 3
-    #define __Pyx_PyObject_FormatSimple(s, f) (\
-        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
-        likely(PyString_CheckExact(s)) ? PyUnicode_FromEncodedObject(s, NULL, "strict") :\
-        PyObject_Format(s, f))
-#elif CYTHON_USE_TYPE_SLOTS
-    #define __Pyx_PyObject_FormatSimple(s, f) (\
-        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
-        likely(PyLong_CheckExact(s)) ? PyLong_Type.tp_str(s) :\
-        likely(PyFloat_CheckExact(s)) ? PyFloat_Type.tp_str(s) :\
-        PyObject_Format(s, f))
-#else
-    #define __Pyx_PyObject_FormatSimple(s, f) (\
-        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
-        PyObject_Format(s, f))
-#endif
-
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
@@ -1295,21 +1302,14 @@
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
 /* PyUnicode_Unicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj);
 
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* JoinPyUnicode.proto */
-static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
-                                      Py_UCS4 max_char);
-
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* FetchCommonType.proto */
@@ -1487,15 +1487,16 @@
 /* Module declarations from 'viso_sdk.redis.redis_wrapper' */
 #define __Pyx_MODULE_NAME "viso_sdk.redis.redis_wrapper"
 extern int __pyx_module_is_main_viso_sdk__redis__redis_wrapper;
 int __pyx_module_is_main_viso_sdk__redis__redis_wrapper = 0;
 
 /* Implementation of 'viso_sdk.redis.redis_wrapper' */
 static PyObject *__pyx_builtin_staticmethod;
-static const char __pyx_k_[] = " - ";
+static const char __pyx_k_[] = "_";
+static const char __pyx_k__2[] = " - ";
 static const char __pyx_k_fx[] = "fx";
 static const char __pyx_k_fy[] = "fy";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_Any[] = "Any";
 static const char __pyx_k_cv2[] = "cv2";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_err[] = "err";
@@ -1511,40 +1512,44 @@
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_port[] = "port";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_zoom[] = "zoom";
+static const char __pyx_k_LOCAL[] = "LOCAL";
 static const char __pyx_k_REDIS[] = "REDIS";
 static const char __pyx_k_Union[] = "Union";
 static const char __pyx_k_bytes[] = "bytes";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_frame[] = "frame";
 static const char __pyx_k_image[] = "image";
 static const char __pyx_k_jpg_2[] = "jpg";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_redis[] = "redis";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_tuple[] = "tuple";
 static const char __pyx_k_uint8[] = "uint8";
+static const char __pyx_k_PREFIX[] = "PREFIX";
+static const char __pyx_k_STATUS[] = "STATUS";
 static const char __pyx_k_Thread[] = "Thread";
 static const char __pyx_k_base64[] = "base64";
 static const char __pyx_k_delete[] = "delete";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_logger[] = "logger";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_resize[] = "resize";
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_target[] = "target";
 static const char __pyx_k_thread[] = "thread";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_img_arr[] = "_img_arr";
 static const char __pyx_k_ndarray[] = "ndarray";
+static const char __pyx_k_node_id[] = "node_id";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_unicode[] = "unicode";
 static const char __pyx_k_warning[] = "warning";
 static const char __pyx_k_Optional[] = "Optional";
 static const char __pyx_k_imdecode[] = "imdecode";
 static const char __pyx_k_imencode[] = "imencode";
 static const char __pyx_k_put_data[] = "put_data";
@@ -1571,15 +1576,18 @@
 static const char __pyx_k_redis_client[] = "_redis_client";
 static const char __pyx_k_staticmethod[] = "staticmethod";
 static const char __pyx_k_base64_to_img[] = "base64_to_img";
 static const char __pyx_k_write_to_redis[] = "_write_to_redis";
 static const char __pyx_k_img_to_base64str[] = "img_to_base64str";
 static const char __pyx_k_viso_sdk_logging[] = "viso_sdk.logging";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_viso_sdk_constants[] = "viso_sdk.constants";
 static const char __pyx_k_RedisWrapper___init[] = "RedisWrapper.__init__";
+static const char __pyx_k_gen_redis_key_local[] = "gen_redis_key_local";
+static const char __pyx_k_gen_redis_key_status[] = "gen_redis_key_status";
 static const char __pyx_k_RedisWrapper_put_data[] = "RedisWrapper.put_data";
 static const char __pyx_k_RedisWrapper_get_frame[] = "RedisWrapper.get_frame";
 static const char __pyx_k_RedisWrapper_read_data[] = "RedisWrapper.read_data";
 static const char __pyx_k_RedisWrapper_delete_data[] = "RedisWrapper.delete_data";
 static const char __pyx_k_RedisWrapper_write_frame[] = "RedisWrapper.write_frame";
 static const char __pyx_k_RedisWrapper_base64_to_img[] = "RedisWrapper.base64_to_img";
 static const char __pyx_k_Redis_Wrapper_from_viso_ai[] = "\nRedis Wrapper from viso.ai\n";
@@ -1587,38 +1595,47 @@
 static const char __pyx_k_viso_sdk_redis_redis_wrapper[] = "viso_sdk.redis.redis_wrapper";
 static const char __pyx_k_RedisWrapper_img_to_base64str[] = "RedisWrapper.img_to_base64str";
 static const char __pyx_k_Failed_to_get_redis_frame_from[] = "Failed to get redis frame from ";
 static const char __pyx_k_Failed_to_write_frame_to_redis[] = "Failed to write frame to redis - ";
 static const char __pyx_k_viso_sdk_redis_redis_wrapper_py[] = "viso_sdk/redis/redis_wrapper.py";
 static const char __pyx_k_Failed_to_convert_base64_to_imag[] = "Failed to convert base64 to image - ";
 static const char __pyx_k_Failed_to_convert_stream_to_writ[] = "Failed to convert stream to write to redis";
+static const char __pyx_k_RedisWrapper_gen_redis_key_local[] = "RedisWrapper.gen_redis_key_local";
+static const char __pyx_k_RedisWrapper_gen_redis_key_statu[] = "RedisWrapper.gen_redis_key_status";
 static const char __pyx_k_Represents_a_redis_client_specif[] = "Represents a redis client specified for the containers.\n\n    Args:\n        thread(bool): Use threading or not\n        host(str): Redis server host\n        port(int): Redis server port\n    ";
-static PyObject *__pyx_kp_u_;
+static PyObject *__pyx_n_u_;
 static PyObject *__pyx_n_s_Any;
 static PyObject *__pyx_kp_u_Failed_to_convert_base64_to_imag;
 static PyObject *__pyx_kp_u_Failed_to_convert_stream_to_writ;
 static PyObject *__pyx_kp_u_Failed_to_get_redis_frame_from;
 static PyObject *__pyx_kp_u_Failed_to_write_frame_to_redis;
+static PyObject *__pyx_n_s_LOCAL;
 static PyObject *__pyx_kp_u_None;
 static PyObject *__pyx_n_s_Optional;
+static PyObject *__pyx_n_s_PREFIX;
+static PyObject *__pyx_n_s_REDIS;
 static PyObject *__pyx_n_u_REDIS;
 static PyObject *__pyx_n_s_RedisWrapper;
 static PyObject *__pyx_n_s_RedisWrapper___init;
 static PyObject *__pyx_n_s_RedisWrapper__write_to_redis;
 static PyObject *__pyx_n_s_RedisWrapper_base64_to_img;
 static PyObject *__pyx_n_s_RedisWrapper_delete_data;
+static PyObject *__pyx_n_s_RedisWrapper_gen_redis_key_local;
+static PyObject *__pyx_n_s_RedisWrapper_gen_redis_key_statu;
 static PyObject *__pyx_n_s_RedisWrapper_get_frame;
 static PyObject *__pyx_n_s_RedisWrapper_img_to_base64str;
 static PyObject *__pyx_n_s_RedisWrapper_put_data;
 static PyObject *__pyx_n_s_RedisWrapper_read_data;
 static PyObject *__pyx_n_s_RedisWrapper_write_frame;
 static PyObject *__pyx_kp_s_Represents_a_redis_client_specif;
+static PyObject *__pyx_n_s_STATUS;
 static PyObject *__pyx_n_s_StrictRedis;
 static PyObject *__pyx_n_s_Thread;
 static PyObject *__pyx_n_s_Union;
+static PyObject *__pyx_kp_u__2;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_b64_bytes;
 static PyObject *__pyx_n_s_b64decode;
 static PyObject *__pyx_n_s_b64encode;
 static PyObject *__pyx_n_s_base64;
 static PyObject *__pyx_n_s_base64_to_img;
 static PyObject *__pyx_n_u_bytes;
@@ -1631,14 +1648,16 @@
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_err;
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_frame;
 static PyObject *__pyx_n_s_frombuffer;
 static PyObject *__pyx_n_s_fx;
 static PyObject *__pyx_n_s_fy;
+static PyObject *__pyx_n_s_gen_redis_key_local;
+static PyObject *__pyx_n_s_gen_redis_key_status;
 static PyObject *__pyx_n_s_get;
 static PyObject *__pyx_n_s_get_frame;
 static PyObject *__pyx_n_s_get_logger;
 static PyObject *__pyx_n_s_host;
 static PyObject *__pyx_n_s_image;
 static PyObject *__pyx_n_s_imdecode;
 static PyObject *__pyx_n_s_imencode;
@@ -1653,14 +1672,15 @@
 static PyObject *__pyx_n_u_localhost;
 static PyObject *__pyx_n_s_logger;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_ndarray;
+static PyObject *__pyx_n_s_node_id;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_n_s_port;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_put_data;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_read_data;
@@ -1680,60 +1700,67 @@
 static PyObject *__pyx_n_s_thread;
 static PyObject *__pyx_n_s_threading;
 static PyObject *__pyx_n_u_tuple;
 static PyObject *__pyx_n_s_typing;
 static PyObject *__pyx_n_s_uint8;
 static PyObject *__pyx_n_u_unicode;
 static PyObject *__pyx_n_s_use_thread;
+static PyObject *__pyx_n_s_viso_sdk_constants;
 static PyObject *__pyx_n_s_viso_sdk_logging;
 static PyObject *__pyx_n_s_viso_sdk_redis_redis_wrapper;
 static PyObject *__pyx_kp_s_viso_sdk_redis_redis_wrapper_py;
 static PyObject *__pyx_n_s_warning;
 static PyObject *__pyx_n_s_write_frame;
 static PyObject *__pyx_n_s_write_to_redis;
 static PyObject *__pyx_n_s_zoom;
 static PyObject *__pyx_n_s_zoom_ratio;
 static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_thread, PyObject *__pyx_v_host, PyObject *__pyx_v_port); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_2base64_to_img(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_b64_bytes); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_4img_to_base64str(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_image, PyObject *__pyx_v_zoom_ratio); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6write_frame(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_zoom); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8_write_to_redis(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_zoom); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10delete_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12put_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14read_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16get_frame(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_2gen_redis_key_local(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_4gen_redis_key_status(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6base64_to_img(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_b64_bytes); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8img_to_base64str(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_image, PyObject *__pyx_v_zoom_ratio); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10write_frame(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_zoom); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12_write_to_redis(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_zoom); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14delete_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16put_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_18read_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_20get_frame(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key); /* proto */
 static PyObject *__pyx_float_1_0;
 static PyObject *__pyx_int_6379;
 static PyObject *__pyx_int_neg_1;
-static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
+static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__13;
-static PyObject *__pyx_tuple__14;
+static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__21;
-static PyObject *__pyx_tuple__23;
-static PyObject *__pyx_codeobj__4;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_tuple__22;
+static PyObject *__pyx_tuple__24;
+static PyObject *__pyx_tuple__26;
+static PyObject *__pyx_tuple__28;
+static PyObject *__pyx_codeobj__5;
+static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_codeobj__10;
 static PyObject *__pyx_codeobj__12;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_codeobj__17;
 static PyObject *__pyx_codeobj__20;
-static PyObject *__pyx_codeobj__22;
-static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_codeobj__23;
+static PyObject *__pyx_codeobj__25;
+static PyObject *__pyx_codeobj__27;
+static PyObject *__pyx_codeobj__29;
 /* Late includes */
 
-/* "viso_sdk/redis/redis_wrapper.py":29
+/* "viso_sdk/redis/redis_wrapper.py":30
  *     """
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             thread: bool = True,
  */
 
@@ -1751,15 +1778,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_thread,&__pyx_n_s_host,&__pyx_n_s_port,0};
     PyObject* values[4] = {0,0,0,0};
 
-    /* "viso_sdk/redis/redis_wrapper.py":31
+    /* "viso_sdk/redis/redis_wrapper.py":32
  *     def __init__(
  *             self,
  *             thread: bool = True,             # <<<<<<<<<<<<<<
  *             host: str = "localhost",
  *             port: int = 6379,
  */
     values[1] = ((PyObject *)((PyObject *)Py_True));
@@ -1801,15 +1828,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_port);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 29, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 30, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -1823,24 +1850,24 @@
     __pyx_v_self = values[0];
     __pyx_v_thread = values[1];
     __pyx_v_host = ((PyObject*)values[2]);
     __pyx_v_port = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 29, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 30, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_host), (&PyUnicode_Type), 1, "host", 1))) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_host), (&PyUnicode_Type), 1, "host", 1))) __PYX_ERR(0, 33, __pyx_L1_error)
   __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper___init__(__pyx_self, __pyx_v_self, __pyx_v_thread, __pyx_v_host, __pyx_v_port);
 
-  /* "viso_sdk/redis/redis_wrapper.py":29
+  /* "viso_sdk/redis/redis_wrapper.py":30
  *     """
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             thread: bool = True,
  */
 
@@ -1863,33 +1890,33 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "viso_sdk/redis/redis_wrapper.py":35
+  /* "viso_sdk/redis/redis_wrapper.py":36
  *             port: int = 6379,
  *     ):
  *         self._use_thread = thread             # <<<<<<<<<<<<<<
  *         self._redis_client = redis.StrictRedis(host, port)
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_use_thread, __pyx_v_thread) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_use_thread, __pyx_v_thread) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
 
-  /* "viso_sdk/redis/redis_wrapper.py":36
+  /* "viso_sdk/redis/redis_wrapper.py":37
  *     ):
  *         self._use_thread = thread
  *         self._redis_client = redis.StrictRedis(host, port)             # <<<<<<<<<<<<<<
  * 
  *         _img_arr = None
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_redis); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_redis); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_StrictRedis); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_StrictRedis); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -1899,58 +1926,58 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_host, __pyx_v_port};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_host, __pyx_v_port};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_v_host);
     __Pyx_GIVEREF(__pyx_v_host);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_host);
     __Pyx_INCREF(__pyx_v_port);
     __Pyx_GIVEREF(__pyx_v_port);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_port);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_redis_client, __pyx_t_1) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_redis_client, __pyx_t_1) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":38
+  /* "viso_sdk/redis/redis_wrapper.py":39
  *         self._redis_client = redis.StrictRedis(host, port)
  * 
  *         _img_arr = None             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_INCREF(Py_None);
   __pyx_v__img_arr = Py_None;
 
-  /* "viso_sdk/redis/redis_wrapper.py":29
+  /* "viso_sdk/redis/redis_wrapper.py":30
  *     """
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             thread: bool = True,
  */
 
@@ -1967,46 +1994,374 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v__img_arr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/redis/redis_wrapper.py":41
+/* "viso_sdk/redis/redis_wrapper.py":42
+ * 
+ *     @staticmethod
+ *     def gen_redis_key_local(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.REDIS.LOCAL}_{node_id}_{port}"
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3gen_redis_key_local(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3gen_redis_key_local = {"gen_redis_key_local", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3gen_redis_key_local, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3gen_redis_key_local(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_node_id = 0;
+  PyObject *__pyx_v_port = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen_redis_key_local (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node_id,&__pyx_n_s_port,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node_id)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_port)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen_redis_key_local", 1, 2, 2, 1); __PYX_ERR(0, 42, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gen_redis_key_local") < 0)) __PYX_ERR(0, 42, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_node_id = values[0];
+    __pyx_v_port = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("gen_redis_key_local", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 42, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.gen_redis_key_local", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_2gen_redis_key_local(__pyx_self, __pyx_v_node_id, __pyx_v_port);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_2gen_redis_key_local(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  Py_UCS4 __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("gen_redis_key_local", 0);
+
+  /* "viso_sdk/redis/redis_wrapper.py":43
+ *     @staticmethod
+ *     def gen_redis_key_local(node_id, port):
+ *         return f"{PREFIX.REDIS.LOCAL}_{node_id}_{port}"             # <<<<<<<<<<<<<<
+ * 
+ *     @staticmethod
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 127;
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_PREFIX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_REDIS); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_LOCAL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_node_id, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_port, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
+  goto __pyx_L0;
+
+  /* "viso_sdk/redis/redis_wrapper.py":42
+ * 
+ *     @staticmethod
+ *     def gen_redis_key_local(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.REDIS.LOCAL}_{node_id}_{port}"
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.gen_redis_key_local", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "viso_sdk/redis/redis_wrapper.py":46
+ * 
+ *     @staticmethod
+ *     def gen_redis_key_status(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.REDIS.STATUS}_{node_id}_{port}"
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5gen_redis_key_status(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5gen_redis_key_status = {"gen_redis_key_status", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5gen_redis_key_status, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5gen_redis_key_status(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_node_id = 0;
+  PyObject *__pyx_v_port = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen_redis_key_status (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node_id,&__pyx_n_s_port,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node_id)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_port)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen_redis_key_status", 1, 2, 2, 1); __PYX_ERR(0, 46, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gen_redis_key_status") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_node_id = values[0];
+    __pyx_v_port = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("gen_redis_key_status", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.gen_redis_key_status", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_4gen_redis_key_status(__pyx_self, __pyx_v_node_id, __pyx_v_port);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_4gen_redis_key_status(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node_id, PyObject *__pyx_v_port) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  Py_UCS4 __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("gen_redis_key_status", 0);
+
+  /* "viso_sdk/redis/redis_wrapper.py":47
+ *     @staticmethod
+ *     def gen_redis_key_status(node_id, port):
+ *         return f"{PREFIX.REDIS.STATUS}_{node_id}_{port}"             # <<<<<<<<<<<<<<
+ * 
+ *     @staticmethod
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 127;
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_PREFIX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_REDIS); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_STATUS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_node_id, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __Pyx_INCREF(__pyx_n_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_n_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_n_u_);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_port, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
+  goto __pyx_L0;
+
+  /* "viso_sdk/redis/redis_wrapper.py":46
+ * 
+ *     @staticmethod
+ *     def gen_redis_key_status(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.REDIS.STATUS}_{node_id}_{port}"
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.gen_redis_key_status", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "viso_sdk/redis/redis_wrapper.py":50
  * 
  *     @staticmethod
  *     def base64_to_img(b64_bytes: bytes) -> Union[None, np.ndarray]:             # <<<<<<<<<<<<<<
  *         """Convert base64 string to opencv frame"""
  *         try:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3base64_to_img(PyObject *__pyx_self, PyObject *__pyx_v_b64_bytes); /*proto*/
-static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_2base64_to_img[] = "Convert base64 string to opencv frame";
-static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3base64_to_img = {"base64_to_img", (PyCFunction)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3base64_to_img, METH_O, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_2base64_to_img};
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3base64_to_img(PyObject *__pyx_self, PyObject *__pyx_v_b64_bytes) {
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7base64_to_img(PyObject *__pyx_self, PyObject *__pyx_v_b64_bytes); /*proto*/
+static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6base64_to_img[] = "Convert base64 string to opencv frame";
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7base64_to_img = {"base64_to_img", (PyCFunction)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7base64_to_img, METH_O, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6base64_to_img};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7base64_to_img(PyObject *__pyx_self, PyObject *__pyx_v_b64_bytes) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("base64_to_img (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b64_bytes), (&PyBytes_Type), 1, "b64_bytes", 1))) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_2base64_to_img(__pyx_self, ((PyObject*)__pyx_v_b64_bytes));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b64_bytes), (&PyBytes_Type), 1, "b64_bytes", 1))) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6base64_to_img(__pyx_self, ((PyObject*)__pyx_v_b64_bytes));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_2base64_to_img(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_b64_bytes) {
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6base64_to_img(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_b64_bytes) {
   PyObject *__pyx_v_str_frame = NULL;
   PyObject *__pyx_v__img_arr = NULL;
   PyObject *__pyx_v_image = NULL;
   PyObject *__pyx_v_err = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -2029,15 +2384,15 @@
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("base64_to_img", 0);
 
-  /* "viso_sdk/redis/redis_wrapper.py":43
+  /* "viso_sdk/redis/redis_wrapper.py":52
  *     def base64_to_img(b64_bytes: bytes) -> Union[None, np.ndarray]:
  *         """Convert base64 string to opencv frame"""
  *         try:             # <<<<<<<<<<<<<<
  *             str_frame = base64.b64decode(b64_bytes)
  *             _img_arr = np.frombuffer(str_frame, dtype=np.uint8)
  */
   {
@@ -2045,92 +2400,92 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "viso_sdk/redis/redis_wrapper.py":44
+      /* "viso_sdk/redis/redis_wrapper.py":53
  *         """Convert base64 string to opencv frame"""
  *         try:
  *             str_frame = base64.b64decode(b64_bytes)             # <<<<<<<<<<<<<<
  *             _img_arr = np.frombuffer(str_frame, dtype=np.uint8)
  *             image = cv2.imdecode(  # pylint: disable=no-member
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_base64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 44, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_base64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 44, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
         }
       }
       __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_b64_bytes) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_b64_bytes);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L3_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_v_str_frame = __pyx_t_4;
       __pyx_t_4 = 0;
 
-      /* "viso_sdk/redis/redis_wrapper.py":45
+      /* "viso_sdk/redis/redis_wrapper.py":54
  *         try:
  *             str_frame = base64.b64decode(b64_bytes)
  *             _img_arr = np.frombuffer(str_frame, dtype=np.uint8)             # <<<<<<<<<<<<<<
  *             image = cv2.imdecode(  # pylint: disable=no-member
  *                 _img_arr, -1
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 45, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 45, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_frombuffer); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 45, __pyx_L3_error)
+      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_v_str_frame);
       __Pyx_GIVEREF(__pyx_v_str_frame);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_str_frame);
-      __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 45, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 45, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 54, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 45, __pyx_L3_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_uint8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 54, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 45, __pyx_L3_error)
+      if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 54, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 45, __pyx_L3_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 54, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v__img_arr = __pyx_t_8;
       __pyx_t_8 = 0;
 
-      /* "viso_sdk/redis/redis_wrapper.py":46
+      /* "viso_sdk/redis/redis_wrapper.py":55
  *             str_frame = base64.b64decode(b64_bytes)
  *             _img_arr = np.frombuffer(str_frame, dtype=np.uint8)
  *             image = cv2.imdecode(  # pylint: disable=no-member             # <<<<<<<<<<<<<<
  *                 _img_arr, -1
  *             )
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_cv2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 46, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_cv2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_imdecode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_imdecode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 55, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "viso_sdk/redis/redis_wrapper.py":47
+      /* "viso_sdk/redis/redis_wrapper.py":56
  *             _img_arr = np.frombuffer(str_frame, dtype=np.uint8)
  *             image = cv2.imdecode(  # pylint: disable=no-member
  *                 _img_arr, -1             # <<<<<<<<<<<<<<
  *             )
  *             # self._img_arr = None
  */
       __pyx_t_5 = NULL;
@@ -2144,107 +2499,107 @@
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v__img_arr, __pyx_int_neg_1};
-        __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 46, __pyx_L3_error)
+        __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 55, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_8);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v__img_arr, __pyx_int_neg_1};
-        __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 46, __pyx_L3_error)
+        __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 55, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_8);
       } else
       #endif
       {
-        __pyx_t_6 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 46, __pyx_L3_error)
+        __pyx_t_6 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 55, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         if (__pyx_t_5) {
           __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
         }
         __Pyx_INCREF(__pyx_v__img_arr);
         __Pyx_GIVEREF(__pyx_v__img_arr);
         PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_9, __pyx_v__img_arr);
         __Pyx_INCREF(__pyx_int_neg_1);
         __Pyx_GIVEREF(__pyx_int_neg_1);
         PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_9, __pyx_int_neg_1);
-        __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 46, __pyx_L3_error)
+        __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 55, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_image = __pyx_t_8;
       __pyx_t_8 = 0;
 
-      /* "viso_sdk/redis/redis_wrapper.py":50
+      /* "viso_sdk/redis/redis_wrapper.py":59
  *             )
  *             # self._img_arr = None
  *             return image             # <<<<<<<<<<<<<<
  *         except Exception as err:
  *             logger.warning(f"Failed to convert base64 to image - {err}")
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_image);
       __pyx_r = __pyx_v_image;
       goto __pyx_L7_try_return;
 
-      /* "viso_sdk/redis/redis_wrapper.py":43
+      /* "viso_sdk/redis/redis_wrapper.py":52
  *     def base64_to_img(b64_bytes: bytes) -> Union[None, np.ndarray]:
  *         """Convert base64 string to opencv frame"""
  *         try:             # <<<<<<<<<<<<<<
  *             str_frame = base64.b64decode(b64_bytes)
  *             _img_arr = np.frombuffer(str_frame, dtype=np.uint8)
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":51
+    /* "viso_sdk/redis/redis_wrapper.py":60
  *             # self._img_arr = None
  *             return image
  *         except Exception as err:             # <<<<<<<<<<<<<<
  *             logger.warning(f"Failed to convert base64 to image - {err}")
  *         return None
  */
     __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_9) {
       __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.base64_to_img", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_4, &__pyx_t_6) < 0) __PYX_ERR(0, 51, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_4, &__pyx_t_6) < 0) __PYX_ERR(0, 60, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_v_err = __pyx_t_4;
       /*try:*/ {
 
-        /* "viso_sdk/redis/redis_wrapper.py":52
+        /* "viso_sdk/redis/redis_wrapper.py":61
  *             return image
  *         except Exception as err:
  *             logger.warning(f"Failed to convert base64 to image - {err}")             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logger); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 52, __pyx_L14_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logger); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 61, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_warning); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 52, __pyx_L14_error)
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_warning); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 61, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_err, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 52, __pyx_L14_error)
+        __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_err, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 61, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Failed_to_convert_base64_to_imag, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 52, __pyx_L14_error)
+        __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Failed_to_convert_base64_to_imag, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 61, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_10);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
@@ -2252,21 +2607,21 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_10, function);
           }
         }
         __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_7, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_11);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L14_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 61, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
 
-      /* "viso_sdk/redis/redis_wrapper.py":51
+      /* "viso_sdk/redis/redis_wrapper.py":60
  *             # self._img_arr = None
  *             return image
  *         except Exception as err:             # <<<<<<<<<<<<<<
  *             logger.warning(f"Failed to convert base64 to image - {err}")
  *         return None
  */
       /*finally:*/ {
@@ -2317,15 +2672,15 @@
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L4_exception_handled;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "viso_sdk/redis/redis_wrapper.py":43
+    /* "viso_sdk/redis/redis_wrapper.py":52
  *     def base64_to_img(b64_bytes: bytes) -> Union[None, np.ndarray]:
  *         """Convert base64 string to opencv frame"""
  *         try:             # <<<<<<<<<<<<<<
  *             str_frame = base64.b64decode(b64_bytes)
  *             _img_arr = np.frombuffer(str_frame, dtype=np.uint8)
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -2342,26 +2697,26 @@
     __pyx_L4_exception_handled:;
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
   }
 
-  /* "viso_sdk/redis/redis_wrapper.py":53
+  /* "viso_sdk/redis/redis_wrapper.py":62
  *         except Exception as err:
  *             logger.warning(f"Failed to convert base64 to image - {err}")
  *         return None             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":41
+  /* "viso_sdk/redis/redis_wrapper.py":50
  * 
  *     @staticmethod
  *     def base64_to_img(b64_bytes: bytes) -> Union[None, np.ndarray]:             # <<<<<<<<<<<<<<
  *         """Convert base64 string to opencv frame"""
  *         try:
  */
 
@@ -2382,27 +2737,27 @@
   __Pyx_XDECREF(__pyx_v_image);
   __Pyx_XDECREF(__pyx_v_err);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/redis/redis_wrapper.py":56
+/* "viso_sdk/redis/redis_wrapper.py":65
  * 
  *     @staticmethod
  *     def img_to_base64str(image: np.ndarray, zoom_ratio: Optional[float] = 1.0) -> tuple:             # <<<<<<<<<<<<<<
  *         """Convert opencv frame to base64 encoded string"""
  *         if zoom_ratio != 1.0:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5img_to_base64str(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_4img_to_base64str[] = "Convert opencv frame to base64 encoded string";
-static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5img_to_base64str = {"img_to_base64str", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5img_to_base64str, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_4img_to_base64str};
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5img_to_base64str(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9img_to_base64str(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8img_to_base64str[] = "Convert opencv frame to base64 encoded string";
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9img_to_base64str = {"img_to_base64str", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9img_to_base64str, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8img_to_base64str};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9img_to_base64str(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_image = 0;
   PyObject *__pyx_v_zoom_ratio = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2431,15 +2786,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_zoom_ratio);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "img_to_base64str") < 0)) __PYX_ERR(0, 56, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "img_to_base64str") < 0)) __PYX_ERR(0, 65, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -2447,28 +2802,28 @@
       }
     }
     __pyx_v_image = values[0];
     __pyx_v_zoom_ratio = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("img_to_base64str", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 56, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("img_to_base64str", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 65, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.img_to_base64str", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_4img_to_base64str(__pyx_self, __pyx_v_image, __pyx_v_zoom_ratio);
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8img_to_base64str(__pyx_self, __pyx_v_image, __pyx_v_zoom_ratio);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_4img_to_base64str(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_image, PyObject *__pyx_v_zoom_ratio) {
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8img_to_base64str(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_image, PyObject *__pyx_v_zoom_ratio) {
   PyObject *__pyx_v_ret = NULL;
   PyObject *__pyx_v_jpg = NULL;
   PyObject *__pyx_v_jpg_as_text = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -2479,94 +2834,94 @@
   PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("img_to_base64str", 0);
   __Pyx_INCREF(__pyx_v_image);
 
-  /* "viso_sdk/redis/redis_wrapper.py":58
+  /* "viso_sdk/redis/redis_wrapper.py":67
  *     def img_to_base64str(image: np.ndarray, zoom_ratio: Optional[float] = 1.0) -> tuple:
  *         """Convert opencv frame to base64 encoded string"""
  *         if zoom_ratio != 1.0:             # <<<<<<<<<<<<<<
  *             image = cv2.resize(  # pylint: disable=no-member
  *                 image, None, fx=zoom_ratio, fy=zoom_ratio
  */
-  __pyx_t_1 = __Pyx_PyFloat_NeObjC(__pyx_v_zoom_ratio, __pyx_float_1_0, 1.0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyFloat_NeObjC(__pyx_v_zoom_ratio, __pyx_float_1_0, 1.0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "viso_sdk/redis/redis_wrapper.py":59
+    /* "viso_sdk/redis/redis_wrapper.py":68
  *         """Convert opencv frame to base64 encoded string"""
  *         if zoom_ratio != 1.0:
  *             image = cv2.resize(  # pylint: disable=no-member             # <<<<<<<<<<<<<<
  *                 image, None, fx=zoom_ratio, fy=zoom_ratio
  *             )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_cv2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_cv2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_resize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_resize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":60
+    /* "viso_sdk/redis/redis_wrapper.py":69
  *         if zoom_ratio != 1.0:
  *             image = cv2.resize(  # pylint: disable=no-member
  *                 image, None, fx=zoom_ratio, fy=zoom_ratio             # <<<<<<<<<<<<<<
  *             )
  *         ret, jpg = cv2.imencode(".jpg", image)  # pylint: disable=no-member
  */
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_image);
     __Pyx_GIVEREF(__pyx_v_image);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_image);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     PyTuple_SET_ITEM(__pyx_t_1, 1, Py_None);
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_fx, __pyx_v_zoom_ratio) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_fy, __pyx_v_zoom_ratio) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_fx, __pyx_v_zoom_ratio) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_fy, __pyx_v_zoom_ratio) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
 
-    /* "viso_sdk/redis/redis_wrapper.py":59
+    /* "viso_sdk/redis/redis_wrapper.py":68
  *         """Convert opencv frame to base64 encoded string"""
  *         if zoom_ratio != 1.0:
  *             image = cv2.resize(  # pylint: disable=no-member             # <<<<<<<<<<<<<<
  *                 image, None, fx=zoom_ratio, fy=zoom_ratio
  *             )
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_image, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":58
+    /* "viso_sdk/redis/redis_wrapper.py":67
  *     def img_to_base64str(image: np.ndarray, zoom_ratio: Optional[float] = 1.0) -> tuple:
  *         """Convert opencv frame to base64 encoded string"""
  *         if zoom_ratio != 1.0:             # <<<<<<<<<<<<<<
  *             image = cv2.resize(  # pylint: disable=no-member
  *                 image, None, fx=zoom_ratio, fy=zoom_ratio
  */
   }
 
-  /* "viso_sdk/redis/redis_wrapper.py":62
+  /* "viso_sdk/redis/redis_wrapper.py":71
  *                 image, None, fx=zoom_ratio, fy=zoom_ratio
  *             )
  *         ret, jpg = cv2.imencode(".jpg", image)  # pylint: disable=no-member             # <<<<<<<<<<<<<<
  *         jpg_as_text = base64.b64encode(jpg)
  *         return ret, jpg_as_text
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_cv2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_cv2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_imencode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_imencode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
@@ -2576,146 +2931,146 @@
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_kp_u_jpg, __pyx_v_image};
-    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_5);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_kp_u_jpg, __pyx_v_image};
-    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_5);
   } else
   #endif
   {
-    __pyx_t_3 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_kp_u_jpg);
     __Pyx_GIVEREF(__pyx_kp_u_jpg);
     PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_6, __pyx_kp_u_jpg);
     __Pyx_INCREF(__pyx_v_image);
     __Pyx_GIVEREF(__pyx_v_image);
     PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_6, __pyx_v_image);
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
     PyObject* sequence = __pyx_t_5;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 62, __pyx_L1_error)
+      __PYX_ERR(0, 71, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_4 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_4 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_7 = Py_TYPE(__pyx_t_4)->tp_iternext;
     index = 0; __pyx_t_1 = __pyx_t_7(__pyx_t_4); if (unlikely(!__pyx_t_1)) goto __pyx_L4_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_1);
     index = 1; __pyx_t_3 = __pyx_t_7(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L4_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_4), 2) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_4), 2) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
     __pyx_t_7 = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L5_unpacking_done;
     __pyx_L4_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_7 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 62, __pyx_L1_error)
+    __PYX_ERR(0, 71, __pyx_L1_error)
     __pyx_L5_unpacking_done:;
   }
   __pyx_v_ret = __pyx_t_1;
   __pyx_t_1 = 0;
   __pyx_v_jpg = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":63
+  /* "viso_sdk/redis/redis_wrapper.py":72
  *             )
  *         ret, jpg = cv2.imencode(".jpg", image)  # pylint: disable=no-member
  *         jpg_as_text = base64.b64encode(jpg)             # <<<<<<<<<<<<<<
  *         return ret, jpg_as_text
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_jpg) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_jpg);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_jpg_as_text = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":64
+  /* "viso_sdk/redis/redis_wrapper.py":73
  *         ret, jpg = cv2.imencode(".jpg", image)  # pylint: disable=no-member
  *         jpg_as_text = base64.b64encode(jpg)
  *         return ret, jpg_as_text             # <<<<<<<<<<<<<<
  * 
  *     def write_frame(
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_ret);
   __Pyx_GIVEREF(__pyx_v_ret);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_ret);
   __Pyx_INCREF(__pyx_v_jpg_as_text);
   __Pyx_GIVEREF(__pyx_v_jpg_as_text);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_jpg_as_text);
   __pyx_r = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":56
+  /* "viso_sdk/redis/redis_wrapper.py":65
  * 
  *     @staticmethod
  *     def img_to_base64str(image: np.ndarray, zoom_ratio: Optional[float] = 1.0) -> tuple:             # <<<<<<<<<<<<<<
  *         """Convert opencv frame to base64 encoded string"""
  *         if zoom_ratio != 1.0:
  */
 
@@ -2733,27 +3088,27 @@
   __Pyx_XDECREF(__pyx_v_jpg_as_text);
   __Pyx_XDECREF(__pyx_v_image);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/redis/redis_wrapper.py":66
+/* "viso_sdk/redis/redis_wrapper.py":75
  *         return ret, jpg_as_text
  * 
  *     def write_frame(             # <<<<<<<<<<<<<<
  *             self, frame: np.ndarray, redis_key: str, zoom: Optional[float] = 1.0
  *     ) -> bool:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7write_frame(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6write_frame[] = "Write video frame to the target redis key\n\n        Args:\n                frame(np.ndarray): numpy frame to be written.\n                redis_key(str): Target redis key.\n                zoom(float): Zoom ratio(optional).\n        ";
-static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7write_frame = {"write_frame", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7write_frame, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6write_frame};
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7write_frame(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11write_frame(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10write_frame[] = "Write video frame to the target redis key\n\n        Args:\n                frame(np.ndarray): numpy frame to be written.\n                redis_key(str): Target redis key.\n                zoom(float): Zoom ratio(optional).\n        ";
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11write_frame = {"write_frame", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11write_frame, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10write_frame};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11write_frame(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_frame = 0;
   PyObject *__pyx_v_redis_key = 0;
   PyObject *__pyx_v_zoom = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -2784,31 +3139,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("write_frame", 0, 3, 4, 1); __PYX_ERR(0, 66, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("write_frame", 0, 3, 4, 1); __PYX_ERR(0, 75, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_redis_key)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("write_frame", 0, 3, 4, 2); __PYX_ERR(0, 66, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("write_frame", 0, 3, 4, 2); __PYX_ERR(0, 75, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_zoom);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "write_frame") < 0)) __PYX_ERR(0, 66, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "write_frame") < 0)) __PYX_ERR(0, 75, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -2820,168 +3175,168 @@
     __pyx_v_self = values[0];
     __pyx_v_frame = values[1];
     __pyx_v_redis_key = ((PyObject*)values[2]);
     __pyx_v_zoom = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("write_frame", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 66, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("write_frame", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 75, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.write_frame", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 67, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6write_frame(__pyx_self, __pyx_v_self, __pyx_v_frame, __pyx_v_redis_key, __pyx_v_zoom);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10write_frame(__pyx_self, __pyx_v_self, __pyx_v_frame, __pyx_v_redis_key, __pyx_v_zoom);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_6write_frame(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_zoom) {
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10write_frame(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_zoom) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("write_frame", 0);
 
-  /* "viso_sdk/redis/redis_wrapper.py":76
+  /* "viso_sdk/redis/redis_wrapper.py":85
  *                 zoom(float): Zoom ratio(optional).
  *         """
  *         if self._use_thread:             # <<<<<<<<<<<<<<
  *             threading.Thread(
  *                 target=self._write_to_redis, args=(frame, redis_key, zoom)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_use_thread); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_use_thread); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "viso_sdk/redis/redis_wrapper.py":77
+    /* "viso_sdk/redis/redis_wrapper.py":86
  *         """
  *         if self._use_thread:
  *             threading.Thread(             # <<<<<<<<<<<<<<
  *                 target=self._write_to_redis, args=(frame, redis_key, zoom)
  *             ).start()
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_threading); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_threading); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Thread); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Thread); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":78
+    /* "viso_sdk/redis/redis_wrapper.py":87
  *         if self._use_thread:
  *             threading.Thread(
  *                 target=self._write_to_redis, args=(frame, redis_key, zoom)             # <<<<<<<<<<<<<<
  *             ).start()
  *             return True
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_write_to_redis); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_write_to_redis); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_target, __pyx_t_5) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_target, __pyx_t_5) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_frame);
     __Pyx_GIVEREF(__pyx_v_frame);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_frame);
     __Pyx_INCREF(__pyx_v_redis_key);
     __Pyx_GIVEREF(__pyx_v_redis_key);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_redis_key);
     __Pyx_INCREF(__pyx_v_zoom);
     __Pyx_GIVEREF(__pyx_v_zoom);
     PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_zoom);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_args, __pyx_t_5) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_args, __pyx_t_5) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":77
+    /* "viso_sdk/redis/redis_wrapper.py":86
  *         """
  *         if self._use_thread:
  *             threading.Thread(             # <<<<<<<<<<<<<<
  *                 target=self._write_to_redis, args=(frame, redis_key, zoom)
  *             ).start()
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":79
+    /* "viso_sdk/redis/redis_wrapper.py":88
  *             threading.Thread(
  *                 target=self._write_to_redis, args=(frame, redis_key, zoom)
  *             ).start()             # <<<<<<<<<<<<<<
  *             return True
  *         return self._write_to_redis(frame, redis_key, zoom)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":80
+    /* "viso_sdk/redis/redis_wrapper.py":89
  *                 target=self._write_to_redis, args=(frame, redis_key, zoom)
  *             ).start()
  *             return True             # <<<<<<<<<<<<<<
  *         return self._write_to_redis(frame, redis_key, zoom)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":76
+    /* "viso_sdk/redis/redis_wrapper.py":85
  *                 zoom(float): Zoom ratio(optional).
  *         """
  *         if self._use_thread:             # <<<<<<<<<<<<<<
  *             threading.Thread(
  *                 target=self._write_to_redis, args=(frame, redis_key, zoom)
  */
   }
 
-  /* "viso_sdk/redis/redis_wrapper.py":81
+  /* "viso_sdk/redis/redis_wrapper.py":90
  *             ).start()
  *             return True
  *         return self._write_to_redis(frame, redis_key, zoom)             # <<<<<<<<<<<<<<
  * 
  *     def _write_to_redis(
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_write_to_redis); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_write_to_redis); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -2990,52 +3345,52 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_v_frame, __pyx_v_redis_key, __pyx_v_zoom};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_v_frame, __pyx_v_redis_key, __pyx_v_zoom};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_v_frame);
     __Pyx_GIVEREF(__pyx_v_frame);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_v_frame);
     __Pyx_INCREF(__pyx_v_redis_key);
     __Pyx_GIVEREF(__pyx_v_redis_key);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_v_redis_key);
     __Pyx_INCREF(__pyx_v_zoom);
     __Pyx_GIVEREF(__pyx_v_zoom);
     PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_6, __pyx_v_zoom);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":66
+  /* "viso_sdk/redis/redis_wrapper.py":75
  *         return ret, jpg_as_text
  * 
  *     def write_frame(             # <<<<<<<<<<<<<<
  *             self, frame: np.ndarray, redis_key: str, zoom: Optional[float] = 1.0
  *     ) -> bool:
  */
 
@@ -3049,27 +3404,27 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/redis/redis_wrapper.py":83
+/* "viso_sdk/redis/redis_wrapper.py":92
  *         return self._write_to_redis(frame, redis_key, zoom)
  * 
  *     def _write_to_redis(             # <<<<<<<<<<<<<<
  *             self,
  *             frame: Union[np.ndarray, None],
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9_write_to_redis(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8_write_to_redis[] = "Internal function that is executed in background thread";
-static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9_write_to_redis = {"_write_to_redis", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9_write_to_redis, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8_write_to_redis};
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9_write_to_redis(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13_write_to_redis(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12_write_to_redis[] = "Internal function that is executed in background thread";
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13_write_to_redis = {"_write_to_redis", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13_write_to_redis, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12_write_to_redis};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13_write_to_redis(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_frame = 0;
   PyObject *__pyx_v_redis_key = 0;
   PyObject *__pyx_v_zoom = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3100,31 +3455,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_write_to_redis", 0, 3, 4, 1); __PYX_ERR(0, 83, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_write_to_redis", 0, 3, 4, 1); __PYX_ERR(0, 92, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_redis_key)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_write_to_redis", 0, 3, 4, 2); __PYX_ERR(0, 83, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_write_to_redis", 0, 3, 4, 2); __PYX_ERR(0, 92, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_zoom);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_write_to_redis") < 0)) __PYX_ERR(0, 83, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_write_to_redis") < 0)) __PYX_ERR(0, 92, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -3136,33 +3491,33 @@
     __pyx_v_self = values[0];
     __pyx_v_frame = values[1];
     __pyx_v_redis_key = ((PyObject*)values[2]);
     __pyx_v_zoom = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_write_to_redis", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 83, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_write_to_redis", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 92, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper._write_to_redis", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 86, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8_write_to_redis(__pyx_self, __pyx_v_self, __pyx_v_frame, __pyx_v_redis_key, __pyx_v_zoom);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12_write_to_redis(__pyx_self, __pyx_v_self, __pyx_v_frame, __pyx_v_redis_key, __pyx_v_zoom);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_8_write_to_redis(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_zoom) {
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12_write_to_redis(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_frame, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_zoom) {
   PyObject *__pyx_v_ret = NULL;
   PyObject *__pyx_v_jpg_as_text = NULL;
   PyObject *__pyx_v_err = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
@@ -3187,33 +3542,33 @@
   PyObject *__pyx_t_21 = NULL;
   PyObject *__pyx_t_22 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_write_to_redis", 0);
 
-  /* "viso_sdk/redis/redis_wrapper.py":90
+  /* "viso_sdk/redis/redis_wrapper.py":99
  *     ) -> bool:
  *         """Internal function that is executed in background thread"""
  *         if frame is not None:             # <<<<<<<<<<<<<<
  *             ret, jpg_as_text = self.img_to_base64str(frame, zoom)
  *             if ret:
  */
   __pyx_t_1 = (__pyx_v_frame != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "viso_sdk/redis/redis_wrapper.py":91
+    /* "viso_sdk/redis/redis_wrapper.py":100
  *         """Internal function that is executed in background thread"""
  *         if frame is not None:
  *             ret, jpg_as_text = self.img_to_base64str(frame, zoom)             # <<<<<<<<<<<<<<
  *             if ret:
  *                 try:
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_img_to_base64str); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_img_to_base64str); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -3222,106 +3577,106 @@
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_frame, __pyx_v_zoom};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_frame, __pyx_v_zoom};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_INCREF(__pyx_v_frame);
       __Pyx_GIVEREF(__pyx_v_frame);
       PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_frame);
       __Pyx_INCREF(__pyx_v_zoom);
       __Pyx_GIVEREF(__pyx_v_zoom);
       PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_zoom);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 91, __pyx_L1_error)
+        __PYX_ERR(0, 100, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_7);
       #else
-      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_5 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_5 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_8 = Py_TYPE(__pyx_t_5)->tp_iternext;
       index = 0; __pyx_t_4 = __pyx_t_8(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L4_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
       index = 1; __pyx_t_7 = __pyx_t_8(__pyx_t_5); if (unlikely(!__pyx_t_7)) goto __pyx_L4_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_7);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_5), 2) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_5), 2) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
       __pyx_t_8 = NULL;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L5_unpacking_done;
       __pyx_L4_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_8 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 91, __pyx_L1_error)
+      __PYX_ERR(0, 100, __pyx_L1_error)
       __pyx_L5_unpacking_done:;
     }
     __pyx_v_ret = __pyx_t_4;
     __pyx_t_4 = 0;
     __pyx_v_jpg_as_text = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":92
+    /* "viso_sdk/redis/redis_wrapper.py":101
  *         if frame is not None:
  *             ret, jpg_as_text = self.img_to_base64str(frame, zoom)
  *             if ret:             # <<<<<<<<<<<<<<
  *                 try:
  *                     return bool(self._redis_client.set(redis_key, jpg_as_text))
  */
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_ret); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_ret); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
     if (__pyx_t_2) {
 
-      /* "viso_sdk/redis/redis_wrapper.py":93
+      /* "viso_sdk/redis/redis_wrapper.py":102
  *             ret, jpg_as_text = self.img_to_base64str(frame, zoom)
  *             if ret:
  *                 try:             # <<<<<<<<<<<<<<
  *                     return bool(self._redis_client.set(redis_key, jpg_as_text))
  *                 except Exception as err:
  */
       {
@@ -3329,25 +3684,25 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
         __Pyx_XGOTREF(__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_10);
         __Pyx_XGOTREF(__pyx_t_11);
         /*try:*/ {
 
-          /* "viso_sdk/redis/redis_wrapper.py":94
+          /* "viso_sdk/redis/redis_wrapper.py":103
  *             if ret:
  *                 try:
  *                     return bool(self._redis_client.set(redis_key, jpg_as_text))             # <<<<<<<<<<<<<<
  *                 except Exception as err:
  *                     logger.error(f"Failed to write frame to redis - {err}")
  */
           __Pyx_XDECREF(__pyx_r);
-          __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 94, __pyx_L7_error)
+          __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 103, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_7);
-          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_set); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L7_error)
+          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_set); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           __pyx_t_7 = NULL;
           __pyx_t_6 = 0;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
             __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
             if (likely(__pyx_t_7)) {
@@ -3357,99 +3712,99 @@
               __Pyx_DECREF_SET(__pyx_t_4, function);
               __pyx_t_6 = 1;
             }
           }
           #if CYTHON_FAST_PYCALL
           if (PyFunction_Check(__pyx_t_4)) {
             PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_redis_key, __pyx_v_jpg_as_text};
-            __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L7_error)
             __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
             __Pyx_GOTREF(__pyx_t_3);
           } else
           #endif
           #if CYTHON_FAST_PYCCALL
           if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
             PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_redis_key, __pyx_v_jpg_as_text};
-            __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L7_error)
             __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
             __Pyx_GOTREF(__pyx_t_3);
           } else
           #endif
           {
-            __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L7_error)
+            __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 103, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_5);
             if (__pyx_t_7) {
               __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7); __pyx_t_7 = NULL;
             }
             __Pyx_INCREF(__pyx_v_redis_key);
             __Pyx_GIVEREF(__pyx_v_redis_key);
             PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_v_redis_key);
             __Pyx_INCREF(__pyx_v_jpg_as_text);
             __Pyx_GIVEREF(__pyx_v_jpg_as_text);
             PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_v_jpg_as_text);
-            __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 94, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 103, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_3 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_r = __pyx_t_3;
           __pyx_t_3 = 0;
           goto __pyx_L11_try_return;
 
-          /* "viso_sdk/redis/redis_wrapper.py":93
+          /* "viso_sdk/redis/redis_wrapper.py":102
  *             ret, jpg_as_text = self.img_to_base64str(frame, zoom)
  *             if ret:
  *                 try:             # <<<<<<<<<<<<<<
  *                     return bool(self._redis_client.set(redis_key, jpg_as_text))
  *                 except Exception as err:
  */
         }
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "viso_sdk/redis/redis_wrapper.py":95
+        /* "viso_sdk/redis/redis_wrapper.py":104
  *                 try:
  *                     return bool(self._redis_client.set(redis_key, jpg_as_text))
  *                 except Exception as err:             # <<<<<<<<<<<<<<
  *                     logger.error(f"Failed to write frame to redis - {err}")
  *             logger.warning("Failed to convert stream to write to redis")
  */
         __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
         if (__pyx_t_6) {
           __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper._write_to_redis", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 95, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 104, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_4);
           __pyx_v_err = __pyx_t_4;
           /*try:*/ {
 
-            /* "viso_sdk/redis/redis_wrapper.py":96
+            /* "viso_sdk/redis/redis_wrapper.py":105
  *                     return bool(self._redis_client.set(redis_key, jpg_as_text))
  *                 except Exception as err:
  *                     logger.error(f"Failed to write frame to redis - {err}")             # <<<<<<<<<<<<<<
  *             logger.warning("Failed to convert stream to write to redis")
  *             return False
  */
-            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 96, __pyx_L18_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 105, __pyx_L18_error)
             __Pyx_GOTREF(__pyx_t_12);
-            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_error); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 96, __pyx_L18_error)
+            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_error); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 105, __pyx_L18_error)
             __Pyx_GOTREF(__pyx_t_13);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __pyx_t_12 = __Pyx_PyObject_FormatSimple(__pyx_v_err, __pyx_empty_unicode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 96, __pyx_L18_error)
+            __pyx_t_12 = __Pyx_PyObject_FormatSimple(__pyx_v_err, __pyx_empty_unicode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 105, __pyx_L18_error)
             __Pyx_GOTREF(__pyx_t_12);
-            __pyx_t_14 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Failed_to_write_frame_to_redis, __pyx_t_12); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 96, __pyx_L18_error)
+            __pyx_t_14 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Failed_to_write_frame_to_redis, __pyx_t_12); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 105, __pyx_L18_error)
             __Pyx_GOTREF(__pyx_t_14);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             __pyx_t_12 = NULL;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_13))) {
               __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
               if (likely(__pyx_t_12)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
@@ -3457,21 +3812,21 @@
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_13, function);
               }
             }
             __pyx_t_7 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_12, __pyx_t_14) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_t_14);
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-            if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L18_error)
+            if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 105, __pyx_L18_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           }
 
-          /* "viso_sdk/redis/redis_wrapper.py":95
+          /* "viso_sdk/redis/redis_wrapper.py":104
  *                 try:
  *                     return bool(self._redis_client.set(redis_key, jpg_as_text))
  *                 except Exception as err:             # <<<<<<<<<<<<<<
  *                     logger.error(f"Failed to write frame to redis - {err}")
  *             logger.warning("Failed to convert stream to write to redis")
  */
           /*finally:*/ {
@@ -3522,15 +3877,15 @@
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           goto __pyx_L8_exception_handled;
         }
         goto __pyx_L9_except_error;
         __pyx_L9_except_error:;
 
-        /* "viso_sdk/redis/redis_wrapper.py":93
+        /* "viso_sdk/redis/redis_wrapper.py":102
  *             ret, jpg_as_text = self.img_to_base64str(frame, zoom)
  *             if ret:
  *                 try:             # <<<<<<<<<<<<<<
  *                     return bool(self._redis_client.set(redis_key, jpg_as_text))
  *                 except Exception as err:
  */
         __Pyx_XGIVEREF(__pyx_t_9);
@@ -3547,110 +3902,110 @@
         __pyx_L8_exception_handled:;
         __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_XGIVEREF(__pyx_t_11);
         __Pyx_ExceptionReset(__pyx_t_9, __pyx_t_10, __pyx_t_11);
       }
 
-      /* "viso_sdk/redis/redis_wrapper.py":92
+      /* "viso_sdk/redis/redis_wrapper.py":101
  *         if frame is not None:
  *             ret, jpg_as_text = self.img_to_base64str(frame, zoom)
  *             if ret:             # <<<<<<<<<<<<<<
  *                 try:
  *                     return bool(self._redis_client.set(redis_key, jpg_as_text))
  */
     }
 
-    /* "viso_sdk/redis/redis_wrapper.py":97
+    /* "viso_sdk/redis/redis_wrapper.py":106
  *                 except Exception as err:
  *                     logger.error(f"Failed to write frame to redis - {err}")
  *             logger.warning("Failed to convert stream to write to redis")             # <<<<<<<<<<<<<<
  *             return False
  *         return bool(self._redis_client.delete(redis_key))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_Failed_to_convert_stream_to_writ) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_Failed_to_convert_stream_to_writ);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":98
+    /* "viso_sdk/redis/redis_wrapper.py":107
  *                     logger.error(f"Failed to write frame to redis - {err}")
  *             logger.warning("Failed to convert stream to write to redis")
  *             return False             # <<<<<<<<<<<<<<
  *         return bool(self._redis_client.delete(redis_key))
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":90
+    /* "viso_sdk/redis/redis_wrapper.py":99
  *     ) -> bool:
  *         """Internal function that is executed in background thread"""
  *         if frame is not None:             # <<<<<<<<<<<<<<
  *             ret, jpg_as_text = self.img_to_base64str(frame, zoom)
  *             if ret:
  */
   }
 
-  /* "viso_sdk/redis/redis_wrapper.py":99
+  /* "viso_sdk/redis/redis_wrapper.py":108
  *             logger.warning("Failed to convert stream to write to redis")
  *             return False
  *         return bool(self._redis_client.delete(redis_key))             # <<<<<<<<<<<<<<
  * 
  *     def delete_data(self, redis_key: str) -> bool:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_delete); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_delete); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_redis_key) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_redis_key);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":83
+  /* "viso_sdk/redis/redis_wrapper.py":92
  *         return self._write_to_redis(frame, redis_key, zoom)
  * 
  *     def _write_to_redis(             # <<<<<<<<<<<<<<
  *             self,
  *             frame: Union[np.ndarray, None],
  */
 
@@ -3670,27 +4025,27 @@
   __Pyx_XDECREF(__pyx_v_jpg_as_text);
   __Pyx_XDECREF(__pyx_v_err);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/redis/redis_wrapper.py":101
+/* "viso_sdk/redis/redis_wrapper.py":110
  *         return bool(self._redis_client.delete(redis_key))
  * 
  *     def delete_data(self, redis_key: str) -> bool:             # <<<<<<<<<<<<<<
  *         """Delete data from the target redis location
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11delete_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10delete_data[] = "Delete data from the target redis location\n\n        Args:\n            redis_key(str): Target redis key.\n        ";
-static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11delete_data = {"delete_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11delete_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10delete_data};
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11delete_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15delete_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14delete_data[] = "Delete data from the target redis location\n\n        Args:\n            redis_key(str): Target redis key.\n        ";
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15delete_data = {"delete_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15delete_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14delete_data};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15delete_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_redis_key = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3714,98 +4069,98 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_redis_key)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("delete_data", 1, 2, 2, 1); __PYX_ERR(0, 101, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("delete_data", 1, 2, 2, 1); __PYX_ERR(0, 110, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "delete_data") < 0)) __PYX_ERR(0, 101, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "delete_data") < 0)) __PYX_ERR(0, 110, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_redis_key = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("delete_data", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 101, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("delete_data", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 110, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.delete_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10delete_data(__pyx_self, __pyx_v_self, __pyx_v_redis_key);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14delete_data(__pyx_self, __pyx_v_self, __pyx_v_redis_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_10delete_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key) {
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14delete_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("delete_data", 0);
 
-  /* "viso_sdk/redis/redis_wrapper.py":107
+  /* "viso_sdk/redis/redis_wrapper.py":116
  *             redis_key(str): Target redis key.
  *         """
  *         return bool(self._redis_client.delete(redis_key))             # <<<<<<<<<<<<<<
  * 
  *     def put_data(self, redis_key: str, data: str) -> bool:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_delete); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_delete); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_redis_key) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_redis_key);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_4))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_4))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":101
+  /* "viso_sdk/redis/redis_wrapper.py":110
  *         return bool(self._redis_client.delete(redis_key))
  * 
  *     def delete_data(self, redis_key: str) -> bool:             # <<<<<<<<<<<<<<
  *         """Delete data from the target redis location
  * 
  */
 
@@ -3818,27 +4173,27 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/redis/redis_wrapper.py":109
+/* "viso_sdk/redis/redis_wrapper.py":118
  *         return bool(self._redis_client.delete(redis_key))
  * 
  *     def put_data(self, redis_key: str, data: str) -> bool:             # <<<<<<<<<<<<<<
  *         """Write data to the target redis location
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13put_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12put_data[] = "Write data to the target redis location\n\n        Args:\n            redis_key(str): Target redis key.\n            data(str): Data to be written.\n        ";
-static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13put_data = {"put_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13put_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12put_data};
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13put_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17put_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16put_data[] = "Write data to the target redis location\n\n        Args:\n            redis_key(str): Target redis key.\n            data(str): Data to be written.\n        ";
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17put_data = {"put_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17put_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16put_data};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17put_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_redis_key = 0;
   PyObject *__pyx_v_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -3865,83 +4220,83 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_redis_key)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("put_data", 1, 3, 3, 1); __PYX_ERR(0, 109, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("put_data", 1, 3, 3, 1); __PYX_ERR(0, 118, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("put_data", 1, 3, 3, 2); __PYX_ERR(0, 109, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("put_data", 1, 3, 3, 2); __PYX_ERR(0, 118, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "put_data") < 0)) __PYX_ERR(0, 109, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "put_data") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_redis_key = ((PyObject*)values[1]);
     __pyx_v_data = ((PyObject*)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("put_data", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 109, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("put_data", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.put_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 109, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyUnicode_Type), 1, "data", 1))) __PYX_ERR(0, 109, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12put_data(__pyx_self, __pyx_v_self, __pyx_v_redis_key, __pyx_v_data);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyUnicode_Type), 1, "data", 1))) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16put_data(__pyx_self, __pyx_v_self, __pyx_v_redis_key, __pyx_v_data);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_12put_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_data) {
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16put_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key, PyObject *__pyx_v_data) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("put_data", 0);
 
-  /* "viso_sdk/redis/redis_wrapper.py":116
+  /* "viso_sdk/redis/redis_wrapper.py":125
  *             data(str): Data to be written.
  *         """
  *         return bool(self._redis_client.set(redis_key, data))             # <<<<<<<<<<<<<<
  * 
  *     def read_data(self, redis_key: str) -> Any:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -3951,53 +4306,53 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_redis_key, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_redis_key, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_v_redis_key);
     __Pyx_GIVEREF(__pyx_v_redis_key);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_redis_key);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_data);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_6))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_6))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":109
+  /* "viso_sdk/redis/redis_wrapper.py":118
  *         return bool(self._redis_client.delete(redis_key))
  * 
  *     def put_data(self, redis_key: str, data: str) -> bool:             # <<<<<<<<<<<<<<
  *         """Write data to the target redis location
  * 
  */
 
@@ -4011,27 +4366,27 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/redis/redis_wrapper.py":118
+/* "viso_sdk/redis/redis_wrapper.py":127
  *         return bool(self._redis_client.set(redis_key, data))
  * 
  *     def read_data(self, redis_key: str) -> Any:             # <<<<<<<<<<<<<<
  *         """Read data from the target redis location
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15read_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14read_data[] = "Read data from the target redis location\n\n        Args:\n            redis_key(str): Target redis key.\n        ";
-static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15read_data = {"read_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15read_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14read_data};
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15read_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_19read_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_18read_data[] = "Read data from the target redis location\n\n        Args:\n            redis_key(str): Target redis key.\n        ";
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_19read_data = {"read_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_19read_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_18read_data};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_19read_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_redis_key = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4055,93 +4410,93 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_redis_key)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_data", 1, 2, 2, 1); __PYX_ERR(0, 118, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_data", 1, 2, 2, 1); __PYX_ERR(0, 127, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_data") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_data") < 0)) __PYX_ERR(0, 127, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_redis_key = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_data", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_data", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 127, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.read_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 118, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14read_data(__pyx_self, __pyx_v_self, __pyx_v_redis_key);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_18read_data(__pyx_self, __pyx_v_self, __pyx_v_redis_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_14read_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key) {
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_18read_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_data", 0);
 
-  /* "viso_sdk/redis/redis_wrapper.py":124
+  /* "viso_sdk/redis/redis_wrapper.py":133
  *             redis_key(str): Target redis key.
  *         """
  *         return self._redis_client.get(redis_key)             # <<<<<<<<<<<<<<
  * 
  *     def get_frame(self, redis_key: str) -> Union[np.ndarray, None]:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_redis_key) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_redis_key);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":118
+  /* "viso_sdk/redis/redis_wrapper.py":127
  *         return bool(self._redis_client.set(redis_key, data))
  * 
  *     def read_data(self, redis_key: str) -> Any:             # <<<<<<<<<<<<<<
  *         """Read data from the target redis location
  * 
  */
 
@@ -4154,27 +4509,27 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/redis/redis_wrapper.py":126
+/* "viso_sdk/redis/redis_wrapper.py":135
  *         return self._redis_client.get(redis_key)
  * 
  *     def get_frame(self, redis_key: str) -> Union[np.ndarray, None]:             # <<<<<<<<<<<<<<
  *         """Read video frame from a given redis key
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17get_frame(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16get_frame[] = "Read video frame from a given redis key\n\n        Args:\n            redis_key(str): Target redis key.\n        ";
-static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17get_frame = {"get_frame", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17get_frame, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16get_frame};
-static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17get_frame(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_21get_frame(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_20get_frame[] = "Read video frame from a given redis key\n\n        Args:\n            redis_key(str): Target redis key.\n        ";
+static PyMethodDef __pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_21get_frame = {"get_frame", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_21get_frame, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_20get_frame};
+static PyObject *__pyx_pw_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_21get_frame(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_redis_key = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4198,50 +4553,50 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_redis_key)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_frame", 1, 2, 2, 1); __PYX_ERR(0, 126, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_frame", 1, 2, 2, 1); __PYX_ERR(0, 135, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_frame") < 0)) __PYX_ERR(0, 126, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_frame") < 0)) __PYX_ERR(0, 135, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_redis_key = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_frame", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 126, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_frame", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 135, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.get_frame", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 126, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16get_frame(__pyx_self, __pyx_v_self, __pyx_v_redis_key);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_redis_key), (&PyUnicode_Type), 1, "redis_key", 1))) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_20get_frame(__pyx_self, __pyx_v_self, __pyx_v_redis_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_16get_frame(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key) {
+static PyObject *__pyx_pf_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_20get_frame(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_redis_key) {
   PyObject *__pyx_v_b64_bytes = NULL;
   PyObject *__pyx_v_err = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -4267,15 +4622,15 @@
   PyObject *__pyx_t_23 = NULL;
   PyObject *__pyx_t_24 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_frame", 0);
 
-  /* "viso_sdk/redis/redis_wrapper.py":132
+  /* "viso_sdk/redis/redis_wrapper.py":141
  *             redis_key(str): Target redis key.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             b64_bytes = self._redis_client.get(redis_key)
  *             if b64_bytes and isinstance(b64_bytes, bytes):
  */
   {
@@ -4283,102 +4638,102 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "viso_sdk/redis/redis_wrapper.py":133
+      /* "viso_sdk/redis/redis_wrapper.py":142
  *         """
  *         try:
  *             b64_bytes = self._redis_client.get(redis_key)             # <<<<<<<<<<<<<<
  *             if b64_bytes and isinstance(b64_bytes, bytes):
  *                 return self.base64_to_img(b64_bytes)
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 133, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_redis_client); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 142, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 133, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 142, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
         }
       }
       __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_redis_key) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_redis_key);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L3_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_v_b64_bytes = __pyx_t_4;
       __pyx_t_4 = 0;
 
-      /* "viso_sdk/redis/redis_wrapper.py":134
+      /* "viso_sdk/redis/redis_wrapper.py":143
  *         try:
  *             b64_bytes = self._redis_client.get(redis_key)
  *             if b64_bytes and isinstance(b64_bytes, bytes):             # <<<<<<<<<<<<<<
  *                 return self.base64_to_img(b64_bytes)
  *         except Exception as err:
  */
-      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_b64_bytes); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
+      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_b64_bytes); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 143, __pyx_L3_error)
       if (__pyx_t_8) {
       } else {
         __pyx_t_7 = __pyx_t_8;
         goto __pyx_L10_bool_binop_done;
       }
       __pyx_t_8 = PyBytes_Check(__pyx_v_b64_bytes); 
       __pyx_t_9 = (__pyx_t_8 != 0);
       __pyx_t_7 = __pyx_t_9;
       __pyx_L10_bool_binop_done:;
       if (__pyx_t_7) {
 
-        /* "viso_sdk/redis/redis_wrapper.py":135
+        /* "viso_sdk/redis/redis_wrapper.py":144
  *             b64_bytes = self._redis_client.get(redis_key)
  *             if b64_bytes and isinstance(b64_bytes, bytes):
  *                 return self.base64_to_img(b64_bytes)             # <<<<<<<<<<<<<<
  *         except Exception as err:
  *             logger.warning(f"Failed to get redis frame from {redis_key} - {err}")
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_base64_to_img); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 135, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_base64_to_img); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 144, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
             __Pyx_INCREF(__pyx_t_5);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_6, function);
           }
         }
         __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_b64_bytes) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_b64_bytes);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L3_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 144, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_r = __pyx_t_4;
         __pyx_t_4 = 0;
         goto __pyx_L7_try_return;
 
-        /* "viso_sdk/redis/redis_wrapper.py":134
+        /* "viso_sdk/redis/redis_wrapper.py":143
  *         try:
  *             b64_bytes = self._redis_client.get(redis_key)
  *             if b64_bytes and isinstance(b64_bytes, bytes):             # <<<<<<<<<<<<<<
  *                 return self.base64_to_img(b64_bytes)
  *         except Exception as err:
  */
       }
 
-      /* "viso_sdk/redis/redis_wrapper.py":132
+      /* "viso_sdk/redis/redis_wrapper.py":141
  *             redis_key(str): Target redis key.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             b64_bytes = self._redis_client.get(redis_key)
  *             if b64_bytes and isinstance(b64_bytes, bytes):
  */
     }
@@ -4387,70 +4742,70 @@
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "viso_sdk/redis/redis_wrapper.py":136
+    /* "viso_sdk/redis/redis_wrapper.py":145
  *             if b64_bytes and isinstance(b64_bytes, bytes):
  *                 return self.base64_to_img(b64_bytes)
  *         except Exception as err:             # <<<<<<<<<<<<<<
  *             logger.warning(f"Failed to get redis frame from {redis_key} - {err}")
  *         return None
  */
     __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_10) {
       __Pyx_AddTraceback("viso_sdk.redis.redis_wrapper.RedisWrapper.get_frame", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_5) < 0) __PYX_ERR(0, 136, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_5) < 0) __PYX_ERR(0, 145, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_err = __pyx_t_6;
       /*try:*/ {
 
-        /* "viso_sdk/redis/redis_wrapper.py":137
+        /* "viso_sdk/redis/redis_wrapper.py":146
  *                 return self.base64_to_img(b64_bytes)
  *         except Exception as err:
  *             logger.warning(f"Failed to get redis frame from {redis_key} - {err}")             # <<<<<<<<<<<<<<
  *         return None
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 137, __pyx_L17_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_logger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 146, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_warning); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 137, __pyx_L17_error)
+        __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_warning); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 146, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __pyx_t_12 = PyTuple_New(4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 137, __pyx_L17_error)
+        __pyx_t_12 = PyTuple_New(4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 146, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_12);
         __pyx_t_14 = 0;
         __pyx_t_15 = 127;
         __Pyx_INCREF(__pyx_kp_u_Failed_to_get_redis_frame_from);
         __pyx_t_14 += 31;
         __Pyx_GIVEREF(__pyx_kp_u_Failed_to_get_redis_frame_from);
         PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_kp_u_Failed_to_get_redis_frame_from);
-        __pyx_t_16 = __Pyx_PyUnicode_Unicode(__pyx_v_redis_key); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 137, __pyx_L17_error)
+        __pyx_t_16 = __Pyx_PyUnicode_Unicode(__pyx_v_redis_key); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 146, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_16);
         __pyx_t_15 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_16) > __pyx_t_15) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_16) : __pyx_t_15;
         __pyx_t_14 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_16);
         __Pyx_GIVEREF(__pyx_t_16);
         PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_16);
         __pyx_t_16 = 0;
-        __Pyx_INCREF(__pyx_kp_u_);
+        __Pyx_INCREF(__pyx_kp_u__2);
         __pyx_t_14 += 3;
-        __Pyx_GIVEREF(__pyx_kp_u_);
-        PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_kp_u_);
-        __pyx_t_16 = __Pyx_PyObject_FormatSimple(__pyx_v_err, __pyx_empty_unicode); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 137, __pyx_L17_error)
+        __Pyx_GIVEREF(__pyx_kp_u__2);
+        PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_kp_u__2);
+        __pyx_t_16 = __Pyx_PyObject_FormatSimple(__pyx_v_err, __pyx_empty_unicode); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 146, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_16);
         __pyx_t_15 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_16) > __pyx_t_15) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_16) : __pyx_t_15;
         __pyx_t_14 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_16);
         __Pyx_GIVEREF(__pyx_t_16);
         PyTuple_SET_ITEM(__pyx_t_12, 3, __pyx_t_16);
         __pyx_t_16 = 0;
-        __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_12, 4, __pyx_t_14, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 137, __pyx_L17_error)
+        __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_12, 4, __pyx_t_14, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 146, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_13))) {
           __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
           if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
@@ -4458,21 +4813,21 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_13, function);
           }
         }
         __pyx_t_11 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_12, __pyx_t_16) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_t_16);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 137, __pyx_L17_error)
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 146, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       }
 
-      /* "viso_sdk/redis/redis_wrapper.py":136
+      /* "viso_sdk/redis/redis_wrapper.py":145
  *             if b64_bytes and isinstance(b64_bytes, bytes):
  *                 return self.base64_to_img(b64_bytes)
  *         except Exception as err:             # <<<<<<<<<<<<<<
  *             logger.warning(f"Failed to get redis frame from {redis_key} - {err}")
  *         return None
  */
       /*finally:*/ {
@@ -4523,15 +4878,15 @@
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L4_exception_handled;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "viso_sdk/redis/redis_wrapper.py":132
+    /* "viso_sdk/redis/redis_wrapper.py":141
  *             redis_key(str): Target redis key.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             b64_bytes = self._redis_client.get(redis_key)
  *             if b64_bytes and isinstance(b64_bytes, bytes):
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -4549,24 +4904,24 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     __pyx_L8_try_end:;
   }
 
-  /* "viso_sdk/redis/redis_wrapper.py":138
+  /* "viso_sdk/redis/redis_wrapper.py":147
  *         except Exception as err:
  *             logger.warning(f"Failed to get redis frame from {redis_key} - {err}")
  *         return None             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":126
+  /* "viso_sdk/redis/redis_wrapper.py":135
  *         return self._redis_client.get(redis_key)
  * 
  *     def get_frame(self, redis_key: str) -> Union[np.ndarray, None]:             # <<<<<<<<<<<<<<
  *         """Read video frame from a given redis key
  * 
  */
 
@@ -4631,37 +4986,44 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
+  {&__pyx_n_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 1},
   {&__pyx_n_s_Any, __pyx_k_Any, sizeof(__pyx_k_Any), 0, 0, 1, 1},
   {&__pyx_kp_u_Failed_to_convert_base64_to_imag, __pyx_k_Failed_to_convert_base64_to_imag, sizeof(__pyx_k_Failed_to_convert_base64_to_imag), 0, 1, 0, 0},
   {&__pyx_kp_u_Failed_to_convert_stream_to_writ, __pyx_k_Failed_to_convert_stream_to_writ, sizeof(__pyx_k_Failed_to_convert_stream_to_writ), 0, 1, 0, 0},
   {&__pyx_kp_u_Failed_to_get_redis_frame_from, __pyx_k_Failed_to_get_redis_frame_from, sizeof(__pyx_k_Failed_to_get_redis_frame_from), 0, 1, 0, 0},
   {&__pyx_kp_u_Failed_to_write_frame_to_redis, __pyx_k_Failed_to_write_frame_to_redis, sizeof(__pyx_k_Failed_to_write_frame_to_redis), 0, 1, 0, 0},
+  {&__pyx_n_s_LOCAL, __pyx_k_LOCAL, sizeof(__pyx_k_LOCAL), 0, 0, 1, 1},
   {&__pyx_kp_u_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 1, 0, 0},
   {&__pyx_n_s_Optional, __pyx_k_Optional, sizeof(__pyx_k_Optional), 0, 0, 1, 1},
+  {&__pyx_n_s_PREFIX, __pyx_k_PREFIX, sizeof(__pyx_k_PREFIX), 0, 0, 1, 1},
+  {&__pyx_n_s_REDIS, __pyx_k_REDIS, sizeof(__pyx_k_REDIS), 0, 0, 1, 1},
   {&__pyx_n_u_REDIS, __pyx_k_REDIS, sizeof(__pyx_k_REDIS), 0, 1, 0, 1},
   {&__pyx_n_s_RedisWrapper, __pyx_k_RedisWrapper, sizeof(__pyx_k_RedisWrapper), 0, 0, 1, 1},
   {&__pyx_n_s_RedisWrapper___init, __pyx_k_RedisWrapper___init, sizeof(__pyx_k_RedisWrapper___init), 0, 0, 1, 1},
   {&__pyx_n_s_RedisWrapper__write_to_redis, __pyx_k_RedisWrapper__write_to_redis, sizeof(__pyx_k_RedisWrapper__write_to_redis), 0, 0, 1, 1},
   {&__pyx_n_s_RedisWrapper_base64_to_img, __pyx_k_RedisWrapper_base64_to_img, sizeof(__pyx_k_RedisWrapper_base64_to_img), 0, 0, 1, 1},
   {&__pyx_n_s_RedisWrapper_delete_data, __pyx_k_RedisWrapper_delete_data, sizeof(__pyx_k_RedisWrapper_delete_data), 0, 0, 1, 1},
+  {&__pyx_n_s_RedisWrapper_gen_redis_key_local, __pyx_k_RedisWrapper_gen_redis_key_local, sizeof(__pyx_k_RedisWrapper_gen_redis_key_local), 0, 0, 1, 1},
+  {&__pyx_n_s_RedisWrapper_gen_redis_key_statu, __pyx_k_RedisWrapper_gen_redis_key_statu, sizeof(__pyx_k_RedisWrapper_gen_redis_key_statu), 0, 0, 1, 1},
   {&__pyx_n_s_RedisWrapper_get_frame, __pyx_k_RedisWrapper_get_frame, sizeof(__pyx_k_RedisWrapper_get_frame), 0, 0, 1, 1},
   {&__pyx_n_s_RedisWrapper_img_to_base64str, __pyx_k_RedisWrapper_img_to_base64str, sizeof(__pyx_k_RedisWrapper_img_to_base64str), 0, 0, 1, 1},
   {&__pyx_n_s_RedisWrapper_put_data, __pyx_k_RedisWrapper_put_data, sizeof(__pyx_k_RedisWrapper_put_data), 0, 0, 1, 1},
   {&__pyx_n_s_RedisWrapper_read_data, __pyx_k_RedisWrapper_read_data, sizeof(__pyx_k_RedisWrapper_read_data), 0, 0, 1, 1},
   {&__pyx_n_s_RedisWrapper_write_frame, __pyx_k_RedisWrapper_write_frame, sizeof(__pyx_k_RedisWrapper_write_frame), 0, 0, 1, 1},
   {&__pyx_kp_s_Represents_a_redis_client_specif, __pyx_k_Represents_a_redis_client_specif, sizeof(__pyx_k_Represents_a_redis_client_specif), 0, 0, 1, 0},
+  {&__pyx_n_s_STATUS, __pyx_k_STATUS, sizeof(__pyx_k_STATUS), 0, 0, 1, 1},
   {&__pyx_n_s_StrictRedis, __pyx_k_StrictRedis, sizeof(__pyx_k_StrictRedis), 0, 0, 1, 1},
   {&__pyx_n_s_Thread, __pyx_k_Thread, sizeof(__pyx_k_Thread), 0, 0, 1, 1},
   {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
+  {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_b64_bytes, __pyx_k_b64_bytes, sizeof(__pyx_k_b64_bytes), 0, 0, 1, 1},
   {&__pyx_n_s_b64decode, __pyx_k_b64decode, sizeof(__pyx_k_b64decode), 0, 0, 1, 1},
   {&__pyx_n_s_b64encode, __pyx_k_b64encode, sizeof(__pyx_k_b64encode), 0, 0, 1, 1},
   {&__pyx_n_s_base64, __pyx_k_base64, sizeof(__pyx_k_base64), 0, 0, 1, 1},
   {&__pyx_n_s_base64_to_img, __pyx_k_base64_to_img, sizeof(__pyx_k_base64_to_img), 0, 0, 1, 1},
   {&__pyx_n_u_bytes, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 1, 0, 1},
@@ -4674,14 +5036,16 @@
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_err, __pyx_k_err, sizeof(__pyx_k_err), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_frame, __pyx_k_frame, sizeof(__pyx_k_frame), 0, 0, 1, 1},
   {&__pyx_n_s_frombuffer, __pyx_k_frombuffer, sizeof(__pyx_k_frombuffer), 0, 0, 1, 1},
   {&__pyx_n_s_fx, __pyx_k_fx, sizeof(__pyx_k_fx), 0, 0, 1, 1},
   {&__pyx_n_s_fy, __pyx_k_fy, sizeof(__pyx_k_fy), 0, 0, 1, 1},
+  {&__pyx_n_s_gen_redis_key_local, __pyx_k_gen_redis_key_local, sizeof(__pyx_k_gen_redis_key_local), 0, 0, 1, 1},
+  {&__pyx_n_s_gen_redis_key_status, __pyx_k_gen_redis_key_status, sizeof(__pyx_k_gen_redis_key_status), 0, 0, 1, 1},
   {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
   {&__pyx_n_s_get_frame, __pyx_k_get_frame, sizeof(__pyx_k_get_frame), 0, 0, 1, 1},
   {&__pyx_n_s_get_logger, __pyx_k_get_logger, sizeof(__pyx_k_get_logger), 0, 0, 1, 1},
   {&__pyx_n_s_host, __pyx_k_host, sizeof(__pyx_k_host), 0, 0, 1, 1},
   {&__pyx_n_s_image, __pyx_k_image, sizeof(__pyx_k_image), 0, 0, 1, 1},
   {&__pyx_n_s_imdecode, __pyx_k_imdecode, sizeof(__pyx_k_imdecode), 0, 0, 1, 1},
   {&__pyx_n_s_imencode, __pyx_k_imencode, sizeof(__pyx_k_imencode), 0, 0, 1, 1},
@@ -4696,14 +5060,15 @@
   {&__pyx_n_u_localhost, __pyx_k_localhost, sizeof(__pyx_k_localhost), 0, 1, 0, 1},
   {&__pyx_n_s_logger, __pyx_k_logger, sizeof(__pyx_k_logger), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_ndarray, __pyx_k_ndarray, sizeof(__pyx_k_ndarray), 0, 0, 1, 1},
+  {&__pyx_n_s_node_id, __pyx_k_node_id, sizeof(__pyx_k_node_id), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_n_s_port, __pyx_k_port, sizeof(__pyx_k_port), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_put_data, __pyx_k_put_data, sizeof(__pyx_k_put_data), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_read_data, __pyx_k_read_data, sizeof(__pyx_k_read_data), 0, 0, 1, 1},
@@ -4723,165 +5088,190 @@
   {&__pyx_n_s_thread, __pyx_k_thread, sizeof(__pyx_k_thread), 0, 0, 1, 1},
   {&__pyx_n_s_threading, __pyx_k_threading, sizeof(__pyx_k_threading), 0, 0, 1, 1},
   {&__pyx_n_u_tuple, __pyx_k_tuple, sizeof(__pyx_k_tuple), 0, 1, 0, 1},
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
   {&__pyx_n_s_uint8, __pyx_k_uint8, sizeof(__pyx_k_uint8), 0, 0, 1, 1},
   {&__pyx_n_u_unicode, __pyx_k_unicode, sizeof(__pyx_k_unicode), 0, 1, 0, 1},
   {&__pyx_n_s_use_thread, __pyx_k_use_thread, sizeof(__pyx_k_use_thread), 0, 0, 1, 1},
+  {&__pyx_n_s_viso_sdk_constants, __pyx_k_viso_sdk_constants, sizeof(__pyx_k_viso_sdk_constants), 0, 0, 1, 1},
   {&__pyx_n_s_viso_sdk_logging, __pyx_k_viso_sdk_logging, sizeof(__pyx_k_viso_sdk_logging), 0, 0, 1, 1},
   {&__pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_k_viso_sdk_redis_redis_wrapper, sizeof(__pyx_k_viso_sdk_redis_redis_wrapper), 0, 0, 1, 1},
   {&__pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_k_viso_sdk_redis_redis_wrapper_py, sizeof(__pyx_k_viso_sdk_redis_redis_wrapper_py), 0, 0, 1, 0},
   {&__pyx_n_s_warning, __pyx_k_warning, sizeof(__pyx_k_warning), 0, 0, 1, 1},
   {&__pyx_n_s_write_frame, __pyx_k_write_frame, sizeof(__pyx_k_write_frame), 0, 0, 1, 1},
   {&__pyx_n_s_write_to_redis, __pyx_k_write_to_redis, sizeof(__pyx_k_write_to_redis), 0, 0, 1, 1},
   {&__pyx_n_s_zoom, __pyx_k_zoom, sizeof(__pyx_k_zoom), 0, 0, 1, 1},
   {&__pyx_n_s_zoom_ratio, __pyx_k_zoom_ratio, sizeof(__pyx_k_zoom_ratio), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 41, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "viso_sdk/redis/redis_wrapper.py":17
+  /* "viso_sdk/redis/redis_wrapper.py":18
  * 
  * 
  * logger = get_logger("REDIS")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_u_REDIS); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_u_REDIS); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "viso_sdk/redis/redis_wrapper.py":29
+  /* "viso_sdk/redis/redis_wrapper.py":30
  *     """
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             thread: bool = True,
  */
-  __pyx_tuple__3 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_thread, __pyx_n_s_host, __pyx_n_s_port, __pyx_n_s_img_arr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_init, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __pyx_tuple__5 = PyTuple_Pack(3, ((PyObject *)Py_True), ((PyObject*)__pyx_n_u_localhost), ((PyObject *)__pyx_int_6379)); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_thread, __pyx_n_s_host, __pyx_n_s_port, __pyx_n_s_img_arr); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_init, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(3, ((PyObject *)Py_True), ((PyObject*)__pyx_n_u_localhost), ((PyObject *)__pyx_int_6379)); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "viso_sdk/redis/redis_wrapper.py":41
+  /* "viso_sdk/redis/redis_wrapper.py":42
+ * 
+ *     @staticmethod
+ *     def gen_redis_key_local(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.REDIS.LOCAL}_{node_id}_{port}"
+ * 
+ */
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_node_id, __pyx_n_s_port); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_gen_redis_key_local, 42, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 42, __pyx_L1_error)
+
+  /* "viso_sdk/redis/redis_wrapper.py":46
+ * 
+ *     @staticmethod
+ *     def gen_redis_key_status(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.REDIS.STATUS}_{node_id}_{port}"
+ * 
+ */
+  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_s_node_id, __pyx_n_s_port); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_gen_redis_key_status, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 46, __pyx_L1_error)
+
+  /* "viso_sdk/redis/redis_wrapper.py":50
  * 
  *     @staticmethod
  *     def base64_to_img(b64_bytes: bytes) -> Union[None, np.ndarray]:             # <<<<<<<<<<<<<<
  *         """Convert base64 string to opencv frame"""
  *         try:
  */
-  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_b64_bytes, __pyx_n_s_str_frame, __pyx_n_s_img_arr, __pyx_n_s_image, __pyx_n_s_err); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 41, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_base64_to_img, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_b64_bytes, __pyx_n_s_str_frame, __pyx_n_s_img_arr, __pyx_n_s_image, __pyx_n_s_err); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_base64_to_img, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 50, __pyx_L1_error)
 
-  /* "viso_sdk/redis/redis_wrapper.py":56
+  /* "viso_sdk/redis/redis_wrapper.py":65
  * 
  *     @staticmethod
  *     def img_to_base64str(image: np.ndarray, zoom_ratio: Optional[float] = 1.0) -> tuple:             # <<<<<<<<<<<<<<
  *         """Convert opencv frame to base64 encoded string"""
  *         if zoom_ratio != 1.0:
  */
-  __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_image, __pyx_n_s_zoom_ratio, __pyx_n_s_ret, __pyx_n_s_jpg_2, __pyx_n_s_jpg_as_text); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 56, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_img_to_base64str, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 56, __pyx_L1_error)
-  __pyx_tuple__10 = PyTuple_Pack(1, ((PyObject*)__pyx_float_1_0)); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 56, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__13 = PyTuple_Pack(5, __pyx_n_s_image, __pyx_n_s_zoom_ratio, __pyx_n_s_ret, __pyx_n_s_jpg_2, __pyx_n_s_jpg_as_text); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_img_to_base64str, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, ((PyObject*)__pyx_float_1_0)); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "viso_sdk/redis/redis_wrapper.py":66
+  /* "viso_sdk/redis/redis_wrapper.py":75
  *         return ret, jpg_as_text
  * 
  *     def write_frame(             # <<<<<<<<<<<<<<
  *             self, frame: np.ndarray, redis_key: str, zoom: Optional[float] = 1.0
  *     ) -> bool:
  */
-  __pyx_tuple__11 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_frame, __pyx_n_s_redis_key, __pyx_n_s_zoom); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 66, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_write_frame, 66, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 66, __pyx_L1_error)
-  __pyx_tuple__13 = PyTuple_Pack(1, ((PyObject*)__pyx_float_1_0)); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 66, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__16 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_frame, __pyx_n_s_redis_key, __pyx_n_s_zoom); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_write_frame, 75, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, ((PyObject*)__pyx_float_1_0)); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "viso_sdk/redis/redis_wrapper.py":83
+  /* "viso_sdk/redis/redis_wrapper.py":92
  *         return self._write_to_redis(frame, redis_key, zoom)
  * 
  *     def _write_to_redis(             # <<<<<<<<<<<<<<
  *             self,
  *             frame: Union[np.ndarray, None],
  */
-  __pyx_tuple__14 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_frame, __pyx_n_s_redis_key, __pyx_n_s_zoom, __pyx_n_s_ret, __pyx_n_s_jpg_as_text, __pyx_n_s_err); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_write_to_redis, 83, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 83, __pyx_L1_error)
-  __pyx_tuple__16 = PyTuple_Pack(1, ((PyObject*)__pyx_float_1_0)); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__19 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_frame, __pyx_n_s_redis_key, __pyx_n_s_zoom, __pyx_n_s_ret, __pyx_n_s_jpg_as_text, __pyx_n_s_err); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_write_to_redis, 92, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(1, ((PyObject*)__pyx_float_1_0)); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
-  /* "viso_sdk/redis/redis_wrapper.py":101
+  /* "viso_sdk/redis/redis_wrapper.py":110
  *         return bool(self._redis_client.delete(redis_key))
  * 
  *     def delete_data(self, redis_key: str) -> bool:             # <<<<<<<<<<<<<<
  *         """Delete data from the target redis location
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_redis_key); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_delete_data, 101, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_redis_key); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_delete_data, 110, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 110, __pyx_L1_error)
 
-  /* "viso_sdk/redis/redis_wrapper.py":109
+  /* "viso_sdk/redis/redis_wrapper.py":118
  *         return bool(self._redis_client.delete(redis_key))
  * 
  *     def put_data(self, redis_key: str, data: str) -> bool:             # <<<<<<<<<<<<<<
  *         """Write data to the target redis location
  * 
  */
-  __pyx_tuple__19 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_redis_key, __pyx_n_s_data); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_put_data, 109, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_redis_key, __pyx_n_s_data); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_put_data, 118, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 118, __pyx_L1_error)
 
-  /* "viso_sdk/redis/redis_wrapper.py":118
+  /* "viso_sdk/redis/redis_wrapper.py":127
  *         return bool(self._redis_client.set(redis_key, data))
  * 
  *     def read_data(self, redis_key: str) -> Any:             # <<<<<<<<<<<<<<
  *         """Read data from the target redis location
  * 
  */
-  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_redis_key); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 118, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_read_data, 118, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_redis_key); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_read_data, 127, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 127, __pyx_L1_error)
 
-  /* "viso_sdk/redis/redis_wrapper.py":126
+  /* "viso_sdk/redis/redis_wrapper.py":135
  *         return self._redis_client.get(redis_key)
  * 
  *     def get_frame(self, redis_key: str) -> Union[np.ndarray, None]:             # <<<<<<<<<<<<<<
  *         """Read video frame from a given redis key
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_redis_key, __pyx_n_s_b64_bytes, __pyx_n_s_err); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 126, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_get_frame, 126, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_redis_key, __pyx_n_s_b64_bytes, __pyx_n_s_err); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_redis_redis_wrapper_py, __pyx_n_s_get_frame, 135, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5257,439 +5647,506 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_redis, __pyx_t_2) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "viso_sdk/redis/redis_wrapper.py":14
  * 
  * 
- * from viso_sdk.logging import get_logger             # <<<<<<<<<<<<<<
- * 
+ * from viso_sdk.constants import PREFIX             # <<<<<<<<<<<<<<
+ * from viso_sdk.logging import get_logger
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_get_logger);
-  __Pyx_GIVEREF(__pyx_n_s_get_logger);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_get_logger);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_viso_sdk_logging, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_PREFIX);
+  __Pyx_GIVEREF(__pyx_n_s_PREFIX);
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PREFIX);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_viso_sdk_constants, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_get_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_PREFIX); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_logger, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_PREFIX, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":17
+  /* "viso_sdk/redis/redis_wrapper.py":15
  * 
- * 
- * logger = get_logger("REDIS")             # <<<<<<<<<<<<<<
+ * from viso_sdk.constants import PREFIX
+ * from viso_sdk.logging import get_logger             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_get_logger);
+  __Pyx_GIVEREF(__pyx_n_s_get_logger);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_get_logger);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_viso_sdk_logging, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logger, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_get_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_logger, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "viso_sdk/redis/redis_wrapper.py":18
+ * 
+ * 
+ * logger = get_logger("REDIS")             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logger, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":20
+  /* "viso_sdk/redis/redis_wrapper.py":21
  * 
  * 
  * class RedisWrapper:             # <<<<<<<<<<<<<<
  *     """Represents a redis client specified for the containers.
  * 
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_RedisWrapper, __pyx_n_s_RedisWrapper, (PyObject *) NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_kp_s_Represents_a_redis_client_specif); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_RedisWrapper, __pyx_n_s_RedisWrapper, (PyObject *) NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_kp_s_Represents_a_redis_client_specif); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
 
-  /* "viso_sdk/redis/redis_wrapper.py":29
+  /* "viso_sdk/redis/redis_wrapper.py":30
  *     """
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             thread: bool = True,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
 
-  /* "viso_sdk/redis/redis_wrapper.py":31
+  /* "viso_sdk/redis/redis_wrapper.py":32
  *     def __init__(
  *             self,
  *             thread: bool = True,             # <<<<<<<<<<<<<<
  *             host: str = "localhost",
  *             port: int = 6379,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_thread, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_host, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_port, __pyx_n_u_int) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_thread, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_host, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_port, __pyx_n_u_int) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
 
-  /* "viso_sdk/redis/redis_wrapper.py":29
+  /* "viso_sdk/redis/redis_wrapper.py":30
  *     """
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             thread: bool = True,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_1__init__, 0, __pyx_n_s_RedisWrapper___init, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_1__init__, 0, __pyx_n_s_RedisWrapper___init, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__5);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_1);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__6);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
+  /* "viso_sdk/redis/redis_wrapper.py":42
+ * 
+ *     @staticmethod
+ *     def gen_redis_key_local(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.REDIS.LOCAL}_{node_id}_{port}"
+ * 
+ */
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3gen_redis_key_local, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_RedisWrapper_gen_redis_key_local, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+
   /* "viso_sdk/redis/redis_wrapper.py":41
+ *         _img_arr = None
+ * 
+ *     @staticmethod             # <<<<<<<<<<<<<<
+ *     def gen_redis_key_local(node_id, port):
+ *         return f"{PREFIX.REDIS.LOCAL}_{node_id}_{port}"
+ */
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_gen_redis_key_local, __pyx_t_2) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "viso_sdk/redis/redis_wrapper.py":46
+ * 
+ *     @staticmethod
+ *     def gen_redis_key_status(node_id, port):             # <<<<<<<<<<<<<<
+ *         return f"{PREFIX.REDIS.STATUS}_{node_id}_{port}"
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5gen_redis_key_status, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_RedisWrapper_gen_redis_key_statu, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "viso_sdk/redis/redis_wrapper.py":45
+ *         return f"{PREFIX.REDIS.LOCAL}_{node_id}_{port}"
+ * 
+ *     @staticmethod             # <<<<<<<<<<<<<<
+ *     def gen_redis_key_status(node_id, port):
+ *         return f"{PREFIX.REDIS.STATUS}_{node_id}_{port}"
+ */
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_gen_redis_key_status, __pyx_t_3) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "viso_sdk/redis/redis_wrapper.py":50
  * 
  *     @staticmethod
  *     def base64_to_img(b64_bytes: bytes) -> Union[None, np.ndarray]:             # <<<<<<<<<<<<<<
  *         """Convert base64 string to opencv frame"""
  *         try:
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_b64_bytes, __pyx_n_u_bytes) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Union); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_b64_bytes, __pyx_n_u_bytes) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_4, 0, Py_None);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_3base64_to_img, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_RedisWrapper_base64_to_img, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7base64_to_img, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_RedisWrapper_base64_to_img, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":40
- *         _img_arr = None
+  /* "viso_sdk/redis/redis_wrapper.py":49
+ *         return f"{PREFIX.REDIS.STATUS}_{node_id}_{port}"
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def base64_to_img(b64_bytes: bytes) -> Union[None, np.ndarray]:
  *         """Convert base64 string to opencv frame"""
  */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_base64_to_img, __pyx_t_3) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_base64_to_img, __pyx_t_3) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":56
+  /* "viso_sdk/redis/redis_wrapper.py":65
  * 
  *     @staticmethod
  *     def img_to_base64str(image: np.ndarray, zoom_ratio: Optional[float] = 1.0) -> tuple:             # <<<<<<<<<<<<<<
  *         """Convert opencv frame to base64 encoded string"""
  *         if zoom_ratio != 1.0:
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_image, __pyx_t_4) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_image, __pyx_t_4) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Optional); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Optional); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_4, ((PyObject *)(&PyFloat_Type))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_4, ((PyObject *)(&PyFloat_Type))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_zoom_ratio, __pyx_t_5) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_zoom_ratio, __pyx_t_5) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_u_tuple) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_5img_to_base64str, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_RedisWrapper_img_to_base64str, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_u_tuple) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9img_to_base64str, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_RedisWrapper_img_to_base64str, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__10);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__15);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":55
+  /* "viso_sdk/redis/redis_wrapper.py":64
  *         return None
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def img_to_base64str(image: np.ndarray, zoom_ratio: Optional[float] = 1.0) -> tuple:
  *         """Convert opencv frame to base64 encoded string"""
  */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_img_to_base64str, __pyx_t_3) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_img_to_base64str, __pyx_t_3) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":66
+  /* "viso_sdk/redis/redis_wrapper.py":75
  *         return ret, jpg_as_text
  * 
  *     def write_frame(             # <<<<<<<<<<<<<<
  *             self, frame: np.ndarray, redis_key: str, zoom: Optional[float] = 1.0
  *     ) -> bool:
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "viso_sdk/redis/redis_wrapper.py":67
+  /* "viso_sdk/redis/redis_wrapper.py":76
  * 
  *     def write_frame(
  *             self, frame: np.ndarray, redis_key: str, zoom: Optional[float] = 1.0             # <<<<<<<<<<<<<<
  *     ) -> bool:
  *         """Write video frame to the target redis key
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_frame, __pyx_t_4) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_frame, __pyx_t_4) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Optional); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Optional); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_4, ((PyObject *)(&PyFloat_Type))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_4, ((PyObject *)(&PyFloat_Type))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_zoom, __pyx_t_5) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_zoom, __pyx_t_5) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":68
+  /* "viso_sdk/redis/redis_wrapper.py":77
  *     def write_frame(
  *             self, frame: np.ndarray, redis_key: str, zoom: Optional[float] = 1.0
  *     ) -> bool:             # <<<<<<<<<<<<<<
  *         """Write video frame to the target redis key
  * 
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
 
-  /* "viso_sdk/redis/redis_wrapper.py":66
+  /* "viso_sdk/redis/redis_wrapper.py":75
  *         return ret, jpg_as_text
  * 
  *     def write_frame(             # <<<<<<<<<<<<<<
  *             self, frame: np.ndarray, redis_key: str, zoom: Optional[float] = 1.0
  *     ) -> bool:
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_7write_frame, 0, __pyx_n_s_RedisWrapper_write_frame, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11write_frame, 0, __pyx_n_s_RedisWrapper_write_frame, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__13);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__18);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_write_frame, __pyx_t_5) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_write_frame, __pyx_t_5) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":83
+  /* "viso_sdk/redis/redis_wrapper.py":92
  *         return self._write_to_redis(frame, redis_key, zoom)
  * 
  *     def _write_to_redis(             # <<<<<<<<<<<<<<
  *             self,
  *             frame: Union[np.ndarray, None],
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "viso_sdk/redis/redis_wrapper.py":85
+  /* "viso_sdk/redis/redis_wrapper.py":94
  *     def _write_to_redis(
  *             self,
  *             frame: Union[np.ndarray, None],             # <<<<<<<<<<<<<<
  *             redis_key: str,
  *             zoom: Optional[float] = 1.0,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_4, 1, Py_None);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_frame, __pyx_t_1) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_frame, __pyx_t_2) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
 
-  /* "viso_sdk/redis/redis_wrapper.py":87
+  /* "viso_sdk/redis/redis_wrapper.py":96
  *             frame: Union[np.ndarray, None],
  *             redis_key: str,
  *             zoom: Optional[float] = 1.0,             # <<<<<<<<<<<<<<
  *     ) -> bool:
  *         """Internal function that is executed in background thread"""
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Optional); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_1, ((PyObject *)(&PyFloat_Type))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Optional); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_2, ((PyObject *)(&PyFloat_Type))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_zoom, __pyx_t_4) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_zoom, __pyx_t_4) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":88
+  /* "viso_sdk/redis/redis_wrapper.py":97
  *             redis_key: str,
  *             zoom: Optional[float] = 1.0,
  *     ) -> bool:             # <<<<<<<<<<<<<<
  *         """Internal function that is executed in background thread"""
  *         if frame is not None:
  */
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
 
-  /* "viso_sdk/redis/redis_wrapper.py":83
+  /* "viso_sdk/redis/redis_wrapper.py":92
  *         return self._write_to_redis(frame, redis_key, zoom)
  * 
  *     def _write_to_redis(             # <<<<<<<<<<<<<<
  *             self,
  *             frame: Union[np.ndarray, None],
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_9_write_to_redis, 0, __pyx_n_s_RedisWrapper__write_to_redis, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13_write_to_redis, 0, __pyx_n_s_RedisWrapper__write_to_redis, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__16);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__21);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_write_to_redis, __pyx_t_4) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_write_to_redis, __pyx_t_4) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":101
+  /* "viso_sdk/redis/redis_wrapper.py":110
  *         return bool(self._redis_client.delete(redis_key))
  * 
  *     def delete_data(self, redis_key: str) -> bool:             # <<<<<<<<<<<<<<
  *         """Delete data from the target redis location
  * 
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_11delete_data, 0, __pyx_n_s_RedisWrapper_delete_data, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15delete_data, 0, __pyx_n_s_RedisWrapper_delete_data, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_delete_data, __pyx_t_5) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_delete_data, __pyx_t_5) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":109
+  /* "viso_sdk/redis/redis_wrapper.py":118
  *         return bool(self._redis_client.delete(redis_key))
  * 
  *     def put_data(self, redis_key: str, data: str) -> bool:             # <<<<<<<<<<<<<<
  *         """Write data to the target redis location
  * 
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_data, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_13put_data, 0, __pyx_n_s_RedisWrapper_put_data, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_data, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17put_data, 0, __pyx_n_s_RedisWrapper_put_data, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_put_data, __pyx_t_4) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_put_data, __pyx_t_4) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":118
+  /* "viso_sdk/redis/redis_wrapper.py":127
  *         return bool(self._redis_client.set(redis_key, data))
  * 
  *     def read_data(self, redis_key: str) -> Any:             # <<<<<<<<<<<<<<
  *         """Read data from the target redis location
  * 
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Any); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Any); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_15read_data, 0, __pyx_n_s_RedisWrapper_read_data, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_19read_data, 0, __pyx_n_s_RedisWrapper_read_data, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_read_data, __pyx_t_5) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_read_data, __pyx_t_5) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":126
+  /* "viso_sdk/redis/redis_wrapper.py":135
  *         return self._redis_client.get(redis_key)
  * 
  *     def get_frame(self, redis_key: str) -> Union[np.ndarray, None]:             # <<<<<<<<<<<<<<
  *         """Read video frame from a given redis key
  * 
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Union); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_redis_key, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Union); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, Py_None);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_3) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_3) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_17get_frame, 0, __pyx_n_s_RedisWrapper_get_frame, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_5redis_13redis_wrapper_12RedisWrapper_21get_frame, 0, __pyx_n_s_RedisWrapper_get_frame, NULL, __pyx_n_s_viso_sdk_redis_redis_wrapper, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_frame, __pyx_t_3) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_frame, __pyx_t_3) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "viso_sdk/redis/redis_wrapper.py":20
+  /* "viso_sdk/redis/redis_wrapper.py":21
  * 
  * 
  * class RedisWrapper:             # <<<<<<<<<<<<<<
  *     """Represents a redis client specified for the containers.
  * 
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_RedisWrapper, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_RedisWrapper, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RedisWrapper, __pyx_t_3) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RedisWrapper, __pyx_t_3) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "viso_sdk/redis/redis_wrapper.py":1
  * """             # <<<<<<<<<<<<<<
  * Redis Wrapper from viso.ai
  * """
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -6157,14 +6614,76 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
+/* JoinPyUnicode */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      CYTHON_UNUSED Py_UCS4 max_char) {
+#if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    PyObject *result_uval;
+    int result_ukind;
+    Py_ssize_t i, char_pos;
+    void *result_udata;
+#if CYTHON_PEP393_ENABLED
+    result_uval = PyUnicode_New(result_ulength, max_char);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
+    result_udata = PyUnicode_DATA(result_uval);
+#else
+    result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = sizeof(Py_UNICODE);
+    result_udata = PyUnicode_AS_UNICODE(result_uval);
+#endif
+    char_pos = 0;
+    for (i=0; i < value_count; i++) {
+        int ukind;
+        Py_ssize_t ulength;
+        void *udata;
+        PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
+        if (unlikely(__Pyx_PyUnicode_READY(uval)))
+            goto bad;
+        ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
+        if (unlikely(!ulength))
+            continue;
+        if (unlikely(char_pos + ulength < 0))
+            goto overflow;
+        ukind = __Pyx_PyUnicode_KIND(uval);
+        udata = __Pyx_PyUnicode_DATA(uval);
+        if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
+            memcpy((char *)result_udata + char_pos * result_ukind, udata, (size_t) (ulength * result_ukind));
+        } else {
+            #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
+            _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
+            #else
+            Py_ssize_t j;
+            for (j=0; j < ulength; j++) {
+                Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
+                __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
+            }
+            #endif
+        }
+        char_pos += ulength;
+    }
+    return result_uval;
+overflow:
+    PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
+bad:
+    Py_DECREF(result_uval);
+    return NULL;
+#else
+    result_ulength++;
+    value_count++;
+    return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
+#endif
+}
+
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -6627,76 +7146,14 @@
 /* PyUnicode_Unicode */
   static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj) {
     if (unlikely(obj == Py_None))
         obj = __pyx_kp_u_None;
     return __Pyx_NewRef(obj);
 }
 
-/* JoinPyUnicode */
-  static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
-                                      CYTHON_UNUSED Py_UCS4 max_char) {
-#if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    PyObject *result_uval;
-    int result_ukind;
-    Py_ssize_t i, char_pos;
-    void *result_udata;
-#if CYTHON_PEP393_ENABLED
-    result_uval = PyUnicode_New(result_ulength, max_char);
-    if (unlikely(!result_uval)) return NULL;
-    result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
-    result_udata = PyUnicode_DATA(result_uval);
-#else
-    result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
-    if (unlikely(!result_uval)) return NULL;
-    result_ukind = sizeof(Py_UNICODE);
-    result_udata = PyUnicode_AS_UNICODE(result_uval);
-#endif
-    char_pos = 0;
-    for (i=0; i < value_count; i++) {
-        int ukind;
-        Py_ssize_t ulength;
-        void *udata;
-        PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
-        if (unlikely(__Pyx_PyUnicode_READY(uval)))
-            goto bad;
-        ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
-        if (unlikely(!ulength))
-            continue;
-        if (unlikely(char_pos + ulength < 0))
-            goto overflow;
-        ukind = __Pyx_PyUnicode_KIND(uval);
-        udata = __Pyx_PyUnicode_DATA(uval);
-        if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
-            memcpy((char *)result_udata + char_pos * result_ukind, udata, (size_t) (ulength * result_ukind));
-        } else {
-            #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
-            _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
-            #else
-            Py_ssize_t j;
-            for (j=0; j < ulength; j++) {
-                Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
-                __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
-            }
-            #endif
-        }
-        char_pos += ulength;
-    }
-    return result_uval;
-overflow:
-    PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
-bad:
-    Py_DECREF(result_uval);
-    return NULL;
-#else
-    result_ulength++;
-    value_count++;
-    return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
-#endif
-}
-
 /* Import */
   static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *empty_list = 0;
     PyObject *module = 0;
     PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
     PyObject *list;
```

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/redis/redis_wrapper.py` & `viso-sdk-python-0.0.5/viso_sdk/redis/redis_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, Optional, Union
 
 import cv2  # type: ignore
 import numpy as np
 import redis
 
 
+from viso_sdk.constants import PREFIX
 from viso_sdk.logging import get_logger
 
 
 logger = get_logger("REDIS")
 
 
 class RedisWrapper:
@@ -34,14 +35,22 @@
     ):
         self._use_thread = thread
         self._redis_client = redis.StrictRedis(host, port)
 
         _img_arr = None
 
     @staticmethod
+    def gen_redis_key_local(node_id, port):
+        return f"{PREFIX.REDIS.LOCAL}_{node_id}_{port}"
+
+    @staticmethod
+    def gen_redis_key_status(node_id, port):
+        return f"{PREFIX.REDIS.STATUS}_{node_id}_{port}"
+
+    @staticmethod
     def base64_to_img(b64_bytes: bytes) -> Union[None, np.ndarray]:
         """Convert base64 string to opencv frame"""
         try:
             str_frame = base64.b64decode(b64_bytes)
             _img_arr = np.frombuffer(str_frame, dtype=np.uint8)
             image = cv2.imdecode(  # pylint: disable=no-member
                 _img_arr, -1
```

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/__init__.c` & `viso-sdk-python-0.0.5/viso_sdk/visualize/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/custom_font.c` & `viso-sdk-python-0.0.5/viso_sdk/visualize/custom_font.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/custom_font.py` & `viso-sdk-python-0.0.5/viso_sdk/visualize/custom_font.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/palette.c` & `viso-sdk-python-0.0.5/viso_sdk/visualize/palette.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/palette.py` & `viso-sdk-python-0.0.5/viso_sdk/visualize/palette.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/visualization.c` & `viso-sdk-python-0.0.5/viso_sdk/visualize/visualization.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk/visualize/visualization.py` & `viso-sdk-python-0.0.5/viso_sdk/visualize/visualization.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk_python.egg-info/PKG-INFO` & `viso-sdk-python-0.0.5/viso_sdk_python.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,15 @@
 Metadata-Version: 2.1
 Name: viso-sdk-python
-Version: 0.0.4.dev0
-Summary: VisoSDK: A SDK in Python for viso containers
+Version: 0.0.5
+Summary: VisoSDK: A Python SDK for use in Viso containers
 Home-page: https://gitlab.com/TopKamera/03_edge/Base/viso-sdk-python-public.git
 Author: support@viso.ai
 Author-email: support@viso.ai
 License: LGPLv3
-Description: # viso-sdk-python
-        
-        **viso-sdk-python** is a utility for [viso.ai](https://viso.ai) containers.
-        
-        ## Installation
-        
-        Use `pip` to install the latest stable version of **viso-sdk-python**:
-        
-        ```shell
-        pip install viso-sdk-python
-        ```
-        
-        
-        ## Build
-        ```shell
-        python3 -m pip install -e .
-        python3 setup.py sdist bdist_wheel
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
@@ -36,7 +17,30 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: AUTHORS
+
+# viso-sdk-python
+
+**viso-sdk-python** is a utility for [viso.ai](https://viso.ai) containers.
+
+## Installation
+
+Use `pip` to install the latest stable version of **viso-sdk-python**:
+
+```shell
+pip install viso-sdk-python
+```
+
+
+## Build
+```shell
+python3 -m pip install -e .
+python3 setup.py sdist bdist_wheel
+```
+
+
```

### Comparing `viso-sdk-python-0.0.4.dev0/viso_sdk_python.egg-info/SOURCES.txt` & `viso-sdk-python-0.0.5/viso_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

