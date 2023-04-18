# Comparing `tmp/reign_airflow_utils-0.1.0.tar.gz` & `tmp/reign_airflow_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reign_airflow_utils-0.1.0.tar", last modified: Wed Apr  5 15:51:48 2023, max compression
+gzip compressed data, was "reign_airflow_utils-0.1.4.tar", last modified: Tue Apr 18 21:58:43 2023, max compression
```

## Comparing `reign_airflow_utils-0.1.0.tar` & `reign_airflow_utils-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:48.305719 reign_airflow_utils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-05 15:51:48.305719 reign_airflow_utils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-05 15:51:48.305719 reign_airflow_utils-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:48.301719 reign_airflow_utils-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:48.305719 reign_airflow_utils-0.1.0/src/reign_airflow_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:48.305719 reign_airflow_utils-0.1.0/src/reign_airflow_utils/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils/hooks/oracle_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:48.305719 reign_airflow_utils-0.1.0/src/reign_airflow_utils/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:48.305719 reign_airflow_utils-0.1.0/src/reign_airflow_utils/operators/oracle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils/operators/oracle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils/operators/oracle/dump_expert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-05 15:51:39.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils/secret_backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:51:48.305719 reign_airflow_utils-0.1.0/src/reign_airflow_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-05 15:51:48.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-05 15:51:48.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:51:48.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-05 15:51:48.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-05 15:51:48.000000 reign_airflow_utils-0.1.0/src/reign_airflow_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:43.334598 reign_airflow_utils-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-18 21:58:43.334598 reign_airflow_utils-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-18 21:58:43.334598 reign_airflow_utils-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:43.330598 reign_airflow_utils-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:43.330598 reign_airflow_utils-0.1.4/src/reign_airflow_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:43.334598 reign_airflow_utils-0.1.4/src/reign_airflow_utils/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils/hooks/oracle_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:43.334598 reign_airflow_utils-0.1.4/src/reign_airflow_utils/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:43.334598 reign_airflow_utils-0.1.4/src/reign_airflow_utils/operators/oracle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils/operators/oracle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils/operators/oracle/dump_expert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-18 21:58:34.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils/secret_backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:43.330598 reign_airflow_utils-0.1.4/src/reign_airflow_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-18 21:58:43.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-18 21:58:43.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:58:43.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 21:58:43.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 21:58:43.000000 reign_airflow_utils-0.1.4/src/reign_airflow_utils.egg-info/top_level.txt
```

### Comparing `reign_airflow_utils-0.1.0/LICENSE` & `reign_airflow_utils-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reign_airflow_utils-0.1.0/src/reign_airflow_utils/hooks/oracle_hook.py` & `reign_airflow_utils-0.1.4/src/reign_airflow_utils/hooks/oracle_hook.py`

 * *Files identical despite different names*

### Comparing `reign_airflow_utils-0.1.0/src/reign_airflow_utils/secret_backends.py` & `reign_airflow_utils-0.1.4/src/reign_airflow_utils/secret_backends.py`

 * *Files identical despite different names*

### Comparing `reign_airflow_utils-0.1.0/src/reign_airflow_utils.egg-info/SOURCES.txt` & `reign_airflow_utils-0.1.4/src/reign_airflow_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

