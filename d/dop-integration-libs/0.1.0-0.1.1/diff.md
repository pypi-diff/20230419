# Comparing `tmp/dop_integration_libs-0.1.0.tar.gz` & `tmp/dop_integration_libs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dop_integration_libs-0.1.0.tar", max compression
+gzip compressed data, was "dop_integration_libs-0.1.1.tar", max compression
```

## Comparing `dop_integration_libs-0.1.0.tar` & `dop_integration_libs-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.0/dop_integration_libs/__init__.py
--rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.0/dop_integration_libs/__main__.py
--rw-r--r--   0        0        0      162 2023-04-19 13:17:52.910751 dop_integration_libs-0.1.0/dop_integration_libs/envirement.py
--rw-r--r--   0        0        0      389 2023-04-19 13:14:07.511380 dop_integration_libs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.1/dop_integration_libs/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.1/dop_integration_libs/__main__.py
+-rw-r--r--   0        0        0      388 2023-04-19 13:31:27.868704 dop_integration_libs-0.1.1/dop_integration_libs/environment.py
+-rw-r--r--   0        0        0      389 2023-04-19 13:31:45.957425 dop_integration_libs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.1/PKG-INFO
```

