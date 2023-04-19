# Comparing `tmp/gitlab_data_export-0.2.0.tar.gz` & `tmp/gitlab_data_export-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_data_export-0.2.0.tar", last modified: Wed Apr 19 16:24:38 2023, max compression
+gzip compressed data, was "gitlab_data_export-0.3.0.tar", last modified: Wed Apr 19 20:54:46 2023, max compression
```

## Comparing `gitlab_data_export-0.2.0.tar` & `gitlab_data_export-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7735 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6644 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.916166 gitlab_data_export-0.2.0/gitlab_data_export/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/gitlab_data_export/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21990 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/api/bigquery.py
--rw-rw-rw-   0 root         (0) root         (0)     5151 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/api/datastore.py
--rw-rw-rw-   0 root         (0) root         (0)     8897 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/api/gitlab_export.py
--rw-rw-rw-   0 root         (0) root         (0)     3286 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/checkpointing.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/driver.py
--rw-rw-rw-   0 root         (0) root         (0)     2517 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.916166 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7735 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      703 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/tests/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1519 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/api/test_gitlab_export.py
--rw-rw-rw-   0 root         (0) root         (0)     1606 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/test_checkpointing.py
--rw-rw-rw-   0 root         (0) root         (0)      968 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/test_driver.py
--rw-rw-rw-   0 root         (0) root         (0)     2411 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:54:46.709637 gitlab_data_export-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7735 2023-04-19 20:54:46.709637 gitlab_data_export-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6644 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:54:46.707636 gitlab_data_export-0.3.0/gitlab_data_export/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/gitlab_data_export/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:54:46.708637 gitlab_data_export-0.3.0/gitlab_data_export/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/gitlab_data_export/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23111 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/gitlab_data_export/api/bigquery.py
+-rw-rw-rw-   0 root         (0) root         (0)     5151 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/gitlab_data_export/api/datastore.py
+-rw-rw-rw-   0 root         (0) root         (0)     8950 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/gitlab_data_export/api/gitlab_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     3286 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/gitlab_data_export/checkpointing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/gitlab_data_export/driver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/gitlab_data_export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:54:46.707636 gitlab_data_export-0.3.0/gitlab_data_export.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7735 2023-04-19 20:54:46.000000 gitlab_data_export-0.3.0/gitlab_data_export.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      703 2023-04-19 20:54:46.000000 gitlab_data_export-0.3.0/gitlab_data_export.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 20:54:46.000000 gitlab_data_export-0.3.0/gitlab_data_export.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-19 20:54:46.000000 gitlab_data_export-0.3.0/gitlab_data_export.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-04-19 20:54:46.000000 gitlab_data_export-0.3.0/gitlab_data_export.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-19 20:54:46.000000 gitlab_data_export-0.3.0/gitlab_data_export.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-19 20:54:46.709637 gitlab_data_export-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:54:46.708637 gitlab_data_export-0.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:54:46.709637 gitlab_data_export-0.3.0/tests/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/tests/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/tests/api/test_gitlab_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/tests/test_checkpointing.py
+-rw-rw-rw-   0 root         (0) root         (0)      968 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/tests/test_driver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2023-04-19 20:54:17.000000 gitlab_data_export-0.3.0/tests/test_util.py
```

### Comparing `gitlab_data_export-0.2.0/LICENSE.txt` & `gitlab_data_export-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/PKG-INFO` & `gitlab_data_export-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab_data_export
-Version: 0.2.0
+Version: 0.3.0
 Summary: Export GitLab data to external data stores
 Home-page: https://gitlab.com/belvederetrading/public/gitlab-data-export
 Author: Belvedere Trading
 Project-URL: Bug Reports, https://gitlab.com/belvederetrading/public/gitlab-data-export/-/issues
 Project-URL: Source, https://gitlab.com/belvederetrading/public/gitlab-data-export
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `gitlab_data_export-0.2.0/README.md` & `gitlab_data_export-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/gitlab_data_export/api/bigquery.py` & `gitlab_data_export-0.3.0/gitlab_data_export/api/bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,36 @@
     bigquery.SchemaField('labels', 'STRING', mode='REPEATED'),
     bigquery.SchemaField('upvotes', 'INTEGER'),
     bigquery.SchemaField('downvotes', 'INTEGER'),
     bigquery.SchemaField('merge_requests_count', 'INTEGER'),
     bigquery.SchemaField('user_notes_count', 'INTEGER'),
     bigquery.SchemaField('due_date', 'DATE'),
     bigquery.SchemaField('web_url', 'STRING'),
+    bigquery.SchemaField('weight', 'INTEGER'),
+    bigquery.SchemaField('epic', 'RECORD', fields=[
+        bigquery.SchemaField('id', 'INTEGER', mode='REQUIRED'),
+        bigquery.SchemaField('iid', 'INTEGER', mode='REQUIRED'),
+        bigquery.SchemaField('title', 'STRING', mode='REQUIRED'),
+        bigquery.SchemaField('url', 'STRING', mode='REQUIRED'),
+        bigquery.SchemaField('group_id', 'INTEGER', mode='REQUIRED')
+    ]),
+    bigquery.SchemaField('iteration', 'RECORD', fields=[
+        bigquery.SchemaField('id', 'INTEGER'),
+        bigquery.SchemaField('iid', 'INTEGER'),
+        bigquery.SchemaField('sequence', 'INTEGER'),
+        bigquery.SchemaField('group_id', 'INTEGER'),
+        bigquery.SchemaField('title', 'STRING'),
+        bigquery.SchemaField('description', 'STRING'),
+        bigquery.SchemaField('state', 'INTEGER'),
+        bigquery.SchemaField('created_at', 'TIMESTAMP'),
+        bigquery.SchemaField('updated_at', 'TIMESTAMP'),
+        bigquery.SchemaField('start_date', 'DATE'),
+        bigquery.SchemaField('due_date', 'DATE'),
+        bigquery.SchemaField('web_url', 'STRING')
+    ]),
     bigquery.SchemaField('references', 'RECORD', fields=[
         bigquery.SchemaField('short', 'STRING'),
         bigquery.SchemaField('relative', 'STRING'),
         bigquery.SchemaField('full', 'STRING')
     ]),
     bigquery.SchemaField('time_stats', 'RECORD', fields=[
         bigquery.SchemaField('time_estimate', 'INTEGER'),
```

### Comparing `gitlab_data_export-0.2.0/gitlab_data_export/api/datastore.py` & `gitlab_data_export-0.3.0/gitlab_data_export/api/datastore.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/gitlab_data_export/api/gitlab_export.py` & `gitlab_data_export-0.3.0/gitlab_data_export/api/gitlab_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,18 @@
         will be inserted.
 
         Args:
             datastore: a Datastore implementation
             checkpoint: the prior Checkpoint
             now: a datetime representing the current time in UTC
         """
+        datastore.ensure_storage()
         now = now or datetime.utcnow()
-        since = checkpoint.previous if checkpoint is not None else self.options.backfill_timestamp
+        since = checkpoint.previous if checkpoint is not None else self.options.backfill_timestamp(
+            now)
 
         resource_type, identifier = self.resource
         result = Result.success()
         if resource_type == ResourceType.GITLAB_PROJECT:
             result.bind(self._export_project(
                 identifier, datastore, since, now))
         elif resource_type == ResourceType.GITLAB_GROUP:
```

### Comparing `gitlab_data_export-0.2.0/gitlab_data_export/checkpointing.py` & `gitlab_data_export-0.3.0/gitlab_data_export/checkpointing.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/gitlab_data_export/driver.py` & `gitlab_data_export-0.3.0/gitlab_data_export/driver.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/gitlab_data_export/util.py` & `gitlab_data_export-0.3.0/gitlab_data_export/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Ubiquitously useful utilities."""
 from __future__ import annotations
 import logging
 import os
 import sys
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Optional
 
 TIMESTAMP_FORMAT = '%Y-%m-%d %H:%M:%S'
 
 
 def format_time(dt: datetime) -> str:
     """Formats a datetime to ISO standard format."""
     return dt.strftime(TIMESTAMP_FORMAT)
```

### Comparing `gitlab_data_export-0.2.0/gitlab_data_export.egg-info/PKG-INFO` & `gitlab_data_export-0.3.0/gitlab_data_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-data-export
-Version: 0.2.0
+Version: 0.3.0
 Summary: Export GitLab data to external data stores
 Home-page: https://gitlab.com/belvederetrading/public/gitlab-data-export
 Author: Belvedere Trading
 Project-URL: Bug Reports, https://gitlab.com/belvederetrading/public/gitlab-data-export/-/issues
 Project-URL: Source, https://gitlab.com/belvederetrading/public/gitlab-data-export
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `gitlab_data_export-0.2.0/gitlab_data_export.egg-info/SOURCES.txt` & `gitlab_data_export-0.3.0/gitlab_data_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/setup.py` & `gitlab_data_export-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/tests/api/test_gitlab_export.py` & `gitlab_data_export-0.3.0/tests/api/test_gitlab_export.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/tests/test_checkpointing.py` & `gitlab_data_export-0.3.0/tests/test_checkpointing.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/tests/test_driver.py` & `gitlab_data_export-0.3.0/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.2.0/tests/test_util.py` & `gitlab_data_export-0.3.0/tests/test_util.py`

 * *Files identical despite different names*

