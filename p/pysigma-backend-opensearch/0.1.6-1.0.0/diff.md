# Comparing `tmp/pysigma_backend_opensearch-0.1.6.tar.gz` & `tmp/pysigma_backend_opensearch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_opensearch-0.1.6.tar", max compression
+gzip compressed data, was "pysigma_backend_opensearch-1.0.0.tar", max compression
```

## Comparing `pysigma_backend_opensearch-0.1.6.tar` & `pysigma_backend_opensearch-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     7653 2023-04-15 00:36:16.389696 pysigma_backend_opensearch-0.1.6/LICENSE
--rw-r--r--   0        0        0      632 2023-04-15 00:36:16.389696 pysigma_backend_opensearch-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      106 2023-04-15 00:36:16.389696 pysigma_backend_opensearch-0.1.6/sigma/backends/opensearch/__init__.py
--rw-r--r--   0        0        0     4791 2023-04-15 00:36:16.389696 pysigma_backend_opensearch-0.1.6/sigma/backends/opensearch/opensearch.py
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 pysigma_backend_opensearch-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-04-19 19:54:23.654017 pysigma_backend_opensearch-1.0.0/LICENSE
+-rw-r--r--   0        0        0      957 2023-04-19 19:54:23.658017 pysigma_backend_opensearch-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-04-19 19:54:23.658017 pysigma_backend_opensearch-1.0.0/sigma/backends/opensearch/__init__.py
+-rw-r--r--   0        0        0     4304 2023-04-19 19:54:23.658017 pysigma_backend_opensearch-1.0.0/sigma/backends/opensearch/opensearch.py
+-rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 pysigma_backend_opensearch-1.0.0/PKG-INFO
```

### Comparing `pysigma_backend_opensearch-0.1.6/LICENSE` & `pysigma_backend_opensearch-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_opensearch-0.1.6/sigma/backends/opensearch/opensearch.py` & `pysigma_backend_opensearch-1.0.0/sigma/backends/opensearch/opensearch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,46 @@
+from typing import ClassVar, Dict, List, Optional
 from sigma.conversion.state import ConversionState
 from sigma.rule import SigmaRule
-import sigma
-import json
-from typing import ClassVar, Dict, List, Optional
 from sigma.backends.elasticsearch import LuceneBackend
+import sigma
+
 
 class OpensearchLuceneBackend(LuceneBackend):
     """OpensearchLuceneBackend backend."""
-    name : ClassVar[str] = "OpenSearch Lucene"            # A descriptive name of the backend
-    formats : ClassVar[Dict[str, str]] = {                # Output formats provided by the backend as name -> description mapping. The name should match to finalize_output_<name>.
+    name: ClassVar[str] = "OpenSearch Lucene"            # A descriptive name of the backend
+    formats: ClassVar[Dict[str, str]] = {                # Output formats provided by the backend as name -> description mapping. The name should match to finalize_output_<name>.
         "default": "Plain OpenSearch Lucene queries",
         "dashboards_ndjson": "OpenSearch Dashboards NDJSON import file with Lucene queries",
         "monitor_rule": "OpenSearch monitor rule with embedded Lucene query",
         "dsl_lucene": "OpenSearch query DSL with embedded Lucene queries",
     }
-    requires_pipeline : ClassVar[bool] = True             # Does the backend requires that a processing pipeline is provided?
+    # Does the backend requires that a processing pipeline is provided?
+    requires_pipeline: ClassVar[bool] = True
 
     def __init__(self, processing_pipeline: Optional["sigma.processing.pipeline.ProcessingPipeline"] = None,
-        collect_errors: bool = False, index_names : List = ["beats-*"], monitor_interval : int = 5,
-        monitor_interval_unit : str = "MINUTES", **kwargs):
+                 collect_errors: bool = False, index_names: List = ["beats-*"], monitor_interval: int = 5,
+                 monitor_interval_unit: str = "MINUTES", **kwargs):
 
         super().__init__(processing_pipeline, collect_errors, **kwargs)
         self.index_names = index_names or ["beats-*"]
         self.monitor_interval = monitor_interval or 5
         self.monitor_interval_unit = monitor_interval_unit or "MINUTES"
 
     def finalize_query_monitor_rule(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> dict:
-        # TODO: implement the per-query output for the output format lql here. Usually, the generated query is
-        # embedded into a template, e.g. a JSON format with additional information from the Sigma rule.
         severity_mapping = {
             5: 1,
             4: 2,
             3: 3,
             2: 4,
             1: 5
         }
         monitor_rule = {
             "type": "monitor",
-            "name": "SIGMA - {}".format(rule.title),
+            "name": f"SIGMA - {rule.title}",
             "description": rule.description,
             "enabled": True,
             "schedule": {
                 "period": {
                     "interval": self.monitor_interval,
                     "unit": self.monitor_interval_unit
                 }
@@ -64,15 +63,15 @@
                                     ]
                                 }
                             }
                         }
                     }
                 }
             ],
-            "tags": ["{}-{}".format(n.namespace, n.name) for n in rule.tags],
+            "tags": [f"{n.namespace}-{n.name}" for n in rule.tags],
             "triggers": [
                 {
                     "name": "generated-trigger",
                     "severity": severity_mapping[rule.level.value] if rule.level is not None else 1,
                     "condition": {
                         "script": {
                             "source": "ctx.results[0].hits.total.value > 0",
@@ -88,19 +87,16 @@
             },
             "references": rule.references
         }
 
         return monitor_rule
 
     def finalize_output_monitor_rule(self, queries: List[str]) -> str:
-        # TODO: implement the output finalization for all generated queries for the format lql here. Usually,
-        # the single generated queries are embedded into a structure, e.g. some JSON or XML that can be imported into
-        # the SIEM.
         return list(queries)
 
     def finalize_query_dashboards_ndjson(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> str:
         """Alias to Kibana NDJSON query finalization."""
         return self.finalize_query_kibana_ndjson(rule, query, index, state)
 
     def finalize_output_dashboards_ndjson(self, queries: List[str]) -> str:
         """Alias to Kibana NDJSON output finalization."""
-        return self.finalize_output_kibana_ndjson(queries)
+        return self.finalize_output_kibana_ndjson(queries)
```

### Comparing `pysigma_backend_opensearch-0.1.6/PKG-INFO` & `pysigma_backend_opensearch-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-opensearch
-Version: 0.1.6
+Version: 1.0.0
 Summary: pySigma OpenSearch backend
 Home-page: https://github.com/SigmaHQ/pySigma-backend-opensearch
 License: LGPL-3.0-only
 Author: Hendrik Baecker
 Author-email: hendrik.baecker@dcso.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

