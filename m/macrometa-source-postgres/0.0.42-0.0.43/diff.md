# Comparing `tmp/macrometa-source-postgres-0.0.42.tar.gz` & `tmp/macrometa-source-postgres-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.42.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-0.0.43.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.42.tar` & `macrometa-source-postgres-0.0.43.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/LICENSE
--rw-r--r--   0        0        0    35130 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8580 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     8974 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    28921 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3698 2023-04-18 02:51:35.535316 macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1512 2023-04-18 02:51:35.807317 macrometa-source-postgres-0.0.42/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.42/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.42/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/LICENSE
+-rw-r--r--   0        0        0    35128 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8580 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     8974 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    28921 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3698 2023-04-19 07:19:31.334522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1512 2023-04-19 07:19:31.582520 macrometa-source-postgres-0.0.43/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.43/setup.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.43/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.42/LICENSE` & `macrometa-source-postgres-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.42/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-0.0.43/macrometa_source_postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                            placeholder_value='postgres_host'),
             ConfigProperty('port', 'Port', ConfigAttributeType.INT, True, False,
                            description='PostgreSQL port.',
                            default_value='5432'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
                            description='PostgreSQL user.',
                            default_value='postgres'),
-            ConfigProperty('password', 'Password', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, True, False,
                            description='PostgreSQL password.',
                            placeholder_value='password'),
             ConfigProperty('dbname', 'Database Name', ConfigAttributeType.STRING, True, False,
                            description='PostgreSQL database name.',
                            default_value='postgres'),
             ConfigProperty('filter_schemas', 'Source Schema', ConfigAttributeType.STRING, True, True,
                            description='Source Schema to scan.',
@@ -190,26 +190,26 @@
                            description='Choose from LOG_BASED, FULL_TABLE.',
                            default_value='FULL_TABLE'),
             ConfigProperty('ssl', 'Use SSL', ConfigAttributeType.BOOLEAN, False, False,
                            description='If set to `true` then use SSL via postgres sslmode `require` option. '
 			   	       'If the server does not accept SSL connections or the client certificate is not recognized'
 			               ' then the connection will fail.',
                            default_value='false'),
-            ConfigProperty('ssl_root_ca_cert', 'SSL CA Certificate', ConfigAttributeType.STRING, False, False,
+            ConfigProperty('ssl_root_ca_cert', 'SSL CA Certificate', ConfigAttributeType.FILE, False, False,
                            description='Specific CA certificate in PEM string format. This is most often the case '
                                        'when using `self-signed` server certificate.',
                            placeholder_value="my_ca_certificate"),
-            ConfigProperty('ssl_client_certificate', 'SSL Client Certificate', ConfigAttributeType.STRING, False, False,
+            ConfigProperty('ssl_client_certificate', 'SSL Client Certificate', ConfigAttributeType.FILE, False, False,
                            description='Specific client certificate in PEM string format. The private key for client '
                                        'certificate should be specfied in a different parameter, SSL Client Key.',
                            placeholder_value="my_client_certificate"),
-            ConfigProperty('ssl_client_key', 'SSL Client Key', ConfigAttributeType.STRING, False, False,
+            ConfigProperty('ssl_client_key', 'SSL Client Key', ConfigAttributeType.FILE, False, False,
                            description='Specific client key in PEM string format.',
                            placeholder_value="my_client_key"),
-            ConfigProperty('ssl_client_password', 'SSL Client Password', ConfigAttributeType.STRING, False, False,
+            ConfigProperty('ssl_client_password', 'SSL Client Password', ConfigAttributeType.PASSWORD, False, False,
                            description='If the private key contained in the SSL Client Key is encrypted, users can provide a '
                                        'password or passphrase to decrypt the encrypted private keys.',
                            placeholder_value="my_client_password"),
             ConfigProperty('logical_poll_total_seconds', 'Break at No Data Received (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Stop running when no data received from WAL after certain number of seconds.',
                            default_value='10800'),
```

### Comparing `macrometa-source-postgres-0.0.42/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-0.0.43/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.42/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-0.0.43/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.42/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.42/pyproject.toml` & `macrometa-source-postgres-0.0.43/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.42'
+version='0.0.43'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-postgres-0.0.42/setup.py` & `macrometa-source-postgres-0.0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.42',
+    'version': '0.0.43',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.42/PKG-INFO` & `macrometa-source-postgres-0.0.43/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.42
+Version: 0.0.43
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

