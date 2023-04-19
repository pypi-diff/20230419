# Comparing `tmp/ampel_lsst-0.8.3a1.tar.gz` & `tmp/ampel_lsst-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_lsst-0.8.3a1.tar", max compression
+gzip compressed data, was "ampel_lsst-0.8.4.tar", max compression
```

## Comparing `ampel_lsst-0.8.3a1.tar` & `ampel_lsst-0.8.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1512 2023-01-17 09:51:54.850469 ampel_lsst-0.8.3a1/LICENSE
--rw-r--r--   0        0        0      301 2023-01-17 09:51:54.850469 ampel_lsst-0.8.3a1/README.md
--rw-r--r--   0        0        0     3188 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/alert/ElasticcAlertSupplier.py
--rw-r--r--   0        0        0     2467 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/alert/LSSTAlertSupplier.py
--rw-r--r--   0        0        0    20353 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/alert/load/ElasticcDirAlertLoader.py
--rw-r--r--   0        0        0    10648 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/alert/load/ElasticcTrainingsetLoader.py
--rw-r--r--   0        0        0    22084 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/alert/load/KafkaAlertLoader.py
--rw-r--r--   0        0        0     1583 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/alert/load/MultiAvroAlertLoader.py
--rw-r--r--   0        0        0      690 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/aux/LSSTDPFilter.py
--rw-r--r--   0        0        0      686 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/aux/LSSTFPFilter.py
--rw-r--r--   0        0        0      671 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/aux/LSSTObjFilter.py
--rw-r--r--   0        0        0      750 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/ingest/LSSTCompilerOptions.py
--rwxr-xr-x   0        0        0     2986 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/ingest/LSSTDataPointShaper.py
--rw-r--r--   0        0        0     4945 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/ingest/LSSTMongoMuxer.py
--rw-r--r--   0        0        0     3110 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/t0/ReallySimpleLSSTFilter.py
--rw-r--r--   0        0        0     8807 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/t0/SimpleLSSTFilter.py
--rw-r--r--   0        0        0      296 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/t1/LSSTT1Combiner.py
--rw-r--r--   0        0        0     2168 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/t2/T2GetAlertId.py
--rw-r--r--   0        0        0      912 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/t2/T2GetAlertJournal.py
--rw-r--r--   0        0        0     1159 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/t2/T2GetDiaObject.py
--rw-r--r--   0        0        0     2253 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/template/ElasticcAlertConsumerTemplate.py
--rw-r--r--   0        0        0     3187 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/lsst/view/LSSTT2Tabulator.py
--rw-r--r--   0        0        0        0 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/ampel/py.typed
--rw-r--r--   0        0        0     1206 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/conf/ampel-lsst/ampel.yml
--rw-r--r--   0        0        0     2173 2023-01-17 09:51:54.854470 ampel_lsst-0.8.3a1/pyproject.toml
--rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 ampel_lsst-0.8.3a1/setup.py
--rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 ampel_lsst-0.8.3a1/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/LICENSE
+-rw-r--r--   0        0        0      301 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/README.md
+-rw-r--r--   0        0        0     3188 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/ElasticcAlertSupplier.py
+-rw-r--r--   0        0        0     2467 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/LSSTAlertSupplier.py
+-rw-r--r--   0        0        0    20365 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/load/ElasticcDirAlertLoader.py
+-rw-r--r--   0        0        0    10648 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/load/ElasticcTrainingsetLoader.py
+-rw-r--r--   0        0        0    22184 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/load/KafkaAlertLoader.py
+-rw-r--r--   0        0        0     1583 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/alert/load/MultiAvroAlertLoader.py
+-rw-r--r--   0        0        0      690 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/aux/LSSTDPFilter.py
+-rw-r--r--   0        0        0      686 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/aux/LSSTFPFilter.py
+-rw-r--r--   0        0        0      671 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/aux/LSSTObjFilter.py
+-rw-r--r--   0        0        0      750 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTCompilerOptions.py
+-rwxr-xr-x   0        0        0     2986 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTDataPointShaper.py
+-rw-r--r--   0        0        0     4945 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTMongoMuxer.py
+-rw-r--r--   0        0        0     3110 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/t0/ReallySimpleLSSTFilter.py
+-rw-r--r--   0        0        0     8807 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/t0/SimpleLSSTFilter.py
+-rw-r--r--   0        0        0      296 2023-04-19 12:45:10.283786 ampel_lsst-0.8.4/ampel/lsst/t1/LSSTT1Combiner.py
+-rw-r--r--   0        0        0     2168 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/t2/T2GetAlertId.py
+-rw-r--r--   0        0        0      912 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/t2/T2GetAlertJournal.py
+-rw-r--r--   0        0        0     1159 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/t2/T2GetDiaObject.py
+-rw-r--r--   0        0        0      440 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/template/ElasticcAlertConsumerTemplate.py
+-rw-r--r--   0        0        0      490 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/template/LSSTAlertConsumerTemplate.py
+-rw-r--r--   0        0        0     3187 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/lsst/view/LSSTT2Tabulator.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/ampel/py.typed
+-rw-r--r--   0        0        0     1281 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/conf/ampel-lsst/ampel.yml
+-rw-r--r--   0        0        0     2191 2023-04-19 12:45:10.287786 ampel_lsst-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     1481 1970-01-01 00:00:00.000000 ampel_lsst-0.8.4/PKG-INFO
```

### Comparing `ampel_lsst-0.8.3a1/LICENSE` & `ampel_lsst-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/alert/ElasticcAlertSupplier.py` & `ampel_lsst-0.8.4/ampel/lsst/alert/ElasticcAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/alert/LSSTAlertSupplier.py` & `ampel_lsst-0.8.4/ampel/lsst/alert/LSSTAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/alert/load/ElasticcDirAlertLoader.py` & `ampel_lsst-0.8.4/ampel/lsst/alert/load/ElasticcDirAlertLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,15 +493,15 @@
     """
 
     #: Message schema
     avro_schema: dict = DEFAULT_SCHEMA
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.schema: dict = fastavro.schema.parse_schema(self.avro_schema)
+        self.alert_schema: dict = fastavro.schema.parse_schema(self.avro_schema)
 
     def __next__(self) -> StringIO | BytesIO:
 
         if not self.files:
             self.build_file_list()
             self.iter_files = iter(self.files)
 
@@ -509,10 +509,10 @@
             raise StopIteration
 
         if self.logger.verbose > 1:
             self.logger.debug("Loading " + fpath)
 
         with gzip.open(fpath, self.open_mode) as alert_file:
 
-            alert = fastavro.schemaless_reader(alert_file, self.schema)
+            alert = fastavro.schemaless_reader(alert_file, self.alert_schema)
             # Assuming one alert per file
             return alert
```

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/alert/load/ElasticcTrainingsetLoader.py` & `ampel_lsst-0.8.4/ampel/lsst/alert/load/ElasticcTrainingsetLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/alert/load/KafkaAlertLoader.py` & `ampel_lsst-0.8.4/ampel/lsst/alert/load/KafkaAlertLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,23 +501,28 @@
     #: Message schema
     avro_schema: dict = DEFAULT_SCHEMA
     #: Consumer group name
     group_name: str = str(uuid.uuid1())
     #: time to wait for messages before giving up, in seconds
     timeout: int = 1
     #: extra configuration to pass to confluent_kafka.Consumer
-    kafka_consumer_properties: dict[str,Any] = {}
+    kafka_consumer_properties: dict[str, Any] = {}
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         config = {"group.id": self.group_name} | self.kafka_consumer_properties
 
         self._consumer = AllConsumingConsumer(
-            self.bootstrap, timeout=self.timeout, topics=self.topics, **config
+            self.bootstrap,
+            timeout=self.timeout,
+            topics=self.topics,
+            auto_commit=True,
+            logger=self.logger,
+            **config,
         )
         self._it = None
 
     @staticmethod
     def _add_message_metadata(alert: dict, message: confluent_kafka.Message):
         meta = {}
         timestamp_kind, timestamp = message.timestamp()
```

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/alert/load/MultiAvroAlertLoader.py` & `ampel_lsst-0.8.4/ampel/lsst/alert/load/MultiAvroAlertLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/aux/LSSTDPFilter.py` & `ampel_lsst-0.8.4/ampel/lsst/aux/LSSTDPFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/aux/LSSTFPFilter.py` & `ampel_lsst-0.8.4/ampel/lsst/aux/LSSTFPFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/aux/LSSTObjFilter.py` & `ampel_lsst-0.8.4/ampel/lsst/aux/LSSTObjFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/ingest/LSSTCompilerOptions.py` & `ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTCompilerOptions.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/ingest/LSSTDataPointShaper.py` & `ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTDataPointShaper.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/ingest/LSSTMongoMuxer.py` & `ampel_lsst-0.8.4/ampel/lsst/ingest/LSSTMongoMuxer.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/t0/ReallySimpleLSSTFilter.py` & `ampel_lsst-0.8.4/ampel/lsst/t0/ReallySimpleLSSTFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/t0/SimpleLSSTFilter.py` & `ampel_lsst-0.8.4/ampel/lsst/t0/SimpleLSSTFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/t2/T2GetAlertId.py` & `ampel_lsst-0.8.4/ampel/lsst/t2/T2GetAlertId.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/t2/T2GetAlertJournal.py` & `ampel_lsst-0.8.4/ampel/lsst/t2/T2GetAlertJournal.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/t2/T2GetDiaObject.py` & `ampel_lsst-0.8.4/ampel/lsst/t2/T2GetDiaObject.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/ampel/lsst/view/LSSTT2Tabulator.py` & `ampel_lsst-0.8.4/ampel/lsst/view/LSSTT2Tabulator.py`

 * *Files identical despite different names*

### Comparing `ampel_lsst-0.8.3a1/conf/ampel-lsst/ampel.yml` & `ampel_lsst-0.8.4/conf/ampel-lsst/ampel.yml`

 * *Files 14% similar despite different names*

```diff
@@ -34,8 +34,9 @@
       select: first
     '%LSST_Obj':
       filter: LSSTObjFilter
       sort: diaObjectId
       select: last
 
 template:
-  elasticc_alerts: ampel.lsst.template.ElasticcAlertConsumerTemplate
+  ingest_elasticc_alerts: ampel.lsst.template.ElasticcAlertConsumerTemplate
+  ingest_lsst_alerts: ampel.lsst.template.LSSTAlertConsumerTemplate
```

### Comparing `ampel_lsst-0.8.3a1/pyproject.toml` & `ampel_lsst-0.8.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-lsst"
-version = "0.8.3-alpha.1"
+version = "0.8.4"
 description = "Legacy Survey of Space and Time support for the Ampel system"
 authors = [
     "Marcus Fenner <mf@physik.hu-berlinn.de>",
     "Valery Brinnel",
     "Jakob van Santen <jakob.van.santen@desy.de>",
     "Jakob Nordin",
 ]
@@ -34,30 +34,31 @@
     'conf/*/*/*.yaml',
     'conf/*/*.yml',
     'conf/*/*/*.yml',
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.11"
+python = ">=3.10,<3.12"
 astropy = "^5.0.2"
 fastavro = "^1.3.2"
-ampel-ztf = {version = ">=0.8.3a2,<0.8.4", allow-prereleases = true, extras = ["kafka"]}
+ampel-ztf = {version = "^0.8.5", extras = ["kafka"]}
+ampel-alerts = {version = "^0.8.5"}
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-pytest-cov = "^3.0.0"
-pytest-mock = "^3.6.1"
-mongomock = "^3.23.0"
-mypy = "^0.981"
-pytest-timeout = "^1.4.2"
-pytest-asyncio = "^0.15.1"
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
+pytest-mock = "^3.10.0"
+mongomock = "^4.1.2"
+mypy = "^1.1.1"
+pytest-timeout = "^2.1.0"
+pytest-asyncio = "^0.21.0"
 types-requests = "^2.25.9"
 before_after = "^1.0.1"
-isort = "^5.10.1"
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools >= 40.6.0", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 relative_files = true
@@ -65,14 +66,15 @@
 [tool.mypy]
 namespace_packages = true
 plugins = [
   "pydantic.mypy",
   "numpy.typing.mypy_plugin"
 ]
 show_error_codes = true
+check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = [
   "astropy.*",
   "bson.*",
   "fastavro.*",
   "pymongo.*",
```

### Comparing `ampel_lsst-0.8.3a1/PKG-INFO` & `ampel_lsst-0.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: ampel-lsst
-Version: 0.8.3a1
+Version: 0.8.4
 Summary: Legacy Survey of Space and Time support for the Ampel system
 Home-page: https://ampelproject.github.io
 License: BSD-3-Clause
 Author: Marcus Fenner
 Author-email: mf@physik.hu-berlinn.de
 Maintainer: Marcus Fenner
 Maintainer-email: mf@physik.hu-berlinn.de
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Typing :: Typed
-Requires-Dist: ampel-ztf[kafka] (>=0.8.3a2,<0.8.4)
+Requires-Dist: ampel-alerts (>=0.8.5,<0.9.0)
+Requires-Dist: ampel-ztf[kafka] (>=0.8.5,<0.9.0)
 Requires-Dist: astropy (>=5.0.2,<6.0.0)
 Requires-Dist: fastavro (>=1.3.2,<2.0.0)
 Project-URL: Repository, https://github.com/AmpelProject/Ampel-LSST
 Description-Content-Type: text/markdown
```

