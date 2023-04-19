# Comparing `tmp/prophecy-libs-1.4.8.tar.gz` & `tmp/prophecy-libs-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.4.8.tar", last modified: Fri Mar 24 09:34:59 2023, max compression
+gzip compressed data, was "prophecy-libs-1.4.9.tar", last modified: Wed Apr 19 07:08:13 2023, max compression
```

## Comparing `prophecy-libs-1.4.8.tar` & `prophecy-libs-1.4.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-03-24 09:34:59.066238 prophecy-libs-1.4.8/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-03-24 09:34:59.066238 prophecy-libs-1.4.8/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2022-05-09 11:20:58.000000 prophecy-libs-1.4.8/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-03-24 09:34:59.054238 prophecy-libs-1.4.8/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2022-05-09 11:20:58.000000 prophecy-libs-1.4.8/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-03-24 09:34:59.058238 prophecy-libs-1.4.8/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2022-06-16 09:48:35.000000 prophecy-libs-1.4.8/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-07 11:01:04.000000 prophecy-libs-1.4.8/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2858 2023-03-09 05:37:36.000000 prophecy-libs-1.4.8/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-03-24 09:34:59.058238 prophecy-libs-1.4.8/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-02-07 17:59:57.000000 prophecy-libs-1.4.8/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      619 2023-03-13 07:13:11.000000 prophecy-libs-1.4.8/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-03-24 09:34:59.058238 prophecy-libs-1.4.8/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-01-12 10:34:24.000000 prophecy-libs-1.4.8/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2022-06-16 09:48:35.000000 prophecy-libs-1.4.8/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-01-19 08:09:44.000000 prophecy-libs-1.4.8/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-03-24 09:34:59.058238 prophecy-libs-1.4.8/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-01-05 10:22:12.000000 prophecy-libs-1.4.8/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-01-19 08:09:44.000000 prophecy-libs-1.4.8/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-03-24 09:34:59.062238 prophecy-libs-1.4.8/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2022-05-20 06:30:35.000000 prophecy-libs-1.4.8/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      638 2023-03-24 09:34:57.000000 prophecy-libs-1.4.8/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9067 2023-02-07 17:59:57.000000 prophecy-libs-1.4.8/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-03-24 09:34:59.062238 prophecy-libs-1.4.8/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2022-08-05 09:55:48.000000 prophecy-libs-1.4.8/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-01-12 10:34:24.000000 prophecy-libs-1.4.8/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-01-12 10:34:24.000000 prophecy-libs-1.4.8/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      985 2023-02-24 12:01:48.000000 prophecy-libs-1.4.8/prophecy/udfs/scala_udf_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     7642 2023-03-24 09:34:57.000000 prophecy-libs-1.4.8/prophecy/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-03-24 09:34:59.066238 prophecy-libs-1.4.8/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-03-24 09:34:58.000000 prophecy-libs-1.4.8/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)      773 2023-03-24 09:34:59.000000 prophecy-libs-1.4.8/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-24 09:34:58.000000 prophecy-libs-1.4.8/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2022-05-09 11:23:57.000000 prophecy-libs-1.4.8/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-03-24 09:34:58.000000 prophecy-libs-1.4.8/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-03-24 09:34:58.000000 prophecy-libs-1.4.8/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-03-24 09:34:59.066238 prophecy-libs-1.4.8/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-03-24 09:34:57.000000 prophecy-libs-1.4.8/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:08:13.910470 prophecy-libs-1.4.9/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-04-19 07:08:13.910470 prophecy-libs-1.4.9/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:08:13.906469 prophecy-libs-1.4.9/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:08:13.906469 prophecy-libs-1.4.9/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2858 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:08:13.906469 prophecy-libs-1.4.9/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      619 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:08:13.906469 prophecy-libs-1.4.9/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:08:13.906469 prophecy-libs-1.4.9/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:08:13.910470 prophecy-libs-1.4.9/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      638 2023-04-12 12:00:52.000000 prophecy-libs-1.4.9/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9185 2023-04-19 07:08:12.000000 prophecy-libs-1.4.9/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:08:13.910470 prophecy-libs-1.4.9/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      985 2023-03-12 14:51:36.000000 prophecy-libs-1.4.9/prophecy/udfs/scala_udf_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     8981 2023-04-12 12:00:52.000000 prophecy-libs-1.4.9/prophecy/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-04-19 07:08:13.910470 prophecy-libs-1.4.9/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-04-19 07:08:13.000000 prophecy-libs-1.4.9/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      773 2023-04-19 07:08:13.000000 prophecy-libs-1.4.9/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-04-19 07:08:13.000000 prophecy-libs-1.4.9/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.4.9/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-04-19 07:08:13.000000 prophecy-libs-1.4.9/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-04-19 07:08:13.000000 prophecy-libs-1.4.9/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-04-19 07:08:13.910470 prophecy-libs-1.4.9/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-04-19 07:08:12.000000 prophecy-libs-1.4.9/setup.py
```

### Comparing `prophecy-libs-1.4.8/prophecy/config/config_base.py` & `prophecy-libs-1.4.9/prophecy/config/config_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.4.8/prophecy/config/utils.py` & `prophecy-libs-1.4.9/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.4.8/prophecy/libs/utils.py` & `prophecy-libs-1.4.9/prophecy/libs/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.4.8/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.4.9/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.4.8/prophecy/random_data_creator.py` & `prophecy-libs-1.4.9/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.4.8/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.4.9/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.4.8/prophecy/test/base_test_case.py` & `prophecy-libs-1.4.9/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.4.8/prophecy/test/utils.py` & `prophecy-libs-1.4.9/prophecy/test/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         return datetime.now()
     elif isinstance(type, TimestampType):
         return datetime.now()
     elif isinstance(type, DecimalType):
         return Decimal(0)
     elif isinstance(type, ArrayType):
         return []
+    elif isinstance(type, NullType):
+        return ""
     elif isinstance(type, StructType):
         fields = {}
         for field in type.fields:
             fields[field.name] = defaultForDatatype(field.dataType)
         return fields
     else:
         raise Exception(f"default value for datatype: {type} not found")
@@ -69,14 +71,16 @@
         newValue = 0 if isNull(value) else int(value)
     elif isinstance(dataType, FloatType) or isinstance(dataType, DoubleType):
         newValue = 0.0 if isNull(value) else float(value)
     elif isinstance(dataType, BinaryType):
         newValue = bytearray(0) if isNull(value) else bytearray(value.encode("utf-8"))
     elif isinstance(dataType, BooleanType):
         newValue = False if isNull(value) else (value == "true")
+    elif isinstance(dataType, NullType):
+        newValue = ""
     elif isinstance(dataType, DateType):
         newValue = (
             datetime.now() if isNull(value) else datetime.strptime(value, "%Y-%m-%d")
         )
     elif isinstance(dataType, TimestampType):
         newValue = (
             datetime.now()
```

### Comparing `prophecy-libs-1.4.8/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.4.9/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.4.8/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.4.9/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.4.8/prophecy/utils.py` & `prophecy-libs-1.4.9/prophecy/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,39 +80,67 @@
         self.interimOutput = None
 
 
 interimConfig = InterimConfig()
 
 
 class ProphecyDebugger:
+    @classmethod
+    def sparkSqlShow(cls, spark: SparkSession, query: str):
+        spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.sparkSqlShow(spark._jsparkSession, query)
 
     @classmethod
     def sparkSql(cls, spark: SparkSession, query: str):
-        return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.sparkSql(spark._jsparkSession, query)
+        jdf = spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.sparkSql(spark._jsparkSession, query)
+        return DataFrame(jdf, spark)
 
     @classmethod
     def exception(cls, spark: SparkSession):
         spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.exception(spark._jsparkSession)
 
     @classmethod
     def class_details(cls, spark: SparkSession, name: str):
         return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.classDetails(spark._jsparkSession, name)
 
     @classmethod
     def spark_conf(cls, spark: SparkSession):
         return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.sparkConf(spark._jsparkSession)
+
     @classmethod
     def runtime_conf(cls, spark: SparkSession):
         return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.runtimeConf(spark._jsparkSession)
+
     @classmethod
     def local_properties(cls, spark: SparkSession):
         return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.localProperties(spark._jsparkSession)
+
+    @classmethod
+    def local_property(cls, spark: SparkSession, key: str):
+        return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.localProperty(spark._jsparkSession, key)
+
+    @classmethod
+    def local_property_async(cls, spark: SparkSession, key: str):
+        return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.localPropertyAsync(spark._jsparkSession,
+                                                                                                key)
+
     @classmethod
     def get_scala_object(cls, spark: SparkSession, className: str):
-        return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.getScalaObject(spark._jsparkSession, className)
+        return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.getScalaObject(spark._jsparkSession,
+                                                                                            className)
+
+    @classmethod
+    def call_scala_object_method(cls, spark: SparkSession, className: str, methodName: str, args: list = []):
+        return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.callScalaObjectMethod(
+            spark._jsparkSession, className, methodName, args)
+
+    @classmethod
+    def call_scala_object_method_async(cls, spark: SparkSession, className: str, methodName: str, args: list = []):
+        return spark.sparkContext._jvm.org.apache.spark.sql.ProphecyDebugger.callScalaObjectMethodAsync(
+            spark._jsparkSession, className, methodName, args)
+
 
 class MetricsCollector:
 
     # Called only for interactive execution and metrics mode.
     @classmethod
     def initializeMetrics(cls, spark: SparkSession):
         spark.sparkContext._jvm.org.apache.spark.sql.MetricsCollector.initializeMetrics(
@@ -182,15 +210,15 @@
             {
                 "Authorization": "Splunk " + props["token"],
                 "Content-Encoding": "gzip",
                 "BatchId": props.get("batchId", None),
             }
         )
         res = session.post(
-            props["url"], gzip.compress(bytes(payload, encoding="utf8")), verify=(not props.get("skipSsl", False)), cert=props.get("certFilePath")
+            props["url"], gzip.compress(bytes(payload, encoding="utf8"))
         )
         print(f"IN SESSION URL={props['url']} res.status_code = {res.status_code} res={res.text}")
         if res.status_code != 200 and props.get("stopOnFailure", False):
             raise HTTPError(res.reason)
 
 
 def splunkHECForEachWriter(props: dict):
```

### Comparing `prophecy-libs-1.4.8/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.4.9/prophecy_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

