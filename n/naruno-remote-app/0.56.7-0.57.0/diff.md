# Comparing `tmp/naruno_remote_app-0.56.7.tar.gz` & `tmp/naruno_remote_app-0.57.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_remote_app-0.56.7.tar", last modified: Wed Apr 19 00:40:52 2023, max compression
+gzip compressed data, was "naruno_remote_app-0.57.0.tar", last modified: Wed Apr 19 11:38:12 2023, max compression
```

## Comparing `naruno_remote_app-0.56.7.tar` & `naruno_remote_app-0.57.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:40:52.315648 naruno_remote_app-0.56.7/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 00:40:52.315648 naruno_remote_app-0.56.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:40:52.315648 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:40:52.000000 naruno_remote_app-0.56.7/naruno_remote_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:40:52.315648 naruno_remote_app-0.56.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-19 00:40:28.000000 naruno_remote_app-0.56.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:38:11.998513 naruno_remote_app-0.57.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 11:38:11.998513 naruno_remote_app-0.57.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:38:11.998513 naruno_remote_app-0.57.0/naruno_remote_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 11:38:11.000000 naruno_remote_app-0.57.0/naruno_remote_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-19 11:38:11.000000 naruno_remote_app-0.57.0/naruno_remote_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:38:11.000000 naruno_remote_app-0.57.0/naruno_remote_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:38:11.000000 naruno_remote_app-0.57.0/naruno_remote_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 11:38:11.000000 naruno_remote_app-0.57.0/naruno_remote_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:38:11.000000 naruno_remote_app-0.57.0/naruno_remote_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:38:11.998513 naruno_remote_app-0.57.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-19 11:37:54.000000 naruno_remote_app-0.57.0/setup.py
```

