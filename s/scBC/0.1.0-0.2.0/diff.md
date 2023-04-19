# Comparing `tmp/scBC-0.1.0.tar.gz` & `tmp/scBC-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scBC-0.1.0.tar", last modified: Mon Apr 17 09:57:36 2023, max compression
+gzip compressed data, was "scBC-0.2.0.tar", last modified: Wed Apr 19 03:44:51 2023, max compression
```

## Comparing `scBC-0.1.0.tar` & `scBC-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,17 @@
-drwxrwxr-x   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)        0 2023-04-17 09:57:36.265910 scBC-0.1.0/
--rw-rw-r--   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)      319 2023-04-17 09:57:36.265698 scBC-0.1.0/PKG-INFO
-drwxrwxr-x   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)        0 2023-04-17 09:57:36.265203 scBC-0.1.0/scBC.egg-info/
--rw-rw-r--   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)      319 2023-04-17 09:57:36.263678 scBC-0.1.0/scBC.egg-info/PKG-INFO
--rw-rw-r--   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)      147 2023-04-17 09:57:36.264098 scBC-0.1.0/scBC.egg-info/SOURCES.txt
--rw-rw-r--   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)        1 2023-04-17 09:57:36.264514 scBC-0.1.0/scBC.egg-info/dependency_links.txt
--rw-rw-r--   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)       11 2023-04-17 09:57:36.264906 scBC-0.1.0/scBC.egg-info/requires.txt
--rw-rw-r--   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)        1 2023-04-17 09:57:36.265284 scBC-0.1.0/scBC.egg-info/top_level.txt
--rw-rw-r--   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)       38 2023-04-17 09:57:36.265998 scBC-0.1.0/setup.cfg
--rw-rw-r--   0 clsyzs-gyq  (8054) clsyzs-gyq  (8054)      732 2023-04-17 09:45:53.000000 scBC-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 03:44:51.746107 scBC-0.2.0/
+-rw-rw-rw-   0        0        0     1065 2023-04-19 03:17:25.000000 scBC-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    10969 2023-04-19 03:44:51.745112 scBC-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10403 2023-04-19 03:14:30.000000 scBC-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 03:44:51.736101 scBC-0.2.0/scBC/
+-rw-rw-rw-   0        0        0     6095 2023-04-19 03:14:30.000000 scBC-0.2.0/scBC/DWL.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 03:14:30.000000 scBC-0.2.0/scBC/__init__.py
+-rw-rw-rw-   0        0        0     4240 2023-04-19 03:14:30.000000 scBC-0.2.0/scBC/data.py
+-rw-rw-rw-   0        0        0    18655 2023-04-19 03:14:30.000000 scBC-0.2.0/scBC/model.py
+drwxrwxrwx   0        0        0        0 2023-04-19 03:44:51.742107 scBC-0.2.0/scBC.egg-info/
+-rw-rw-rw-   0        0        0    10969 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-19 03:44:49.000000 scBC-0.2.0/scBC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 03:44:51.746107 scBC-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-04-19 03:44:45.000000 scBC-0.2.0/setup.py
```

