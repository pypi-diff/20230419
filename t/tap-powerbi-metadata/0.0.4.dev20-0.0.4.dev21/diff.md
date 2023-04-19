# Comparing `tmp/tap_powerbi_metadata-0.0.4.dev20.tar.gz` & `tmp/tap_powerbi_metadata-0.0.4.dev21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_powerbi_metadata-0.0.4.dev20.tar", max compression
+gzip compressed data, was "tap_powerbi_metadata-0.0.4.dev21.tar", max compression
```

## Comparing `tap_powerbi_metadata-0.0.4.dev20.tar` & `tap_powerbi_metadata-0.0.4.dev21.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-04-04 17:25:59.089821 tap_powerbi_metadata-0.0.4.dev20/LICENSE
--rw-r--r--   0        0        0      591 2023-04-04 17:26:24.782204 tap_powerbi_metadata-0.0.4.dev20/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-04 17:25:59.089821 tap_powerbi_metadata-0.0.4.dev20/tap_powerbi_metadata/__init__.py
--rw-r--r--   0        0        0    18414 2023-04-04 17:25:59.089821 tap_powerbi_metadata-0.0.4.dev20/tap_powerbi_metadata/streams.py
--rw-r--r--   0        0        0     1065 2023-04-04 17:25:59.089821 tap_powerbi_metadata-0.0.4.dev20/tap_powerbi_metadata/tap.py
--rw-r--r--   0        0        0      638 2023-04-04 17:25:59.089821 tap_powerbi_metadata-0.0.4.dev20/tap_powerbi_metadata/tests/test_standard_tests.py
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 tap_powerbi_metadata-0.0.4.dev20/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-04 20:56:40.312584 tap_powerbi_metadata-0.0.4.dev21/LICENSE
+-rw-r--r--   0        0        0      591 2023-04-04 20:57:03.716728 tap_powerbi_metadata-0.0.4.dev21/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-04 20:56:40.312584 tap_powerbi_metadata-0.0.4.dev21/tap_powerbi_metadata/__init__.py
+-rw-r--r--   0        0        0    18625 2023-04-04 20:56:40.312584 tap_powerbi_metadata-0.0.4.dev21/tap_powerbi_metadata/streams.py
+-rw-r--r--   0        0        0     1065 2023-04-04 20:56:40.312584 tap_powerbi_metadata-0.0.4.dev21/tap_powerbi_metadata/tap.py
+-rw-r--r--   0        0        0      638 2023-04-04 20:56:40.316584 tap_powerbi_metadata-0.0.4.dev21/tap_powerbi_metadata/tests/test_standard_tests.py
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 tap_powerbi_metadata-0.0.4.dev21/PKG-INFO
```

### Comparing `tap_powerbi_metadata-0.0.4.dev20/LICENSE` & `tap_powerbi_metadata-0.0.4.dev21/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_powerbi_metadata-0.0.4.dev20/pyproject.toml` & `tap_powerbi_metadata-0.0.4.dev21/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-powerbi-metadata"
-version = "0.0.4-dev.20"
+version = "0.0.4-dev.21"
 description = "`tap-powerbi-metadata` is Singer-compliant PowerBIMetadata tap built with Singer SDK."
 authors = ["AJ Steers <aaaronsteers@gmail.com>", "John Timeus <john.timeus@slalom.com>"]
 license = "Apache v2"
 
 [tool.poetry.dependencies]
 python = ">=3.6,<3.9"
 singer-sdk = "^0.1.0"
```

### Comparing `tap_powerbi_metadata-0.0.4.dev20/tap_powerbi_metadata/streams.py` & `tap_powerbi_metadata-0.0.4.dev21/tap_powerbi_metadata/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,18 @@
                 )
             )
         ),
         Property("PinReportToTabInformation", 
             ObjectType(
                 Property("ChannelId", StringType),
                 Property("ChannelName", StringType),
+                Property("DatasetId", StringType),
+                Property("DatasetName", StringType),
                 Property("ReportId", StringType),
+                Property("ReportName", StringType),
                 Property("TabName", StringType),
                 Property("TeamId", StringType),
                 Property("TeamName", StringType),
                 Property("TeamsAppId", StringType),
                 Property("UserId", StringType),
             )
         ),
@@ -385,14 +388,15 @@
                     Property("RecipientName", StringType),
                 )
             )
         ),
         Property(
             "SubscriptionSchedule",
             ObjectType(
+                Property("DaysOfTheMonth",StringType),
                 Property("EndDate", DateTimeType),
                 Property("StartDate", DateTimeType),
                 Property(
                     "Time",
                     ArrayType(StringType)
                 ),
                 Property("TimeZone", StringType),
```

### Comparing `tap_powerbi_metadata-0.0.4.dev20/tap_powerbi_metadata/tap.py` & `tap_powerbi_metadata-0.0.4.dev21/tap_powerbi_metadata/tap.py`

 * *Files identical despite different names*

### Comparing `tap_powerbi_metadata-0.0.4.dev20/tap_powerbi_metadata/tests/test_standard_tests.py` & `tap_powerbi_metadata-0.0.4.dev21/tap_powerbi_metadata/tests/test_standard_tests.py`

 * *Files identical despite different names*

### Comparing `tap_powerbi_metadata-0.0.4.dev20/PKG-INFO` & `tap_powerbi_metadata-0.0.4.dev21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-powerbi-metadata
-Version: 0.0.4.dev20
+Version: 0.0.4.dev21
 Summary: `tap-powerbi-metadata` is Singer-compliant PowerBIMetadata tap built with Singer SDK.
 License: Apache v2
 Author: AJ Steers
 Author-email: aaaronsteers@gmail.com
 Requires-Python: >=3.6,<3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

