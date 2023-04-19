# Comparing `tmp/dbsqlclone-0.1.8-py3-none-any.whl.zip` & `tmp/dbsqlclone-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9951 bytes, number of entries: 12
+Zip file size: 10047 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        2 b- defN 23-Jan-11 16:51 dbsqlclone/__init__.py
 -rw-r--r--  2.0 unx     1757 b- defN 23-Jan-11 11:52 dbsqlclone/clone_resources.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-08 07:26 dbsqlclone/utils/__init__.py
 -rw-r--r--  2.0 unx      618 b- defN 23-Jan-11 11:11 dbsqlclone/utils/client.py
--rw-r--r--  2.0 unx     4961 b- defN 23-Jan-11 12:51 dbsqlclone/utils/clone_dashboard.py
--rw-r--r--  2.0 unx     2643 b- defN 23-Jan-16 14:36 dbsqlclone/utils/dump_dashboard.py
--rw-r--r--  2.0 unx    11079 b- defN 23-Jan-17 17:02 dbsqlclone/utils/load_dashboard.py
--rw-r--r--  2.0 unx     3437 b- defN 23-Jan-17 17:03 dbsqlclone-0.1.8.dist-info/LICENCE
--rw-r--r--  2.0 unx      140 b- defN 23-Jan-17 17:03 dbsqlclone-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-17 17:03 dbsqlclone-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jan-17 17:03 dbsqlclone-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1001 b- defN 23-Jan-17 17:03 dbsqlclone-0.1.8.dist-info/RECORD
-12 files, 25741 bytes uncompressed, 8253 bytes compressed:  67.9%
+-rw-r--r--  2.0 unx     4961 b- defN 23-Jan-24 13:57 dbsqlclone/utils/clone_dashboard.py
+-rw-r--r--  2.0 unx     2783 b- defN 23-Jan-20 10:39 dbsqlclone/utils/dump_dashboard.py
+-rw-r--r--  2.0 unx    11403 b- defN 23-Jan-25 09:57 dbsqlclone/utils/load_dashboard.py
+-rw-r--r--  2.0 unx     3437 b- defN 23-Jan-25 10:05 dbsqlclone-0.1.9.dist-info/LICENCE
+-rw-r--r--  2.0 unx      140 b- defN 23-Jan-25 10:05 dbsqlclone-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-25 10:05 dbsqlclone-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jan-25 10:05 dbsqlclone-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1001 b- defN 23-Jan-25 10:05 dbsqlclone-0.1.9.dist-info/RECORD
+12 files, 26205 bytes uncompressed, 8349 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: dbsqlclone/utils/dump_dashboard.py
 Comment: 
 
 Filename: dbsqlclone/utils/load_dashboard.py
 Comment: 
 
-Filename: dbsqlclone-0.1.8.dist-info/LICENCE
+Filename: dbsqlclone-0.1.9.dist-info/LICENCE
 Comment: 
 
-Filename: dbsqlclone-0.1.8.dist-info/METADATA
+Filename: dbsqlclone-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: dbsqlclone-0.1.8.dist-info/WHEEL
+Filename: dbsqlclone-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: dbsqlclone-0.1.8.dist-info/top_level.txt
+Filename: dbsqlclone-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dbsqlclone-0.1.8.dist-info/RECORD
+Filename: dbsqlclone-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dbsqlclone/utils/dump_dashboard.py

```diff
@@ -23,19 +23,21 @@
 
 def get_dashboard_definition_by_id(source_client: Client, dashboard_id):
     logging.debug(f"getting dashboard definition from {dashboard_id}...")
     result = {"queries": [], "id": dashboard_id}
     dashboard = requests.get(source_client.url+"/api/2.0/preview/sql/dashboards/"+dashboard_id, headers = source_client.headers).json()
     result["dashboard"] = dashboard
     query_ids = list()
+    param_query_ids = set()
 
     def recursively_append_param_queries(q):
         for p in q["options"]["parameters"]:
             if "queryId" in p:
                 query_ids.insert(0, p["queryId"])
+                param_query_ids.add(p["queryId"])
                 #get the details of the underlying query to recursively append children queries from parameters if any
                 child_q = requests.get(source_client.url + "/api/2.0/preview/sql/queries/" + p["queryId"], headers=source_client.headers).json()
                 recursively_append_param_queries(child_q)
     #fetch all the queries required for the widgets, recursively
     for widget in dashboard["widgets"]:
         if "visualization" in widget:
             #First we need to add the queries from the parameters to make sure we clone them too
@@ -44,9 +46,10 @@
                 recursively_append_param_queries(widget["visualization"]["query"])
             query_ids.append(widget["visualization"]["query"]["id"])
 
     #removes duplicated but keep order (we need to start with the param queries first)
     query_ids = list(dict.fromkeys(query_ids))
     for query_id in query_ids:
         q = requests.get(source_client.url + "/api/2.0/preview/sql/queries/" + query_id, headers=source_client.headers).json()
+        q["is_parameter_query"] = query_id in param_query_ids
         result["queries"].append(q)
     return result
```

## dbsqlclone/utils/load_dashboard.py

```diff
@@ -62,25 +62,32 @@
         #We need to replace the param queries with the newly created one
         if "parameters" in q["options"]:
             for p in q["options"]["parameters"]:
                 if "queryId" in p:
                     p["queryId"] = dashboard_state["queries"][p["queryId"]]["new_id"]
                     if "parentQueryId" in p:
                         del p["parentQueryId"]
-                    del p["value"]
+                    #if "value" in p:
+                    #    del p["value"]
+                    #if "$$value" in p:
+                    #    del p["$$value"]
         new_query = clone_or_update_query(dashboard_state, q, target_client, parent)
         logging.debug(new_query)
         if target_client.permisions_defined():
-            permissions = requests.post(target_client.url+"/api/2.0/preview/sql/permissions/queries/"+new_query["id"], headers = target_client.headers, json=target_client.permissions).json()
+            permissions = requests.post(target_client.url+"/api/2.0/preview/sql/permissions/queries/"+new_query["id"], headers = target_client.headers, json=target_client.permissions)
             logging.debug(f"     Permissions set to {permissions}")
         visualizations = clone_query_visualization(target_client, q, new_query)
         dashboard_state["queries"][q["id"]] = {"new_id": new_query["id"], "visualizations": visualizations}
 
+    for q in dashboard["queries"] :
+        if "is_parameter_query" not in q or q["is_parameter_query"]:
+            load_query(q)
+
     with ThreadPoolExecutor(max_workers=10) as executor:
-        collections.deque(executor.map(load_query, dashboard["queries"]))
+        collections.deque(executor.map(load_query, [q for q in dashboard["queries"] if "is_parameter_query" in q and not q["is_parameter_query"]]))
 
     duplicate_dashboard(target_client, dashboard["dashboard"], dashboard_state, parent)
     return dashboard_state
 
 def clone_or_update_query(dashboard_state, q, target_client, parent):
     q_creation = {
         "data_source_id": target_client.data_source_id,
```

## Comparing `dbsqlclone-0.1.8.dist-info/LICENCE` & `dbsqlclone-0.1.9.dist-info/LICENCE`

 * *Files identical despite different names*

