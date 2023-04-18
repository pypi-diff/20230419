# Comparing `tmp/airflow_metrics_gbq-0.0.2.tar.gz` & `tmp/airflow_metrics_gbq-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_metrics_gbq-0.0.2.tar", max compression
+gzip compressed data, was "airflow_metrics_gbq-0.0.3a0.tar", max compression
```

## Comparing `airflow_metrics_gbq-0.0.2.tar` & `airflow_metrics_gbq-0.0.3a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1296 2023-04-16 13:00:16.804609 airflow_metrics_gbq-0.0.2/LICENSE
--rw-r--r--   0        0        0      422 2023-04-17 22:56:38.265504 airflow_metrics_gbq-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-17 19:15:43.320228 airflow_metrics_gbq-0.0.2/airflow_metrics_gbq/__init__.py
--rw-r--r--   0        0        0     7591 2023-04-17 22:56:52.678202 airflow_metrics_gbq-0.0.2/airflow_metrics_gbq/metrics.py
--rw-r--r--   0        0        0      700 2023-04-17 22:56:52.607080 airflow_metrics_gbq-0.0.2/airflow_metrics_gbq/utils/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-17 22:56:52.617152 airflow_metrics_gbq-0.0.2/airflow_metrics_gbq/utils/gbq_connector.py
--rw-r--r--   0        0        0     1264 2023-04-18 21:49:51.081830 airflow_metrics_gbq-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-04-16 13:00:16.804609 airflow_metrics_gbq-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0      422 2023-04-17 22:56:38.265504 airflow_metrics_gbq-0.0.3a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 19:15:43.320228 airflow_metrics_gbq-0.0.3a0/airflow_metrics_gbq/__init__.py
+-rw-r--r--   0        0        0     7591 2023-04-17 22:56:52.678202 airflow_metrics_gbq-0.0.3a0/airflow_metrics_gbq/metrics.py
+-rw-r--r--   0        0        0      700 2023-04-17 22:56:52.607080 airflow_metrics_gbq-0.0.3a0/airflow_metrics_gbq/utils/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-17 22:56:52.617152 airflow_metrics_gbq-0.0.3a0/airflow_metrics_gbq/utils/gbq_connector.py
+-rw-r--r--   0        0        0     1266 2023-04-18 22:44:54.869896 airflow_metrics_gbq-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.3a0/PKG-INFO
```

### Comparing `airflow_metrics_gbq-0.0.2/LICENSE` & `airflow_metrics_gbq-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.2/airflow_metrics_gbq/metrics.py` & `airflow_metrics_gbq-0.0.3a0/airflow_metrics_gbq/metrics.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.2/airflow_metrics_gbq/utils/__init__.py` & `airflow_metrics_gbq-0.0.3a0/airflow_metrics_gbq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.2/airflow_metrics_gbq/utils/gbq_connector.py` & `airflow_metrics_gbq-0.0.3a0/airflow_metrics_gbq/utils/gbq_connector.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.2/pyproject.toml` & `airflow_metrics_gbq-0.0.3a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-metrics-gbq"
-version = "0.0.2"
+version = "0.0.3a0"
 description = "Airflow metrics to Google BigQuery"
 authors = ["Shaurya Rawat <rawatshaurya1994@gmail.com>"]
 license = "BSD2"
 readme = "README.md"
 homepage="https://github.com/abyssnlp/airflow-metrics-gbq"
 repository="https://github.com/abyssnlp/airflow-metrics-gbq"
 include=[
```

### Comparing `airflow_metrics_gbq-0.0.2/PKG-INFO` & `airflow_metrics_gbq-0.0.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-metrics-gbq
-Version: 0.0.2
+Version: 0.0.3a0
 Summary: Airflow metrics to Google BigQuery
 Home-page: https://github.com/abyssnlp/airflow-metrics-gbq
 License: BSD2
 Author: Shaurya Rawat
 Author-email: rawatshaurya1994@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

