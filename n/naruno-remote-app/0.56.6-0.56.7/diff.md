# Comparing `tmp/naruno_remote_app-0.56.6.tar.gz` & `tmp/naruno_remote_app-0.56.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_remote_app-0.56.6.tar", last modified: Tue Apr 18 23:57:28 2023, max compression
+gzip compressed data, was "naruno_remote_app-0.56.7.tar", last modified: Wed Apr 19 00:40:52 2023, max compression
```

## Comparing `naruno_remote_app-0.56.6.tar` & `naruno_remote_app-0.56.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:57:28.277058 naruno_remote_app-0.56.6/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-18 23:57:28.277058 naruno_remote_app-0.56.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:57:28.277058 naruno_remote_app-0.56.6/naruno_remote_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-18 23:57:28.000000 naruno_remote_app-0.56.6/naruno_remote_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 23:57:28.000000 naruno_remote_app-0.56.6/naruno_remote_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:57:28.000000 naruno_remote_app-0.56.6/naruno_remote_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:57:28.000000 naruno_remote_app-0.56.6/naruno_remote_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 23:57:28.000000 naruno_remote_app-0.56.6/naruno_remote_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:57:28.000000 naruno_remote_app-0.56.6/naruno_remote_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 23:57:28.277058 naruno_remote_app-0.56.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-18 23:57:07.000000 naruno_remote_app-0.56.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:40:52.315648 naruno_remote_app-0.56.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 00:40:52.315648 naruno_remote_app-0.56.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:40:52.315648 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:40:52.315648 naruno_remote_app-0.56.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-19 00:40:28.000000 naruno_remote_app-0.56.7/setup.py
```

