# Comparing `tmp/requestlib-1.0.0.tar.gz` & `tmp/requestlib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestlib-1.0.0.tar", last modified: Wed Apr 19 11:18:07 2023, max compression
+gzip compressed data, was "requestlib-1.0.2.tar", last modified: Wed Apr 19 16:20:28 2023, max compression
```

## Comparing `requestlib-1.0.0.tar` & `requestlib-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:18:07.753704 requestlib-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-19 11:18:07.753704 requestlib-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:18:07.753704 requestlib-1.0.0/requestlib/
--rw-r--r--   0 root         (0) root         (0)     1690 2023-04-19 11:18:07.000000 requestlib-1.0.0/requestlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:18:07.753704 requestlib-1.0.0/requestlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-19 11:18:07.000000 requestlib-1.0.0/requestlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-19 11:18:07.000000 requestlib-1.0.0/requestlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 11:18:07.000000 requestlib-1.0.0/requestlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 11:18:07.000000 requestlib-1.0.0/requestlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 11:18:07.753704 requestlib-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-04-19 11:18:06.000000 requestlib-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:20:28.098900 requestlib-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-19 16:20:28.098900 requestlib-1.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:20:28.098900 requestlib-1.0.2/requestlib/
+-rw-r--r--   0 root         (0) root         (0)    82161 2023-04-19 16:20:27.000000 requestlib-1.0.2/requestlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:20:28.098900 requestlib-1.0.2/requestlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-19 16:20:28.000000 requestlib-1.0.2/requestlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-19 16:20:28.000000 requestlib-1.0.2/requestlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:20:28.000000 requestlib-1.0.2/requestlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 16:20:28.000000 requestlib-1.0.2/requestlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 16:20:28.098900 requestlib-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      540 2023-04-19 16:20:27.000000 requestlib-1.0.2/setup.py
```

