# Comparing `tmp/pysigma_backend_elasticsearch-1.0.1.tar.gz` & `tmp/pysigma_backend_elasticsearch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_elasticsearch-1.0.1.tar", max compression
+gzip compressed data, was "pysigma_backend_elasticsearch-1.0.2.tar", max compression
```

## Comparing `pysigma_backend_elasticsearch-1.0.1.tar` & `pysigma_backend_elasticsearch-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7653 2023-04-15 00:12:32.651280 pysigma_backend_elasticsearch-1.0.1/LICENSE
--rw-r--r--   0        0        0      572 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       92 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/backends/elasticsearch/__init__.py
--rw-r--r--   0        0        0    14661 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/backends/elasticsearch/elasticsearch.py
--rw-r--r--   0        0        0      307 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/__init__.py
--rw-r--r--   0        0        0    10111 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/windows.py
--rw-r--r--   0        0        0    61044 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/zeek.py
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pysigma_backend_elasticsearch-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-04-19 19:26:25.483530 pysigma_backend_elasticsearch-1.0.2/LICENSE
+-rw-r--r--   0        0        0      957 2023-04-19 19:26:25.483530 pysigma_backend_elasticsearch-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-04-19 19:26:25.483530 pysigma_backend_elasticsearch-1.0.2/sigma/backends/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    14835 2023-04-19 19:26:25.483530 pysigma_backend_elasticsearch-1.0.2/sigma/backends/elasticsearch/elasticsearch.py
+-rw-r--r--   0        0        0      308 2023-04-19 19:26:25.483530 pysigma_backend_elasticsearch-1.0.2/sigma/pipelines/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    10115 2023-04-19 19:26:25.483530 pysigma_backend_elasticsearch-1.0.2/sigma/pipelines/elasticsearch/windows.py
+-rw-r--r--   0        0        0    60963 2023-04-19 19:26:25.483530 pysigma_backend_elasticsearch-1.0.2/sigma/pipelines/elasticsearch/zeek.py
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pysigma_backend_elasticsearch-1.0.2/PKG-INFO
```

### Comparing `pysigma_backend_elasticsearch-1.0.1/LICENSE` & `pysigma_backend_elasticsearch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.1/sigma/backends/elasticsearch/elasticsearch.py` & `pysigma_backend_elasticsearch-1.0.2/sigma/backends/elasticsearch/elasticsearch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,115 +1,153 @@
+import re
+import json
+from typing import ClassVar, Dict, List, Optional, Pattern, Tuple
+
 from sigma.conversion.state import ConversionState
 from sigma.rule import SigmaRule
 from sigma.conversion.base import TextQueryBackend
 from sigma.conditions import ConditionItem, ConditionAND, ConditionOR, ConditionNOT
 from sigma.types import SigmaCompareExpression
 import sigma
-import re
-import json
-from typing import ClassVar, Dict, List, Optional, Pattern, Tuple
+
 
 class LuceneBackend(TextQueryBackend):
     """
-    Elasticsearch query string backend. Generates query strings described here in the Elasticsearch documentation:
+    Elasticsearch query string backend. Generates query strings described here in the 
+    Elasticsearch documentation:
 
     https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-query-string-query.html#query-string-syntax
     """
-    name : ClassVar[str] = "Elasticsearch Lucene"               # A descriptive name of the backend
-    formats : ClassVar[Dict[str, str]] = {                # Output formats provided by the backend as name -> description mapping. The name should match to finalize_output_<name>.
+    # A descriptive name of the backend
+    name: ClassVar[str] = "Elasticsearch Lucene"
+    # Output formats provided by the backend as name -> description mapping.
+    # The name should match to finalize_output_<name>.
+    formats: ClassVar[Dict[str, str]] = {
         "default": "Plain Elasticsearch Lucene queries",
         "kibana_ndjson": "Kibana NDJSON import file with Lucene queries",
         "dsl_lucene": "Elasticsearch query DSL with embedded Lucene queries",
+        "siem_rule": "Elasticsearch query DSL as SIEM Rules in JSON Format",
+        "siem_rule_ndjson": "Elasticsearch query DSL as SIEM Rules in NDJSON Format",
     }
-    requires_pipeline : ClassVar[bool] = True             # Does the backend requires that a processing pipeline is provided?
+    # Does the backend requires that a processing pipeline is provided?
+    requires_pipeline: ClassVar[bool] = True
 
     # Operator precedence: tuple of Condition{AND,OR,NOT} in order of precedence.
     # The backend generates grouping if required
-    precedence : ClassVar[Tuple[ConditionItem, ConditionItem, ConditionItem]] = (ConditionNOT, ConditionOR, ConditionAND)
-    group_expression : ClassVar[str] = "({expr})"   # Expression for precedence override grouping as format string with {expr} placeholder
+    precedence: ClassVar[Tuple[ConditionItem, ConditionItem, ConditionItem]] = (
+        ConditionNOT, ConditionOR, ConditionAND)
+    # Expression for precedence override grouping as format string with {expr} placeholder
+    group_expression: ClassVar[str] = "({expr})"
     parenthesize: bool = True
 
     # Generated query tokens
-    token_separator : str = " "     # separator inserted between all boolean operators
-    or_token : ClassVar[str] = "OR"
-    and_token : ClassVar[str] = "AND"
-    not_token : ClassVar[str] = "NOT"
-    eq_token : ClassVar[str] = ":"  # Token inserted between field and value (without separator)
+    token_separator: str = " "     # separator inserted between all boolean operators
+    or_token: ClassVar[str] = "OR"
+    and_token: ClassVar[str] = "AND"
+    not_token: ClassVar[str] = "NOT"
+    # Token inserted between field and value (without separator)
+    eq_token: ClassVar[str] = ":"
 
     # String output
-    ## Fields
-    ### No quoting of field names
-    ### Escaping
-    field_escape : ClassVar[str] = "\\"               # Character to escape particular parts defined in field_escape_pattern.
-    field_escape_pattern : ClassVar[Pattern] = re.compile("[\\s*]")   # All matches of this pattern are prepended with the string contained in field_escape.
-
-    ## Values
-    str_quote       : ClassVar[str] = '"'     # string quoting character (added as escaping character)
+    # Fields
+    # No quoting of field names
+    # Escaping
+    # Character to escape particular parts defined in field_escape_pattern.
+    field_escape: ClassVar[str] = "\\"
+    # All matches of this pattern are prepended with the string contained in field_escape.
+    field_escape_pattern: ClassVar[Pattern] = re.compile("[\\s*]")
+
+    # Values
+    # string quoting character (added as escaping character)
+    str_quote: ClassVar[str] = '"'
     str_quote_pattern: ClassVar[Pattern] = re.compile(".")
     str_quote_pattern_negation: ClassVar[bool] = True
-    escape_char     : ClassVar[str] = "\\"    # Escaping character for special characrers inside string
-    wildcard_multi  : ClassVar[str] = "*"     # Character used as multi-character wildcard
-    wildcard_single : ClassVar[str] = "?"     # Character used as single-character wildcard
-    add_escaped     : ClassVar[str] = '+-=&|!(){}[]^"~*?:\\/ '    # Characters quoted in addition to wildcards and string quote
-    filter_chars    : ClassVar[str] = "<>"      # Characters filtered
-    bool_values     : ClassVar[Dict[bool, str]] = {   # Values to which boolean values are mapped.
+    # Escaping character for special characrers inside string
+    escape_char: ClassVar[str] = "\\"
+    # Character used as multi-character wildcard
+    wildcard_multi: ClassVar[str] = "*"
+    # Character used as single-character wildcard
+    wildcard_single: ClassVar[str] = "?"
+    # Characters quoted in addition to wildcards and string quote
+    add_escaped: ClassVar[str] = '+-=&|!(){}[]^"~*?:\\/ '
+    filter_chars: ClassVar[str] = "<>"      # Characters filtered
+    bool_values: ClassVar[Dict[bool, str]] = {   # Values to which boolean values are mapped.
         True: "true",
         False: "false",
     }
 
     # Regular expressions
-    re_expression : ClassVar[str] = "{field}:/{regex}/" # Regular expression query as format string with placeholders {field} and {regex}
-    re_escape_char : ClassVar[str] = "\\"               # Character used for escaping in regular expressions
-    re_escape : ClassVar[Tuple[str]] = ("/",)
-    re_escape_escape_char : ClassVar[bool] = False      # Don't escape the escape char
+    # Regular expression query as format string with placeholders {field} and {regex}
+    re_expression: ClassVar[str] = "{field}:/{regex}/"
+    # Character used for escaping in regular expressions
+    re_escape_char: ClassVar[str] = "\\"
+    re_escape: ClassVar[Tuple[str]] = ("/",)
+    # Don't escape the escape char
+    re_escape_escape_char: ClassVar[bool] = False
 
     # cidr expressions
-    cidr_expression : ClassVar[str] = "{field}:{network}\\/{prefixlen}"    # CIDR expression query as format string with placeholders {field} = {value}
+    # CIDR expression query as format string with placeholders {field} = {value}
+    cidr_expression: ClassVar[str] = "{field}:{network}\\/{prefixlen}"
 
     # Numeric comparison operators
-    compare_op_expression : ClassVar[str] = "{field}:{operator}{value}"  # Compare operation query as format string with placeholders {field}, {operator} and {value}
-    # Mapping between CompareOperators elements and strings used as replacement for {operator} in compare_op_expression
-    compare_operators : ClassVar[Dict[SigmaCompareExpression.CompareOperators, str]] = {
-        SigmaCompareExpression.CompareOperators.LT  : "<",
-        SigmaCompareExpression.CompareOperators.LTE : "<=",
-        SigmaCompareExpression.CompareOperators.GT  : ">",
-        SigmaCompareExpression.CompareOperators.GTE : ">=",
+    # Compare operation query as format string with placeholders {field}, {operator} and {value}
+    compare_op_expression: ClassVar[str] = "{field}:{operator}{value}"
+    # Mapping between CompareOperators elements and strings used as replacement
+    # for {operator} in compare_op_expression
+    compare_operators: ClassVar[Dict[SigmaCompareExpression.CompareOperators, str]] = {
+        SigmaCompareExpression.CompareOperators.LT: "<",
+        SigmaCompareExpression.CompareOperators.LTE: "<=",
+        SigmaCompareExpression.CompareOperators.GT: ">",
+        SigmaCompareExpression.CompareOperators.GTE: ">=",
     }
 
     # Null/None expressions
-    field_null_expression : ClassVar[str] = "NOT _exists_:{field}"          # Expression for field has null value as format string with {field} placeholder for field name
+    # Expression for field has null value as format string with {field} placeholder for field name
+    field_null_expression: ClassVar[str] = "NOT _exists_:{field}"
 
     # Field value in list, e.g. "field in (value list)" or "field containsall (value list)"
-    convert_or_as_in : ClassVar[bool] = True                     # Convert OR as in-expression
-    convert_and_as_in : ClassVar[bool] = False                   # Convert AND as in-expression
-    in_expressions_allow_wildcards : ClassVar[bool] = True       # Values in list can contain wildcards. If set to False (default) only plain values are converted into in-expressions.
-    field_in_list_expression : ClassVar[str] = "{field}{op}({list})"  # Expression for field in list of values as format string with placeholders {field}, {op} and {list}
-    or_in_operator : ClassVar[str] = ":"               # Operator used to convert OR into in-expressions. Must be set if convert_or_as_in is set
-    list_separator : ClassVar[str] = " OR "               # List element separator
+    # Convert OR as in-expression
+    convert_or_as_in: ClassVar[bool] = True
+    # Convert AND as in-expression
+    convert_and_as_in: ClassVar[bool] = False
+    # Values in list can contain wildcards. If set to False (default)
+    # only plain values are converted into in-expressions.
+    in_expressions_allow_wildcards: ClassVar[bool] = True
+    # Expression for field in list of values as format string with
+    # placeholders {field}, {op} and {list}
+    field_in_list_expression: ClassVar[str] = "{field}{op}({list})"
+    # Operator used to convert OR into in-expressions. Must be set if convert_or_as_in is set
+    or_in_operator: ClassVar[str] = ":"
+    # List element separator
+    list_separator: ClassVar[str] = " OR "
 
     # Value not bound to a field
-    unbound_value_str_expression : ClassVar[str] = '"{value}"'   # Expression for string value not bound to a field as format string with placeholder {value}
-    unbound_value_num_expression : ClassVar[str] = '{value}'   # Expression for number value not bound to a field as format string with placeholder {value}
-
-    def __init__(self, processing_pipeline: Optional["sigma.processing.pipeline.ProcessingPipeline"] = None,
+    # Expression for string value not bound to a field as format string with placeholder {value}
+    unbound_value_str_expression: ClassVar[str] = '"{value}"'
+    # Expression for number value not bound to a field as format string with placeholder {value}
+    unbound_value_num_expression: ClassVar[str] = '{value}'
+
+    def __init__(
+        self,
+        processing_pipeline: Optional["sigma.processing.pipeline.ProcessingPipeline"] = None,
         collect_errors: bool = False,
-        index_names : List = [
+        index_names: List = [
             "apm-*-transaction*",
             "auditbeat-*",
             "endgame-*",
             "filebeat-*",
             "logs-*",
             "packetbeat-*",
             "traces-apm*",
             "winlogbeat-*",
             "-*elastic-cloud-logs-*"
         ],
-        schedule_interval : int = 5,
-        schedule_interval_unit : str = "m",
-        **kwargs):
+            schedule_interval: int = 5,
+            schedule_interval_unit: str = "m",
+            **kwargs):
 
         super().__init__(processing_pipeline, collect_errors, **kwargs)
         self.index_names = index_names or [
             "apm-*-transaction*",
             "auditbeat-*",
             "endgame-*",
             "filebeat-*",
@@ -118,22 +156,28 @@
             "traces-apm*",
             "winlogbeat-*",
             "-*elastic-cloud-logs-*"
         ]
         self.schedule_interval = schedule_interval or 5
         self.schedule_interval_unit = schedule_interval_unit or "m"
         self.severity_risk_mapping = {
-            "INFORMATIONAL" : 1,
-            "LOW" : 21,
-            "MEDIUM" : 47,
-            "HIGH" : 73,
-            "CRITICAL" : 99
+            "INFORMATIONAL": 1,
+            "LOW": 21,
+            "MEDIUM": 47,
+            "HIGH": 73,
+            "CRITICAL": 99
         }
 
-    def finalize_query_dsl_lucene(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> Dict:
+    def finalize_query_dsl_lucene(
+            self,
+            rule: SigmaRule,
+            query: str,
+            index: int,
+            state: ConversionState) -> Dict:
+
         return {
             "query": {
                 "bool": {
                     "must": [
                         {
                             "query_string": {
                                 "query": query,
@@ -144,86 +188,100 @@
                 }
             }
         }
 
     def finalize_output_dsl_lucene(self, queries: List[Dict]) -> Dict:
         return list(queries)
 
-    def finalize_query_kibana_ndjson(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> Dict:
-        # TODO: implement the per-query output for the output format kibana here. Usually, the generated query is
-        # embedded into a template, e.g. a JSON format with additional information from the Sigma rule.
-        columns = list()
+    def finalize_query_kibana_ndjson(
+        self,
+        rule: SigmaRule,
+        query: str,
+        index: int,
+        state: ConversionState
+    ) -> Dict:
+
+        # TODO: implement the per-query output for the output format kibana here. Usually, the
+        # generated query is embedded into a template, e.g. a JSON format with additional
+        # information from the Sigma rule.
+        columns = []
         index = "beats-*"
         ndjson = {
             "id": str(rule.id),
             "type": "search",
             "attributes": {
-                "title": "SIGMA - {}".format(rule.title),
+                "title": f"SIGMA - {rule.title}",
                 "description": rule.description,
                 "hits": 0,
                 "columns": columns,
                 "sort": ["@timestamp", "desc"],
                 "version": 1,
                 "kibanaSavedObjectMeta": {
                     "searchSourceJSON": str(json.dumps({
                         "index": index,
                         "filter":  [],
                         "highlight": {
                             "pre_tags": ["@kibana-highlighted-field@"],
                             "post_tags": ["@/kibana-highlighted-field@"],
-                            "fields": { "*":{} },
+                            "fields": {"*": {}},
                             "require_field_match": False,
                             "fragment_size": 2147483647
-                            },
+                        },
                         "query": {
                             "query_string": {
                                 "query": query,
                                 "analyze_wildcard": True
-                                }
                             }
-                        })
+                        }
+                    })
                     )
                 }
             },
             "references": [
                 {
                     "id": index,
                     "name": "kibanaSavedObjectMeta.searchSourceJSON.index",
                     "type": "index-pattern"
                 }
             ]
         }
         return ndjson
 
     def finalize_output_kibana_ndjson(self, queries: List[str]) -> List[Dict]:
-        # TODO: implement the output finalization for all generated queries for the format kibana here. Usually,
-        # the single generated queries are embedded into a structure, e.g. some JSON or XML that can be imported into
-        # the SIEM.
+        # TODO: implement the output finalization for all generated queries for the format kibana
+        # here. Usually, the single generated queries are embedded into a structure, e.g. some
+        # JSON or XML that can be imported into the SIEM.
         return list(queries)
 
-    def finalize_query_siem_rule(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> Dict:
+    def finalize_query_siem_rule(
+        self,
+        rule: SigmaRule,
+        query: str,
+        index: int,
+        state: ConversionState
+    ) -> Dict:
         """
-        Create SIEM Rules in JSON Format. These rules could be imported into Kibana using the Create Rule API
-        https://www.elastic.co/guide/en/kibana/8.6/create-rule-api.html
+        Create SIEM Rules in JSON Format. These rules could be imported into Kibana using the 
+        Create Rule API https://www.elastic.co/guide/en/kibana/8.6/create-rule-api.html
         This API (and generated data) is NOT the same like importing Detection Rules via:
         Kibana -> Security -> Alerts -> Manage Rules -> Import
         If you want to have a nice importable NDJSON File for the Security Rule importer
         use pySigma Format 'siem_rule_ndjson' instead.
         """
 
         siem_rule = {
-            "name":"SIGMA - {}".format(rule.title),
-            "tags": ["{}-{}".format(n.namespace, n.name) for n in rule.tags],
+            "name": f"SIGMA - {rule.title}",
+            "tags": [f"{n.namespace}-{n.name}" for n in rule.tags],
             "consumer": "siem",
             "enabled": True,
             "throttle": None,
-            "schedule":{
+            "schedule": {
                 "interval": f"{self.schedule_interval}{self.schedule_interval_unit}"
             },
-            "params":{
+            "params": {
                 "author": [rule.author] if rule.author is not None else [],
                 "description": rule.description if rule.description is not None else "No description",
                 "ruleId": str(rule.id),
                 "falsePositives": rule.falsepositives,
                 "from": f"now-{self.schedule_interval}{self.schedule_interval_unit}",
                 "immutable": False,
                 "license": "DRL",
@@ -246,34 +304,34 @@
                 "setup": "",
                 "type": "query",
                 "language": "lucene",
                 "index": self.index_names,
                 "query": query,
                 "filters": []
             },
-            "rule_type_id":"siem.queryRule",
-            "notify_when":"onActiveAlert",
-            "actions":[]
-            }
+            "rule_type_id": "siem.queryRule",
+            "notify_when": "onActiveAlert",
+            "actions": []
+        }
         return siem_rule
 
     def finalize_output_siem_rule(self, queries: List[Dict]) -> Dict:
         return list(queries)
 
     def finalize_query_siem_rule_ndjson(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> Dict:
         """
         Generating SIEM/Detection Rules in NDJSON Format. Compatible with
 
         https://www.elastic.co/guide/en/security/8.6/rules-ui-management.html#import-export-rules-ui
         """
 
         siem_rule = {
             "id": str(rule.id),
-            "name":"SIGMA - {}".format(rule.title),
-            "tags": ["{}-{}".format(n.namespace, n.name) for n in rule.tags],
+            "name": f"SIGMA - {rule.title}",
+            "tags": [f"{n.namespace}-{n.name}" for n in rule.tags],
             "enabled": True,
             "throttle": "no_actions",
             "interval": f"{self.schedule_interval}{self.schedule_interval_unit}",
             "author": [rule.author] if rule.author is not None else [],
             "description": rule.description if rule.description is not None else "No description",
             "rule_id": str(rule.id),
             "false_positives": rule.falsepositives,
@@ -298,13 +356,13 @@
             "required_fields": [],
             "setup": "",
             "type": "query",
             "language": "lucene",
             "index": self.index_names,
             "query": query,
             "filters": [],
-            "actions":[]
-            }
+            "actions": []
+        }
         return siem_rule
 
     def finalize_output_siem_rule_ndjson(self, queries: List[Dict]) -> Dict:
-        return list(queries)
+        return list(queries)
```

### Comparing `pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/windows.py` & `pysigma_backend_elasticsearch-1.0.2/sigma/pipelines/elasticsearch/windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from sigma.pipelines.common import logsource_windows, windows_logsource_mapping, generate_windows_logsource_items
-from sigma.processing.transformations import FieldMappingTransformation, AddFieldnamePrefixTransformation, AddConditionTransformation
+from sigma.pipelines.common import generate_windows_logsource_items
+from sigma.processing.transformations import FieldMappingTransformation, AddFieldnamePrefixTransformation
 from sigma.processing.conditions import LogsourceCondition, IncludeFieldCondition, FieldNameProcessingItemAppliedCondition
 from sigma.processing.pipeline import ProcessingItem, ProcessingPipeline
 
 ecs_windows_variable_mappings = {
     "FileVersion": (
         ("category", "process_creation", "process.pe.file_version"),
         ("category", "image_load", "file.pe.file_version"),
@@ -62,34 +62,35 @@
         ("service", "security", "user.id"),
     ),
     "TargetLogonId": (
         ("service", "security", "winlog.logon.id"),
     ),
 }
 
+
 def ecs_windows():
     return ProcessingPipeline(
         name="Elastic Common Schema (ECS) Windows log mappings from Winlogbeat from version 7",
         priority=20,
         allowed_backends=("elasticsearch", "opensearch"),
         items=generate_windows_logsource_items("winlog.channel", "{source}") + [                   # Variable field mappinga depending on category/service
-           ProcessingItem(
+            ProcessingItem(
                 identifier=f"elasticsearch_windows-{field}-{logsrc_field}-{logsrc}",
                 transformation=FieldMappingTransformation({
                     field: mapped
                 }),
                 rule_conditions=[
                     LogsourceCondition(**{
                         "product": "windows",
                         logsrc_field: logsrc,
                     }),
                 ]
-           )
-           for field, mappings in ecs_windows_variable_mappings.items()
-           for (logsrc_field, logsrc, mapped) in mappings
+            )
+            for field, mappings in ecs_windows_variable_mappings.items()
+            for (logsrc_field, logsrc, mapped) in mappings
         ] + [
             ProcessingItem(     # Field mappings
                 identifier="ecs_windows_field_mapping",
                 transformation=FieldMappingTransformation({
                     "EventID": "event.code",
                     "Channel": "winlog.channel",
                     "Provider_Name": "winlog.provider_name",
@@ -163,28 +164,31 @@
                 }),
                 rule_conditions=[
                     LogsourceCondition(product="windows")
                 ],
             ),
             ProcessingItem(         # Prepend each field that was not processed by previous field mapping transformation with "winlog.event_data."
                 identifier="ecs_windows_winlog_eventdata_prefix",
-                transformation=AddFieldnamePrefixTransformation("winlog.event_data."),
+                transformation=AddFieldnamePrefixTransformation(
+                    "winlog.event_data."),
                 field_name_conditions=[
-                    FieldNameProcessingItemAppliedCondition("ecs_windows_field_mapping"),
+                    FieldNameProcessingItemAppliedCondition(
+                        "ecs_windows_field_mapping"),
                     IncludeFieldCondition(fields=["\\w+\\."], type="re"),
                 ],
                 field_name_condition_negation=True,
                 field_name_condition_linking=any,
                 rule_conditions=[
                     LogsourceCondition(product="windows")
                 ],
             )
         ],
     )
 
+
 def ecs_windows_old():
     return ProcessingPipeline(
         name="Elastic Common Schema (ECS) Windows log mappings from Winlogbeat up to version 6",
         priority=20,
         allowed_backends=("elasticsearch", "opensearch"),
         items=generate_windows_logsource_items("winlog.channel", "{source}") + [
             ProcessingItem(     # Field mappings
@@ -197,18 +201,19 @@
                     LogsourceCondition(product="windows")
                 ],
             ),
             ProcessingItem(         # Prepend each field that was not processed by previous field mapping transformation with "winlog.event_data."
                 identifier="ecs_windows_eventdata_prefix",
                 transformation=AddFieldnamePrefixTransformation("event_data."),
                 field_name_conditions=[
-                    FieldNameProcessingItemAppliedCondition("ecs_windows_field_mapping"),
+                    FieldNameProcessingItemAppliedCondition(
+                        "ecs_windows_field_mapping"),
                     IncludeFieldCondition(fields=["\\w+\\."], type="re"),
                 ],
                 field_name_condition_negation=True,
                 field_name_condition_linking=any,
                 rule_conditions=[
                     LogsourceCondition(product="windows")
                 ],
             )
         ],
-    )
+    )
```

### Comparing `pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/zeek.py` & `pysigma_backend_elasticsearch-1.0.2/sigma/pipelines/elasticsearch/zeek.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from sigma.processing.transformations import FieldMappingTransformation, AddFieldnamePrefixTransformation, AddConditionTransformation, ChangeLogsourceTransformation
-from sigma.processing.conditions import LogsourceCondition, IncludeFieldCondition, ExcludeFieldCondition, RuleProcessingItemAppliedCondition
+# pylint: disable=too-many-lines
+
+from sigma.processing.transformations import FieldMappingTransformation, AddConditionTransformation, ChangeLogsourceTransformation
+from sigma.processing.conditions import LogsourceCondition
 from sigma.processing.pipeline import ProcessingItem, ProcessingPipeline
 
 ecs_zeek_beats_category_service_mapping = {
     "accounting": "syslog",
     "firewall": "conn",
     "dns": "dns",
     "proxy": "http",
@@ -1083,8 +1085,8 @@
                     "source.port": "id.orig_p",
                 }),
                 rule_conditions=[
                 LogsourceCondition(product="zeek"),
             ],
         ),
     ],
-)
+)
```

### Comparing `pysigma_backend_elasticsearch-1.0.1/PKG-INFO` & `pysigma_backend_elasticsearch-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-elasticsearch
-Version: 1.0.1
+Version: 1.0.2
 Summary: pySigma Elasticsearch backend
 Home-page: https://github.com/SigmaHQ/pySigma-backend-elasticsearch
 License: LGPL-3.0-only
 Author: Thomas Patzke
 Author-email: thomas@patzke.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

