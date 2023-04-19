# Comparing `tmp/monarch_py-0.6.1.tar.gz` & `tmp/monarch_py-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.6.1.tar", max compression
+gzip compressed data, was "monarch_py-0.6.2.tar", max compression
```

## Comparing `monarch_py-0.6.1.tar` & `monarch_py-0.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      955 2023-04-11 00:16:06.217694 monarch_py-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       77 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     5897 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0     6595 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     6272 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    15888 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8913 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2345 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     3732 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2051 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     8269 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3794 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     3657 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4262 2023-04-11 00:16:06.217694 monarch_py-0.6.1/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-04-19 20:22:07.897810 monarch_py-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     5897 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0     6595 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     6327 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3300 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    15875 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8913 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2345 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     3732 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2051 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     8269 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3794 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     3657 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4262 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.6.2/PKG-INFO
```

### Comparing `monarch_py-0.6.1/pyproject.toml` & `monarch_py-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.6.1"
+version = "0.6.2"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.6.1/src/monarch_py/cli.py` & `monarch_py-0.6.2/src/monarch_py/cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/datamodels/model.py` & `monarch_py-0.6.2/src/monarch_py/datamodels/model.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.6.2/src/monarch_py/datamodels/model.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,17 @@
     - stage_qualifier
     - pathway
     - relation
   AssociationCount:
     is_a: FacetValue
     slots:
       - id
+    slot_usage:
+      label:
+        identifier: false
   AssociationResults:
     is_a: Results
     slots: 
       - items
     slot_usage:
       items:
         range: Association
```

### Comparing `monarch_py-0.6.1/src/monarch_py/datamodels/solr.py` & `monarch_py-0.6.2/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.6.2/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
     ) -> SolrQuery:
         """Populate a SolrQuery object with association filters"""
 
         query = SolrQuery(start=offset, rows=limit)
 
         subject_field = "subject" if direct else "subject_closure"
         object_field = "object" if direct else "object_closure"
-            
 
         if category:
             query.add_field_filter_query("category", category)
         if predicate:
             query.add_field_filter_query("predicate", predicate)
         if subject:
             query.add_field_filter_query(subject_field, subject)
```

### Comparing `monarch_py-0.6.1/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.6.2/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.6.2/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.6.2/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.6.2/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.6.2/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/service/solr_service.py` & `monarch_py-0.6.2/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/solr_cli.py` & `monarch_py-0.6.2/src/monarch_py/solr_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/sql_cli.py` & `monarch_py-0.6.2/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.6.2/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/src/monarch_py/utils/utils.py` & `monarch_py-0.6.2/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.1/PKG-INFO` & `monarch_py-0.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.6.1
+Version: 0.6.2
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

