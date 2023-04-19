# Comparing `tmp/telstra_messaging-3.0.2.tar.gz` & `tmp/telstra_messaging-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telstra_messaging-3.0.2.tar", max compression
+gzip compressed data, was "telstra_messaging-3.0.3.tar", max compression
```

## Comparing `telstra_messaging-3.0.2.tar` & `telstra_messaging-3.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11378 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/LICENSE
--rw-r--r--   0        0        0    25497 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/README.md
--rw-r--r--   0        0        0      888 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/pyproject.toml
--rw-r--r--   0        0        0       32 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/__init__.py
--rw-r--r--   0        0        0       40 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/__init__.py
--rw-r--r--   0        0        0      762 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/exceptions.py
--rw-r--r--   0        0        0     4682 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/free_trial_numbers.py
--rw-r--r--   0        0        0     1063 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/health_check.py
--rw-r--r--   0        0        0    31574 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/message.py
--rw-r--r--   0        0        0     2847 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/oauth.py
--rw-r--r--   0        0        0     8901 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/reports.py
--rw-r--r--   0        0        0      903 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/types.py
--rw-r--r--   0        0        0       38 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/__init__.py
--rw-r--r--   0        0        0      743 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/callback_url.py
--rw-r--r--   0        0        0     6152 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/config.py
--rw-r--r--   0        0        0     1315 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/error_response.py
--rw-r--r--   0        0        0     2043 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/free_trial_number.py
--rw-r--r--   0        0        0      933 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/message_id.py
--rw-r--r--   0        0        0      409 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/querystring.py
--rw-r--r--   0        0        0     2961 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/reports_dates.py
--rw-r--r--   0        0        0      929 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/schedule_send.py
--rw-r--r--   0        0        0     1662 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/virtual_number.py
--rw-r--r--   0        0        0    16507 2023-04-18 23:01:43.964254 telstra_messaging-3.0.2/telstra/messaging/virtual_number.py
--rw-r--r--   0        0        0    25995 1970-01-01 00:00:00.000000 telstra_messaging-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11378 2023-04-19 02:06:20.277949 telstra_messaging-3.0.3/LICENSE
+-rw-r--r--   0        0        0    25497 2023-04-19 02:06:20.277949 telstra_messaging-3.0.3/README.md
+-rw-r--r--   0        0        0      888 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/__init__.py
+-rw-r--r--   0        0        0      762 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/exceptions.py
+-rw-r--r--   0        0        0     4682 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/free_trial_numbers.py
+-rw-r--r--   0        0        0     1063 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/health_check.py
+-rw-r--r--   0        0        0    31574 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/message.py
+-rw-r--r--   0        0        0     2847 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/oauth.py
+-rw-r--r--   0        0        0     8901 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/reports.py
+-rw-r--r--   0        0        0      903 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/types.py
+-rw-r--r--   0        0        0       38 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/callback_url.py
+-rw-r--r--   0        0        0     6152 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/config.py
+-rw-r--r--   0        0        0     1315 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/error_response.py
+-rw-r--r--   0        0        0     2043 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/free_trial_number.py
+-rw-r--r--   0        0        0      933 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/message_id.py
+-rw-r--r--   0        0        0      409 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/querystring.py
+-rw-r--r--   0        0        0     2961 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/reports_dates.py
+-rw-r--r--   0        0        0      929 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/schedule_send.py
+-rw-r--r--   0        0        0     1662 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/utils/virtual_number.py
+-rw-r--r--   0        0        0    16507 2023-04-19 02:06:20.281949 telstra_messaging-3.0.3/telstra/messaging/virtual_number.py
+-rw-r--r--   0        0        0    25995 1970-01-01 00:00:00.000000 telstra_messaging-3.0.3/PKG-INFO
```

### Comparing `telstra_messaging-3.0.2/LICENSE` & `telstra_messaging-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/README.md` & `telstra_messaging-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/pyproject.toml` & `telstra_messaging-3.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telstra.messaging"
-version = "3.0.2"
+version = "3.0.3"
 readme = "README.md"
 description = "SDK for the Telstra Messaging API V3 - Beta"
 license = "Apache-2.0"
 authors = ["David Andersson <david-andersson@users.noreply.github.com >"]
 include = ["telstra"]
 exclude = ["tests"]
 packages = [
```

### Comparing `telstra_messaging-3.0.2/telstra/messaging/exceptions.py` & `telstra_messaging-3.0.3/telstra/messaging/exceptions.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/free_trial_numbers.py` & `telstra_messaging-3.0.3/telstra/messaging/free_trial_numbers.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/health_check.py` & `telstra_messaging-3.0.3/telstra/messaging/health_check.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/message.py` & `telstra_messaging-3.0.3/telstra/messaging/message.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/oauth.py` & `telstra_messaging-3.0.3/telstra/messaging/oauth.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/reports.py` & `telstra_messaging-3.0.3/telstra/messaging/reports.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/types.py` & `telstra_messaging-3.0.3/telstra/messaging/types.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/utils/callback_url.py` & `telstra_messaging-3.0.3/telstra/messaging/utils/callback_url.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/utils/config.py` & `telstra_messaging-3.0.3/telstra/messaging/utils/config.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/utils/error_response.py` & `telstra_messaging-3.0.3/telstra/messaging/utils/error_response.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/utils/free_trial_number.py` & `telstra_messaging-3.0.3/telstra/messaging/utils/free_trial_number.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/utils/message_id.py` & `telstra_messaging-3.0.3/telstra/messaging/utils/message_id.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/utils/reports_dates.py` & `telstra_messaging-3.0.3/telstra/messaging/utils/reports_dates.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/utils/schedule_send.py` & `telstra_messaging-3.0.3/telstra/messaging/utils/schedule_send.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/utils/virtual_number.py` & `telstra_messaging-3.0.3/telstra/messaging/utils/virtual_number.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/telstra/messaging/virtual_number.py` & `telstra_messaging-3.0.3/telstra/messaging/virtual_number.py`

 * *Files identical despite different names*

### Comparing `telstra_messaging-3.0.2/PKG-INFO` & `telstra_messaging-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telstra-messaging
-Version: 3.0.2
+Version: 3.0.3
 Summary: SDK for the Telstra Messaging API V3 - Beta
 License: Apache-2.0
 Author: David Andersson
 Author-email: david-andersson@users.noreply.github.com 
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

