# Comparing `tmp/macrometa-target-collection-0.0.55.tar.gz` & `tmp/macrometa-target-collection-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.55.tar", last modified: Mon Apr 17 09:52:38 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.56.tar", last modified: Wed Apr 19 05:53:07 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.55.tar` & `macrometa-target-collection-0.0.56.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:38.058284 macrometa-target-collection-0.0.55/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-17 09:52:15.000000 macrometa-target-collection-0.0.55/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-17 09:52:38.058284 macrometa-target-collection-0.0.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 09:52:15.000000 macrometa-target-collection-0.0.55/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:38.058284 macrometa-target-collection-0.0.55/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-17 09:52:15.000000 macrometa-target-collection-0.0.55/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13888 2023-04-17 09:52:15.000000 macrometa-target-collection-0.0.55/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:38.058284 macrometa-target-collection-0.0.55/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-17 09:52:38.000000 macrometa-target-collection-0.0.55/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-17 09:52:38.000000 macrometa-target-collection-0.0.55/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:52:38.000000 macrometa-target-collection-0.0.55/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 09:52:38.000000 macrometa-target-collection-0.0.55/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 09:52:38.000000 macrometa-target-collection-0.0.55/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 09:52:38.000000 macrometa-target-collection-0.0.55/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-17 09:52:15.000000 macrometa-target-collection-0.0.55/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 09:52:38.058284 macrometa-target-collection-0.0.55/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:53:07.150036 macrometa-target-collection-0.0.56/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-19 05:53:07.150036 macrometa-target-collection-0.0.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:53:07.146036 macrometa-target-collection-0.0.56/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13889 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:53:07.150036 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 05:53:07.000000 macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 05:52:47.000000 macrometa-target-collection-0.0.56/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 05:53:07.150036 macrometa-target-collection-0.0.56/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.55/LICENSE` & `macrometa-target-collection-0.0.56/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.55/PKG-INFO` & `macrometa-target-collection-0.0.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.55
+Version: 0.0.56
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.55/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.56/macrometa_target_collection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,34 +51,34 @@
 
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
             ConfigProperty('region', 'Region URL', ConfigAttributeType.STRING, True, False,
                            description="Fully qualified region URL.",
                            placeholder_value='api-sample-ap-west.eng.macrometa.io'),
-            ConfigProperty('api_key', 'API Key', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('api_key', 'API Key', ConfigAttributeType.PASSWORD, True, False,
                            description="API key.",
                            placeholder_value='my_apikey'),
             ConfigProperty('fabric', 'Fabric', ConfigAttributeType.STRING, True, False,
                            description="Fabric name.",
                            default_value='_system'),
             ConfigProperty('target_collection', 'Target Collection', ConfigAttributeType.STRING, True, True,
                            description="Target collection name.",
                            placeholder_value='my_collection'),
             ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
                            description='Maximum number of rows inserted per batch.',
-                           default_value='50'),
+                           default_value='100'),
             ConfigProperty('batch_flush_interval', 'Batch Flush Interval (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Time between batch flush executions.',
-                           default_value='60'),
+                           default_value='10'),
             ConfigProperty('batch_flush_min_time_gap', 'Batch Flush Minimum Time Gap (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Minimum time gap between two batch flush tasks.',
-                           default_value='60'),
+                           default_value='10'),
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
         return []
```

### Comparing `macrometa-target-collection-0.0.55/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.56/macrometa_target_collection/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 from c8.collection import StandardCollection
 from jsonschema import Draft4Validator
 from prometheus_client import Counter, Gauge, start_http_server
 from singer import get_logger
 
 logger = get_logger('macrometa_target_collection')
 
-DEFAULT_BATCH_SIZE_ROWS = 50
-DEFAULT_BATCH_FLUSH_INTERVAL = 60
-DEFAULT_MIN_BATCH_FLUSH_TIME_GAP = 60
+DEFAULT_BATCH_SIZE_ROWS = 100
+DEFAULT_BATCH_FLUSH_INTERVAL = 10
+DEFAULT_MIN_BATCH_FLUSH_TIME_GAP = 10
 
 # Prometheus metrics
 ingested_bytes = Counter('ingested_bytes', 'Total number of bytes ingested', ['region', 'tenant', 'fabric', 'workflow'])
 ingested_documents = Counter('ingested_documents', 'Total number of documents ingested', ['region', 'tenant', 'fabric', 'workflow'])
 ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion', ['region', 'tenant', 'fabric', 'workflow'])
 ingest_lag = Gauge('ingest_lag', 'Average time lag between data changes in GDN collections and external data sources', ['region', 'tenant', 'fabric', 'workflow'])
 scrape_complete_flag = Counter("scrape_complete_flag", "Flag to check if the last scrape has been completed", ['workflow'])
```

### Comparing `macrometa-target-collection-0.0.55/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.56/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.55
+Version: 0.0.56
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.55/pyproject.toml` & `macrometa-target-collection-0.0.56/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.55"
+version = "0.0.56"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

