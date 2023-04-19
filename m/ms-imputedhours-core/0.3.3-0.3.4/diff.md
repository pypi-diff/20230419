# Comparing `tmp/ms_imputedhours_core-0.3.3.tar.gz` & `tmp/ms_imputedhours_core-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_imputedhours_core-0.3.3.tar", last modified: Tue Apr 18 12:10:55 2023, max compression
+gzip compressed data, was "ms_imputedhours_core-0.3.4.tar", max compression
```

## Comparing `ms_imputedhours_core-0.3.3.tar` & `ms_imputedhours_core-0.3.4.tar`

### file list

```diff
@@ -1,88 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/__pycache__/test_agreements.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/test_agreements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/__pycache__/test_employee.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/test_employee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/bigquery.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/constants.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/__pycache__/test_data.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/alert.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/bigquery.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/dates.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_alert.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_bigquery.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_dates.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/__pycache__/hours.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/hours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/__pycache__/test_office.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/test_office.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/setup.py
+-rw-r--r--   0        0        0    35149 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2401 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/README.md
+-rw-r--r--   0        0        0       22 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/__init__.py
+-rw-r--r--   0        0        0     3238 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__tests__/__init__.py
+-rw-r--r--   0        0        0     3228 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__tests__/test_agreements.py
+-rw-r--r--   0        0        0     4113 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__tests__/__init__.py
+-rw-r--r--   0        0        0     6179 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__tests__/test_employee.py
+-rw-r--r--   0        0        0     6933 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__tests__/__init__.py
+-rw-r--r--   0        0        0     9019 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__tests__/test_data.py
+-rw-r--r--   0        0        0    10444 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/bigquery.py
+-rw-r--r--   0        0        0      171 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/constants.py
+-rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
+-rw-r--r--   0        0        0     4491 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
+-rw-r--r--   0        0        0     6206 2023-04-19 11:43:12.729574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0      776 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
+-rw-r--r--   0        0        0      655 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/alert.py
+-rw-r--r--   0        0        0     3599 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/bigquery.py
+-rw-r--r--   0        0        0      423 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/dates.py
+-rw-r--r--   0        0        0        0 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/transformers/__init__.py
+-rw-r--r--   0        0        0     3828 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/transformers/hours.py
+-rw-r--r--   0        0        0      203 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/office/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/office/__tests__/__init__.py
+-rw-r--r--   0        0        0      678 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/ms_imputedhours_core/office/__tests__/test_office.py
+-rw-r--r--   0        0        0      950 2023-04-19 11:43:12.733574 ms_imputedhours_core-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.4/PKG-INFO
```

### Comparing `ms_imputedhours_core-0.3.3/LICENSE` & `ms_imputedhours_core-0.3.4/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__init__.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 import os
 from datetime import datetime
-from gc_google_services_api.gsheet import GSheet
 
+from gc_google_services_api.gsheet import GSheet
 
 RANGE_NAME = os.getenv('GOOGLE_SHEET_AGREEMENT_RANGE', 'A2:B8000')
 CREDENTIALS_BASE64 = os.getenv('GOOGLE_SHEET_CREDENTIALS', '')
 SHEET_NAMES_TO_IGNORE = ['Summary']
 
 
 class Agreements(object):
     def __init__(self, spreadsheet_id) -> None:
         self.spreadsheet_id = spreadsheet_id
         self.service = GSheet()
 
     def get_hours_by_month(self, month, year, sheet_name):
         try:
             values = self.service.read_gsheet(
-                sheet_name, self.spreadsheet_id, RANGE_NAME)
+                sheet_name, self.spreadsheet_id, RANGE_NAME
+            )
         except Exception as e:
             print('[ERROR] - get_hours_by_month: ', e)
             values = {'values': []}
 
-        day_hours_data = {
-            'totalHours': 0.0,
-            'days': {}
-        }
+        day_hours_data = {'totalHours': 0.0, 'days': {}}
         for day_data in values['values']:
             day_obj = datetime.strptime(day_data[0], '%d/%m/%Y')
 
             if day_obj.month == month and day_obj.year == year:
                 day_hours = '{}'.format(day_data[1]).replace(',', '.')
                 day_hours_data['totalHours'] += float(day_hours)
                 day_hours_data['days'][day_obj.day] = day_hours
 
         return day_hours_data
 
     def get_hours_by_range(self, from_date, to_date, sheet_name):
         try:
             values = self.service.read_gsheet(
-                sheet_name, self.spreadsheet_id, RANGE_NAME)
+                sheet_name, self.spreadsheet_id, RANGE_NAME
+            )
         except Exception as e:
             print('[ERROR] - get_hours_by_range: ', e)
             values = {'values': []}
 
-        day_hours_data = {
-            'totalHours': 0.0,
-            'days': {}
-        }
+        day_hours_data = {'totalHours': 0.0, 'days': {}}
 
         for day_data in values['values']:
             day_obj = datetime.strptime(day_data[0], '%d/%m/%Y')
             is_date_after_from_date = (day_obj.month, day_obj.year) >= (
-                from_date.month, from_date.year)
+                from_date.month,
+                from_date.year,
+            )
             is_date_before_to_date = (day_obj.month, day_obj.year) <= (
-                to_date.month, to_date.year)
+                to_date.month,
+                to_date.year,
+            )
 
             if is_date_after_from_date and is_date_before_to_date:
                 is_day_after_from_date = (day_obj.day, day_obj.month) >= (
-                    from_date.day, from_date.month)
+                    from_date.day,
+                    from_date.month,
+                )
                 is_dat_before_to_date = (day_obj.day, day_obj.month) <= (
-                    to_date.day, to_date.month)
+                    to_date.day,
+                    to_date.month,
+                )
 
                 if is_day_after_from_date and is_dat_before_to_date:
                     day_key = '{}-{}'.format(day_obj.day, day_obj.month)
                     day_hours = '{}'.format(day_data[1]).replace(',', '.')
                     day_hours_data['totalHours'] += float(day_hours)
                     day_hours_data['days'][day_key] = day_hours
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/test_agreements.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/agreements/__tests__/test_agreements.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,96 @@
 import unittest
-from unittest.mock import Mock, patch
 from datetime import datetime
+from unittest.mock import Mock, patch
 
 
 class TestSuite(unittest.TestCase):
     def _create_GSheet_mock():
         service_mock = Mock()
 
         read_gsheet_mock = Mock()
-        read_gsheet_mock.read_gsheet.return_value = {'values': [
-            ['10/09/2022', '0'],
-            ['11/09/2022', '0'],
-            ['12/09/2022', '8'],
-            ['13/09/2022', '8'],
-            ['14/09/2022', '8'],
-            ['15/09/2022', '8'],
-            ['16/09/2022', '5.5'],
-            ['17/09/2022', '0'],
-            ['18/09/2022', '0'],
-            ['19/09/2022', '8'],
-        ]}
-        read_gsheet_mock.get_sheetnames.return_value = {'sheets': [
-            {
-                'properties': {
-                    'title': 'Summary'
-                }
-            },
-            {
-                'properties': {
-                    'title': 'Sheet 1'
-                }
-            },
-            {
-                'properties': {
-                    'title': 'Sheet 2'
-                }
-            }
-        ]}
+        read_gsheet_mock.read_gsheet.return_value = {
+            'values': [
+                ['10/09/2022', '0'],
+                ['11/09/2022', '0'],
+                ['12/09/2022', '8'],
+                ['13/09/2022', '8'],
+                ['14/09/2022', '8'],
+                ['15/09/2022', '8'],
+                ['16/09/2022', '5.5'],
+                ['17/09/2022', '0'],
+                ['18/09/2022', '0'],
+                ['19/09/2022', '8'],
+            ]
+        }
+        read_gsheet_mock.get_sheetnames.return_value = {
+            'sheets': [
+                {'properties': {'title': 'Summary'}},
+                {'properties': {'title': 'Sheet 1'}},
+                {'properties': {'title': 'Sheet 2'}},
+            ]
+        }
         service_mock.return_value = read_gsheet_mock
         return service_mock
 
     @patch('ms_imputedhours_core.agreements.GSheet', new=_create_GSheet_mock())
-    def test_read_gsheet_should_call_google_api_with_credentials_and_correct_params(self):  # noqa: E501
+    def test_read_gsheet_should_call_google_api_with_credentials_and_correct_params(
+        self,
+    ):  # noqa: E501
         expected_result = {
             'totalHours': 45.5,
             'days': {
                 10: '0',
                 11: '0',
                 12: '8',
                 13: '8',
                 14: '8',
                 15: '8',
                 16: '5.5',
                 17: '0',
                 18: '0',
                 19: '8',
-            }}
+            },
+        }
         spreadsheet_id = '111111'
         sheet_name = 'SHEET_NAME_TEST'
         month = 9
         year = 2022
 
         from ms_imputedhours_core.agreements import Agreements
 
         response = Agreements(spreadsheet_id).get_hours_by_month(
-            month, year, sheet_name)
+            month, year, sheet_name
+        )
 
         self.assertEqual(response, expected_result)
 
     @patch('ms_imputedhours_core.agreements.GSheet', new=_create_GSheet_mock())
     def test_get_hours_by_range_return_agreement_hours_by_range(self):
         expected_result = {
             'days': {
-                '12-9': '8', '13-9': '8', '14-9': '8',
-                '15-9': '8', '16-9': '5.5', '17-9': '0'
+                '12-9': '8',
+                '13-9': '8',
+                '14-9': '8',
+                '15-9': '8',
+                '16-9': '5.5',
+                '17-9': '0',
             },
-            'totalHours': 37.5}
+            'totalHours': 37.5,
+        }
         spreadsheet_id = '111111'
         from_date = datetime.strptime('12/09/2022', '%d/%m/%Y')
         to_date = datetime.strptime('17/09/2022', '%d/%m/%Y')
         sheet_name = 'SHEET_NAME_TEST'
 
         from ms_imputedhours_core.agreements import Agreements
 
         response = Agreements(spreadsheet_id).get_hours_by_range(
-            from_date, to_date, sheet_name)
+            from_date, to_date, sheet_name
+        )
 
         self.assertEqual(response, expected_result)
 
     @patch('ms_imputedhours_core.agreements.GSheet', new=_create_GSheet_mock())
     def test_get_all_office_names_returns_all_sheet_names(self):
         expected_result = ['Sheet 1', 'Sheet 2']
         spreadsheet_id = '111111'
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__init__.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 
 HUNDRED_PERCENT = 100
 DEFAULT_FTE = 1.0  # 100 %
 
 
 def get_real_fte(successfactor, employeeFTE, date):
-    """ Calculate employee FTE.
+    """Calculate employee FTE.
     When we want to calculate the FTE of an employee, we do it for a specific
     month since this can change.
 
      Rules:
          - If the date we want to calculate the FTE is from the current
            month into the future, then we will take the FTE value returned
            by the Success factor Bigquery table.
@@ -38,78 +38,90 @@
     if employeeFTE and is_past_date:
         fte = employeeFTE['fte']
 
     return fte
 
 
 def calculate_real_capacity(
-        agreement_hours,
-        hiringdate,
-        end_date,
-        date,
-        to_date,
-        fte,
-        calculate_range=False):
+    agreement_hours,
+    hiringdate,
+    end_date,
+    date,
+    to_date,
+    fte,
+    calculate_range=False,
+):
     def _is_date_before_hired():
         return hiringdate and (
-            (date.year, date.month) < (
-                hiringdate.year, hiringdate.month))
+            (date.year, date.month) < (hiringdate.year, hiringdate.month)
+        )
 
     def _is_date_same_hired():
         return hiringdate and (
-            (date.year, date.month) == (
-                hiringdate.year, hiringdate.month))
+            (date.year, date.month) == (hiringdate.year, hiringdate.month)
+        )
 
     def _is_date_between_hired_and_end_date():
         is_date_before_end_date = not end_date or (
-            (date.year, date.month) < (end_date.year, end_date.month))
-        return is_date_before_end_date and hiringdate and (
-            (date.year, date.month) >= (
-                hiringdate.year, hiringdate.month))
+            (date.year, date.month) < (end_date.year, end_date.month)
+        )
+        return (
+            is_date_before_end_date
+            and hiringdate
+            and (
+                (date.year, date.month) >= (hiringdate.year, hiringdate.month)
+            )
+        )
 
     def _is_date_same_end_date():
         return end_date and (
-            (date.year, date.month) == (end_date.year, end_date.month))
+            (date.year, date.month) == (end_date.year, end_date.month)
+        )
 
     def _is_date_after_end_date():
         return end_date and (
-            (date.year, date.month) > (end_date.year, end_date.month))
+            (date.year, date.month) > (end_date.year, end_date.month)
+        )
 
     real_capacity = agreement_hours.get('totalHours', 0)
 
     if _is_date_before_hired():
         # Months prior to hiring the employee
         real_capacity = 0
     elif calculate_range and _is_date_between_hired_and_end_date():
         # Just when we want to calculate hours by range of date
         real_capacity = 0
         days = agreement_hours.get('days', {})
         for dayMonth, hours in days.items():
             day, month = dayMonth.split('-')
-            is_date_after_from = (int(day), int(
-                month)) >= (date.day, date.month)
+            is_date_after_from = (int(day), int(month)) >= (
+                date.day,
+                date.month,
+            )
             is_date_before_to = (int(day), int(month)) <= (
-                to_date.day, to_date.month)
+                to_date.day,
+                to_date.month,
+            )
             if is_date_after_from and is_date_before_to:
                 real_capacity += float(hours.replace(',', '.'))
     elif _is_date_same_hired():
         # Same month of hiring the employee
         real_capacity = 0
         days = agreement_hours.get('days', {})
 
         for day, hours in days.items():
-            if (int(day) >= hiringdate.day):
+            if int(day) >= hiringdate.day:
                 real_capacity += float(hours.replace(',', '.'))
 
     if _is_date_same_end_date():
         # Same month of the termination of the employment contract
         real_capacity = 0
         days = agreement_hours.get('days', {})
         for day, hours in days.items():
-            if (int(day) <= end_date.day):
+            if int(day) <= end_date.day:
                 real_capacity += float(hours.replace(',', '.'))
 
     elif _is_date_after_end_date():
         # Months after the termination of the employee's contract
         real_capacity = 0
 
     return real_capacity * fte
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/test_employee.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/__tests__/test_employee.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import unittest
-from unittest.mock import Mock
 from datetime import datetime
-from freezegun import freeze_time
+from unittest.mock import Mock
 
-from ms_imputedhours_core.employee import (
-    get_real_fte,
-    calculate_real_capacity,
-)
+from freezegun import freeze_time
 
+from ms_imputedhours_core.employee import calculate_real_capacity, get_real_fte
 
 DEFAULT_AGREEMENT_HOURS = {
     'totalHours': 150.0,
     'days': {
         1: '0',
         2: '8',
         3: '8',
@@ -37,61 +34,69 @@
         23: '8',
         24: '8',
         25: '5.5',
         26: '0',
         27: '0',
         28: '8',
         29: '8',
-        30: '8'
-    }
+        30: '8',
+    },
 }
 
 
 class TestSuite(unittest.TestCase):
     @freeze_time("2022-11-11")
-    def test_get_real_fte_returns_successfactor_fte_when_date_is_not_future_and_employee_has_not_fte(self):  # noqa: E501
+    def test_get_real_fte_returns_successfactor_fte_when_date_is_not_future_and_employee_has_not_fte(
+        self,
+    ):  # noqa: E501
         expected_result = 1.0  # 1.0 === 100%
         successfactor_data = {'FTE': 100}
         employeeFTE = {}
         date = Mock()
         date.year = 2021
         date.month = 10
 
         result = get_real_fte(successfactor_data, employeeFTE, date)
 
         self.assertEqual(result, expected_result)
 
     @freeze_time("2022-11-11")
-    def test_get_real_fte_returns_employee_fte_when_date_is_not_future_and_employee_has_fte(self):  # noqa: E501
+    def test_get_real_fte_returns_employee_fte_when_date_is_not_future_and_employee_has_fte(
+        self,
+    ):  # noqa: E501
         expected_result = 0.5  # 0.5 === 50%
         successfactor_data = {'FTE': 100}
         employeeFTE = {'fte': 0.5}
         date = Mock()
         date.year = 2021
         date.month = 10
 
         result = get_real_fte(successfactor_data, employeeFTE, date)
 
         self.assertEqual(result, expected_result)
 
     @freeze_time("2021-11-11")
-    def test_get_real_fte_returns_successfactor_fte_when_date_is_for_future(self):  # noqa: E501
+    def test_get_real_fte_returns_successfactor_fte_when_date_is_for_future(
+        self,
+    ):  # noqa: E501
         expected_result = 1  # 100%
         successfactor_data = {'FTE': 100}
         employeeFTE = {'fte': 50}
         date = Mock()
         date.year = 2022
         date.month = 10
 
         result = get_real_fte(successfactor_data, employeeFTE, date)
 
         self.assertEqual(result, expected_result)
 
     @freeze_time("2022-11-11")
-    def test_calculate_real_capacity_return_full_capacity_when_is_normal_month(self):  # noqa: E501
+    def test_calculate_real_capacity_return_full_capacity_when_is_normal_month(
+        self,
+    ):  # noqa: E501
         """
         A normal month is a definition for a month where the employee
         will work 100% of the hours of his agreement, and does not
         coincide with any special date as the end or start
         of the employment contract.
         """
         expected_result = 150.0
@@ -111,15 +116,17 @@
             fte,
             calculate_range,
         )
 
         self.assertEqual(result, expected_result)
 
     @freeze_time("2022-11-11")
-    def test_calculate_real_capacity_return_half_capacity_when_is_normal_month_and_fte_zero_point_five(self):  # noqa: E501
+    def test_calculate_real_capacity_return_half_capacity_when_is_normal_month_and_fte_zero_point_five(
+        self,
+    ):  # noqa: E501
         """
         A normal month is a definition for a month where the employee
         will work 100% of the hours of his agreement, and does not
         coincide with any special date as the end or start
         of the employment contract.
         """
         expected_result = 75.0
@@ -139,15 +146,17 @@
             fte,
             calculate_range,
         )
 
         self.assertEqual(result, expected_result)
 
     @freeze_time("2022-11-11")
-    def test_calculate_real_capacity_return_zero_when_date_is_before_hired(self):  # noqa: E501
+    def test_calculate_real_capacity_return_zero_when_date_is_before_hired(
+        self,
+    ):  # noqa: E501
         """
         A normal month is a definition for a month where the employee
         will work 100% of the hours of his agreement, and does not
         coincide with any special date as the end or start
         of the employment contract.
         """
         expected_result = 0.0
@@ -167,15 +176,17 @@
             fte,
             calculate_range,
         )
 
         self.assertEqual(result, expected_result)
 
     @freeze_time("2022-11-11")
-    def test_calculate_real_capacity_return_only_work_days_when_employee_has_end_date(self):  # noqa: E501
+    def test_calculate_real_capacity_return_only_work_days_when_employee_has_end_date(
+        self,
+    ):  # noqa: E501
         """
         A normal month is a definition for a month where the employee
         will work 100% of the hours of his agreement, and does not
         coincide with any special date as the end or start
         of the employment contract.
         """
         expected_result = 33.5
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__init__.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ms_imputedhours_core.agreements import Agreements
-from ms_imputedhours_core.employee import get_real_fte, calculate_real_capacity
-from ms_imputedhours_core.office import get_real_office_name
+from ms_imputedhours_core.employee import calculate_real_capacity, get_real_fte
 from ms_imputedhours_core.employee.data.bigquery import (
-    get_successfactor_all_data,
     get_all_data,
     get_all_data_by_dates,
     get_all_employee_capacity,
     get_imputed_hours,
     get_out_date_imputations,
+    get_successfactor_all_data,
 )
 from ms_imputedhours_core.employee.data.helpers.alert import (
     should_exclude_employee,
 )
 from ms_imputedhours_core.employee.data.transformers.hours import (
-    transform_all_capacities,
-    transform_successfactor_all_data,
     group_task_by_email,
     group_task_by_outdated,
+    transform_all_capacities,
+    transform_successfactor_all_data,
 )
+from ms_imputedhours_core.office import get_real_office_name
 
 AGREEMENTS_SPREADSHEET_ID = '1gMQ30Sl0QHhocTQgbYpWvS6DarhcRIeBIANW8FYLTTQ'
 AWAIT_FOR_GOOLE_API_BACK_PRESSURE = 5
 EMPTY_SUCCESSFACTOR_DATA = {
     'office_name': '',
     'FTE': 0,
     'hiring_date': None,
@@ -36,41 +36,49 @@
     'successfactor_data': EMPTY_SUCCESSFACTOR_DATA,
 }
 GOOGLE_API_MAX_REQUESTS_PER_SEG = 60
 
 
 def get_all_employees_monthly_data_by_office(date, office_name):
     data = {}
-    agreement_hours = Agreements(AGREEMENTS_SPREADSHEET_ID)\
-        .get_hours_by_month(date.month, date.year, office_name)
+    agreement_hours = Agreements(AGREEMENTS_SPREADSHEET_ID).get_hours_by_month(
+        date.month, date.year, office_name
+    )
     successfactor_all_data = transform_successfactor_all_data(
-        get_successfactor_all_data(office_name))
+        get_successfactor_all_data(office_name)
+    )
     if successfactor_all_data:
         office_emails = successfactor_all_data.keys()
         current_month_data = group_task_by_email(
-            get_all_data(date, office_emails))
+            get_all_data(date, office_emails)
+        )
         all_employee_ftes = transform_all_capacities(
-            get_all_employee_capacity(date.month, date.year))
+            get_all_employee_capacity(date.month, date.year)
+        )
 
         for email in office_emails:
             successfactor_data = successfactor_all_data.get(
-                email, EMPTY_SUCCESSFACTOR_DATA)
+                email, EMPTY_SUCCESSFACTOR_DATA
+            )
 
             if should_exclude_employee(
-                    email,
-                    date,
-                    successfactor_data['hiring_date'],
-                    successfactor_data['enddate']):
+                email,
+                date,
+                successfactor_data['hiring_date'],
+                successfactor_data['enddate'],
+            ):
                 continue
 
             office_name = get_real_office_name(
-                successfactor_data.get('office_name'))
+                successfactor_data.get('office_name')
+            )
 
-            fte = get_real_fte(successfactor_data,
-                               all_employee_ftes.get(email), date)
+            fte = get_real_fte(
+                successfactor_data, all_employee_ftes.get(email), date
+            )
 
             real_capacity = calculate_real_capacity(
                 agreement_hours,
                 successfactor_data.get('hiring_date'),
                 successfactor_data.get('enddate'),
                 date,
                 date,
@@ -80,16 +88,16 @@
             # Updating fte value
             successfactor_data['FTE'] = fte
 
             if email not in data.keys():
                 data[email] = {
                     'data': {
                         'totalTimeSpent': current_month_data.get(
-                            email,
-                            {}).get('totalHours', 0)
+                            email, {}
+                        ).get('totalHours', 0)
                     },
                     'agreementHours': {
                         'totalHours': agreement_hours.get('totalHours', 0),
                         'realcapacity': real_capacity,
                     },
                     'successfactor_data': successfactor_data,
                     'yearSelected': date.year,
@@ -97,89 +105,106 @@
                 }
 
     return data
 
 
 def get_all_employee_data_by_range(from_date, to_date, office_name):
     employees_data = {}
-    agreement_hours = Agreements(AGREEMENTS_SPREADSHEET_ID)\
-        .get_hours_by_range(from_date, to_date, office_name)
+    agreement_hours = Agreements(AGREEMENTS_SPREADSHEET_ID).get_hours_by_range(
+        from_date, to_date, office_name
+    )
     successfactor_all_data = transform_successfactor_all_data(
-        get_successfactor_all_data(office_name))
+        get_successfactor_all_data(office_name)
+    )
     office_emails = successfactor_all_data.keys()
     current_month_data = group_task_by_email(
-        get_all_data_by_dates(from_date, to_date,  office_emails))
+        get_all_data_by_dates(from_date, to_date, office_emails)
+    )
     all_employee_ftes = transform_all_capacities(
-        get_all_employee_capacity(from_date.month, from_date.year))
+        get_all_employee_capacity(from_date.month, from_date.year)
+    )
 
     for email in office_emails:
         successfactor_data = successfactor_all_data.get(
-            email, EMPTY_SUCCESSFACTOR_DATA)
+            email, EMPTY_SUCCESSFACTOR_DATA
+        )
 
         if should_exclude_employee(
-                email,
-                from_date,
-                successfactor_data['hiring_date'],
-                successfactor_data['enddate']):
+            email,
+            from_date,
+            successfactor_data['hiring_date'],
+            successfactor_data['enddate'],
+        ):
             continue
 
         employee_fte = get_real_fte(
-            successfactor_data, all_employee_ftes.get(email), from_date)
-        employee_current_capacity = current_month_data.get(
-            email, EMPTY_AGREEMENT_HOURS_DATA)['totalHours'] / 3600
+            successfactor_data, all_employee_ftes.get(email), from_date
+        )
+        employee_current_capacity = (
+            current_month_data.get(email, EMPTY_AGREEMENT_HOURS_DATA)[
+                'totalHours'
+            ]
+            / 3600
+        )
         employee_real_capacity = calculate_real_capacity(
             agreement_hours,
             successfactor_data.get('hiring_date'),
             successfactor_data.get('enddate'),
             from_date,
             to_date,
             employee_fte,
-            calculate_range=True
+            calculate_range=True,
         )
 
         capacity_percentage = 0
         if employee_real_capacity == 0:
             capacity_percentage = 100
         else:
             capacity_percentage = round(
-                (employee_current_capacity * 100) / employee_real_capacity, 2)
+                (employee_current_capacity * 100) / employee_real_capacity, 2
+            )
 
         employees_data[email] = {
             'real_capacity': employee_real_capacity,
             'current_capacity': employee_current_capacity,
             'current_percentage_hours_imputed': capacity_percentage,
             'supervisor': successfactor_data['supervisor'],
             'name': successfactor_data['name'],
         }
 
     return employees_data
 
 
 def get_all_imputations_per_day(from_date, to_date):
     current_month_data = group_task_by_email(
-        get_imputed_hours(from_date, to_date))
+        get_imputed_hours(from_date, to_date)
+    )
 
     return current_month_data
 
 
 def get_all_out_date_imputations(first_day, last_day, office_name):
     successfactor_all_data = transform_successfactor_all_data(
-        get_successfactor_all_data(office_name))
+        get_successfactor_all_data(office_name)
+    )
     current_data = group_task_by_outdated(
-        get_out_date_imputations(first_day, last_day))
+        get_out_date_imputations(first_day, last_day)
+    )
     employees_data = {}
     for email in successfactor_all_data.keys():
         successfactor_data = successfactor_all_data.get(
-            email, EMPTY_SUCCESSFACTOR_DATA)
+            email, EMPTY_SUCCESSFACTOR_DATA
+        )
 
         if should_exclude_employee(
-                email,
-                first_day,
-                successfactor_data['hiring_date'],
-                successfactor_data['enddate']):
+            email,
+            first_day,
+            successfactor_data['hiring_date'],
+            successfactor_data['enddate'],
+        ):
             continue
 
         if current_data.get(email):
             supervisor_email = successfactor_data['supervisor']
             if supervisor_email not in employees_data.keys():
                 employees_data[supervisor_email] = {}
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/test_data.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/__tests__/test_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
+from datetime import date, datetime
 from unittest.mock import Mock, patch
-from datetime import datetime, date
+
 from freezegun import freeze_time
 
 from ms_imputedhours_core.employee.data import get_all_employee_data_by_range
 
-
 DEFAULT_AGREEMENT_HOURS = {
     'totalHours': 142.0,
     'days': {
         '1-4': '0',
         '2-4': '0',
         '3-4': '8',
         '4-4': '5.5',
@@ -34,23 +34,25 @@
         '23-4': '8',
         '24-4': '8',
         '25-4': '5.5',
         '26-4': '0',
         '27-4': '0',
         '28-4': '8',
         '29-4': '8',
-        '30-4': '8'
-    }
+        '30-4': '8',
+    },
 }
 
 
 class TestSuite(unittest.TestCase):
     def _create_Agreements_mock(self, Agreements):
         get_hours_by_range_mock = Mock()
-        get_hours_by_range_mock.get_hours_by_range.return_value = DEFAULT_AGREEMENT_HOURS  # noqa: E501
+        get_hours_by_range_mock.get_hours_by_range.return_value = (
+            DEFAULT_AGREEMENT_HOURS  # noqa: E501
+        )
 
         Agreements.return_value = get_hours_by_range_mock
         return Agreements
 
     def _create_successfactor_all_data_mock(self, get_successfactor_all_data):
         get_successfactor_all_data.return_value = [
             {
@@ -88,15 +90,15 @@
                 'hiringdate': date(2022, 4, 1),
                 'internshipdate': None,
                 'fte': '50',
                 'supervisor': 'employee2@makingscience.com',
                 'office': 'Madrid - Ing',
                 'name': 'Employee4',
                 'lastname': 'Doe',
-            }
+            },
         ]
         return get_successfactor_all_data
 
     def _create_get_all_data_by_dates_mock(self, get_all_data_by_dates):
         get_all_data_by_dates.return_value = [
             {
                 'timeSpent': 28800,
@@ -118,15 +120,17 @@
                 'authorEmail': 'employee4@makingscience.com',
                 'started': date(2022, 4, 16),
             },
         ]
 
         return get_all_data_by_dates
 
-    def _create_get_all_employee_capacity_mock(self, get_all_employee_capacity):  # noqa: E501
+    def _create_get_all_employee_capacity_mock(
+        self, get_all_employee_capacity
+    ):  # noqa: E501
         get_all_employee_capacity.return_value = [
             {
                 'email': 'employee1@makingscience.com',
                 'fte': 1.0,
             },
             {
                 'email': 'employee2@makingscience.com',
@@ -149,45 +153,50 @@
         Agreements,
         get_successfactor_all_data,
         get_all_data_by_dates,
         get_all_employee_capacity,
     ):
         Agreements = self._create_Agreements_mock(Agreements)
         get_successfactor_all_data = self._create_successfactor_all_data_mock(
-            get_successfactor_all_data)
+            get_successfactor_all_data
+        )
         get_all_data_by_dates = self._create_get_all_data_by_dates_mock(
-            get_all_data_by_dates)
-        get_all_employee_capacity = self._create_get_all_employee_capacity_mock(  # noqa: E501
-            get_all_employee_capacity)
+            get_all_data_by_dates
+        )
+        get_all_employee_capacity = (
+            self._create_get_all_employee_capacity_mock(  # noqa: E501
+                get_all_employee_capacity
+            )
+        )
 
         from_date = datetime.strptime('2022-04-1', '%Y-%m-%d').date()
         to_date = datetime.strptime('2022-04-2', '%Y-%m-%d').date()
         office_name = 'Madrid - ing'
         expected_result = {
             'employee1@makingscience.com': {
                 'real_capacity': 0.0,
                 'current_capacity': 16.0,
                 'current_percentage_hours_imputed': 100,
                 'supervisor': 'employee2@makingscience.com',
-                'name': 'Employee1 Doe'
+                'name': 'Employee1 Doe',
             },
             'employee2@makingscience.com': {
                 'real_capacity': 0.0,
                 'current_capacity': 0.0,
                 'current_percentage_hours_imputed': 100,
                 'supervisor': 'employee20@makingscience.com',
-                'name': 'Employee2 Doe'
+                'name': 'Employee2 Doe',
             },
             'employee4@makingscience.com': {
                 'real_capacity': 0.0,
                 'current_capacity': 16.0,
                 'current_percentage_hours_imputed': 100,
                 'supervisor': 'employee2@makingscience.com',
-                'name': 'Employee4 Doe'
-            }
+                'name': 'Employee4 Doe',
+            },
         }
         result = get_all_employee_data_by_range(
             from_date,
             to_date,
             office_name,
         )
 
@@ -203,44 +212,49 @@
         Agreements,
         get_successfactor_all_data,
         get_all_data_by_dates,
         get_all_employee_capacity,
     ):
         Agreements = self._create_Agreements_mock(Agreements)
         get_successfactor_all_data = self._create_successfactor_all_data_mock(
-            get_successfactor_all_data)
+            get_successfactor_all_data
+        )
         get_all_data_by_dates = self._create_get_all_data_by_dates_mock(
-            get_all_data_by_dates)
-        get_all_employee_capacity = self._create_get_all_employee_capacity_mock(  # noqa: E501
-            get_all_employee_capacity)
+            get_all_data_by_dates
+        )
+        get_all_employee_capacity = (
+            self._create_get_all_employee_capacity_mock(  # noqa: E501
+                get_all_employee_capacity
+            )
+        )
         from_date = datetime.strptime('2022-04-1', '%Y-%m-%d').date()
         to_date = datetime.strptime('2022-04-15', '%Y-%m-%d').date()
         office_name = 'Madrid - ing'
         expected_result = {
             'employee1@makingscience.com': {
                 'real_capacity': 59.0,
                 'current_capacity': 16.0,
                 'current_percentage_hours_imputed': 27.12,
                 'supervisor': 'employee2@makingscience.com',
-                'name': 'Employee1 Doe'
+                'name': 'Employee1 Doe',
             },
             'employee2@makingscience.com': {
                 'real_capacity': 59.0,
                 'current_capacity': 0.0,
                 'current_percentage_hours_imputed': 0.0,
                 'supervisor': 'employee20@makingscience.com',
-                'name': 'Employee2 Doe'
+                'name': 'Employee2 Doe',
             },
             'employee4@makingscience.com': {
                 'real_capacity': 29.5,
                 'current_capacity': 16.0,
                 'current_percentage_hours_imputed': 54.24,
                 'supervisor': 'employee2@makingscience.com',
-                'name': 'Employee4 Doe'
-            }
+                'name': 'Employee4 Doe',
+            },
         }
         result = get_all_employee_data_by_range(
             from_date,
             to_date,
             office_name,
         )
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/bigquery.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 import os
+
 from gc_google_services_api.bigquery import execute_query
 
-from ms_imputedhours_core.employee.data.helpers.bigquery import BigqueryUpdateQueryBuilder
-from ms_imputedhours_core.employee.data.helpers.dates import get_first_day, get_last_day
+from ms_imputedhours_core.employee.data.helpers.bigquery import (
+    BigqueryUpdateQueryBuilder,
+)
+from ms_imputedhours_core.employee.data.helpers.dates import (
+    get_first_day,
+    get_last_day,
+)
 
 BIGQUERY_JIRA_DATA_TYPES = os.getenv(
-    'BIGQUERY_JIRA_DATA_TYPES_TABLE', 'ms--tiber-happeo--pro--aa82.jiradataintegration.jiradatatypes')
+    'BIGQUERY_JIRA_DATA_TYPES_TABLE',
+    'ms--tiber-happeo--pro--aa82.jiradataintegration.jiradatatypes',
+)
 BIGQUERY_SUCCESS_FACTOR = os.getenv(
-    'BIGQUERY_SUCCESS_FACTOR_TABLE', 'ms--tiber-happeo--pro--aa82.jiradataintegration.dataemployees')
+    'BIGQUERY_SUCCESS_FACTOR_TABLE',
+    'ms--tiber-happeo--pro--aa82.jiradataintegration.dataemployees',
+)
 BIGQUERY_EMPLOYEE_CAPACITY = os.getenv(
-    'BIGQUERY_EMPLOYEE_CAPACITY_TABLE', 'ms--tiber-happeo--pro--aa82.jiradataintegration.employeecapacity')
+    'BIGQUERY_EMPLOYEE_CAPACITY_TABLE',
+    'ms--tiber-happeo--pro--aa82.jiradataintegration.employeecapacity',
+)
 
 QUERY_HOURS_IMPUTED_OFFICE_EMPLOYEES = """
     SELECT
         *
     FROM
         `{BIGQUERY_JIRA_DATA_TYPES}`
     WHERE
@@ -136,75 +148,78 @@
 
 MS_FOR_HOUR = 3600000
 
 
 def get_all_data(date, office_emails):
     from_date = get_first_day(date).strftime("%Y-%m-%d")
     to_date = get_last_day(date).strftime("%Y-%m-%d")
-    email_query_list = ",".join(["'{}'".format(email)
-                                for email in office_emails])
+    email_query_list = ",".join(
+        ["'{}'".format(email) for email in office_emails]
+    )
     query = QUERY_HOURS_IMPUTED_OFFICE_EMPLOYEES.format(
         from_date=from_date,
         to_date=to_date,
         emails=email_query_list,
-        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES
+        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES,
     )
 
     return execute_query(query, error_value=[])
 
 
 def get_imputed_hours(from_date, to_date):
     from_date = from_date.strftime("%Y-%m-%d")
     to_date = to_date.strftime("%Y-%m-%d")
     query = QUERY_HOURS_IMPUTED_ALL_EMPLOYEES.format(
         from_date=from_date,
         to_date=to_date,
-        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES
+        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES,
     )
 
     return execute_query(query, error_value=[])
 
 
 def get_all_data_by_dates(from_date, to_date, office_emails):
-    email_query_list = ",".join(["'{}'".format(email)
-                                for email in office_emails])
+    email_query_list = ",".join(
+        ["'{}'".format(email) for email in office_emails]
+    )
     query = QUERY_HOURS_IMPUTED_OFFICE_EMPLOYEES.format(
         from_date=from_date,
         to_date=to_date,
         emails=email_query_list,
-        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES
+        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES,
     )
 
     return execute_query(query, error_value=[])
 
 
 def get_data_from_email(email, date):
     from_date = get_first_day(date).strftime("%Y-%m-%d")
     to_date = get_last_day(date).strftime("%Y-%m-%d")
     query = QUERY_HOURS_IMPUTED.format(
         from_date=from_date,
         to_date=to_date,
         email=email,
-        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES)
+        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES,
+    )
 
     return execute_query(query, error_value=[])
 
 
 def get_successfactor_data(email):
     query = QUERY_SUCCESS_FACTOR.format(
-        email=email,
-        BIGQUERY_SUCCESS_FACTOR=BIGQUERY_SUCCESS_FACTOR)
+        email=email, BIGQUERY_SUCCESS_FACTOR=BIGQUERY_SUCCESS_FACTOR
+    )
 
     return execute_query(query, error_value=[])
 
 
 def get_successfactor_all_data(office_name):
     query = QUERY_SUCCESS_FACTOR_ALL.format(
         BIGQUERY_SUCCESS_FACTOR=BIGQUERY_SUCCESS_FACTOR,
-        office_name=office_name
+        office_name=office_name,
     )
     return execute_query(query, error_value=[])
 
 
 def get_successfactor_all_offices():
     query = QUERY_SUCCESS_FACTOR_ALL_DATA.format(
         BIGQUERY_SUCCESS_FACTOR=BIGQUERY_SUCCESS_FACTOR
@@ -222,20 +237,32 @@
 
 
 def get_employee_capacity(email, year, month):
     query = QUERY_EMPLOYEE_CAPACITY.format(
         email=email,
         year=year,
         month=month,
-        BIGQUERY_EMPLOYEE_CAPACITY=BIGQUERY_EMPLOYEE_CAPACITY)
+        BIGQUERY_EMPLOYEE_CAPACITY=BIGQUERY_EMPLOYEE_CAPACITY,
+    )
 
     return execute_query(query, error_value=[])
 
 
-def register_employee_capacity(email, year, month, hours, office, capacity, realcapacity, fte, hiring_date, enddate):  # noqa: E501
+def register_employee_capacity(
+    email,
+    year,
+    month,
+    hours,
+    office,
+    capacity,
+    realcapacity,
+    fte,
+    hiring_date,
+    enddate,
+):  # noqa: E501
     insert_query_builder = BigqueryUpdateQueryBuilder(
         email,
         year,
         month,
         hours,
         fte,
         office,
@@ -245,26 +272,37 @@
         realcapacity,
     )
     query = insert_query_builder.build_insert()
 
     return execute_query(query, error_value=[])
 
 
-def update_employee_capacity(email, year, month, hours, office, capacity, realcapacity, fte, hiring_date, enddate):  # noqa: E501
+def update_employee_capacity(
+    email,
+    year,
+    month,
+    hours,
+    office,
+    capacity,
+    realcapacity,
+    fte,
+    hiring_date,
+    enddate,
+):  # noqa: E501
     update_query_builder = BigqueryUpdateQueryBuilder(
         email,
         year,
         month,
         hours,
         fte,
         office,
         capacity,
         hiring_date,
         enddate,
-        realcapacity
+        realcapacity,
     )
     query = update_query_builder.build_update()
 
     return execute_query(query, error_value=[])
 
 
 def create_or_update_employee(email, data):
@@ -272,44 +310,47 @@
         capacity_data = {}
         for capacity in employee_capacity:
             capacity_data['fte'] = capacity.get('fte', 0.0)
 
         return capacity_data
 
     successfactor_data = data.pop('successfactor_data')
-    employee_capacity = _get_capacity_data(get_employee_capacity(
-        email,
-        data['yearSelected'],
-        data['monthSelected']))
+    employee_capacity = _get_capacity_data(
+        get_employee_capacity(
+            email, data['yearSelected'], data['monthSelected']
+        )
+    )
     totalTimeSpent = data['data']['totalTimeSpent'] * 1000
 
     if employee_capacity:
         update_employee_capacity(
             email,
             data['yearSelected'],
             data['monthSelected'],
             totalTimeSpent,
             successfactor_data['office_name'],
             data['agreementHours']['totalHours'] * MS_FOR_HOUR,
             data['agreementHours']['realcapacity'] * MS_FOR_HOUR,
             successfactor_data['FTE'],
             successfactor_data.get('hiring_date'),
-            successfactor_data.get('enddate'))
+            successfactor_data.get('enddate'),
+        )
     else:
         register_employee_capacity(
             email,
             data['yearSelected'],
             data['monthSelected'],
             totalTimeSpent,
             successfactor_data['office_name'],
             data['agreementHours']['totalHours'] * MS_FOR_HOUR,
             data['agreementHours']['realcapacity'] * MS_FOR_HOUR,
             successfactor_data['FTE'],
             successfactor_data.get('hiring_date'),
-            successfactor_data.get('enddate'))
+            successfactor_data.get('enddate'),
+        )
 
 
 def create_batch_insert_values(email, data):
     def _get_date_value(date_value):
         if date_value:
             return f"'{date_value}'"
         else:
@@ -347,10 +388,11 @@
     return execute_query(query, error_value=[])
 
 
 def get_out_date_imputations(first_day, last_day):
     query = QUERY_HOURS_IMPUTED_OUT_DATE.format(
         first_day=first_day,
         last_day=last_day,
-        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES)
+        BIGQUERY_JIRA_DATA_TYPES=BIGQUERY_JIRA_DATA_TYPES,
+    )
 
     return execute_query(query, error_value=[])
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,105 +1,129 @@
 import unittest
-from unittest.mock import patch
 from datetime import datetime
+from unittest.mock import patch
 
 from ms_imputedhours_core.employee.data.helpers.alert import (
     should_exclude_employee,
 )
 
 
 class TestSuite(unittest.TestCase):
-    def test_should_exclude_employee_should_return_false_when_employee_hired_date_is_lower_than_date(self):  # noqa: E501
+    def test_should_exclude_employee_should_return_false_when_employee_hired_date_is_lower_than_date(
+        self,
+    ):  # noqa: E501
         date = datetime.strptime('02/28/22 00:00:00', '%m/%d/%y %H:%M:%S')
         hired_date = datetime.strptime(
-            '01/01/22 00:00:00', '%m/%d/%y %H:%M:%S')
+            '01/01/22 00:00:00', '%m/%d/%y %H:%M:%S'
+        )
         end_date = None
         expected_result = False
 
         is_exclude_employee = should_exclude_employee(
             email='test@makingscience.com',
             date=date,
             hired_date=hired_date,
             end_date=end_date,
         )
 
         self.assertEqual(is_exclude_employee, expected_result)
 
-    def test_should_exclude_employee_should_return_true_when_employee_hired_date_is_greater_than_date(self):  # noqa: E501
+    def test_should_exclude_employee_should_return_true_when_employee_hired_date_is_greater_than_date(
+        self,
+    ):  # noqa: E501
         date = datetime.strptime('02/28/22 00:00:00', '%m/%d/%y %H:%M:%S')
         hired_date = datetime.strptime(
-            '05/01/22 00:00:00', '%m/%d/%y %H:%M:%S')
+            '05/01/22 00:00:00', '%m/%d/%y %H:%M:%S'
+        )
         end_date = None
         expected_result = True
 
         is_exclude_employee = should_exclude_employee(
             email='test@makingscience.com',
             date=date,
             hired_date=hired_date,
             end_date=end_date,
         )
 
         self.assertEqual(is_exclude_employee, expected_result)
 
-    def test_should_exclude_employee_should_return_false_when_employee_end_date_is_greater_than_date(self):  # noqa: E501
+    def test_should_exclude_employee_should_return_false_when_employee_end_date_is_greater_than_date(
+        self,
+    ):  # noqa: E501
         date = datetime.strptime('02/28/22 00:00:00', '%m/%d/%y %H:%M:%S')
         hired_date = datetime.strptime(
-            '01/01/21 00:00:00', '%m/%d/%y %H:%M:%S')
+            '01/01/21 00:00:00', '%m/%d/%y %H:%M:%S'
+        )
         end_date = datetime.strptime('05/15/22 00:00:00', '%m/%d/%y %H:%M:%S')
         expected_result = False
 
         is_exclude_employee = should_exclude_employee(
             email='test@makingscience.com',
             date=date,
             hired_date=hired_date,
             end_date=end_date,
         )
 
         self.assertEqual(is_exclude_employee, expected_result)
 
-    def test_should_exclude_employee_should_return_true_when_employee_end_date_is_lower_than_date(self):  # noqa: E501
+    def test_should_exclude_employee_should_return_true_when_employee_end_date_is_lower_than_date(
+        self,
+    ):  # noqa: E501
         date = datetime.strptime('02/28/22 00:00:00', '%m/%d/%y %H:%M:%S')
         hired_date = datetime.strptime(
-            '01/01/21 00:00:00', '%m/%d/%y %H:%M:%S')
+            '01/01/21 00:00:00', '%m/%d/%y %H:%M:%S'
+        )
         end_date = datetime.strptime('01/15/22 00:00:00', '%m/%d/%y %H:%M:%S')
         expected_result = True
 
         is_exclude_employee = should_exclude_employee(
             email='test@makingscience.com',
             date=date,
             hired_date=hired_date,
             end_date=end_date,
         )
 
         self.assertEqual(is_exclude_employee, expected_result)
 
-    @patch('ms_imputedhours_core.employee.data.helpers.alert.EXCLUDE_ALERT_EMAILS', ['test@test.com'])  # noqa: E501
-    def test_should_exclude_employee_should_return_true_when_employee_email_is_excluded(self):  # noqa: E501
+    @patch(
+        'ms_imputedhours_core.employee.data.helpers.alert.EXCLUDE_ALERT_EMAILS',
+        ['test@test.com'],
+    )  # noqa: E501
+    def test_should_exclude_employee_should_return_true_when_employee_email_is_excluded(
+        self,
+    ):  # noqa: E501
         date = datetime.strptime('02/28/22 00:00:00', '%m/%d/%y %H:%M:%S')
         hired_date = datetime.strptime(
-            '01/01/22 00:00:00', '%m/%d/%y %H:%M:%S')
+            '01/01/22 00:00:00', '%m/%d/%y %H:%M:%S'
+        )
         end_date = None
         expected_result = True
 
         from ..alert import should_exclude_employee
 
         is_exclude_employee = should_exclude_employee(
             email='jonathan.rodriguez@makingscience.com',
             date=date,
             hired_date=hired_date,
             end_date=end_date,
         )
 
         self.assertEqual(is_exclude_employee, expected_result)
 
-    @patch('ms_imputedhours_core.employee.data.helpers.alert.EXCLUDE_ALERT_EMAILS', ['test@test.com'])  # noqa: E501
-    def test_should_exclude_employee_should_return_true_when_employee_email_not_from_ms(self):  # noqa: E501
+    @patch(
+        'ms_imputedhours_core.employee.data.helpers.alert.EXCLUDE_ALERT_EMAILS',
+        ['test@test.com'],
+    )  # noqa: E501
+    def test_should_exclude_employee_should_return_true_when_employee_email_not_from_ms(
+        self,
+    ):  # noqa: E501
         date = datetime.strptime('02/28/22 00:00:00', '%m/%d/%y %H:%M:%S')
         hired_date = datetime.strptime(
-            '01/01/21 00:00:00', '%m/%d/%y %H:%M:%S')
+            '01/01/21 00:00:00', '%m/%d/%y %H:%M:%S'
+        )
         end_date = datetime.strptime('05/15/22 00:00:00', '%m/%d/%y %H:%M:%S')
         expected_result = True
 
         is_exclude_employee = should_exclude_employee(
             email='test@test.com',
             date=date,
             hired_date=hired_date,
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,16 @@
         self.year = 2022
         self.month = 1
         self.jira_hours = 40
         self.fte = 100
         self.office = 'Madrid'
         self.capacity = 80
         self.hiring_date = datetime.strptime(
-            '02/01/22 00:00:00', '%m/%d/%y %H:%M:%S')
+            '02/01/22 00:00:00', '%m/%d/%y %H:%M:%S'
+        )
         self.enddate = None
         self.realcapacity = 80
 
         self.bigquery_builder = BigqueryUpdateQueryBuilder(
             email=self.email,
             year=self.year,
             month=self.month,
@@ -27,91 +28,115 @@
             office=self.office,
             capacity=self.capacity,
             hiring_date=self.hiring_date,
             enddate=self.enddate,
             realcapacity=self.realcapacity,
         )
 
-    def test_enddate_update_query_should_return_empty_string_when_enddate_is_None(self):
+    def test_enddate_update_query_should_return_empty_string_when_enddate_is_None(
+        self,
+    ):
         expected_enddate_query = ''
         self.assertEqual(
-            self.bigquery_builder._set_enddate_for_update(), expected_enddate_query)
+            self.bigquery_builder._set_enddate_for_update(),
+            expected_enddate_query,
+        )
 
-    def test_hiring_date_update_query_should_return_date_query_when_hiring_date(self):
+    def test_hiring_date_update_query_should_return_date_query_when_hiring_date(
+        self,
+    ):
         expected_hiring_query = ", startdate='2022-02-01 00:00:00'"
         self.assertEqual(
-            self.bigquery_builder._set_startdate_for_update(), expected_hiring_query)
+            self.bigquery_builder._set_startdate_for_update(),
+            expected_hiring_query,
+        )
 
     def test__set_startdate_insert_should_return_startdate_value(self):
         expected_hiring_query = ",'2022-02-01 00:00:00'"
         self.assertEqual(
-            self.bigquery_builder._set_startdate_insert(), expected_hiring_query)
+            self.bigquery_builder._set_startdate_insert(),
+            expected_hiring_query,
+        )
 
     def test__set_enddate_insert_should_return_enddate_value(self):
         expected_enddate_query = ""
         self.assertEqual(
-            self.bigquery_builder._set_enddate_insert(), expected_enddate_query)
+            self.bigquery_builder._set_enddate_insert(), expected_enddate_query
+        )
 
     def test_build_update_shouldd_return_update_capacity_table_query(self):
         expected_query = """
             UPDATE `ms--tiber-happeo--pro--aa82.jiradataintegration.employeecapacity` SET
                 email='test@test.com',
                 month='1',
                 year='2022',
                 fte=100,
                 office='Madrid',
                 jira=40,
                 capacity=80,
                 realcapacity=80
                 , startdate='2022-02-01 00:00:00'
-                
+
             WHERE
                 email='test@test.com' AND
                 month='1' AND
                 year='2022'
         """
-
-        self.assertMultiLineEqual(
-            self.bigquery_builder.build_update(),
-            expected_query,
-        )
-
-    def test_build_insert_shouldd_return_insert_capacity_table_query_without_enddate(self):  # noqa: E501
+        expected_lines = [
+            line.rstrip() for line in expected_query.splitlines()
+        ]
+        actual_lines = [
+            line.rstrip()
+            for line in self.bigquery_builder.build_update().splitlines()
+        ]
+
+        self.assertEqual(expected_lines, actual_lines)
+
+    def test_build_insert_shouldd_return_insert_capacity_table_query_without_enddate(
+        self,
+    ):  # noqa: E501
         expected_query = """
             INSERT INTO `ms--tiber-happeo--pro--aa82.jiradataintegration.employeecapacity` (email, month, year, fte, office, jira, capacity, realcapacity, startdate) VALUES (
                 'test@test.com',
                 '1',
                 '2022',
                 100,
                 'Madrid',
                 40,
                 80,
                 80
                 ,'2022-02-01 00:00:00'
-                
+
             )
         """
-
-        self.assertMultiLineEqual(
-            self.bigquery_builder.build_insert(),
-            expected_query,
-        )
-
-    def test_build_insert_shouldd_return_insert_capacity_table_query_with_enddate(self):  # noqa: E501
+        expected_lines = [
+            line.rstrip() for line in expected_query.splitlines()
+        ]
+        actual_lines = [
+            line.rstrip()
+            for line in self.bigquery_builder.build_insert().splitlines()
+        ]
+
+        self.assertEqual(expected_lines, actual_lines)
+
+    def test_build_insert_shouldd_return_insert_capacity_table_query_with_enddate(
+        self,
+    ):  # noqa: E501
         self.bigquery_builder = BigqueryUpdateQueryBuilder(
             email=self.email,
             year=self.year,
             month=self.month,
             jira=self.jira_hours,
             fte=self.fte,
             office=self.office,
             capacity=self.capacity,
             hiring_date=self.hiring_date,
             enddate=datetime.strptime(
-                '02/01/23 00:00:00', '%m/%d/%y %H:%M:%S'),
+                '02/01/23 00:00:00', '%m/%d/%y %H:%M:%S'
+            ),
             realcapacity=self.realcapacity,
         )
         expected_query = """
             INSERT INTO `ms--tiber-happeo--pro--aa82.jiradataintegration.employeecapacity` (email, month, year, fte, office, jira, capacity, realcapacity, startdate, enddate) VALUES (
                 'test@test.com',
                 '1',
                 '2022',
@@ -126,26 +151,29 @@
         """
 
         self.assertMultiLineEqual(
             self.bigquery_builder.build_insert(),
             expected_query,
         )
 
-    def test_build_insert_should_return_insert_capacity_table_query(self):  # noqa: E501
+    def test_build_insert_should_return_insert_capacity_table_query(
+        self,
+    ):  # noqa: E501
         self.bigquery_builder = BigqueryUpdateQueryBuilder(
             email=self.email,
             year=self.year,
             month=self.month,
             jira=self.jira_hours,
             fte=self.fte,
             office=self.office,
             capacity=self.capacity,
             hiring_date=self.hiring_date,
             enddate=datetime.strptime(
-                '02/01/23 00:00:00', '%m/%d/%y %H:%M:%S'),
+                '02/01/23 00:00:00', '%m/%d/%y %H:%M:%S'
+            ),
             realcapacity=self.realcapacity,
         )
         expected_query = """
             INSERT INTO `ms--tiber-happeo--pro--aa82.jiradataintegration.employeecapacity` (email, month, year, fte, office, jira, capacity, realcapacity, startdate, enddate) VALUES (
                 'test@test.com',
                 '1',
                 '2022',
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import unittest
 import datetime
+import unittest
 
 from ..dates import get_first_day, get_last_day
 
 
 class TestSuite(unittest.TestCase):
     def test_get_first_day_should_return_first_date_from_a_date(self):
         year = 2022
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/bigquery.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/helpers/bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from datetime import datetime
 
-
 BIGQUERY_EMPLOYEE_CAPACITY = os.getenv(
     'BIGQUERY_EMPLOYEE_CAPACITY_TABLE',
-    'ms--tiber-happeo--pro--aa82.jiradataintegration.employeecapacity')
+    'ms--tiber-happeo--pro--aa82.jiradataintegration.employeecapacity',
+)
 
 
 class BigqueryUpdateQueryBuilder(object):
     def __init__(
         self,
         email,
         year,
@@ -70,15 +70,15 @@
             jira=self.jira,
             fte=self.fte,
             office=self.office,
             capacity=self.capacity,
             hiring_date=self._set_startdate_for_update(),
             realcapacity=self.realcapacity,
             enddate=self._set_enddate_for_update(),
-            BIGQUERY_EMPLOYEE_CAPACITY=BIGQUERY_EMPLOYEE_CAPACITY
+            BIGQUERY_EMPLOYEE_CAPACITY=BIGQUERY_EMPLOYEE_CAPACITY,
         )
 
     def _get_insert_columns(self):
         basic_columns = 'email, month, year, fte, office, jira, capacity, realcapacity'  # noqa: E501
 
         if self.hiring_date:
             basic_columns += ', startdate'
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/hours.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/employee/data/transformers/hours.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,40 +28,42 @@
         fte = data.get('fte', EMPTY_FTE) or EMPTY_FTE  # For null values
         data_json[email]['supervisor'] = data.get('supervisor', '')
         data_json[email]['office_name'] = data.get('office', '')
         data_json[email]['FTE'] = float(fte.replace(',', '.'))
         data_json[email]['hiring_date'] = hiringdate
         data_json[email]['enddate'] = enddate
         data_json[email]['name'] = "{} {}".format(
-            data.get('name', ''), data.get('lastname', ''))
+            data.get('name', ''), data.get('lastname', '')
+        )
 
     return data_json
 
 
 def transform_all_capacities(capacities):
     data_json = {}
 
     for data in capacities:
         email = data.get('email')
         if email not in data_json:
-            data_json[email] = {
-                'fte': data.get('fte')
-            }
+            data_json[email] = {'fte': data.get('fte')}
 
     return data_json
 
 
 def group_task_by_email(month_data, group_by_full_date=False):
     data_by_email = {}
     for task in month_data:
         taskTimeSpent = task.get('timeSpent', 0)
         taskEmail = task.get('authorEmail')
         taskStarted = task.get('started')
-        grouped_date = taskStarted.strftime(
-            '%Y-%m-%d') if group_by_full_date else taskStarted.day
+        grouped_date = (
+            taskStarted.strftime('%Y-%m-%d')
+            if group_by_full_date
+            else taskStarted.day
+        )
         if taskEmail not in data_by_email.keys():
             data_by_email[taskEmail] = {'totalHours': 0, 'days': {}}
 
         if grouped_date not in data_by_email[taskEmail]['days']:
             data_by_email[taskEmail]['days'][grouped_date] = 0
 
         data_by_email[taskEmail]['totalHours'] += taskTimeSpent
@@ -81,20 +83,37 @@
 
         if taskEmail not in data_by_email.keys():
             data_by_email[taskEmail] = {'totalHours': 0, 'days': {}}
 
         if taskCreated not in data_by_email[taskEmail]['days']:
             data_by_email[taskEmail]['days'][taskCreated] = {
                 'total': 0,
-                'tasks': {}}
-
-        if taskIssueKey not in data_by_email[taskEmail]['days'][taskCreated]['tasks']:  # noqa: E501
-            data_by_email[taskEmail]['days'][taskCreated]['tasks'][taskIssueKey] = {}  # noqa: E501
+                'tasks': {},
+            }
 
-        if taskStarted not in data_by_email[taskEmail]['days'][taskCreated]['tasks'][taskIssueKey]:  # noqa: E501
-            data_by_email[taskEmail]['days'][taskCreated]['tasks'][taskIssueKey][taskStarted] = 0  # noqa: E501
+        if (
+            taskIssueKey
+            not in data_by_email[taskEmail]['days'][taskCreated]['tasks']
+        ):  # noqa: E501
+            data_by_email[taskEmail]['days'][taskCreated]['tasks'][
+                taskIssueKey
+            ] = {}  # noqa: E501
+
+        if (
+            taskStarted
+            not in data_by_email[taskEmail]['days'][taskCreated]['tasks'][
+                taskIssueKey
+            ]
+        ):  # noqa: E501
+            data_by_email[taskEmail]['days'][taskCreated]['tasks'][
+                taskIssueKey
+            ][
+                taskStarted
+            ] = 0  # noqa: E501
 
         data_by_email[taskEmail]['totalHours'] += taskTimeSpent
         data_by_email[taskEmail]['days'][taskCreated]['total'] += taskTimeSpent
-        data_by_email[taskEmail]['days'][taskCreated]['tasks'][taskIssueKey][taskStarted] += taskTimeSpent  # noqa: E501
+        data_by_email[taskEmail]['days'][taskCreated]['tasks'][taskIssueKey][
+            taskStarted
+        ] += taskTimeSpent  # noqa: E501
 
     return data_by_email
```

### Comparing `ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/test_office.py` & `ms_imputedhours_core-0.3.4/ms_imputedhours_core/office/__tests__/test_office.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import unittest
 
 from ms_imputedhours_core.office import get_real_office_name
 
 
 class TestSuite(unittest.TestCase):
-    def test_get_real_office_name_return_same_param_when_office_name_is_not_mapped(self):  # noqa: E501
+    def test_get_real_office_name_return_same_param_when_office_name_is_not_mapped(
+        self,
+    ):  # noqa: E501
         expected_result = 'Valencia'
         office_name = 'Valencia'
 
         result = get_real_office_name(office_name)
 
         self.assertEqual(result, expected_result)
```

