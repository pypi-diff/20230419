# Comparing `tmp/edge_orm-0.6.3.tar.gz` & `tmp/edge_orm-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_orm-0.6.3.tar", max compression
+gzip compressed data, was "edge_orm-0.6.4.tar", max compression
```

## Comparing `edge_orm-0.6.3.tar` & `edge_orm-0.6.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.6.3/README.md
--rw-r--r--   0        0        0      774 2023-02-27 21:50:15.475075 edge_orm-0.6.3/edge_orm/__init__.py
--rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.6.3/edge_orm/cache.py
--rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.6.3/edge_orm/errors.py
--rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.6.3/edge_orm/execute.py
--rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.6.3/edge_orm/external/encoders.py
--rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.6.3/edge_orm/helpers.py
--rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.6.3/edge_orm/logs.py
--rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.6.3/edge_orm/node/__init__.py
--rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.6.3/edge_orm/node/errors.py
--rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.6.3/edge_orm/node/models.py
--rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.6.3/edge_orm/resolver/__init__.py
--rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.6.3/edge_orm/resolver/enums.py
--rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.6.3/edge_orm/resolver/errors.py
--rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.6.3/edge_orm/resolver/merging.py
--rw-r--r--   0        0        0    42504 2023-04-19 18:00:09.099182 edge_orm-0.6.3/edge_orm/resolver/model.py
--rw-r--r--   0        0        0     5294 2023-02-08 20:21:01.356439 edge_orm-0.6.3/edge_orm/resolver/nested_resolvers.py
--rw-r--r--   0        0        0     3711 2023-04-13 17:11:22.267717 edge_orm-0.6.3/edge_orm/resolver/utils.py
--rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.6.3/edge_orm/span.py
--rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.6.3/edge_orm/types_generator/__init__.py
--rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.6.3/edge_orm/types_generator/introspection.py
--rw-r--r--   0        0        0    39663 2023-04-13 18:56:59.500577 edge_orm-0.6.3/edge_orm/types_generator/main.py
--rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.6.3/edge_orm/unset.py
--rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.6.3/edge_orm/validators.py
--rw-r--r--   0        0        0      785 2023-04-19 17:51:28.075895 edge_orm-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 edge_orm-0.6.3/setup.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.6.4/README.md
+-rw-r--r--   0        0        0      774 2023-02-27 21:50:15.475075 edge_orm-0.6.4/edge_orm/__init__.py
+-rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.6.4/edge_orm/cache.py
+-rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.6.4/edge_orm/errors.py
+-rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.6.4/edge_orm/execute.py
+-rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.6.4/edge_orm/external/encoders.py
+-rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.6.4/edge_orm/helpers.py
+-rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.6.4/edge_orm/logs.py
+-rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.6.4/edge_orm/node/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.6.4/edge_orm/node/errors.py
+-rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.6.4/edge_orm/node/models.py
+-rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.6.4/edge_orm/resolver/__init__.py
+-rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.6.4/edge_orm/resolver/enums.py
+-rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.6.4/edge_orm/resolver/errors.py
+-rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.6.4/edge_orm/resolver/merging.py
+-rw-r--r--   0        0        0    42135 2023-04-19 18:23:45.866983 edge_orm-0.6.4/edge_orm/resolver/model.py
+-rw-r--r--   0        0        0     5294 2023-02-08 20:21:01.356439 edge_orm-0.6.4/edge_orm/resolver/nested_resolvers.py
+-rw-r--r--   0        0        0     3711 2023-04-13 17:11:22.267717 edge_orm-0.6.4/edge_orm/resolver/utils.py
+-rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.6.4/edge_orm/span.py
+-rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.6.4/edge_orm/types_generator/__init__.py
+-rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.6.4/edge_orm/types_generator/introspection.py
+-rw-r--r--   0        0        0    39663 2023-04-13 18:56:59.500577 edge_orm-0.6.4/edge_orm/types_generator/main.py
+-rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.6.4/edge_orm/unset.py
+-rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.6.4/edge_orm/validators.py
+-rw-r--r--   0        0        0      785 2023-04-19 18:16:07.216906 edge_orm-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 edge_orm-0.6.4/setup.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.6.4/PKG-INFO
```

### Comparing `edge_orm-0.6.3/edge_orm/__init__.py` & `edge_orm-0.6.4/edge_orm/__init__.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/cache.py` & `edge_orm-0.6.4/edge_orm/cache.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/execute.py` & `edge_orm-0.6.4/edge_orm/execute.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/external/encoders.py` & `edge_orm-0.6.4/edge_orm/external/encoders.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/helpers.py` & `edge_orm-0.6.4/edge_orm/helpers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/logs.py` & `edge_orm-0.6.4/edge_orm/logs.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/node/models.py` & `edge_orm-0.6.4/edge_orm/node/models.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/resolver/merging.py` & `edge_orm-0.6.4/edge_orm/resolver/merging.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/resolver/model.py` & `edge_orm-0.6.4/edge_orm/resolver/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -749,27 +749,19 @@
 
         if include_changes or include_permissions:
             changes_keys = patch.set_fields_
             if include_changes:
                 if only_one:
                     changes_str = f"_changes := {{ {', '.join([f'{k} := {{ _old := before.{k}, _new := after.{k} }}' for k in changes_keys])} }}"
                 else:
-                    for_str = f"select {{ _id := i.id, {', '.join([f'{k} := i.{k}' for k in changes_keys])} }}"
+                    inner_str = f"{{ id, {', '.join(changes_keys)} }}"
                     changes_str = f"""
                 _changes := {{
-                    before_arr := (
-                        for i in before union (
-                            {for_str}
-                        )
-                    ),
-                    after_arr := (
-                        for i in after union (
-                            {for_str}
-                        )
-                    )
+                    _before := before {inner_str},
+                    _after := after {inner_str}
                 }}
                 """
                     only_one = True
             else:
                 changes_str = ""
             final_update_s = f"""
             with
@@ -880,15 +872,14 @@
         self,
         patch: PatchType,
         *,
         update_all: bool = False,
         client: edgedb.AsyncIOClient,
         mutate_on_update: bool = True,
     ) -> list[NodeType]:
-        # TODO make update_many_with_changes at some point, would not be hard
         if not patch.set_fields_:
             raise errors.ResolverException("Patch is empty.")
         if not update_all:
             if not self.has_filters():
                 raise errors.ResolverException(
                     "You did not give filters which means this will update *all* models. "
                     "If this is your intention, pass update_all=True."
@@ -928,25 +919,25 @@
             include_permissions=False,
             include_changes=True,
         )
         raw_response = T.cast(RAW_RESP_MANY, raw_response)
         nodes = self.parse_obj_with_cache_list(raw_response["after"])
 
         changes_raw = raw_response["_changes"]
-        before_arr, after_arr = changes_raw["before_arr"], changes_raw["after_arr"]
+        before_arr, after_arr = changes_raw["_before"], changes_raw["_after"]
         changes_d: CHANGES_D = {}
         for before_d, after_d in zip(before_arr, after_arr):
-            if before_d["_id"] != after_d["_id"]:
+            if before_d["id"] != after_d["id"]:
                 raise Exception(
                     f"before changes id does not match after changes id, {before_d=}, {after_d=}"
                 )
             changes = {
-                k: (before_d[k], after_d[k]) for k in before_d.keys() if k != "_id"
+                k: (before_d[k], after_d[k]) for k in before_d.keys() if k != "id"
             }
-            changes_d[uuid.UUID(before_d["_id"])] = changes
+            changes_d[uuid.UUID(before_d["id"])] = changes
 
         return nodes, changes_d
 
     async def _delete(
         self,
         *,
         field_name: str = None,
```

### Comparing `edge_orm-0.6.3/edge_orm/resolver/nested_resolvers.py` & `edge_orm-0.6.4/edge_orm/resolver/nested_resolvers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/resolver/utils.py` & `edge_orm-0.6.4/edge_orm/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/span.py` & `edge_orm-0.6.4/edge_orm/span.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/types_generator/introspection.py` & `edge_orm-0.6.4/edge_orm/types_generator/introspection.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/types_generator/main.py` & `edge_orm-0.6.4/edge_orm/types_generator/main.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/unset.py` & `edge_orm-0.6.4/edge_orm/unset.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/edge_orm/validators.py` & `edge_orm-0.6.4/edge_orm/validators.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.3/pyproject.toml` & `edge_orm-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edge-orm"
-version = "0.6.3"
+version = "0.6.4"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = "edge_orm" }]
 exclude = ["tests/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `edge_orm-0.6.3/setup.py` & `edge_orm-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'pydantic[email]>=1.10,<2.0']
 
 extras_require = \
 {'docs': ['mkdocs-material>=8.5.7,<9.0.0']}
 
 setup_kwargs = {
     'name': 'edge-orm',
-    'version': '0.6.3',
+    'version': '0.6.4',
     'description': '',
     'long_description': '# edge orm',
     'author': 'Jeremy Berman',
     'author_email': 'jerber@sas.upenn.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `edge_orm-0.6.3/PKG-INFO` & `edge_orm-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-orm
-Version: 0.6.3
+Version: 0.6.4
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
```

