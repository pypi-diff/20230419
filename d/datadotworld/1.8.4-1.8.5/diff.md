# Comparing `tmp/datadotworld-1.8.4.tar.gz` & `tmp/datadotworld-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadotworld-1.8.4.tar", last modified: Fri Feb  3 15:07:55 2023, max compression
+gzip compressed data, was "datadotworld-1.8.5.tar", last modified: Wed Apr 19 16:09:25 2023, max compression
```

## Comparing `datadotworld-1.8.4.tar` & `datadotworld-1.8.5.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:07:55.508330 datadotworld-1.8.4/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-02-03 15:06:42.000000 datadotworld-1.8.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-03 15:06:42.000000 datadotworld-1.8.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13253 2023-02-03 15:07:55.508330 datadotworld-1.8.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12251 2023-02-03 15:06:42.000000 datadotworld-1.8.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:07:55.488330 datadotworld-1.8.4/datadotworld/
--rw-r--r--   0 root         (0) root         (0)     8877 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:07:55.492330 datadotworld-1.8.4/datadotworld/client/
--rw-r--r--   0 root         (0) root         (0)      682 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:07:55.492330 datadotworld-1.8.4/datadotworld/client/_swagger/
--rw-r--r--   0 root         (0) root         (0)     9608 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26099 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:07:55.496330 datadotworld-1.8.4/datadotworld/client/_swagger/apis/
--rw-r--r--   0 root         (0) root         (0)      868 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22782 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/connections_api.py
--rw-r--r--   0 root         (0) root         (0)    63079 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/datasets_api.py
--rw-r--r--   0 root         (0) root         (0)    31953 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/do_is_api.py
--rw-r--r--   0 root         (0) root         (0)    14485 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/download_api.py
--rw-r--r--   0 root         (0) root         (0)    60948 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/files_api.py
--rw-r--r--   0 root         (0) root         (0)    53754 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/insights_api.py
--rw-r--r--   0 root         (0) root         (0)    38227 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadataanalysis_api.py
--rw-r--r--   0 root         (0) root         (0)    31555 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadatacollections_api.py
--rw-r--r--   0 root         (0) root         (0)    81013 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadatadata_api.py
--rw-r--r--   0 root         (0) root         (0)    38431 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadataglossary_api.py
--rw-r--r--   0 root         (0) root         (0)     8744 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadataproperties_api.py
--rw-r--r--   0 root         (0) root         (0)    28318 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadatarelationships_api.py
--rw-r--r--   0 root         (0) root         (0)    63432 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/projects_api.py
--rw-r--r--   0 root         (0) root         (0)   110972 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/queries_api.py
--rw-r--r--   0 root         (0) root         (0)    13300 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/search_api.py
--rw-r--r--   0 root         (0) root         (0)    16772 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/sparql_api.py
--rw-r--r--   0 root         (0) root         (0)    16725 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/sql_api.py
--rw-r--r--   0 root         (0) root         (0)    35935 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/streams_api.py
--rw-r--r--   0 root         (0) root         (0)     8896 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/tables_api.py
--rw-r--r--   0 root         (0) root         (0)    19032 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/uploads_api.py
--rw-r--r--   0 root         (0) root         (0)    28988 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/user_api.py
--rw-r--r--   0 root         (0) root         (0)     7736 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/users_api.py
--rw-r--r--   0 root         (0) root         (0)    62390 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/apis/webhooks_api.py
--rw-r--r--   0 root         (0) root         (0)     9331 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:07:55.508330 datadotworld-1.8.4/datadotworld/client/_swagger/models/
--rw-r--r--   0 root         (0) root         (0)     7843 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6327 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/agent_hydration_dto.py
--rw-r--r--   0 root         (0) root         (0)     4982 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/analysis_image.py
--rw-r--r--   0 root         (0) root         (0)     5891 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/asset_status.py
--rw-r--r--   0 root         (0) root         (0)    13985 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_analysis_hydration_dto.py
--rw-r--r--   0 root         (0) root         (0)    11170 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_analysis_request.py
--rw-r--r--   0 root         (0) root         (0)    14195 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_business_term_hydration_dto.py
--rw-r--r--   0 root         (0) root         (0)    12308 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_column_hydration_dto.py
--rw-r--r--   0 root         (0) root         (0)    12784 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_column_request.py
--rw-r--r--   0 root         (0) root         (0)     9947 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_concept_hydration_dto.py
--rw-r--r--   0 root         (0) root         (0)    12136 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_glossary_request.py
--rw-r--r--   0 root         (0) root         (0)     9553 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_hydration_dto.py
--rw-r--r--   0 root         (0) root         (0)     5683 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_id.py
--rw-r--r--   0 root         (0) root         (0)     6766 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_request.py
--rw-r--r--   0 root         (0) root         (0)    13442 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_table_hydration_dto.py
--rw-r--r--   0 root         (0) root         (0)    11089 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_table_request.py
--rw-r--r--   0 root         (0) root         (0)     6112 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/concept_entry.py
--rw-r--r--   0 root         (0) root         (0)    15493 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/connection_dto.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/create_dataset_response.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/create_insight_response.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/create_project_response.py
--rw-r--r--   0 root         (0) root         (0)     7542 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/create_query_request.py
--rw-r--r--   0 root         (0) root         (0)     5575 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/create_response.py
--rw-r--r--   0 root         (0) root         (0)     5238 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/custom_dataset_or_project_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     6291 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/database_credentials.py
--rw-r--r--   0 root         (0) root         (0)     9559 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/database_dbo.py
--rw-r--r--   0 root         (0) root         (0)     6155 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/database_source_reference.py
--rw-r--r--   0 root         (0) root         (0)    13076 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_create_request.py
--rw-r--r--   0 root         (0) root         (0)    11649 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_hydration_dto.py
--rw-r--r--   0 root         (0) root         (0)     5797 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_identifier.py
--rw-r--r--   0 root         (0) root         (0)    13004 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_patch_request.py
--rw-r--r--   0 root         (0) root         (0)    12971 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_put_request.py
--rw-r--r--   0 root         (0) root         (0)    20863 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/doi.py
--rw-r--r--   0 root         (0) root         (0)     7489 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/edit_activities_result_dto.py
--rw-r--r--   0 root         (0) root         (0)     5352 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/entry_type.py
--rw-r--r--   0 root         (0) root         (0)     6222 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/error_message.py
--rw-r--r--   0 root         (0) root         (0)     5378 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/file_batch_update_request.py
--rw-r--r--   0 root         (0) root         (0)     8630 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/file_create_or_update_request.py
--rw-r--r--   0 root         (0) root         (0)     8527 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/file_create_request.py
--rw-r--r--   0 root         (0) root         (0)    12670 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/file_source_create_or_update_request.py
--rw-r--r--   0 root         (0) root         (0)    12362 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/file_source_create_request.py
--rw-r--r--   0 root         (0) root         (0)    16194 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/file_source_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     9626 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/file_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     6412 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_body.py
--rw-r--r--   0 root         (0) root         (0)     9823 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_create_request.py
--rw-r--r--   0 root         (0) root         (0)    11616 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_hydration_dto.py
--rw-r--r--   0 root         (0) root         (0)     9653 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_patch_request.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_put_request.py
--rw-r--r--   0 root         (0) root         (0)    13350 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     5469 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/instant.py
--rw-r--r--   0 root         (0) root         (0)    17585 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/json_node.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/linked_dataset_create_or_update_request.py
--rw-r--r--   0 root         (0) root         (0)    15321 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/linked_dataset_summary_response.py
--rw-r--r--   0 root         (0) root         (0)    18804 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/metadata_resource_dto.py
--rw-r--r--   0 root         (0) root         (0)     7538 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/oauth_token_reference.py
--rw-r--r--   0 root         (0) root         (0)     6764 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_connection_results.py
--rw-r--r--   0 root         (0) root         (0)     6746 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_dataset_results.py
--rw-r--r--   0 root         (0) root         (0)     6598 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_insight_results.py
--rw-r--r--   0 root         (0) root         (0)     6872 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_metadata_resource_results.py
--rw-r--r--   0 root         (0) root         (0)     6598 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_project_results.py
--rw-r--r--   0 root         (0) root         (0)     6710 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_query_results.py
--rw-r--r--   0 root         (0) root         (0)     7858 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_search_results_dto.py
--rw-r--r--   0 root         (0) root         (0)     6791 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_subscription_results.py
--rw-r--r--   0 root         (0) root         (0)    12805 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/project_create_request.py
--rw-r--r--   0 root         (0) root         (0)    13177 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/project_patch_request.py
--rw-r--r--   0 root         (0) root         (0)    12424 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/project_put_request.py
--rw-r--r--   0 root         (0) root         (0)    15671 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/project_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     5729 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/query_parameter.py
--rw-r--r--   0 root         (0) root         (0)     6595 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/query_put_request.py
--rw-r--r--   0 root         (0) root         (0)    10756 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/query_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     6066 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/range.py
--rw-r--r--   0 root         (0) root         (0)     6914 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/rdf_term.py
--rw-r--r--   0 root         (0) root         (0)    13784 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/relationship_create_or_delete_request.py
--rw-r--r--   0 root         (0) root         (0)     7693 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/relationship_get_request.py
--rw-r--r--   0 root         (0) root         (0)     6555 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/relationship_get_table_request.py
--rw-r--r--   0 root         (0) root         (0)     5654 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/resource_relationship_dto.py
--rw-r--r--   0 root         (0) root         (0)     6459 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/saved_query_execution_request.py
--rw-r--r--   0 root         (0) root         (0)     5440 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/search_facet_result.py
--rw-r--r--   0 root         (0) root         (0)    11735 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/search_hydrations.py
--rw-r--r--   0 root         (0) root         (0)    12926 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/search_request.py
--rw-r--r--   0 root         (0) root         (0)     7980 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/simple_search_request.py
--rw-r--r--   0 root         (0) root         (0)     8283 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/single_table_metadata_spec.py
--rw-r--r--   0 root         (0) root         (0)     5461 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/source_id.py
--rw-r--r--   0 root         (0) root         (0)     6014 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/sql_query_request.py
--rw-r--r--   0 root         (0) root         (0)     7616 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/ssh_tunnel.py
--rw-r--r--   0 root         (0) root         (0)     6186 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/stream_schema.py
--rw-r--r--   0 root         (0) root         (0)     7901 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/stream_schema_patch_request.py
--rw-r--r--   0 root         (0) root         (0)     4296 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/streams_resource.py
--rw-r--r--   0 root         (0) root         (0)     7612 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5145 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/subscription_api_links.py
--rw-r--r--   0 root         (0) root         (0)     5819 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/subscription_create_request.py
--rw-r--r--   0 root         (0) root         (0)     4952 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/subscription_links.py
--rw-r--r--   0 root         (0) root         (0)     4890 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/success_message.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/table_batch_update_request.py
--rw-r--r--   0 root         (0) root         (0)     7367 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/table_create_or_update_request.py
--rw-r--r--   0 root         (0) root         (0)     6260 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/table_id.py
--rw-r--r--   0 root         (0) root         (0)     6043 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/table_source_create_or_update_request.py
--rw-r--r--   0 root         (0) root         (0)     5266 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     8065 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/user_data_response.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/user_identifier.py
--rw-r--r--   0 root         (0) root         (0)     7592 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/web_authorization.py
--rw-r--r--   0 root         (0) root         (0)     6628 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/models/web_credentials.py
--rw-r--r--   0 root         (0) root         (0)    14754 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/_swagger/rest.py
--rw-r--r--   0 root         (0) root         (0)    69179 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/api.py
--rw-r--r--   0 root         (0) root         (0)      796 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/client/content_negotiating_api_client.py
--rw-r--r--   0 root         (0) root         (0)     7935 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/config.py
--rw-r--r--   0 root         (0) root         (0)    13568 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/datadotworld.py
--rw-r--r--   0 root         (0) root         (0)     8624 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:07:55.508330 datadotworld-1.8.4/datadotworld/hosts/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/hosts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:07:55.508330 datadotworld-1.8.4/datadotworld/models/
--rw-r--r--   0 root         (0) root         (0)      682 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8573 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/models/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4687 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/models/query.py
--rw-r--r--   0 root         (0) root         (0)    11288 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/models/table_schema.py
--rw-r--r--   0 root         (0) root         (0)     6184 2023-02-03 15:06:42.000000 datadotworld-1.8.4/datadotworld/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:07:55.492330 datadotworld-1.8.4/datadotworld.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13253 2023-02-03 15:07:55.000000 datadotworld-1.8.4/datadotworld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8342 2023-02-03 15:07:55.000000 datadotworld-1.8.4/datadotworld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-03 15:07:55.000000 datadotworld-1.8.4/datadotworld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-02-03 15:07:55.000000 datadotworld-1.8.4/datadotworld.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      258 2023-02-03 15:07:55.000000 datadotworld-1.8.4/datadotworld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-03 15:07:55.000000 datadotworld-1.8.4/datadotworld.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      368 2023-02-03 15:07:55.508330 datadotworld-1.8.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3154 2023-02-03 15:06:42.000000 datadotworld-1.8.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:09:25.173494 datadotworld-1.8.5/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-04-19 16:08:25.000000 datadotworld-1.8.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 16:08:25.000000 datadotworld-1.8.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13253 2023-04-19 16:09:25.173494 datadotworld-1.8.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12251 2023-04-19 16:08:25.000000 datadotworld-1.8.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:09:25.157494 datadotworld-1.8.5/datadotworld/
+-rw-r--r--   0 root         (0) root         (0)     8877 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:09:25.157494 datadotworld-1.8.5/datadotworld/client/
+-rw-r--r--   0 root         (0) root         (0)      682 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:09:25.157494 datadotworld-1.8.5/datadotworld/client/_swagger/
+-rw-r--r--   0 root         (0) root         (0)     9608 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26099 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:09:25.161494 datadotworld-1.8.5/datadotworld/client/_swagger/apis/
+-rw-r--r--   0 root         (0) root         (0)      868 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22782 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/connections_api.py
+-rw-r--r--   0 root         (0) root         (0)    63079 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/datasets_api.py
+-rw-r--r--   0 root         (0) root         (0)    31953 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/do_is_api.py
+-rw-r--r--   0 root         (0) root         (0)    14485 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/download_api.py
+-rw-r--r--   0 root         (0) root         (0)    60948 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/files_api.py
+-rw-r--r--   0 root         (0) root         (0)    53754 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/insights_api.py
+-rw-r--r--   0 root         (0) root         (0)    38227 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadataanalysis_api.py
+-rw-r--r--   0 root         (0) root         (0)    31555 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadatacollections_api.py
+-rw-r--r--   0 root         (0) root         (0)    81013 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadatadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    38431 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadataglossary_api.py
+-rw-r--r--   0 root         (0) root         (0)     8744 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadataproperties_api.py
+-rw-r--r--   0 root         (0) root         (0)    28318 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadatarelationships_api.py
+-rw-r--r--   0 root         (0) root         (0)    63432 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/projects_api.py
+-rw-r--r--   0 root         (0) root         (0)   110972 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/queries_api.py
+-rw-r--r--   0 root         (0) root         (0)    13300 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/search_api.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/sparql_api.py
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/sql_api.py
+-rw-r--r--   0 root         (0) root         (0)    35935 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/streams_api.py
+-rw-r--r--   0 root         (0) root         (0)     8896 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/tables_api.py
+-rw-r--r--   0 root         (0) root         (0)    19032 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/uploads_api.py
+-rw-r--r--   0 root         (0) root         (0)    28988 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/user_api.py
+-rw-r--r--   0 root         (0) root         (0)     7736 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/users_api.py
+-rw-r--r--   0 root         (0) root         (0)    62390 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/apis/webhooks_api.py
+-rw-r--r--   0 root         (0) root         (0)     9331 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:09:25.173494 datadotworld-1.8.5/datadotworld/client/_swagger/models/
+-rw-r--r--   0 root         (0) root         (0)     7843 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/agent_hydration_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4982 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/analysis_image.py
+-rw-r--r--   0 root         (0) root         (0)     5891 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/asset_status.py
+-rw-r--r--   0 root         (0) root         (0)    13985 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_analysis_hydration_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11170 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_analysis_request.py
+-rw-r--r--   0 root         (0) root         (0)    14195 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_business_term_hydration_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12308 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_column_hydration_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12784 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_column_request.py
+-rw-r--r--   0 root         (0) root         (0)     9947 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_concept_hydration_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12136 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_glossary_request.py
+-rw-r--r--   0 root         (0) root         (0)     9553 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_hydration_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5683 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_id.py
+-rw-r--r--   0 root         (0) root         (0)     6766 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_request.py
+-rw-r--r--   0 root         (0) root         (0)    13442 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_table_hydration_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11089 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     6112 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/concept_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15493 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/connection_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/create_dataset_response.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/create_insight_response.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/create_project_response.py
+-rw-r--r--   0 root         (0) root         (0)     7542 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/create_query_request.py
+-rw-r--r--   0 root         (0) root         (0)     5575 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/create_response.py
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/custom_dataset_or_project_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     6291 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/database_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     9559 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/database_dbo.py
+-rw-r--r--   0 root         (0) root         (0)     6155 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/database_source_reference.py
+-rw-r--r--   0 root         (0) root         (0)    13076 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    11649 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_hydration_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5797 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    13004 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_patch_request.py
+-rw-r--r--   0 root         (0) root         (0)    12971 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_put_request.py
+-rw-r--r--   0 root         (0) root         (0)    20863 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/doi.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/edit_activities_result_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5352 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/entry_type.py
+-rw-r--r--   0 root         (0) root         (0)     6222 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/error_message.py
+-rw-r--r--   0 root         (0) root         (0)     5378 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/file_batch_update_request.py
+-rw-r--r--   0 root         (0) root         (0)     8630 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/file_create_or_update_request.py
+-rw-r--r--   0 root         (0) root         (0)     8527 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/file_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    12670 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/file_source_create_or_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    12362 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/file_source_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    16194 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/file_source_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     9626 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/file_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     6412 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_body.py
+-rw-r--r--   0 root         (0) root         (0)     9823 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    11616 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_hydration_dto.py
+-rw-r--r--   0 root         (0) root         (0)     9653 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_patch_request.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_put_request.py
+-rw-r--r--   0 root         (0) root         (0)    13350 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     5469 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/instant.py
+-rw-r--r--   0 root         (0) root         (0)    17585 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/json_node.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/linked_dataset_create_or_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    15321 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/linked_dataset_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)    18804 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/metadata_resource_dto.py
+-rw-r--r--   0 root         (0) root         (0)     7538 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/oauth_token_reference.py
+-rw-r--r--   0 root         (0) root         (0)     6764 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_connection_results.py
+-rw-r--r--   0 root         (0) root         (0)     6746 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_dataset_results.py
+-rw-r--r--   0 root         (0) root         (0)     6598 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_insight_results.py
+-rw-r--r--   0 root         (0) root         (0)     6872 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_metadata_resource_results.py
+-rw-r--r--   0 root         (0) root         (0)     6598 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_project_results.py
+-rw-r--r--   0 root         (0) root         (0)     6710 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_query_results.py
+-rw-r--r--   0 root         (0) root         (0)     7858 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_search_results_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6791 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_subscription_results.py
+-rw-r--r--   0 root         (0) root         (0)    12805 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/project_create_request.py
+-rw-r--r--   0 root         (0) root         (0)    13177 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/project_patch_request.py
+-rw-r--r--   0 root         (0) root         (0)    12424 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/project_put_request.py
+-rw-r--r--   0 root         (0) root         (0)    15671 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/project_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     5729 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/query_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/query_put_request.py
+-rw-r--r--   0 root         (0) root         (0)    10756 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/query_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     6066 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/range.py
+-rw-r--r--   0 root         (0) root         (0)     6914 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/rdf_term.py
+-rw-r--r--   0 root         (0) root         (0)    13784 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/relationship_create_or_delete_request.py
+-rw-r--r--   0 root         (0) root         (0)     7693 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/relationship_get_request.py
+-rw-r--r--   0 root         (0) root         (0)     6555 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/relationship_get_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     5654 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/resource_relationship_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6459 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/saved_query_execution_request.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/search_facet_result.py
+-rw-r--r--   0 root         (0) root         (0)    11735 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/search_hydrations.py
+-rw-r--r--   0 root         (0) root         (0)    12926 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/search_request.py
+-rw-r--r--   0 root         (0) root         (0)     7980 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/simple_search_request.py
+-rw-r--r--   0 root         (0) root         (0)     8283 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/single_table_metadata_spec.py
+-rw-r--r--   0 root         (0) root         (0)     5461 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/source_id.py
+-rw-r--r--   0 root         (0) root         (0)     6014 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/sql_query_request.py
+-rw-r--r--   0 root         (0) root         (0)     7616 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/ssh_tunnel.py
+-rw-r--r--   0 root         (0) root         (0)     6186 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/stream_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7901 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/stream_schema_patch_request.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/streams_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7612 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5145 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/subscription_api_links.py
+-rw-r--r--   0 root         (0) root         (0)     5819 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/subscription_create_request.py
+-rw-r--r--   0 root         (0) root         (0)     4952 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/subscription_links.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/success_message.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/table_batch_update_request.py
+-rw-r--r--   0 root         (0) root         (0)     7367 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/table_create_or_update_request.py
+-rw-r--r--   0 root         (0) root         (0)     6260 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/table_id.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/table_source_create_or_update_request.py
+-rw-r--r--   0 root         (0) root         (0)     5266 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     8065 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/user_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/user_identifier.py
+-rw-r--r--   0 root         (0) root         (0)     7592 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/web_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     6628 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/models/web_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    14754 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/_swagger/rest.py
+-rw-r--r--   0 root         (0) root         (0)    69179 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/api.py
+-rw-r--r--   0 root         (0) root         (0)      796 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/client/content_negotiating_api_client.py
+-rw-r--r--   0 root         (0) root         (0)     7935 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/config.py
+-rw-r--r--   0 root         (0) root         (0)    13568 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/datadotworld.py
+-rw-r--r--   0 root         (0) root         (0)     8624 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:09:25.173494 datadotworld-1.8.5/datadotworld/hosts/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/hosts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:09:25.173494 datadotworld-1.8.5/datadotworld/models/
+-rw-r--r--   0 root         (0) root         (0)      682 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8573 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/models/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/models/query.py
+-rw-r--r--   0 root         (0) root         (0)    11288 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/models/table_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2023-04-19 16:08:25.000000 datadotworld-1.8.5/datadotworld/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:09:25.157494 datadotworld-1.8.5/datadotworld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13253 2023-04-19 16:09:25.000000 datadotworld-1.8.5/datadotworld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8342 2023-04-19 16:09:25.000000 datadotworld-1.8.5/datadotworld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:09:25.000000 datadotworld-1.8.5/datadotworld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-19 16:09:25.000000 datadotworld-1.8.5/datadotworld.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-19 16:09:25.000000 datadotworld-1.8.5/datadotworld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 16:09:25.000000 datadotworld-1.8.5/datadotworld.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-19 16:09:25.173494 datadotworld-1.8.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-04-19 16:08:25.000000 datadotworld-1.8.5/setup.py
```

### Comparing `datadotworld-1.8.4/LICENSE.txt` & `datadotworld-1.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/PKG-INFO` & `datadotworld-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadotworld
-Version: 1.8.4
+Version: 1.8.5
 Summary: Python library for data.world
 Home-page: http://github.com/datadotworld/data.world-py
 Author: data.world
 Author-email: help@data.world
 License: Apache 2.0
 Keywords: data.world dataset
 Platform: UNKNOWN
```

### Comparing `datadotworld-1.8.4/README.rst` & `datadotworld-1.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/__init__.py` & `datadotworld-1.8.5/datadotworld/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     FileConfig,
     ChainedConfig,
     InlineConfig,
     EnvConfig
 )
 from datadotworld.datadotworld import DataDotWorld, UriParam  # noqa: F401
 
-__version__ = '1.8.4'
+__version__ = '1.8.5'
 
 # Convenience top-level functions
 
 __instances = weakref.WeakValueDictionary()
 
 
 def _get_instance(profile, **kwargs):
```

### Comparing `datadotworld-1.8.4/datadotworld/cli.py` & `datadotworld-1.8.5/datadotworld/cli.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/__init__.py` & `datadotworld-1.8.5/datadotworld/client/__init__.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/__init__.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/api_client.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/api_client.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/__init__.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/connections_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/connections_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/datasets_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/datasets_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/do_is_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/do_is_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/download_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/download_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/files_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/files_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/insights_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/insights_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadataanalysis_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadataanalysis_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadatacollections_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadatacollections_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadatadata_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadatadata_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadataglossary_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadataglossary_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadataproperties_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadataproperties_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/metadatarelationships_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/metadatarelationships_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/projects_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/projects_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/queries_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/queries_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/search_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/search_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/sparql_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/sparql_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/sql_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/sql_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/streams_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/streams_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/tables_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/tables_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/uploads_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/uploads_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/user_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/user_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/users_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/users_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/apis/webhooks_api.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/apis/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/configuration.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/configuration.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/__init__.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/agent_hydration_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/agent_hydration_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/analysis_image.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/analysis_image.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/asset_status.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/asset_status.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_analysis_hydration_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_analysis_hydration_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_analysis_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_analysis_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_business_term_hydration_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_business_term_hydration_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_column_hydration_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_column_hydration_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_column_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_column_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_concept_hydration_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_concept_hydration_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_glossary_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_glossary_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_hydration_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_hydration_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_id.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_id.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_table_hydration_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_table_hydration_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/catalog_table_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/catalog_table_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/concept_entry.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/concept_entry.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/connection_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/connection_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/create_dataset_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/create_dataset_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/create_insight_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/create_insight_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/create_project_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/create_project_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/create_query_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/create_query_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/create_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/create_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/custom_dataset_or_project_metadata_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/custom_dataset_or_project_metadata_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/database_credentials.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/database_credentials.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/database_dbo.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/database_dbo.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/database_source_reference.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/database_source_reference.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_create_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_create_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_hydration_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_hydration_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_identifier.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_identifier.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_patch_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_patch_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_put_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_put_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/dataset_summary_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/dataset_summary_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/doi.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/doi.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/edit_activities_result_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/edit_activities_result_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/entry_type.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/entry_type.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/error_message.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/error_message.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/file_batch_update_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/file_batch_update_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/file_create_or_update_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/file_create_or_update_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/file_create_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/file_create_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/file_source_create_or_update_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/file_source_create_or_update_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/file_source_create_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/file_source_create_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/file_source_summary_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/file_source_summary_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/file_summary_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/file_summary_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_body.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_body.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_create_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_create_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_hydration_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_hydration_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_patch_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_patch_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_put_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_put_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/insight_summary_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/insight_summary_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/instant.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/instant.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/json_node.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/json_node.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/linked_dataset_create_or_update_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/linked_dataset_create_or_update_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/linked_dataset_summary_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/linked_dataset_summary_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/metadata_resource_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/metadata_resource_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/oauth_token_reference.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/oauth_token_reference.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_connection_results.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_connection_results.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_dataset_results.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_dataset_results.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_insight_results.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_insight_results.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_metadata_resource_results.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_metadata_resource_results.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_project_results.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_project_results.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_query_results.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_query_results.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_search_results_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_search_results_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/paginated_subscription_results.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/paginated_subscription_results.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/project_create_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/project_create_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/project_patch_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/project_patch_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/project_put_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/project_put_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/project_summary_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/project_summary_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/query_parameter.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/query_parameter.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/query_put_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/query_put_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/query_summary_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/query_summary_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/range.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/range.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/rdf_term.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/rdf_term.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/relationship_create_or_delete_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/relationship_create_or_delete_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/relationship_get_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/relationship_get_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/relationship_get_table_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/relationship_get_table_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/resource_relationship_dto.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/resource_relationship_dto.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/saved_query_execution_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/saved_query_execution_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/search_facet_result.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/search_facet_result.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/search_hydrations.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/search_hydrations.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/search_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/search_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/simple_search_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/simple_search_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/single_table_metadata_spec.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/single_table_metadata_spec.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/source_id.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/source_id.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/sql_query_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/sql_query_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/ssh_tunnel.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/stream_schema.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/stream_schema.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/stream_schema_patch_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/stream_schema_patch_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/streams_resource.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/streams_resource.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/subscription.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/subscription.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/subscription_api_links.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/subscription_api_links.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/subscription_create_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/subscription_create_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/subscription_links.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/subscription_links.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/success_message.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/success_message.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/table_batch_update_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/table_batch_update_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/table_create_or_update_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/table_create_or_update_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/table_id.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/table_id.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/table_source_create_or_update_request.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/table_source_create_or_update_request.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/tag.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/tag.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/user_data_response.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/user_data_response.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/user_identifier.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/user_identifier.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/web_authorization.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/web_authorization.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/models/web_credentials.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/models/web_credentials.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/_swagger/rest.py` & `datadotworld-1.8.5/datadotworld/client/_swagger/rest.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/api.py` & `datadotworld-1.8.5/datadotworld/client/api.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/client/content_negotiating_api_client.py` & `datadotworld-1.8.5/datadotworld/client/content_negotiating_api_client.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/config.py` & `datadotworld-1.8.5/datadotworld/config.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/datadotworld.py` & `datadotworld-1.8.5/datadotworld/datadotworld.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/files.py` & `datadotworld-1.8.5/datadotworld/files.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/hosts/__init__.py` & `datadotworld-1.8.5/datadotworld/hosts/__init__.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/models/__init__.py` & `datadotworld-1.8.5/datadotworld/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/models/dataset.py` & `datadotworld-1.8.5/datadotworld/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/models/query.py` & `datadotworld-1.8.5/datadotworld/models/query.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/models/table_schema.py` & `datadotworld-1.8.5/datadotworld/models/table_schema.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld/util.py` & `datadotworld-1.8.5/datadotworld/util.py`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/datadotworld.egg-info/PKG-INFO` & `datadotworld-1.8.5/datadotworld.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadotworld
-Version: 1.8.4
+Version: 1.8.5
 Summary: Python library for data.world
 Home-page: http://github.com/datadotworld/data.world-py
 Author: data.world
 Author-email: help@data.world
 License: Apache 2.0
 Keywords: data.world dataset
 Platform: UNKNOWN
```

### Comparing `datadotworld-1.8.4/datadotworld.egg-info/SOURCES.txt` & `datadotworld-1.8.5/datadotworld.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datadotworld-1.8.4/setup.py` & `datadotworld-1.8.5/setup.py`

 * *Files identical despite different names*

