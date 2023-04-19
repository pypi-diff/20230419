# Comparing `tmp/qwak_core-0.0.25.tar.gz` & `tmp/qwak_core-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.25.tar", max compression
+gzip compressed data, was "qwak_core-0.0.26.tar", max compression
```

## Comparing `qwak_core-0.0.25.tar` & `qwak_core-0.0.26.tar`

### file list

```diff
@@ -1,536 +1,536 @@
--rw-r--r--   0        0        0      264 2023-04-19 07:31:12.015667 qwak_core-0.0.25/README.md
--rw-r--r--   0        0        0        0 2023-04-19 07:31:51.235492 qwak_core-0.0.25/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-04-19 07:31:51.255492 qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-04-19 07:31:36.643557 qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.255492 qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-04-19 07:31:51.251492 qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-04-19 07:31:36.379558 qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.251492 qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-04-19 07:31:51.251492 qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-04-19 07:31:36.511557 qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.255492 qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-04-19 07:31:51.247492 qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-04-19 07:31:35.979560 qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-04-19 07:31:51.247492 qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-19 07:31:51.247492 qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-04-19 07:31:36.115559 qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.247492 qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-04-19 07:31:51.251492 qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-04-19 07:31:36.247559 qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.251492 qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-04-19 07:31:51.235492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-04-19 07:31:35.847561 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-04-19 07:31:51.235492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-04-19 07:31:51.235492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-04-19 07:31:36.779556 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.239492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-04-19 07:31:51.239492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-04-19 07:31:37.043555 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.239492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-04-19 07:31:51.243492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-04-19 07:31:37.179555 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-04-19 07:31:51.243492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-04-19 07:31:51.239492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-04-19 07:31:36.911556 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.239492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-04-19 07:31:51.243492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-04-19 07:31:37.311554 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.243492 qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-04-19 07:31:51.279492 qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-04-19 07:31:39.179546 qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.283492 qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-04-19 07:31:51.283492 qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-04-19 07:31:39.315545 qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-04-19 07:31:51.283492 qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-04-19 07:31:51.339491 qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-04-19 07:31:42.947529 qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.339491 qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-04-19 07:31:51.343491 qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-04-19 07:31:43.079528 qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-04-19 07:31:51.343491 qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-04-19 07:31:51.343491 qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-04-19 07:31:43.787525 qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-04-19 07:31:51.347491 qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-04-19 07:31:51.343491 qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-04-19 07:31:43.647526 qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.343491 qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-04-19 07:31:51.347491 qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-04-19 07:31:43.919525 qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.347491 qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-04-19 07:31:51.347491 qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-04-19 07:31:44.051524 qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-04-19 07:31:51.351492 qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-04-19 07:31:51.399491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-04-19 07:31:47.871507 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.403491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-04-19 07:31:51.399491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-04-19 07:31:47.603508 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.399491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-04-19 07:31:51.399491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-04-19 07:31:47.735508 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.399491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-04-19 07:31:51.395491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-04-19 07:31:47.339509 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-04-19 07:31:51.395491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-04-19 07:31:51.395491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-04-19 07:31:47.471509 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.395491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-04-19 07:31:51.407491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-04-19 07:31:48.263505 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.407491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-04-19 07:31:51.403491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-04-19 07:31:48.131506 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.407491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     3604 2023-04-19 07:31:51.403491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4212 2023-04-19 07:31:48.003506 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.403491 qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-04-19 07:31:51.439491 qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-04-19 07:31:50.727494 qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.439491 qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-04-19 07:31:51.435491 qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-04-19 07:31:50.451496 qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.435491 qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-04-19 07:31:51.439491 qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-04-19 07:31:50.595495 qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-04-19 07:31:51.439491 qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-04-19 07:31:51.371491 qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-04-19 07:31:45.431518 qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-04-19 07:31:51.371491 qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-04-19 07:31:51.371491 qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-04-19 07:31:45.295518 qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.371491 qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-04-19 07:31:51.363491 qwak_core-0.0.25/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-04-19 07:31:45.027520 qwak_core-0.0.25/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.363491 qwak_core-0.0.25/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-04-19 07:31:51.363491 qwak_core-0.0.25/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-04-19 07:31:45.159519 qwak_core-0.0.25/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.363491 qwak_core-0.0.25/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-04-19 07:31:51.367491 qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-04-19 07:31:45.567517 qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-04-19 07:31:51.367491 qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-04-19 07:31:51.367491 qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-04-19 07:31:45.859516 qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-04-19 07:31:51.367491 qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-04-19 07:31:51.375491 qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-04-19 07:31:46.139515 qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.379491 qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-04-19 07:31:51.379491 qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-19 07:31:46.271514 qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-19 07:31:51.379491 qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-04-19 07:31:51.355491 qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-04-19 07:31:44.623521 qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.359491 qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-04-19 07:31:51.359491 qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-04-19 07:31:44.755521 qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-04-19 07:31:51.359491 qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-04-19 07:31:51.351492 qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-04-19 07:31:44.339523 qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.355491 qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-04-19 07:31:51.351492 qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-04-19 07:31:44.195523 qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.351492 qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-04-19 07:31:51.355491 qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-04-19 07:31:44.483522 qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-04-19 07:31:51.355491 qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-04-19 07:31:51.271492 qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-04-19 07:31:38.511549 qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.271492 qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-19 07:31:51.275492 qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-04-19 07:31:38.647548 qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.275492 qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    15709 2023-04-19 07:31:51.275492 qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    16335 2023-04-19 07:31:38.783547 qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-04-19 07:31:51.275492 qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-04-19 07:31:51.323492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-04-19 07:31:42.147532 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.323492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-04-19 07:31:51.319491 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-04-19 07:31:42.015533 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-04-19 07:31:51.323492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-04-19 07:31:51.307492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-04-19 07:31:40.947538 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.307492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-04-19 07:31:51.303492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-04-19 07:31:40.811538 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.303492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-04-19 07:31:51.299492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-04-19 07:31:40.395540 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.299492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-04-19 07:31:51.303492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-04-19 07:31:40.675539 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-04-19 07:31:51.303492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-04-19 07:31:51.307492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-04-19 07:31:41.083537 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.307492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-04-19 07:31:51.311492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-04-19 07:31:41.215537 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-04-19 07:31:51.311492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-04-19 07:31:51.299492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-04-19 07:31:40.535540 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.303492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-04-19 07:31:51.311492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-04-19 07:31:41.347536 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.311492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-04-19 07:31:51.323492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-04-19 07:31:50.863494 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.327492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-04-19 07:31:51.327492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-04-19 07:31:50.999493 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-04-19 07:31:51.327492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-04-19 07:31:51.327492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-04-19 07:31:42.547531 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.331492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-04-19 07:31:51.331492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-04-19 07:31:42.683530 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-04-19 07:31:51.331492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-04-19 07:31:51.331492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-04-19 07:31:42.815529 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.331492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-04-19 07:31:51.335492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-04-19 07:31:43.379527 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.335492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-04-19 07:31:51.335492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-04-19 07:31:43.219528 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-04-19 07:31:51.335492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-04-19 07:31:51.339491 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-04-19 07:31:43.515526 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.339491 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    13329 2023-04-19 07:31:51.315492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23039 2023-04-19 07:31:41.483535 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.315492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-04-19 07:31:51.315492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-04-19 07:31:41.615535 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.315492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-04-19 07:31:51.315492 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-04-19 07:31:41.751534 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-04-19 07:31:51.319491 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-04-19 07:31:51.319491 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-04-19 07:31:41.883534 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.319491 qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-04-19 07:31:51.407491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-04-19 07:31:48.395505 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.407491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-04-19 07:31:51.411491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-04-19 07:31:48.535504 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-19 07:31:51.411491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-04-19 07:31:51.411491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-04-19 07:31:48.671503 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.411491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-04-19 07:31:51.415491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-04-19 07:31:48.811503 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-19 07:31:51.415491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-04-19 07:31:51.415491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-04-19 07:31:48.951502 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-04-19 07:31:51.415491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-04-19 07:31:51.419491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-04-19 07:31:49.087502 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.419491 qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-04-19 07:31:51.379491 qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-04-19 07:31:46.403514 qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.383491 qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-04-19 07:31:51.383491 qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-19 07:31:46.535513 qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-19 07:31:51.383491 qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-04-19 07:31:51.287492 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-04-19 07:31:39.859543 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.287492 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-19 07:31:51.291492 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-04-19 07:31:39.991542 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.291492 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-04-19 07:31:51.291492 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-04-19 07:31:40.127541 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-04-19 07:31:51.295492 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-04-19 07:31:51.295492 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-04-19 07:31:40.255541 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.299492 qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-04-19 07:31:51.359491 qwak_core-0.0.25/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-04-19 07:31:44.891520 qwak_core-0.0.25/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-04-19 07:31:51.359491 qwak_core-0.0.25/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-04-19 07:31:51.419491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-04-19 07:31:49.219501 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.419491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-04-19 07:31:51.419491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-04-19 07:31:49.355500 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.423491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-04-19 07:31:51.423491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-04-19 07:31:49.491500 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.423491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-04-19 07:31:51.423491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-04-19 07:31:49.627499 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.427491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-19 07:31:51.427491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-04-19 07:31:49.767499 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.427491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-04-19 07:31:51.427491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-04-19 07:31:49.915498 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-04-19 07:31:51.431491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-04-19 07:31:51.431491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-04-19 07:31:50.047497 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.431491 qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-04-19 07:31:51.387491 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-04-19 07:31:46.803512 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.387491 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-04-19 07:31:51.391491 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-04-19 07:31:47.203510 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.391491 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-04-19 07:31:51.387491 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-04-19 07:31:46.935511 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-04-19 07:31:51.387491 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-04-19 07:31:51.391491 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-04-19 07:31:47.067510 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.391491 qwak_core-0.0.25/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-04-19 07:31:51.375491 qwak_core-0.0.25/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-04-19 07:31:46.007515 qwak_core-0.0.25/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-04-19 07:31:51.375491 qwak_core-0.0.25/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-04-19 07:31:51.267492 qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-04-19 07:31:39.587544 qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-04-19 07:31:51.267492 qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-04-19 07:31:51.267492 qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-04-19 07:31:39.451544 qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.267492 qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-04-19 07:31:51.271492 qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-04-19 07:31:39.723543 qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-04-19 07:31:51.271492 qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-04-19 07:31:51.375491 qwak_core-0.0.25/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-04-19 07:31:45.707517 qwak_core-0.0.25/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-04-19 07:31:51.375491 qwak_core-0.0.25/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-04-19 07:31:51.383491 qwak_core-0.0.25/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-04-19 07:31:46.671512 qwak_core-0.0.25/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-04-19 07:31:51.383491 qwak_core-0.0.25/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-04-19 07:31:51.263492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-04-19 07:31:37.975551 qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.263492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-04-19 07:31:51.263492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-04-19 07:31:37.843551 qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-04-19 07:31:51.263492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-04-19 07:31:51.255492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-04-19 07:31:37.443553 qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.259492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-04-19 07:31:51.259492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-04-19 07:31:37.571553 qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.259492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-04-19 07:31:51.259492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-04-19 07:31:37.707552 qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-04-19 07:31:51.263492 qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-04-19 07:31:51.435491 qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-04-19 07:31:50.319496 qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-04-19 07:31:51.435491 qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-04-19 07:31:51.431491 qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-04-19 07:31:50.187497 qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.435491 qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-04-19 07:31:51.279492 qwak_core-0.0.25/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-04-19 07:31:38.911547 qwak_core-0.0.25/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.279492 qwak_core-0.0.25/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3001 2023-04-19 07:31:51.279492 qwak_core-0.0.25/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2574 2023-04-19 07:31:39.043546 qwak_core-0.0.25/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 07:31:51.279492 qwak_core-0.0.25/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2107 2023-04-19 07:31:52.539486 qwak_core-0.0.25/pyproject.toml
--rw-r--r--   0        0        0      447 2023-04-19 07:31:52.539486 qwak_core-0.0.25/qwak/__init__.py
--rw-r--r--   0        0        0     1168 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    31798 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5478 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0       77 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/feedback/__init__.py
--rw-r--r--   0        0        0     2710 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/feedback/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4255 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     2585 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     1927 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     2006 2023-04-19 07:31:12.015667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2961 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1730 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    16848 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/const.py
--rw-r--r--   0        0        0     1417 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     6729 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5760 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2109 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0     2272 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/schema.py
--rw-r--r--   0        0        0     5609 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/schema_entities.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak/testing/fixtures.py
--rw-r--r--   0        0        0       46 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     1001 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4116 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13443 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-04-19 07:31:12.019667 qwak_core-0.0.25/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 qwak_core-0.0.25/setup.py
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-04-19 13:17:57.763055 qwak_core-0.0.26/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 13:18:49.615388 qwak_core-0.0.26/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-04-19 13:18:49.635388 qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-04-19 13:18:32.947281 qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.635388 qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-04-19 13:18:49.631389 qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-04-19 13:18:32.643279 qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.635388 qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-04-19 13:18:49.635388 qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-04-19 13:18:32.795281 qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.635388 qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-04-19 13:18:49.627389 qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-04-19 13:18:32.179277 qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-04-19 13:18:49.627389 qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-19 13:18:49.627389 qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-04-19 13:18:32.339278 qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.631389 qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-04-19 13:18:49.631389 qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-04-19 13:18:32.491279 qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.631389 qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-04-19 13:18:49.615388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-04-19 13:18:32.023275 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-04-19 13:18:49.615388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-04-19 13:18:49.619388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-04-19 13:18:33.103283 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.619388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-04-19 13:18:49.623388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-04-19 13:18:33.411285 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.623388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-04-19 13:18:49.623388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-04-19 13:18:33.563285 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-04-19 13:18:49.623388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-04-19 13:18:49.619388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-04-19 13:18:33.255283 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.619388 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-04-19 13:18:49.627389 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-04-19 13:18:33.719286 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.627389 qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-04-19 13:18:49.663389 qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-04-19 13:18:35.867300 qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.663389 qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-04-19 13:18:49.663389 qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-04-19 13:18:36.019301 qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-04-19 13:18:49.667389 qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-04-19 13:18:49.723389 qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-04-19 13:18:40.203328 qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.727389 qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-04-19 13:18:49.727389 qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-04-19 13:18:40.355329 qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-04-19 13:18:49.727389 qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-04-19 13:18:49.731389 qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-04-19 13:18:41.143334 qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-04-19 13:18:49.731389 qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-04-19 13:18:49.727389 qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-04-19 13:18:40.975333 qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.727389 qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-04-19 13:18:49.731389 qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-04-19 13:18:41.299335 qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.731389 qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-04-19 13:18:49.735389 qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-04-19 13:18:41.455336 qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-04-19 13:18:49.735389 qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-04-19 13:18:49.787390 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-04-19 13:18:45.815364 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.787390 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-04-19 13:18:49.783389 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-04-19 13:18:45.507362 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.783389 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-04-19 13:18:49.783389 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-04-19 13:18:45.659363 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.787390 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-04-19 13:18:49.779389 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-04-19 13:18:45.199360 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-04-19 13:18:49.779389 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-04-19 13:18:49.779389 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-04-19 13:18:45.351361 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.783389 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-04-19 13:18:49.791390 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-04-19 13:18:46.267367 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.791390 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-04-19 13:18:49.791390 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-04-19 13:18:46.115366 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.791390 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     3604 2023-04-19 13:18:49.787390 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4212 2023-04-19 13:18:45.963365 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.787390 qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-04-19 13:18:49.827390 qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-04-19 13:18:49.063385 qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.827390 qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-04-19 13:18:49.823390 qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-04-19 13:18:48.751383 qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.823390 qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-04-19 13:18:49.823390 qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-04-19 13:18:48.911384 qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-04-19 13:18:49.823390 qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-04-19 13:18:49.755389 qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-04-19 13:18:43.015346 qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-04-19 13:18:49.759389 qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-04-19 13:18:49.755389 qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-04-19 13:18:42.859345 qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.755389 qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-04-19 13:18:49.747389 qwak_core-0.0.26/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-04-19 13:18:42.551343 qwak_core-0.0.26/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.747389 qwak_core-0.0.26/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-04-19 13:18:49.747389 qwak_core-0.0.26/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-04-19 13:18:42.703344 qwak_core-0.0.26/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.751389 qwak_core-0.0.26/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-04-19 13:18:49.751389 qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-04-19 13:18:43.171347 qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-04-19 13:18:49.751389 qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-04-19 13:18:49.751389 qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-04-19 13:18:43.503349 qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-04-19 13:18:49.755389 qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-04-19 13:18:49.763389 qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-04-19 13:18:43.827351 qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.763389 qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-04-19 13:18:49.763389 qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-19 13:18:43.979352 qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-19 13:18:49.763389 qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-04-19 13:18:49.743389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-04-19 13:18:42.091340 qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.743389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-04-19 13:18:49.743389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-04-19 13:18:42.243341 qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-04-19 13:18:49.743389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-04-19 13:18:49.739389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-04-19 13:18:41.775338 qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.739389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-04-19 13:18:49.735389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-04-19 13:18:41.619337 qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.735389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-04-19 13:18:49.739389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-04-19 13:18:41.935339 qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-04-19 13:18:49.739389 qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-04-19 13:18:49.655389 qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-04-19 13:18:35.095295 qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.655389 qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-19 13:18:49.655389 qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-04-19 13:18:35.247296 qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.655389 qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    15709 2023-04-19 13:18:49.655389 qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    16335 2023-04-19 13:18:35.407297 qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-04-19 13:18:49.659389 qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-04-19 13:18:49.707389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-04-19 13:18:39.283322 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.707389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-04-19 13:18:49.707389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-04-19 13:18:39.131321 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-04-19 13:18:49.707389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-04-19 13:18:49.691389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-04-19 13:18:37.891313 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.691389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-04-19 13:18:49.691389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-04-19 13:18:37.735312 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.691389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-04-19 13:18:49.683389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-04-19 13:18:37.259309 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.683389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-04-19 13:18:49.687389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-04-19 13:18:37.583311 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-04-19 13:18:49.687389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-04-19 13:18:49.691389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-04-19 13:18:38.043314 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.695389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-04-19 13:18:49.695389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-04-19 13:18:38.203315 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-04-19 13:18:49.695389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24876 2023-04-19 13:18:49.687389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    36861 2023-04-19 13:18:37.419310 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.687389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-04-19 13:18:49.695389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-04-19 13:18:38.355316 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.699389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-04-19 13:18:49.711389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-04-19 13:18:49.219386 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.711389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-04-19 13:18:49.711389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-04-19 13:18:49.375387 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-04-19 13:18:49.711389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-04-19 13:18:49.715389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-04-19 13:18:39.743325 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.715389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-04-19 13:18:49.715389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-04-19 13:18:39.899326 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-04-19 13:18:49.715389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-04-19 13:18:49.715389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-04-19 13:18:40.051327 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.719389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-04-19 13:18:49.719389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-04-19 13:18:40.671331 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.723389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-04-19 13:18:49.719389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-04-19 13:18:40.511330 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-04-19 13:18:49.719389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-04-19 13:18:49.723389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-04-19 13:18:40.823332 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.723389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    13329 2023-04-19 13:18:49.699389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23039 2023-04-19 13:18:38.515317 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.699389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-04-19 13:18:49.699389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-04-19 13:18:38.671318 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.703389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-04-19 13:18:49.703389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-04-19 13:18:38.823319 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-04-19 13:18:49.703389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-04-19 13:18:49.703389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-04-19 13:18:38.979320 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.707389 qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-04-19 13:18:49.795390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-04-19 13:18:46.419368 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.795390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-04-19 13:18:49.795390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-04-19 13:18:46.571369 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-19 13:18:49.795390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-04-19 13:18:49.799390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-04-19 13:18:46.723370 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.799390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-04-19 13:18:49.799390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-04-19 13:18:46.883371 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-19 13:18:49.799390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-04-19 13:18:49.799390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-04-19 13:18:47.043372 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-04-19 13:18:49.803390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-04-19 13:18:49.803390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-04-19 13:18:47.195373 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.803390 qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-04-19 13:18:49.767389 qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-04-19 13:18:44.127353 qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.767389 qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-04-19 13:18:49.767389 qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-19 13:18:44.279354 qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-19 13:18:49.767389 qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-04-19 13:18:49.667389 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-04-19 13:18:36.639305 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.671389 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-19 13:18:49.671389 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-04-19 13:18:36.791306 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.675389 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-04-19 13:18:49.675389 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-04-19 13:18:36.943307 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-04-19 13:18:49.679389 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-04-19 13:18:49.679389 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-04-19 13:18:37.099308 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.683389 qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-04-19 13:18:49.743389 qwak_core-0.0.26/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-04-19 13:18:42.395342 qwak_core-0.0.26/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-04-19 13:18:49.747389 qwak_core-0.0.26/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-04-19 13:18:49.803390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-04-19 13:18:47.347374 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.807390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-04-19 13:18:49.807390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-04-19 13:18:47.499375 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.807390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-04-19 13:18:49.807390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-04-19 13:18:47.655376 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.811390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-04-19 13:18:49.811390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-04-19 13:18:47.811377 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.811390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-19 13:18:49.811390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-04-19 13:18:47.975378 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.811390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-04-19 13:18:49.815390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-04-19 13:18:48.139379 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-04-19 13:18:49.815390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-04-19 13:18:49.815390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-04-19 13:18:48.291380 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.815390 qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-04-19 13:18:49.771389 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-04-19 13:18:44.583356 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.771389 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-04-19 13:18:49.775390 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-04-19 13:18:45.039359 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.779389 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-04-19 13:18:49.775390 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-04-19 13:18:44.735357 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-04-19 13:18:49.775390 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-04-19 13:18:49.775390 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-04-19 13:18:44.887358 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.775390 qwak_core-0.0.26/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-04-19 13:18:49.759389 qwak_core-0.0.26/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-04-19 13:18:43.671350 qwak_core-0.0.26/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-04-19 13:18:49.763389 qwak_core-0.0.26/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-04-19 13:18:49.651389 qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-04-19 13:18:36.331303 qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-04-19 13:18:49.651389 qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-04-19 13:18:49.647389 qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-04-19 13:18:36.175302 qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.647389 qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-04-19 13:18:49.651389 qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-04-19 13:18:36.483304 qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-04-19 13:18:49.651389 qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-04-19 13:18:49.759389 qwak_core-0.0.26/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-04-19 13:18:43.335348 qwak_core-0.0.26/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-04-19 13:18:49.759389 qwak_core-0.0.26/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-04-19 13:18:49.771389 qwak_core-0.0.26/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-04-19 13:18:44.431355 qwak_core-0.0.26/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-04-19 13:18:49.771389 qwak_core-0.0.26/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-04-19 13:18:49.647389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-04-19 13:18:34.483291 qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.647389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-04-19 13:18:49.643389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-04-19 13:18:34.331290 qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-04-19 13:18:49.643389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-04-19 13:18:49.639389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-04-19 13:18:33.871287 qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.639389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-04-19 13:18:49.639389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-04-19 13:18:34.023288 qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.639389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-04-19 13:18:49.643389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-04-19 13:18:34.175289 qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-04-19 13:18:49.643389 qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-04-19 13:18:49.819390 qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-04-19 13:18:48.599382 qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-04-19 13:18:49.819390 qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-04-19 13:18:49.819390 qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-04-19 13:18:48.447381 qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.819390 qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-04-19 13:18:49.659389 qwak_core-0.0.26/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-04-19 13:18:35.559298 qwak_core-0.0.26/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.659389 qwak_core-0.0.26/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3001 2023-04-19 13:18:49.659389 qwak_core-0.0.26/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2574 2023-04-19 13:18:35.711299 qwak_core-0.0.26/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 13:18:49.663389 qwak_core-0.0.26/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2107 2023-04-19 13:18:50.963397 qwak_core-0.0.26/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-04-19 13:18:50.963397 qwak_core-0.0.26/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32139 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5478 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0       77 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/feedback/__init__.py
+-rw-r--r--   0        0        0     2710 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/feedback/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4255 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     2585 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0     1201 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.763055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     1927 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     2006 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2961 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1730 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    16848 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/const.py
+-rw-r--r--   0        0        0     1417 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     6729 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5760 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2109 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0     2272 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/schema.py
+-rw-r--r--   0        0        0     5609 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0       46 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     1001 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4116 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13443 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-04-19 13:17:57.767055 qwak_core-0.0.26/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 qwak_core-0.0.26/setup.py
+-rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.26/PKG-INFO
```

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.26/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.26/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/pyproject.toml` & `qwak_core-0.0.26/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.25"
+version = "0.0.26"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak"},
     {include = "_qwak_proto"},
```

### Comparing `qwak_core-0.0.25/qwak/automations/__init__.py` & `qwak_core-0.0.26/qwak/automations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     CustomWebhook,
     DeploymentCondition,
     DeploymentSpecifications,
     GpuResources,
     Metric,
     MetricBasedTrigger,
     MetricType,
+    NoneTrigger,
     Notification,
     QwakBuildDeploy,
     Resources,
     ScheduledTrigger,
     SlackNotification,
     SqlMetric,
     ThresholdDirection,
@@ -42,14 +43,15 @@
     "CustomWebhook",
     "DeploymentCondition",
     "DeploymentSpecifications",
     "GpuResources",
     "Metric",
     "MetricBasedTrigger",
     "MetricType",
+    "NoneTrigger",
     "Notification",
     "QwakBuildDeploy",
     "Resources",
     "ScheduledTrigger",
     "SlackNotification",
     "SqlMetric",
     "ThresholdDirection",
```

### Comparing `qwak_core-0.0.25/qwak/automations/automation_executions.py` & `qwak_core-0.0.26/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/automations/automations.py` & `qwak_core-0.0.26/qwak/automations/automations.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 )
 from _qwak_proto.qwak.automation.v1.notification_pb2 import (
     PostSlackNotification as PostSlackNotificationProto,
 )
 from _qwak_proto.qwak.automation.v1.trigger_pb2 import (
     MetricBasedTrigger as MetricBasedTriggerProto,
 )
+from _qwak_proto.qwak.automation.v1.trigger_pb2 import NoneTrigger as NoneTriggerProto
 from _qwak_proto.qwak.automation.v1.trigger_pb2 import (
     ScheduledTrigger as ScheduledTriggerProto,
 )
 from _qwak_proto.qwak.automation.v1.trigger_pb2 import Trigger as TriggerProto
 from google.protobuf.timestamp_pb2 import Timestamp
 
 
@@ -206,14 +207,24 @@
                 message.metric_based_trigger.threshold_direction
             ),
             override_cron=message.metric_based_trigger.override_cron,
         )
 
 
 @dataclass
+class NoneTrigger(Trigger):
+    def to_proto(self):
+        return TriggerProto(none_trigger=NoneTriggerProto())
+
+    @staticmethod
+    def from_proto(message: TriggerProto):
+        return NoneTrigger()
+
+
+@dataclass
 class SqlMetric(Metric):
     sql_query: str = field(default="")
 
     def to_proto(self):
         return MetricProto(sql_metric=SqlMetricProto(sql_query=self.sql_query))
 
     @staticmethod
@@ -895,14 +906,15 @@
     return mapping.get(auto_scaling_trigger_name)
 
 
 def map_trigger_name_to_class(trigger_name: str):
     mapping = {
         "scheduled_trigger": ScheduledTrigger,
         "metric_based_trigger": MetricBasedTrigger,
+        "none_trigger": NoneTrigger,
     }
 
     return mapping.get(trigger_name)
 
 
 def map_resources_name_to_class(resource_name: str):
     mapping = {"cpu_resources": CpuResources, "gpu_resources": GpuResources}
```

### Comparing `qwak_core-0.0.25/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.26/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.26/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.26/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.26/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.26/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/alert_management/client.py` & `qwak_core-0.0.26/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/analytics/client.py` & `qwak_core-0.0.26/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/audience/client.py` & `qwak_core-0.0.26/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/automation_management/client.py` & `qwak_core-0.0.26/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.26/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.26/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.26/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.26/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/build_management/client.py` & `qwak_core-0.0.26/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.26/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.26/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/deployment/client.py` & `qwak_core-0.0.26/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.26/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.26/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.26/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/feedback/client.py` & `qwak_core-0.0.26/qwak/clients/feedback/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.26/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.26/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/logging_client/client.py` & `qwak_core-0.0.26/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/model_management/client.py` & `qwak_core-0.0.26/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/project/client.py` & `qwak_core-0.0.26/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/secret_service/client.py` & `qwak_core-0.0.26/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.26/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.26/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.26/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.26/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.26/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.26/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.26/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.26/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.26/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.26/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.26/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/const.py` & `qwak_core-0.0.26/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.26/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.26/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.26/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.26/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/singleton_meta.py` & `qwak_core-0.0.26/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/tool/auth.py` & `qwak_core-0.0.26/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.26/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.26/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.26/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.26/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/adapters/__init__.py` & `qwak_core-0.0.26/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.26/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.26/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.26/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.26/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.26/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/base.py` & `qwak_core-0.0.26/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/decorators/api.py` & `qwak_core-0.0.26/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.26/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/experiment_tracking.py` & `qwak_core-0.0.26/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/schema.py` & `qwak_core-0.0.26/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model/schema_entities.py` & `qwak_core-0.0.26/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.26/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.26/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.26/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.26/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.26/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.26/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/qwak_client/client.py` & `qwak_core-0.0.26/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.26/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/qwak_client/models/model.py` & `qwak_core-0.0.26/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.26/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.26/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.26/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/qwak_services_mock/services_mock.py` & `qwak_core-0.0.26/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.25/setup.py` & `qwak_core-0.0.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
  'protobuf>=3.10,<4',
  'python-jose',
  'requests',
  'typeguard>=2,<3']
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.25',
+    'version': '0.0.26',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.25/PKG-INFO` & `qwak_core-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.25
+Version: 0.0.26
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

