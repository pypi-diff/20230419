# Comparing `tmp/whylabs-client-0.4.5.tar.gz` & `tmp/whylabs-client-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs-client-0.4.5.tar", last modified: Mon Apr 10 21:52:27 2023, max compression
+gzip compressed data, was "whylabs-client-0.4.6.tar", last modified: Wed Apr 19 16:58:31 2023, max compression
```

## Comparing `whylabs-client-0.4.5.tar` & `whylabs-client-0.4.6.tar`

### file list

```diff
@@ -1,148 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.841472 whylabs-client-0.4.5/
--rw-r--r--   0 root         (0) root         (0)      396 2023-04-10 21:52:27.841472 whylabs-client-0.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    21762 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-10 21:52:27.841472 whylabs-client-0.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-04-10 21:52:26.000000 whylabs-client-0.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.788666 whylabs-client-0.4.5/whylabs_client/
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.795640 whylabs-client-0.4.5/whylabs_client/api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15394 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/dataset_metadata_api.py
--rw-rw-rw-   0 root         (0) root         (0)    18502 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/dataset_profile_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/feature_weights_api.py
--rw-rw-rw-   0 root         (0) root         (0)    11520 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/log_api.py
--rw-rw-rw-   0 root         (0) root         (0)    20727 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/membership_api.py
--rw-rw-rw-   0 root         (0) root         (0)    67177 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/models_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52337 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/monitor_api.py
--rw-rw-rw-   0 root         (0) root         (0)    48204 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/notification_settings_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/schema_api.py
--rw-rw-rw-   0 root         (0) root         (0)    19879 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/sessions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37575 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.795640 whylabs-client-0.4.5/whylabs_client/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17084 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5075 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.840476 whylabs-client-0.4.5/whylabs_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11664 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/action_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12110 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/add_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12005 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/async_log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13478 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/aws_marketplace_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12443 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/column_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/create_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11207 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/create_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11136 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/create_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13099 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/databricks_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dataset_request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11114 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/datatype_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/delete_analyzer_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/delete_dataset_profiles_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/distribution_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11275 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_auto_scale_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13176 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_aws_attributes_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11715 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_aws_availability_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11665 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_cluster_log_conf_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11338 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_cron_schedule_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11082 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_dbfs_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11745 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_ebs_volume_type_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11928 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_job_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12392 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_job_email_notifications_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    15918 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_job_settings_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    14946 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_new_cluster_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11591 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_notebook_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11909 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_spark_jar_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11493 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_spark_python_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11281 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_spark_submit_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12338 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dtos3_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/email_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12313 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/entity_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11862 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/entity_weight_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11507 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/entity_weight_record_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11225 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11411 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11222 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_dataset_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_default_membership_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11431 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_marketplace_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11485 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11379 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_monitor_config_v2_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11417 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_notification_settings_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11334 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11559 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_jobs_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11260 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_jobs_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_models_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_organization_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11382 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_user_api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    11502 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/log_async_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11354 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11858 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/log_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11441 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/marketplace_dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)    12029 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/membership.py
--rw-rw-rw-   0 root         (0) root         (0)    11756 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/membership_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12260 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/metric_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11120 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/missing_recent_data_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11132 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/missing_recent_profiles_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/missing_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    12569 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/model_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12219 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/monitor_config_version.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/monitor_request_reference.py
--rw-rw-rw-   0 root         (0) root         (0)    11689 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/monitor_request_reference_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11783 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11982 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/notification_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11979 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/notification_settings_day.py
--rw-rw-rw-   0 root         (0) root         (0)    11751 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/notification_sqs_message_cadence.py
--rw-rw-rw-   0 root         (0) root         (0)    14425 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/organization_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    13737 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/organization_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/pager_duty_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12319 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provided_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11680 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11657 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11882 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_new_aws_marketplace_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12226 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_new_marketplace_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12422 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_new_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12315 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/reference_profile_item_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11188 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/refresh_access_token_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11444 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/refresh_connection_by_org_id_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11586 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/refresh_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13668 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/register_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11112 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/register_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11317 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/remove_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13372 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/request_feature_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15325 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11070 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/response.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/role.py
--rw-rw-rw-   0 root         (0) root         (0)    11922 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/run_job_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11089 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/run_job_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11471 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/schema_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/seasonal_arima_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/segment.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/segment_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/segment_weight.py
--rw-rw-rw-   0 root         (0) root         (0)    11948 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/session_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/set_default_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11193 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/slack_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11652 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/subscription_tier.py
--rw-rw-rw-   0 root         (0) root         (0)    11670 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/time_period.py
--rw-rw-rw-   0 root         (0) root         (0)    12934 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/uber_notification_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)    11917 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/unique_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/update_connection_changes.py
--rw-rw-rw-   0 root         (0) root         (0)    11816 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/update_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11650 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/update_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11747 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/user.py
--rw-rw-rw-   0 root         (0) root         (0)    13667 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/user_api_key.py
--rw-rw-rw-   0 root         (0) root         (0)    11220 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/user_api_key_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/why_logs_metric.py
--rw-rw-rw-   0 root         (0) root         (0)    81897 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.840476 whylabs-client-0.4.5/whylabs_client/models/
--rw-rw-rw-   0 root         (0) root         (0)     9219 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14199 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.790658 whylabs-client-0.4.5/whylabs_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      396 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6285 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.307100 whylabs-client-0.4.6/
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-04-19 16:58:31.307100 whylabs-client-0.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    22425 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-19 16:58:31.307100 whylabs-client-0.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.260098 whylabs-client-0.4.6/whylabs_client/
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.266098 whylabs-client-0.4.6/whylabs_client/api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15394 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/dataset_metadata_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    18502 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/dataset_profile_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/feature_weights_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11520 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/log_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20727 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/membership_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    67177 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/models_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52337 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/monitor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    48204 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/notification_settings_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/schema_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    29965 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/sessions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37575 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.266098 whylabs-client-0.4.6/whylabs_client/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17084 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5075 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.306100 whylabs-client-0.4.6/whylabs_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11664 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/action_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12110 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/add_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12005 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/async_log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13478 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/aws_marketplace_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11342 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/batch_log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11655 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/batch_log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12443 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/column_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/create_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11207 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/create_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/create_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13099 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/databricks_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dataset_request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11114 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/datatype_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/delete_analyzer_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/delete_dataset_profiles_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/distribution_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11275 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_auto_scale_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13176 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_aws_attributes_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11715 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_aws_availability_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11665 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_cluster_log_conf_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11338 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_cron_schedule_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11082 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_dbfs_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11745 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_ebs_volume_type_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11928 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_job_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12392 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_job_email_notifications_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    15918 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_job_settings_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14946 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_new_cluster_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11591 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_notebook_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11909 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_spark_jar_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11493 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_spark_python_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11281 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_spark_submit_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12338 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dtos3_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/email_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12313 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/entity_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/entity_weight_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11507 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/entity_weight_record_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11411 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11222 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_dataset_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_default_membership_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11431 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_marketplace_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11485 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11379 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_monitor_config_v2_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11417 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_notification_settings_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11559 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_jobs_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11260 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_jobs_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_models_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_organization_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11382 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_user_api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    11502 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_async_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11858 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11441 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12111 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/marketplace_dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/membership.py
+-rw-rw-rw-   0 root         (0) root         (0)    11756 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/membership_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12260 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/metric_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11120 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/missing_recent_data_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11132 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/missing_recent_profiles_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/missing_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12569 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/model_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12219 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/monitor_config_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/monitor_request_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    11689 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/monitor_request_reference_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11783 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11982 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/notification_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/notification_settings_day.py
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/notification_sqs_message_cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)    14425 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/organization_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    13737 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/organization_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/pager_duty_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12319 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provided_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11680 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11657 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11882 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_new_aws_marketplace_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12226 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_new_marketplace_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12422 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_new_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12315 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/reference_profile_item_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11188 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/refresh_access_token_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11444 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/refresh_connection_by_org_id_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11586 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/refresh_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13668 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/register_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11112 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/register_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11317 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/remove_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13372 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/request_feature_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15325 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11070 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/role.py
+-rw-rw-rw-   0 root         (0) root         (0)    11922 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/run_job_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11089 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/run_job_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11471 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/schema_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/seasonal_arima_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/segment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/segment_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/segment_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)    11948 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/session_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/set_default_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11193 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/slack_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11652 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/subscription_tier.py
+-rw-rw-rw-   0 root         (0) root         (0)    11670 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/time_period.py
+-rw-rw-rw-   0 root         (0) root         (0)    12934 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/uber_notification_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)    11917 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/unique_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/update_connection_changes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11816 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/update_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11650 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/update_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11747 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/user.py
+-rw-rw-rw-   0 root         (0) root         (0)    13667 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/user_api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    11220 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/user_api_key_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/why_logs_metric.py
+-rw-rw-rw-   0 root         (0) root         (0)    81897 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.306100 whylabs-client-0.4.6/whylabs_client/models/
+-rw-rw-rw-   0 root         (0) root         (0)     9500 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14199 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.261098 whylabs-client-0.4.6/whylabs_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6453 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/top_level.txt
```

### Comparing `whylabs-client-0.4.5/README.md` & `whylabs-client-0.4.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # whylabs-client
 WhyLabs API that enables end-to-end AI observability
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1
-- Package version: 0.4.5
+- Package version: 0.4.6
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://whylabs.ai](https://whylabs.ai)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -139,26 +139,30 @@
 *NotificationSettingsApi* | [**get_pager_duty_notification_action_payload**](docs/NotificationSettingsApi.md#get_pager_duty_notification_action_payload) | **GET** /v0/notification-settings/actions/pagerduty/payload | Get dummy notification action payload
 *NotificationSettingsApi* | [**get_slack_notification_action_payload**](docs/NotificationSettingsApi.md#get_slack_notification_action_payload) | **GET** /v0/notification-settings/actions/slack/payload | Get dummy notification action payload
 *NotificationSettingsApi* | [**list_notification_actions**](docs/NotificationSettingsApi.md#list_notification_actions) | **GET** /v0/notification-settings/{org_id}/actions | List notification actions for an org
 *NotificationSettingsApi* | [**put_notification_action**](docs/NotificationSettingsApi.md#put_notification_action) | **PUT** /v0/notification-settings/{org_id}/actions/{type}/{action_id} | Add new notification action
 *NotificationSettingsApi* | [**test_notification_action**](docs/NotificationSettingsApi.md#test_notification_action) | **POST** /v0/notification-settings/{org_id}/actions/{action_id}/test | Test a notification action
 *NotificationSettingsApi* | [**update_notification_action**](docs/NotificationSettingsApi.md#update_notification_action) | **PATCH** /v0/notification-settings/{org_id}/actions/{type}/{action_id} | Update notification action
 *SchemaApi* | [**get_monitor_config_schema**](docs/SchemaApi.md#get_monitor_config_schema) | **GET** /v0/organizations/{org_id}/schema/monitor-config | Get the current supported schema of the monitor configuration
+*SessionsApi* | [**batch_create_reference_profile_upload**](docs/SessionsApi.md#batch_create_reference_profile_upload) | **POST** /v0/sessions/{session_id}/references | Create multiple reference profile uploads for a given session.
+*SessionsApi* | [**claim_guest_session**](docs/SessionsApi.md#claim_guest_session) | **POST** /v0/sessions/{session_id}/claim | Claim a guest session, copying its model data into another org and expiring the session.
 *SessionsApi* | [**create_dataset_profile_upload**](docs/SessionsApi.md#create_dataset_profile_upload) | **POST** /v0/sessions/{session_id}/upload | Create an upload for a given session.
 *SessionsApi* | [**create_reference_profile_upload**](docs/SessionsApi.md#create_reference_profile_upload) | **POST** /v0/sessions/{session_id}/reference | Create a reference profile upload for a given session.
 *SessionsApi* | [**create_session**](docs/SessionsApi.md#create_session) | **POST** /v0/sessions | Create a new session that can be used to upload dataset profiles from whylogs for display in whylabs.
 *SessionsApi* | [**get_session**](docs/SessionsApi.md#get_session) | **GET** /v0/sessions/{session_id} | Get information about a session.
 
 
 ## Documentation For Models
 
  - [AWSMarketplaceMetadata](docs/AWSMarketplaceMetadata.md)
  - [ActionType](docs/ActionType.md)
  - [AddMembershipRequest](docs/AddMembershipRequest.md)
  - [AsyncLogResponse](docs/AsyncLogResponse.md)
+ - [BatchLogReferenceRequest](docs/BatchLogReferenceRequest.md)
+ - [BatchLogSessionReferenceResponse](docs/BatchLogSessionReferenceResponse.md)
  - [ColumnSchema](docs/ColumnSchema.md)
  - [CreateSessionRequest](docs/CreateSessionRequest.md)
  - [CreateSessionResponse](docs/CreateSessionResponse.md)
  - [CreateUserRequest](docs/CreateUserRequest.md)
  - [DTOAutoScaleDTO](docs/DTOAutoScaleDTO.md)
  - [DTOAwsAttributesDTO](docs/DTOAwsAttributesDTO.md)
  - [DTOAwsAvailabilityDTO](docs/DTOAwsAvailabilityDTO.md)
@@ -200,14 +204,15 @@
  - [ListModelsResponse](docs/ListModelsResponse.md)
  - [ListOrganizationMembershipsResponse](docs/ListOrganizationMembershipsResponse.md)
  - [ListUserApiKeys](docs/ListUserApiKeys.md)
  - [LogAsyncRequest](docs/LogAsyncRequest.md)
  - [LogReferenceRequest](docs/LogReferenceRequest.md)
  - [LogReferenceResponse](docs/LogReferenceResponse.md)
  - [LogResponse](docs/LogResponse.md)
+ - [LogSessionReferenceResponse](docs/LogSessionReferenceResponse.md)
  - [MarketplaceDimensions](docs/MarketplaceDimensions.md)
  - [Membership](docs/Membership.md)
  - [MembershipMetadata](docs/MembershipMetadata.md)
  - [MetricSchema](docs/MetricSchema.md)
  - [MissingRecentDataRequestConfig](docs/MissingRecentDataRequestConfig.md)
  - [MissingRecentProfilesRequestConfig](docs/MissingRecentProfilesRequestConfig.md)
  - [MissingValuesMonitorRequestConfig](docs/MissingValuesMonitorRequestConfig.md)
```

### Comparing `whylabs-client-0.4.5/whylabs_client/__init__.py` & `whylabs-client-0.4.6/whylabs_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 0.1
     Contact: support@whylabs.ai
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 
 # import ApiClient
 from whylabs_client.api_client import ApiClient
 
 # import Configuration
 from whylabs_client.configuration import Configuration
```

### Comparing `whylabs-client-0.4.5/whylabs_client/api/dataset_metadata_api.py` & `whylabs-client-0.4.6/whylabs_client/api/dataset_metadata_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/api/dataset_profile_api.py` & `whylabs-client-0.4.6/whylabs_client/api/dataset_profile_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/api/feature_weights_api.py` & `whylabs-client-0.4.6/whylabs_client/api/feature_weights_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/api/log_api.py` & `whylabs-client-0.4.6/whylabs_client/api/log_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/api/membership_api.py` & `whylabs-client-0.4.6/whylabs_client/api/membership_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/api/models_api.py` & `whylabs-client-0.4.6/whylabs_client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/api/monitor_api.py` & `whylabs-client-0.4.6/whylabs_client/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/api/notification_settings_api.py` & `whylabs-client-0.4.6/whylabs_client/api/notification_settings_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/api/schema_api.py` & `whylabs-client-0.4.6/whylabs_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/api/sessions_api.py` & `whylabs-client-0.4.6/whylabs_client/api/sessions_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,33 +19,148 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from whylabs_client.model.async_log_response import AsyncLogResponse
+from whylabs_client.model.batch_log_reference_request import BatchLogReferenceRequest
+from whylabs_client.model.batch_log_session_reference_response import BatchLogSessionReferenceResponse
 from whylabs_client.model.create_session_request import CreateSessionRequest
 from whylabs_client.model.create_session_response import CreateSessionResponse
 from whylabs_client.model.get_session_response import GetSessionResponse
 from whylabs_client.model.log_async_request import LogAsyncRequest
 from whylabs_client.model.log_reference_request import LogReferenceRequest
-from whylabs_client.model.log_reference_response import LogReferenceResponse
+from whylabs_client.model.log_session_reference_response import LogSessionReferenceResponse
 
 
 class SessionsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.batch_create_reference_profile_upload_endpoint = _Endpoint(
+            settings={
+                'response_type': (BatchLogSessionReferenceResponse,),
+                'auth': [],
+                'endpoint_path': '/v0/sessions/{session_id}/references',
+                'operation_id': 'batch_create_reference_profile_upload',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'session_id',
+                    'batch_log_reference_request',
+                ],
+                'required': [
+                    'session_id',
+                    'batch_log_reference_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'session_id':
+                        (str,),
+                    'batch_log_reference_request':
+                        (BatchLogReferenceRequest,),
+                },
+                'attribute_map': {
+                    'session_id': 'session_id',
+                },
+                'location_map': {
+                    'session_id': 'path',
+                    'batch_log_reference_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.claim_guest_session_endpoint = _Endpoint(
+            settings={
+                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/sessions/{session_id}/claim',
+                'operation_id': 'claim_guest_session',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'session_id',
+                    'org_id',
+                ],
+                'required': [
+                    'session_id',
+                    'org_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'session_id':
+                        (str,),
+                    'org_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'session_id': 'session_id',
+                    'org_id': 'org_id',
+                },
+                'location_map': {
+                    'session_id': 'path',
+                    'org_id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.create_dataset_profile_upload_endpoint = _Endpoint(
             settings={
                 'response_type': (AsyncLogResponse,),
                 'auth': [],
                 'endpoint_path': '/v0/sessions/{session_id}/upload',
                 'operation_id': 'create_dataset_profile_upload',
                 'http_method': 'POST',
@@ -96,15 +211,15 @@
                     'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_reference_profile_upload_endpoint = _Endpoint(
             settings={
-                'response_type': (LogReferenceResponse,),
+                'response_type': (LogSessionReferenceResponse,),
                 'auth': [],
                 'endpoint_path': '/v0/sessions/{session_id}/reference',
                 'operation_id': 'create_reference_profile_upload',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
@@ -252,14 +367,164 @@
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
+    def batch_create_reference_profile_upload(
+        self,
+        session_id,
+        batch_log_reference_request,
+        **kwargs
+    ):
+        """Create multiple reference profile uploads for a given session.  # noqa: E501
+
+        Create multiple reference profile uploads for a given session.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.batch_create_reference_profile_upload(session_id, batch_log_reference_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            session_id (str):
+            batch_log_reference_request (BatchLogReferenceRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            BatchLogSessionReferenceResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['session_id'] = \
+            session_id
+        kwargs['batch_log_reference_request'] = \
+            batch_log_reference_request
+        return self.batch_create_reference_profile_upload_endpoint.call_with_http_info(**kwargs)
+
+    def claim_guest_session(
+        self,
+        session_id,
+        org_id,
+        **kwargs
+    ):
+        """Claim a guest session, copying its model data into another org and expiring the session.  # noqa: E501
+
+        Claim a guest session, copying its model data into another org and expiring the session.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.claim_guest_session(session_id, org_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            session_id (str):
+            org_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['session_id'] = \
+            session_id
+        kwargs['org_id'] = \
+            org_id
+        return self.claim_guest_session_endpoint.call_with_http_info(**kwargs)
+
     def create_dataset_profile_upload(
         self,
         session_id,
         log_async_request,
         **kwargs
     ):
         """Create an upload for a given session.  # noqa: E501
@@ -371,15 +636,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            LogReferenceResponse
+            LogSessionReferenceResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `whylabs-client-0.4.5/whylabs_client/api_client.py` & `whylabs-client-0.4.6/whylabs_client/api_client.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/apis/__init__.py` & `whylabs-client-0.4.6/whylabs_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/configuration.py` & `whylabs-client-0.4.6/whylabs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.4.5".\
+               "SDK Package Version: 0.4.6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `whylabs-client-0.4.5/whylabs_client/exceptions.py` & `whylabs-client-0.4.6/whylabs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/action_type.py` & `whylabs-client-0.4.6/whylabs_client/model/action_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/add_membership_request.py` & `whylabs-client-0.4.6/whylabs_client/model/add_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/async_log_response.py` & `whylabs-client-0.4.6/whylabs_client/model/async_log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/aws_marketplace_metadata.py` & `whylabs-client-0.4.6/whylabs_client/model/aws_marketplace_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/column_schema.py` & `whylabs-client-0.4.6/whylabs_client/model/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/create_session_request.py` & `whylabs-client-0.4.6/whylabs_client/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/create_session_response.py` & `whylabs-client-0.4.6/whylabs_client/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/create_user_request.py` & `whylabs-client-0.4.6/whylabs_client/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/databricks_connection.py` & `whylabs-client-0.4.6/whylabs_client/model/databricks_connection.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dataset_request_monitor_config.py` & `whylabs-client-0.4.6/whylabs_client/model/dataset_request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/datatype_monitor_request_config.py` & `whylabs-client-0.4.6/whylabs_client/model/datatype_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/delete_analyzer_results_response.py` & `whylabs-client-0.4.6/whylabs_client/model/delete_analyzer_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/delete_dataset_profiles_response.py` & `whylabs-client-0.4.6/whylabs_client/model/delete_dataset_profiles_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/distribution_monitor_request_config.py` & `whylabs-client-0.4.6/whylabs_client/model/distribution_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_auto_scale_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_auto_scale_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_aws_attributes_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_aws_attributes_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_aws_availability_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_aws_availability_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_cluster_log_conf_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_cluster_log_conf_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_cron_schedule_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_cron_schedule_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_dbfs_storage_info_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_dbfs_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_ebs_volume_type_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_ebs_volume_type_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_job_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_job_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_job_email_notifications_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_job_email_notifications_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_job_settings_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_job_settings_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_new_cluster_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_new_cluster_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_notebook_task_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_notebook_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_spark_jar_task_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_spark_jar_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_spark_python_task_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_spark_python_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dto_spark_submit_task_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dto_spark_submit_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/dtos3_storage_info_dto.py` & `whylabs-client-0.4.6/whylabs_client/model/dtos3_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/email_notification_action.py` & `whylabs-client-0.4.6/whylabs_client/model/email_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/entity_schema.py` & `whylabs-client-0.4.6/whylabs_client/model/entity_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/entity_weight_record.py` & `whylabs-client-0.4.6/whylabs_client/model/entity_weight_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/entity_weight_record_metadata.py` & `whylabs-client-0.4.6/whylabs_client/model/entity_weight_record_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/feature_flags.py` & `whylabs-client-0.4.6/whylabs_client/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/get_connection_request.py` & `whylabs-client-0.4.6/whylabs_client/model/get_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/get_connection_response.py` & `whylabs-client-0.4.6/whylabs_client/model/get_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/get_dataset_metadata_response.py` & `whylabs-client-0.4.6/whylabs_client/model/get_dataset_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/get_default_membership_response.py` & `whylabs-client-0.4.6/whylabs_client/model/get_default_membership_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/get_marketplace_metadata_response.py` & `whylabs-client-0.4.6/whylabs_client/model/get_marketplace_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/get_memberships_response.py` & `whylabs-client-0.4.6/whylabs_client/model/get_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/get_monitor_config_v2_response.py` & `whylabs-client-0.4.6/whylabs_client/model/get_monitor_config_v2_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/get_notification_settings_response.py` & `whylabs-client-0.4.6/whylabs_client/model/get_notification_settings_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/get_session_response.py` & `whylabs-client-0.4.6/whylabs_client/model/get_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/list_jobs_request.py` & `whylabs-client-0.4.6/whylabs_client/model/list_jobs_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/list_jobs_response.py` & `whylabs-client-0.4.6/whylabs_client/model/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/list_models_response.py` & `whylabs-client-0.4.6/whylabs_client/model/list_models_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/list_organization_memberships_response.py` & `whylabs-client-0.4.6/whylabs_client/model/list_organization_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/list_user_api_keys.py` & `whylabs-client-0.4.6/whylabs_client/model/list_user_api_keys.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/log_async_request.py` & `whylabs-client-0.4.6/whylabs_client/model/log_async_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/log_reference_request.py` & `whylabs-client-0.4.6/whylabs_client/model/log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/log_reference_response.py` & `whylabs-client-0.4.6/whylabs_client/model/log_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/log_response.py` & `whylabs-client-0.4.6/whylabs_client/model/log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/marketplace_dimensions.py` & `whylabs-client-0.4.6/whylabs_client/model/marketplace_dimensions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/membership.py` & `whylabs-client-0.4.6/whylabs_client/model/membership.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/membership_metadata.py` & `whylabs-client-0.4.6/whylabs_client/model/membership_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/metric_schema.py` & `whylabs-client-0.4.6/whylabs_client/model/metric_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/missing_recent_data_request_config.py` & `whylabs-client-0.4.6/whylabs_client/model/missing_recent_data_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/missing_recent_profiles_request_config.py` & `whylabs-client-0.4.6/whylabs_client/model/missing_recent_profiles_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/missing_values_monitor_request_config.py` & `whylabs-client-0.4.6/whylabs_client/model/missing_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/model_metadata_response.py` & `whylabs-client-0.4.6/whylabs_client/model/model_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/model_type.py` & `whylabs-client-0.4.6/whylabs_client/model/model_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/monitor_config.py` & `whylabs-client-0.4.6/whylabs_client/model/monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/monitor_config_version.py` & `whylabs-client-0.4.6/whylabs_client/model/monitor_config_version.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/monitor_request_reference.py` & `whylabs-client-0.4.6/whylabs_client/model/monitor_request_reference.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/monitor_request_reference_type.py` & `whylabs-client-0.4.6/whylabs_client/model/monitor_request_reference_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/notification_action.py` & `whylabs-client-0.4.6/whylabs_client/model/notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/notification_settings.py` & `whylabs-client-0.4.6/whylabs_client/model/notification_settings.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/notification_settings_day.py` & `whylabs-client-0.4.6/whylabs_client/model/notification_settings_day.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/notification_sqs_message_cadence.py` & `whylabs-client-0.4.6/whylabs_client/model/notification_sqs_message_cadence.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/organization_metadata.py` & `whylabs-client-0.4.6/whylabs_client/model/organization_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/organization_summary.py` & `whylabs-client-0.4.6/whylabs_client/model/organization_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/pager_duty_notification_action.py` & `whylabs-client-0.4.6/whylabs_client/model/pager_duty_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/provided_config.py` & `whylabs-client-0.4.6/whylabs_client/model/provided_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/provision_databricks_connection_request.py` & `whylabs-client-0.4.6/whylabs_client/model/provision_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/provision_databricks_connection_response.py` & `whylabs-client-0.4.6/whylabs_client/model/provision_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/provision_new_aws_marketplace_user_response.py` & `whylabs-client-0.4.6/whylabs_client/model/provision_new_aws_marketplace_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/provision_new_marketplace_user_request.py` & `whylabs-client-0.4.6/whylabs_client/model/provision_new_marketplace_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/provision_new_user_request.py` & `whylabs-client-0.4.6/whylabs_client/model/provision_new_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/provision_new_user_response.py` & `whylabs-client-0.4.6/whylabs_client/model/provision_new_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/reference_profile_item_response.py` & `whylabs-client-0.4.6/whylabs_client/model/reference_profile_item_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/refresh_access_token_request.py` & `whylabs-client-0.4.6/whylabs_client/model/refresh_access_token_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/refresh_connection_by_org_id_response.py` & `whylabs-client-0.4.6/whylabs_client/model/refresh_connection_by_org_id_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/refresh_connection_request.py` & `whylabs-client-0.4.6/whylabs_client/model/refresh_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/register_databricks_connection_request.py` & `whylabs-client-0.4.6/whylabs_client/model/register_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/register_databricks_connection_response.py` & `whylabs-client-0.4.6/whylabs_client/model/register_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/remove_membership_request.py` & `whylabs-client-0.4.6/whylabs_client/model/remove_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/request_feature_monitor_config.py` & `whylabs-client-0.4.6/whylabs_client/model/request_feature_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/request_monitor_config.py` & `whylabs-client-0.4.6/whylabs_client/model/request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/response.py` & `whylabs-client-0.4.6/whylabs_client/model/response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/role.py` & `whylabs-client-0.4.6/whylabs_client/model/role.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/run_job_request.py` & `whylabs-client-0.4.6/whylabs_client/model/run_job_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/run_job_response.py` & `whylabs-client-0.4.6/whylabs_client/model/run_job_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/schema_metadata.py` & `whylabs-client-0.4.6/whylabs_client/model/schema_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/seasonal_arima_request_config.py` & `whylabs-client-0.4.6/whylabs_client/model/seasonal_arima_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/segment.py` & `whylabs-client-0.4.6/whylabs_client/model/segment.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/segment_tag.py` & `whylabs-client-0.4.6/whylabs_client/model/segment_tag.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/segment_weight.py` & `whylabs-client-0.4.6/whylabs_client/model/segment_weight.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/session_metadata.py` & `whylabs-client-0.4.6/whylabs_client/model/session_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/set_default_membership_request.py` & `whylabs-client-0.4.6/whylabs_client/model/set_default_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/slack_notification_action.py` & `whylabs-client-0.4.6/whylabs_client/model/slack_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/subscription_tier.py` & `whylabs-client-0.4.6/whylabs_client/model/subscription_tier.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/time_period.py` & `whylabs-client-0.4.6/whylabs_client/model/time_period.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/uber_notification_schedule.py` & `whylabs-client-0.4.6/whylabs_client/model/uber_notification_schedule.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/unique_values_monitor_request_config.py` & `whylabs-client-0.4.6/whylabs_client/model/unique_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/update_connection_changes.py` & `whylabs-client-0.4.6/whylabs_client/model/update_connection_changes.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/update_connection_request.py` & `whylabs-client-0.4.6/whylabs_client/model/update_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/update_membership_request.py` & `whylabs-client-0.4.6/whylabs_client/model/update_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/user.py` & `whylabs-client-0.4.6/whylabs_client/model/user.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/user_api_key.py` & `whylabs-client-0.4.6/whylabs_client/model/user_api_key.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/user_api_key_response.py` & `whylabs-client-0.4.6/whylabs_client/model/user_api_key_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model/why_logs_metric.py` & `whylabs-client-0.4.6/whylabs_client/model/why_logs_metric.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/model_utils.py` & `whylabs-client-0.4.6/whylabs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client/models/__init__.py` & `whylabs-client-0.4.6/whylabs_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # import sys
 # sys.setrecursionlimit(n)
 
 from whylabs_client.model.aws_marketplace_metadata import AWSMarketplaceMetadata
 from whylabs_client.model.action_type import ActionType
 from whylabs_client.model.add_membership_request import AddMembershipRequest
 from whylabs_client.model.async_log_response import AsyncLogResponse
+from whylabs_client.model.batch_log_reference_request import BatchLogReferenceRequest
+from whylabs_client.model.batch_log_session_reference_response import BatchLogSessionReferenceResponse
 from whylabs_client.model.column_schema import ColumnSchema
 from whylabs_client.model.create_session_request import CreateSessionRequest
 from whylabs_client.model.create_session_response import CreateSessionResponse
 from whylabs_client.model.create_user_request import CreateUserRequest
 from whylabs_client.model.dto_auto_scale_dto import DTOAutoScaleDTO
 from whylabs_client.model.dto_aws_attributes_dto import DTOAwsAttributesDTO
 from whylabs_client.model.dto_aws_availability_dto import DTOAwsAvailabilityDTO
@@ -58,14 +60,15 @@
 from whylabs_client.model.list_models_response import ListModelsResponse
 from whylabs_client.model.list_organization_memberships_response import ListOrganizationMembershipsResponse
 from whylabs_client.model.list_user_api_keys import ListUserApiKeys
 from whylabs_client.model.log_async_request import LogAsyncRequest
 from whylabs_client.model.log_reference_request import LogReferenceRequest
 from whylabs_client.model.log_reference_response import LogReferenceResponse
 from whylabs_client.model.log_response import LogResponse
+from whylabs_client.model.log_session_reference_response import LogSessionReferenceResponse
 from whylabs_client.model.marketplace_dimensions import MarketplaceDimensions
 from whylabs_client.model.membership import Membership
 from whylabs_client.model.membership_metadata import MembershipMetadata
 from whylabs_client.model.metric_schema import MetricSchema
 from whylabs_client.model.missing_recent_data_request_config import MissingRecentDataRequestConfig
 from whylabs_client.model.missing_recent_profiles_request_config import MissingRecentProfilesRequestConfig
 from whylabs_client.model.missing_values_monitor_request_config import MissingValuesMonitorRequestConfig
```

### Comparing `whylabs-client-0.4.5/whylabs_client/rest.py` & `whylabs-client-0.4.6/whylabs_client/rest.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.5/whylabs_client.egg-info/SOURCES.txt` & `whylabs-client-0.4.6/whylabs_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 whylabs_client/api/sessions_api.py
 whylabs_client/apis/__init__.py
 whylabs_client/model/__init__.py
 whylabs_client/model/action_type.py
 whylabs_client/model/add_membership_request.py
 whylabs_client/model/async_log_response.py
 whylabs_client/model/aws_marketplace_metadata.py
+whylabs_client/model/batch_log_reference_request.py
+whylabs_client/model/batch_log_session_reference_response.py
 whylabs_client/model/column_schema.py
 whylabs_client/model/create_session_request.py
 whylabs_client/model/create_session_response.py
 whylabs_client/model/create_user_request.py
 whylabs_client/model/databricks_connection.py
 whylabs_client/model/dataset_request_monitor_config.py
 whylabs_client/model/datatype_monitor_request_config.py
@@ -74,14 +76,15 @@
 whylabs_client/model/list_models_response.py
 whylabs_client/model/list_organization_memberships_response.py
 whylabs_client/model/list_user_api_keys.py
 whylabs_client/model/log_async_request.py
 whylabs_client/model/log_reference_request.py
 whylabs_client/model/log_reference_response.py
 whylabs_client/model/log_response.py
+whylabs_client/model/log_session_reference_response.py
 whylabs_client/model/marketplace_dimensions.py
 whylabs_client/model/membership.py
 whylabs_client/model/membership_metadata.py
 whylabs_client/model/metric_schema.py
 whylabs_client/model/missing_recent_data_request_config.py
 whylabs_client/model/missing_recent_profiles_request_config.py
 whylabs_client/model/missing_values_monitor_request_config.py
```

