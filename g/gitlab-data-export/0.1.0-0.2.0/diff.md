# Comparing `tmp/gitlab_data_export-0.1.0.tar.gz` & `tmp/gitlab_data_export-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_data_export-0.1.0.tar", last modified: Wed Apr 19 14:08:02 2023, max compression
+gzip compressed data, was "gitlab_data_export-0.2.0.tar", last modified: Wed Apr 19 16:24:38 2023, max compression
```

## Comparing `gitlab_data_export-0.1.0.tar` & `gitlab_data_export-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 local     (1000) local     (1000)        0 2023-04-19 14:08:02.535775 gitlab_data_export-0.1.0/
--rw-rw-r--   0 local     (1000) local     (1000)     1065 2023-04-12 13:10:52.000000 gitlab_data_export-0.1.0/LICENSE.txt
--rw-r--r--   0 local     (1000) local     (1000)     7389 2023-04-19 14:08:02.535775 gitlab_data_export-0.1.0/PKG-INFO
--rw-rw-r--   0 local     (1000) local     (1000)     6298 2023-04-19 13:56:00.000000 gitlab_data_export-0.1.0/README.md
-drwxr-xr-x   0 local     (1000) local     (1000)        0 2023-04-19 14:08:02.535775 gitlab_data_export-0.1.0/gitlab_data_export/
--rw-rw-r--   0 local     (1000) local     (1000)        0 2023-04-12 13:10:52.000000 gitlab_data_export-0.1.0/gitlab_data_export/__init__.py
-drwxr-xr-x   0 local     (1000) local     (1000)        0 2023-04-19 14:08:02.535775 gitlab_data_export-0.1.0/gitlab_data_export/api/
--rw-rw-r--   0 local     (1000) local     (1000)        0 2023-04-12 13:10:52.000000 gitlab_data_export-0.1.0/gitlab_data_export/api/__init__.py
--rw-r--r--   0 local     (1000) local     (1000)    22990 2023-04-19 13:53:55.000000 gitlab_data_export-0.1.0/gitlab_data_export/api/bigquery.py
--rw-r--r--   0 local     (1000) local     (1000)     5151 2023-04-19 13:37:57.000000 gitlab_data_export-0.1.0/gitlab_data_export/api/datastore.py
--rw-r--r--   0 local     (1000) local     (1000)     8518 2023-04-19 13:37:57.000000 gitlab_data_export-0.1.0/gitlab_data_export/api/gitlab_export.py
--rw-r--r--   0 local     (1000) local     (1000)     3286 2023-04-19 13:37:57.000000 gitlab_data_export-0.1.0/gitlab_data_export/checkpointing.py
--rw-r--r--   0 local     (1000) local     (1000)     1356 2023-04-19 14:06:17.000000 gitlab_data_export-0.1.0/gitlab_data_export/driver.py
--rw-r--r--   0 local     (1000) local     (1000)     1502 2023-04-19 13:37:57.000000 gitlab_data_export-0.1.0/gitlab_data_export/util.py
-drwxr-xr-x   0 local     (1000) local     (1000)        0 2023-04-19 14:08:02.535775 gitlab_data_export-0.1.0/gitlab_data_export.egg-info/
--rw-r--r--   0 local     (1000) local     (1000)     7389 2023-04-19 14:08:02.000000 gitlab_data_export-0.1.0/gitlab_data_export.egg-info/PKG-INFO
--rw-r--r--   0 local     (1000) local     (1000)      703 2023-04-19 14:08:02.000000 gitlab_data_export-0.1.0/gitlab_data_export.egg-info/SOURCES.txt
--rw-r--r--   0 local     (1000) local     (1000)        1 2023-04-19 14:08:02.000000 gitlab_data_export-0.1.0/gitlab_data_export.egg-info/dependency_links.txt
--rw-r--r--   0 local     (1000) local     (1000)       70 2023-04-19 14:08:02.000000 gitlab_data_export-0.1.0/gitlab_data_export.egg-info/entry_points.txt
--rw-r--r--   0 local     (1000) local     (1000)      130 2023-04-19 14:08:02.000000 gitlab_data_export-0.1.0/gitlab_data_export.egg-info/requires.txt
--rw-r--r--   0 local     (1000) local     (1000)       25 2023-04-19 14:08:02.000000 gitlab_data_export-0.1.0/gitlab_data_export.egg-info/top_level.txt
--rw-rw-r--   0 local     (1000) local     (1000)       78 2023-04-19 14:08:02.535775 gitlab_data_export-0.1.0/setup.cfg
--rw-rw-r--   0 local     (1000) local     (1000)     1782 2023-04-19 13:58:47.000000 gitlab_data_export-0.1.0/setup.py
-drwxr-xr-x   0 local     (1000) local     (1000)        0 2023-04-19 14:08:02.535775 gitlab_data_export-0.1.0/tests/
--rw-rw-r--   0 local     (1000) local     (1000)        0 2023-04-12 13:10:52.000000 gitlab_data_export-0.1.0/tests/__init__.py
-drwxr-xr-x   0 local     (1000) local     (1000)        0 2023-04-19 14:08:02.535775 gitlab_data_export-0.1.0/tests/api/
--rw-rw-r--   0 local     (1000) local     (1000)        0 2023-04-12 13:10:52.000000 gitlab_data_export-0.1.0/tests/api/__init__.py
--rw-rw-r--   0 local     (1000) local     (1000)     1519 2023-04-12 13:10:52.000000 gitlab_data_export-0.1.0/tests/api/test_gitlab_export.py
--rw-r--r--   0 local     (1000) local     (1000)     1606 2023-04-12 15:19:34.000000 gitlab_data_export-0.1.0/tests/test_checkpointing.py
--rw-rw-r--   0 local     (1000) local     (1000)      968 2023-04-12 13:10:52.000000 gitlab_data_export-0.1.0/tests/test_driver.py
--rw-r--r--   0 local     (1000) local     (1000)     1038 2023-04-19 13:37:57.000000 gitlab_data_export-0.1.0/tests/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7735 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6644 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.916166 gitlab_data_export-0.2.0/gitlab_data_export/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/gitlab_data_export/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21990 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/api/bigquery.py
+-rw-rw-rw-   0 root         (0) root         (0)     5151 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/api/datastore.py
+-rw-rw-rw-   0 root         (0) root         (0)     8897 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/api/gitlab_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     3286 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/checkpointing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/driver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2517 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/gitlab_data_export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.916166 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7735 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      703 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-19 16:24:38.000000 gitlab_data_export-0.2.0/gitlab_data_export.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:38.917166 gitlab_data_export-0.2.0/tests/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/api/test_gitlab_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/test_checkpointing.py
+-rw-rw-rw-   0 root         (0) root         (0)      968 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/test_driver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2023-04-19 16:24:16.000000 gitlab_data_export-0.2.0/tests/test_util.py
```

### Comparing `gitlab_data_export-0.1.0/LICENSE.txt` & `gitlab_data_export-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.1.0/PKG-INFO` & `gitlab_data_export-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab_data_export
-Version: 0.1.0
+Version: 0.2.0
 Summary: Export GitLab data to external data stores
 Home-page: https://gitlab.com/belvederetrading/public/gitlab-data-export
 Author: Belvedere Trading
 Project-URL: Bug Reports, https://gitlab.com/belvederetrading/public/gitlab-data-export/-/issues
 Project-URL: Source, https://gitlab.com/belvederetrading/public/gitlab-data-export
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -60,15 +60,15 @@
 
 ```yaml
 gitlab_export:
   image: python:3.11
   interruptible: true
   needs: []
   before_script:
-    - python3.11 -m pip install .[dev]
+    - python3.11 -m pip install gitlab_data_export --upgrade
   script:
     - python3.11 -m gitlab_data_export.driver
   cache:
     key: global
     paths:
       - gde_checkpoint.json
   rules:
@@ -105,17 +105,18 @@
     * `GITLAB_GROUP`, if set, should contain a fully-qualified path to a GitLab group
     * `GITLAB_PROJECT`, if set, should contain a fully-qualified path to a GitLab project
 
 ### Optional
 
 * `GITLAB_URL`: override the GitLab instance from which data should be exported
     * Defaults to `https://gitlab.com` if unset
-
-* Disabling historical backfill
-* Disabline group recursion
+* `GITLAB_BACKFILL_TIMESTAMP`: if set, overrides the default historical backfill behavior by limiting the
+  `updated_after` time of GitLab resources. Accepted values are either `now` or a timestamp in `%Y-%m-%d %H:%M:%S`
+  format. `now` disables backfill completely, while a timestamp limits backfill
+* `GITLAB_NO_RECURSION`: if set (to any value), completely disables group recursion
 
 ## Data storage design
 
 Data is treated as append-only. Once written, records are _never_ modified or deleted. In addition to the data
 retrieved from the API, every record is enriched with a `data_date` field that users can rely upon in analytical
 queries, representing the time at which the records were loaded into BigQuery.
```

### Comparing `gitlab_data_export-0.1.0/README.md` & `gitlab_data_export-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 ```yaml
 gitlab_export:
   image: python:3.11
   interruptible: true
   needs: []
   before_script:
-    - python3.11 -m pip install .[dev]
+    - python3.11 -m pip install gitlab_data_export --upgrade
   script:
     - python3.11 -m gitlab_data_export.driver
   cache:
     key: global
     paths:
       - gde_checkpoint.json
   rules:
@@ -80,17 +80,18 @@
     * `GITLAB_GROUP`, if set, should contain a fully-qualified path to a GitLab group
     * `GITLAB_PROJECT`, if set, should contain a fully-qualified path to a GitLab project
 
 ### Optional
 
 * `GITLAB_URL`: override the GitLab instance from which data should be exported
     * Defaults to `https://gitlab.com` if unset
-
-* Disabling historical backfill
-* Disabline group recursion
+* `GITLAB_BACKFILL_TIMESTAMP`: if set, overrides the default historical backfill behavior by limiting the
+  `updated_after` time of GitLab resources. Accepted values are either `now` or a timestamp in `%Y-%m-%d %H:%M:%S`
+  format. `now` disables backfill completely, while a timestamp limits backfill
+* `GITLAB_NO_RECURSION`: if set (to any value), completely disables group recursion
 
 ## Data storage design
 
 Data is treated as append-only. Once written, records are _never_ modified or deleted. In addition to the data
 retrieved from the API, every record is enriched with a `data_date` field that users can rely upon in analytical
 queries, representing the time at which the records were loaded into BigQuery.
```

### Comparing `gitlab_data_export-0.1.0/gitlab_data_export/api/bigquery.py` & `gitlab_data_export-0.2.0/gitlab_data_export/api/bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,25 +41,22 @@
         bigquery.SchemaField('state', 'STRING'),
         bigquery.SchemaField('avatar_url', 'STRING'),
         bigquery.SchemaField('web_url', 'STRING')
     ]),
     bigquery.SchemaField('start_date', 'DATE'),
     bigquery.SchemaField('start_date_is_fixed', 'BOOLEAN'),
     bigquery.SchemaField('start_date_fixed', 'DATE'),
-    bigquery.SchemaField('start_date_from_milestones',
-                         'DATE'),
-    bigquery.SchemaField('start_date_from_inherited_source',
-                         'DATE'),
+    bigquery.SchemaField('start_date_from_milestones', 'DATE'),
+    bigquery.SchemaField('start_date_from_inherited_source', 'DATE'),
     bigquery.SchemaField('end_date', 'DATE'),
     bigquery.SchemaField('due_date', 'DATE'),
     bigquery.SchemaField('due_date_is_fixed', 'BOOLEAN'),
     bigquery.SchemaField('due_date_fixed', 'DATE'),
     bigquery.SchemaField('due_date_from_milestones', 'DATE'),
-    bigquery.SchemaField('due_date_from_inherited_source',
-                         'DATE'),
+    bigquery.SchemaField('due_date_from_inherited_source', 'DATE'),
     bigquery.SchemaField('created_at', 'TIMESTAMP', mode='REQUIRED'),
     bigquery.SchemaField('updated_at', 'TIMESTAMP', mode='REQUIRED'),
     bigquery.SchemaField("closed_at", "TIMESTAMP"),
     bigquery.SchemaField('labels', 'STRING', mode='REPEATED'),
     bigquery.SchemaField('upvotes', 'INTEGER'),
     bigquery.SchemaField('downvotes', 'INTEGER'),
     bigquery.SchemaField('color', 'STRING'),
@@ -211,55 +208,51 @@
     bigquery.SchemaField('data_date', 'TIMESTAMP', mode='REQUIRED'),
     bigquery.SchemaField('id', 'INTEGER', mode='REQUIRED'),
     bigquery.SchemaField('iid', 'INTEGER', mode='REQUIRED'),
     bigquery.SchemaField('state', 'STRING', mode='REQUIRED'),
     bigquery.SchemaField('type', 'STRING'),
     bigquery.SchemaField('title', 'STRING'),
     bigquery.SchemaField('description', 'STRING'),
-    bigquery.SchemaField('author', 'RECORD', mode='REQUIRED',
-                         fields=[
-                             bigquery.SchemaField('state', 'STRING'),
-                             bigquery.SchemaField('id', 'INTEGER'),
-                             bigquery.SchemaField('web_url', 'STRING'),
-                             bigquery.SchemaField('name', 'STRING'),
-                             bigquery.SchemaField('avatar_url', 'STRING'),
-                             bigquery.SchemaField('username', 'STRING'),
-                         ]),
-    bigquery.SchemaField('milestone', 'RECORD',
-                         fields=[
-                             bigquery.SchemaField('project_id', 'INTEGER'),
-                             bigquery.SchemaField('description', 'STRING'),
-                             bigquery.SchemaField('state', 'STRING'),
-                             bigquery.SchemaField('due_date', 'DATE'),
-                             bigquery.SchemaField('iid', 'INTEGER'),
-                             bigquery.SchemaField('created_at', 'TIMESTAMP'),
-                             bigquery.SchemaField('title', 'STRING'),
-                             bigquery.SchemaField('id', 'INTEGER'),
-                             bigquery.SchemaField('updated_at', 'TIMESTAMP'),
-                         ]),
+    bigquery.SchemaField('author', 'RECORD', mode='REQUIRED', fields=[
+        bigquery.SchemaField('state', 'STRING'),
+        bigquery.SchemaField('id', 'INTEGER'),
+        bigquery.SchemaField('web_url', 'STRING'),
+        bigquery.SchemaField('name', 'STRING'),
+        bigquery.SchemaField('avatar_url', 'STRING'),
+        bigquery.SchemaField('username', 'STRING'),
+    ]),
+    bigquery.SchemaField('milestone', 'RECORD', fields=[
+        bigquery.SchemaField('project_id', 'INTEGER'),
+        bigquery.SchemaField('description', 'STRING'),
+        bigquery.SchemaField('state', 'STRING'),
+        bigquery.SchemaField('due_date', 'DATE'),
+        bigquery.SchemaField('iid', 'INTEGER'),
+        bigquery.SchemaField('created_at', 'TIMESTAMP'),
+        bigquery.SchemaField('title', 'STRING'),
+        bigquery.SchemaField('id', 'INTEGER'),
+        bigquery.SchemaField('updated_at', 'TIMESTAMP'),
+    ]),
     bigquery.SchemaField('project_id', 'INTEGER', mode='REQUIRED'),
     bigquery.SchemaField('project_name', 'STRING', mode='REQUIRED'),
-    bigquery.SchemaField('assignees', 'RECORD',
-                         fields=[
-                             bigquery.SchemaField('state', 'STRING'),
-                             bigquery.SchemaField('id', 'INTEGER'),
-                             bigquery.SchemaField('name', 'STRING'),
-                             bigquery.SchemaField('web_url', 'STRING'),
-                             bigquery.SchemaField('avatar_url', 'STRING'),
-                             bigquery.SchemaField('username', 'STRING'),
-                         ], mode='REPEATED'),
-    bigquery.SchemaField('assignee', 'RECORD',
-                         fields=[
-                             bigquery.SchemaField('state', 'STRING'),
-                             bigquery.SchemaField('id', 'INTEGER'),
-                             bigquery.SchemaField('name', 'STRING'),
-                             bigquery.SchemaField('web_url', 'STRING'),
-                             bigquery.SchemaField('avatar_url', 'STRING'),
-                             bigquery.SchemaField('username', 'STRING'),
-                         ]),
+    bigquery.SchemaField('assignees', 'RECORD', fields=[
+        bigquery.SchemaField('state', 'STRING'),
+        bigquery.SchemaField('id', 'INTEGER'),
+        bigquery.SchemaField('name', 'STRING'),
+        bigquery.SchemaField('web_url', 'STRING'),
+        bigquery.SchemaField('avatar_url', 'STRING'),
+        bigquery.SchemaField('username', 'STRING'),
+    ], mode='REPEATED'),
+    bigquery.SchemaField('assignee', 'RECORD', fields=[
+        bigquery.SchemaField('state', 'STRING'),
+        bigquery.SchemaField('id', 'INTEGER'),
+        bigquery.SchemaField('name', 'STRING'),
+        bigquery.SchemaField('web_url', 'STRING'),
+        bigquery.SchemaField('avatar_url', 'STRING'),
+        bigquery.SchemaField('username', 'STRING'),
+    ]),
     bigquery.SchemaField('updated_at', 'TIMESTAMP', mode='REQUIRED'),
     bigquery.SchemaField('closed_at', 'TIMESTAMP'),
     bigquery.SchemaField('closed_by', 'RECORD', fields=[
         bigquery.SchemaField('id', 'INTEGER'),
         bigquery.SchemaField('name', 'STRING'),
         bigquery.SchemaField('state', 'STRING'),
         bigquery.SchemaField('web_url', 'STRING'),
@@ -280,30 +273,28 @@
         bigquery.SchemaField('relative', 'STRING'),
         bigquery.SchemaField('full', 'STRING')
     ]),
     bigquery.SchemaField('time_stats', 'RECORD', fields=[
         bigquery.SchemaField('time_estimate', 'INTEGER'),
         bigquery.SchemaField('total_time_spent', 'INTEGER'),
         bigquery.SchemaField('human_time_estimate', 'STRING'),
-        bigquery.SchemaField('human_total_time_spent',
-                             'STRING')
+        bigquery.SchemaField('human_total_time_spent', 'STRING')
     ]),
     bigquery.SchemaField('has_tasks', 'BOOLEAN'),
     bigquery.SchemaField('task_status', 'STRING'),
     bigquery.SchemaField('confidential', 'BOOLEAN'),
     bigquery.SchemaField('discussion_locked', 'BOOLEAN'),
     bigquery.SchemaField('issue_type', 'STRING'),
     bigquery.SchemaField('severity', 'STRING'),
     bigquery.SchemaField('_links', 'RECORD', fields=[
         bigquery.SchemaField('self', 'STRING'),
         bigquery.SchemaField('notes', 'STRING'),
         bigquery.SchemaField('award_emoji', 'STRING'),
         bigquery.SchemaField('project', 'STRING'),
-        bigquery.SchemaField('closed_as_duplicate_of',
-                             'STRING')
+        bigquery.SchemaField('closed_as_duplicate_of', 'STRING')
     ]),
     bigquery.SchemaField('task_completion_status', 'RECORD', fields=[
         bigquery.SchemaField('count', 'INTEGER'),
         bigquery.SchemaField('completed_count', 'INTEGER')
     ])
 ]
 
@@ -484,14 +475,7 @@
     def insert_merge_requests(self, data_date: datetime, project_name: str, merge_requests: Iterable[Dict[str, Any]]) -> Result:
         logging.info('Inserting Merge Requests; Dataset=%s' % self.fq_dataset)
         for mr in merge_requests:
             mr['data_date'] = format_time(data_date)
             mr['project_name'] = project_name
 
         return check_errors(self._durable_insert(self.tables.merge_requests, merge_requests))
-
-
-if __name__ == '__main__':
-    import dotenv
-    dotenv.load_dotenv()
-    bq = BigQuery()
-    bq.ensure_storage()
```

### Comparing `gitlab_data_export-0.1.0/gitlab_data_export/api/datastore.py` & `gitlab_data_export-0.2.0/gitlab_data_export/api/datastore.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.1.0/gitlab_data_export/api/gitlab_export.py` & `gitlab_data_export-0.2.0/gitlab_data_export/api/gitlab_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-"""Interaction with GitLab's REST API.
-"""
+"""Interaction with GitLab's REST API."""
 import logging
 import os
 from datetime import datetime
 from enum import Enum
 from typing import (Any, Callable, Dict, Iterable,
                     Optional, List, Tuple, TypeVar, Union)
 
 import gitlab
 import gitlab.base
 
 from ..checkpointing import Checkpoint
-from ..util import format_time, Result
+from ..util import format_time, parse_time, ExportOptions, Result
 from .datastore import Datastore
 
 
 class AuthType(Enum):
     """GitLab authentication types.
     """
     GITLAB_TOKEN = 1
@@ -81,14 +80,24 @@
 GitlabRestResponse = Union[gitlab.base.RESTObjectList,
                            List[gitlab.base.RESTObject]]
 RESOURCES_PER_PAGE = 100
 
 
 def paginated(after: datetime, before: datetime,
               query: Callable[..., GitlabRestResponse]) -> Iterable[List[Dict[str, Any]]]:
+    """Automatically paginates the results of a GitLab REST operation.
+
+    Args:
+        after: an earliest time bound for GitLab resource modifications
+        before: a latest time bound for GitLab resource modifications
+        query: the GitLab REST operation to run
+
+    Returns:
+        Iterable[List[Dict[str, Any]]]: chunks of results yielded by the GitLab API
+    """
     page = 1
     while True:
         page_results = query(updated_after=format_time(after),
                              updated_before=format_time(before),
                              per_page=RESOURCES_PER_PAGE,
                              page=page)
         yield [result.asdict() for result in page_results]
@@ -104,42 +113,33 @@
     elif auth_type == AuthType.GITLAB_OAUTH:
         return {'oauth_token': cred}
     raise NotImplementedError(
         f'Unimplemented authentication type: {auth_type.name}')
 
 
 class Gitlab:
-    """
-    Semantic access to GitLab's REST API.
+    """Semantic access to GitLab's REST API.
 
     This class is not meant to be a general-purpose API; it supports only the semantic operations
     required for data export functionality.
     """
     GITLAB_DEFAULT_URL = 'https://gitlab.com'
     GITLAB_URL_VAR = 'GITLAB_URL'
 
     def __init__(self, url: Optional[str] = None, auth: Optional[Auth] = None,
-                 resource: Optional[Resource] = None):
+                 resource: Optional[Resource] = None, options: Optional[ExportOptions] = None):
         self.url = url or os.getenv(
             self.GITLAB_URL_VAR, self.GITLAB_DEFAULT_URL)
         logging.debug('Initializing GitLab API connection to %s' % self.url)
         self.auth = auth or auth_from_env()
         self.resource = resource or resource_from_env()
+        self.options = options or ExportOptions.from_env()
         self.gitlab = gitlab.Gitlab(self.url, **_kwargs_from_auth(self.auth))
         self.gitlab.auth()
 
-    def print_users(self):
-        bt = self.gitlab.groups.get('belvederetrading')
-        for group in bt.descendant_groups.list(all=True):
-            group.pprint()
-
-    def get_epics(self):
-        group = self.gitlab.groups.get('belvederetrading/public')
-        return [group.epics.get(1).asdict()]
-
     def _export_project(self, project_id: str, datastore: Datastore, since: datetime,
                         until: datetime) -> Result:
         logging.info('Exporting project data; Project=%s; Since=%s; Until=%s' %
                      (project_id, format_time(since), format_time(until)))
         result = Result.success()
         project = self.gitlab.projects.get(project_id)
 
@@ -186,21 +186,25 @@
         for milestones in paginated(since, until, group.milestones.list):
             if milestones:
                 records += len(milestones)
                 result.bind(datastore.insert_milestones(
                     until, group_id, milestones))
         logging.info('Inserted Milestones; Count=%s' % records)
 
-        for project in group.projects.list():
-            result.bind(self._export_project(
-                project.path_with_namespace, datastore, since, until))
-
-        for subgroup in group.subgroups.list():
-            result.bind(self._export_group(subgroup.full_path,
-                                           datastore, since, until))
+        if self.options.recursion_enabled:
+            for project in group.projects.list():
+                result.bind(self._export_project(
+                    project.path_with_namespace, datastore, since, until))
+
+            for subgroup in group.subgroups.list():
+                result.bind(self._export_group(subgroup.full_path,
+                                               datastore, since, until))
+        else:
+            logging.info(
+                'Group recursion disabled, skipping subgroups and subprojects')
 
         return result
 
     def export_data(self, datastore: Datastore, checkpoint: Optional[Checkpoint],
                     now=None) -> Result:
         """Exports data to an external store based on the previous checkpoint.
 
@@ -210,16 +214,16 @@
 
         Args:
             datastore: a Datastore implementation
             checkpoint: the prior Checkpoint
             now: a datetime representing the current time in UTC
         """
         now = now or datetime.utcnow()
-        since = checkpoint.previous if checkpoint is not None else datetime(
-            1970, 1, 1)
+        since = checkpoint.previous if checkpoint is not None else self.options.backfill_timestamp
+
         resource_type, identifier = self.resource
         result = Result.success()
         if resource_type == ResourceType.GITLAB_PROJECT:
             result.bind(self._export_project(
                 identifier, datastore, since, now))
         elif resource_type == ResourceType.GITLAB_GROUP:
             result.bind(self._export_group(
```

### Comparing `gitlab_data_export-0.1.0/gitlab_data_export/checkpointing.py` & `gitlab_data_export-0.2.0/gitlab_data_export/checkpointing.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 its previous invocation. This information is used by subsequent invocations to
 export only data that has changed since the prior invocation. Combined with the
 materialized `data_date` field available within all exported data, this design
 ensures that previously written data need never be updated while also providing
 historical analytic capabilities to users of the exported data.
 """
 from __future__ import annotations
-from datetime import datetime
 import json
 import logging
 import os
+from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 from .util import TIMESTAMP_FORMAT, format_time
 
 CHECKPOINT_ENV_VAR = 'GDE_CHECKPOINT_PATH'
```

### Comparing `gitlab_data_export-0.1.0/gitlab_data_export/driver.py` & `gitlab_data_export-0.2.0/gitlab_data_export/driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Drivers of data export functionality."""
-from enum import Enum
+"""Executable module to drive data export functionality."""
 import logging
 import os
+from enum import Enum
 from typing import Callable
 
 from .api.bigquery import BigQuery
 from .api.datastore import Datastore
 from .api.gitlab_export import Gitlab
 from .checkpointing import Checkpoint
```

### Comparing `gitlab_data_export-0.1.0/gitlab_data_export.egg-info/PKG-INFO` & `gitlab_data_export-0.2.0/gitlab_data_export.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-data-export
-Version: 0.1.0
+Version: 0.2.0
 Summary: Export GitLab data to external data stores
 Home-page: https://gitlab.com/belvederetrading/public/gitlab-data-export
 Author: Belvedere Trading
 Project-URL: Bug Reports, https://gitlab.com/belvederetrading/public/gitlab-data-export/-/issues
 Project-URL: Source, https://gitlab.com/belvederetrading/public/gitlab-data-export
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -60,15 +60,15 @@
 
 ```yaml
 gitlab_export:
   image: python:3.11
   interruptible: true
   needs: []
   before_script:
-    - python3.11 -m pip install .[dev]
+    - python3.11 -m pip install gitlab_data_export --upgrade
   script:
     - python3.11 -m gitlab_data_export.driver
   cache:
     key: global
     paths:
       - gde_checkpoint.json
   rules:
@@ -105,17 +105,18 @@
     * `GITLAB_GROUP`, if set, should contain a fully-qualified path to a GitLab group
     * `GITLAB_PROJECT`, if set, should contain a fully-qualified path to a GitLab project
 
 ### Optional
 
 * `GITLAB_URL`: override the GitLab instance from which data should be exported
     * Defaults to `https://gitlab.com` if unset
-
-* Disabling historical backfill
-* Disabline group recursion
+* `GITLAB_BACKFILL_TIMESTAMP`: if set, overrides the default historical backfill behavior by limiting the
+  `updated_after` time of GitLab resources. Accepted values are either `now` or a timestamp in `%Y-%m-%d %H:%M:%S`
+  format. `now` disables backfill completely, while a timestamp limits backfill
+* `GITLAB_NO_RECURSION`: if set (to any value), completely disables group recursion
 
 ## Data storage design
 
 Data is treated as append-only. Once written, records are _never_ modified or deleted. In addition to the data
 retrieved from the API, every record is enriched with a `data_date` field that users can rely upon in analytical
 queries, representing the time at which the records were loaded into BigQuery.
```

### Comparing `gitlab_data_export-0.1.0/gitlab_data_export.egg-info/SOURCES.txt` & `gitlab_data_export-0.2.0/gitlab_data_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.1.0/setup.py` & `gitlab_data_export-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
 from typing import List
+import os
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 requirements: List[str] = [
     'google-cloud-bigquery>=3.0.0,<4',
     'python-gitlab>=3.0.0,<4'
 ]
 
+version = os.getenv('CI_COMMIT_TAG', 'v0.0.1').strip('v')
+
 setup(
     name='gitlab_data_export',
-    version='0.1.0',
+    version=version,
     description='Export GitLab data to external data stores',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.com/belvederetrading/public/gitlab-data-export',
     author='Belvedere Trading',
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `gitlab_data_export-0.1.0/tests/api/test_gitlab_export.py` & `gitlab_data_export-0.2.0/tests/api/test_gitlab_export.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.1.0/tests/test_checkpointing.py` & `gitlab_data_export-0.2.0/tests/test_checkpointing.py`

 * *Files identical despite different names*

### Comparing `gitlab_data_export-0.1.0/tests/test_driver.py` & `gitlab_data_export-0.2.0/tests/test_driver.py`

 * *Files identical despite different names*

