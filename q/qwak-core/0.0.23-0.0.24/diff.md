# Comparing `tmp/qwak_core-0.0.23.tar.gz` & `tmp/qwak_core-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.23.tar", max compression
+gzip compressed data, was "qwak_core-0.0.24.tar", max compression
```

## Comparing `qwak_core-0.0.23.tar` & `qwak_core-0.0.24.tar`

### file list

```diff
@@ -1,537 +1,537 @@
--rw-r--r--   0        0        0      264 2023-04-18 13:37:22.335605 qwak_core-0.0.23/README.md
--rw-r--r--   0        0        0        0 2023-04-18 13:38:04.547560 qwak_core-0.0.23/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-04-18 13:38:04.571560 qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-04-18 13:37:48.891577 qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.571560 qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-04-18 13:38:04.567560 qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-04-18 13:37:48.603577 qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.567560 qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-04-18 13:38:04.567560 qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-04-18 13:37:48.743577 qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.571560 qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-04-18 13:38:04.563560 qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-04-18 13:37:48.171578 qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-04-18 13:38:04.563560 qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-18 13:38:04.563560 qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-04-18 13:37:48.315577 qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.563560 qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-04-18 13:38:04.567560 qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-04-18 13:37:48.459577 qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.567560 qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-04-18 13:38:04.551560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-04-18 13:37:48.027578 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-04-18 13:38:04.551560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-04-18 13:38:04.551560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-04-18 13:37:49.035577 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.551560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-04-18 13:38:04.555560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-04-18 13:37:49.319576 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.555560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-04-18 13:38:04.559560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-04-18 13:37:49.467576 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-04-18 13:38:04.559560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-04-18 13:38:04.555560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-04-18 13:37:49.179576 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.555560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-04-18 13:38:04.559560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-04-18 13:37:49.611576 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.559560 qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-04-18 13:38:04.599560 qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-04-18 13:37:51.667574 qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.599560 qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-04-18 13:38:04.599560 qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-04-18 13:37:51.815574 qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-04-18 13:38:04.599560 qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-04-18 13:38:04.659560 qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-04-18 13:37:55.731570 qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.659560 qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-04-18 13:38:04.659560 qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-04-18 13:37:55.879569 qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-04-18 13:38:04.663560 qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-04-18 13:38:04.663560 qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-04-18 13:37:56.603569 qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-04-18 13:38:04.663560 qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-04-18 13:38:04.663560 qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-04-18 13:37:56.459569 qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.663560 qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-04-18 13:38:04.667560 qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-04-18 13:37:56.747568 qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.667560 qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-04-18 13:38:04.667560 qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-04-18 13:37:56.887568 qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-04-18 13:38:04.667560 qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-04-18 13:38:04.723560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-04-18 13:38:00.975564 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.723560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-04-18 13:38:04.719560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-04-18 13:38:00.687564 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.719560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-04-18 13:38:04.723560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-04-18 13:38:00.831564 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.723560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-04-18 13:38:04.715560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-04-18 13:38:00.403565 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-04-18 13:38:04.715560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-04-18 13:38:04.719560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-04-18 13:38:00.547565 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.719560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-04-18 13:38:04.727560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-04-18 13:38:01.403564 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.731560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-04-18 13:38:04.727560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-04-18 13:38:01.263564 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.727560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     3604 2023-04-18 13:38:04.727560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4212 2023-04-18 13:38:01.123564 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.727560 qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-04-18 13:38:04.763560 qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-04-18 13:38:04.019561 qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.767560 qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-04-18 13:38:04.759560 qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-04-18 13:38:03.719561 qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.763560 qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-04-18 13:38:04.763560 qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-04-18 13:38:03.871561 qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-04-18 13:38:04.763560 qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-04-18 13:38:04.691560 qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-04-18 13:37:58.351567 qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-04-18 13:38:04.691560 qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-04-18 13:38:04.691560 qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-04-18 13:37:58.203567 qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.691560 qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-04-18 13:38:04.683560 qwak_core-0.0.23/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-04-18 13:37:57.911567 qwak_core-0.0.23/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.683560 qwak_core-0.0.23/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-04-18 13:38:04.683560 qwak_core-0.0.23/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-04-18 13:37:58.059567 qwak_core-0.0.23/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.683560 qwak_core-0.0.23/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-04-18 13:38:04.687560 qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-04-18 13:37:58.491567 qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-04-18 13:38:04.687560 qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-04-18 13:38:04.687560 qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-04-18 13:37:58.811566 qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-04-18 13:38:04.687560 qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-04-18 13:38:04.699560 qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-04-18 13:37:59.111566 qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.699560 qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-04-18 13:38:04.699560 qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-18 13:37:59.251566 qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-18 13:38:04.699560 qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-04-18 13:38:04.675560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-04-18 13:37:57.479568 qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.675560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-04-18 13:38:04.679560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-04-18 13:37:57.619568 qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-04-18 13:38:04.679560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-04-18 13:38:04.671560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-04-18 13:37:57.187568 qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.671560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-04-18 13:38:04.671560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-04-18 13:37:57.039568 qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.671560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-04-18 13:38:04.675560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-04-18 13:37:57.339568 qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-04-18 13:38:04.675560 qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-04-18 13:38:04.587560 qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-04-18 13:37:50.911575 qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.591560 qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-18 13:38:04.591560 qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-04-18 13:37:51.079574 qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.591560 qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    15709 2023-04-18 13:38:04.591560 qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    16335 2023-04-18 13:37:51.231574 qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-04-18 13:38:04.591560 qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-04-18 13:38:04.639560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-04-18 13:37:54.875571 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.643560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-04-18 13:38:04.639560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-04-18 13:37:54.735571 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-04-18 13:38:04.639560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-04-18 13:38:04.623560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-04-18 13:37:53.575572 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.623560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-04-18 13:38:04.623560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-04-18 13:37:53.431572 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.623560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-04-18 13:38:04.615560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-04-18 13:37:52.979573 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.615560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-04-18 13:38:04.619560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-04-18 13:37:53.287572 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-04-18 13:38:04.619560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-04-18 13:38:04.627560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-04-18 13:37:53.719572 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.627560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-04-18 13:38:04.627560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-04-18 13:37:53.863572 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-04-18 13:38:04.627560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-04-18 13:38:04.619560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-04-18 13:37:53.135572 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.619560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-04-18 13:38:04.627560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-04-18 13:37:54.007571 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.631560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-04-18 13:38:04.643560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-04-18 13:38:04.163561 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.643560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-04-18 13:38:04.643560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-04-18 13:38:04.307561 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-04-18 13:38:04.647560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-04-18 13:38:04.647560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-04-18 13:37:55.303570 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.647560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-04-18 13:38:04.647560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-04-18 13:37:55.443570 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-04-18 13:38:04.651560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-04-18 13:38:04.651560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-04-18 13:37:55.587570 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.651560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-04-18 13:38:04.655560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-04-18 13:37:56.171569 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.655560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-04-18 13:38:04.651560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-04-18 13:37:56.023569 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-04-18 13:38:04.655560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-04-18 13:38:04.655560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-04-18 13:37:56.315569 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.659560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    13329 2023-04-18 13:38:04.631560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23039 2023-04-18 13:37:54.155571 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.631560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-04-18 13:38:04.631560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-04-18 13:37:54.303571 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.635560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-04-18 13:38:04.635560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-04-18 13:37:54.447571 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-04-18 13:38:04.635560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-04-18 13:38:04.635560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-04-18 13:37:54.591571 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.639560 qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-04-18 13:38:04.731560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-04-18 13:38:01.551564 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.731560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-04-18 13:38:04.731560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-04-18 13:38:01.695563 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-18 13:38:04.735560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-04-18 13:38:04.735560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-04-18 13:38:01.835563 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.735560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-04-18 13:38:04.735560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-04-18 13:38:01.983563 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-18 13:38:04.739560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-04-18 13:38:04.739560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-04-18 13:38:02.131563 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-04-18 13:38:04.739560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-04-18 13:38:04.739560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-04-18 13:38:02.275563 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.743560 qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-04-18 13:38:04.703560 qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-04-18 13:37:59.395566 qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.703560 qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-04-18 13:38:04.703560 qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-18 13:37:59.535566 qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-18 13:38:04.703560 qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-04-18 13:38:04.603560 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-04-18 13:37:52.399573 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.603560 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-18 13:38:04.607560 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-04-18 13:37:52.539573 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.607560 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-04-18 13:38:04.611560 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-04-18 13:37:52.683573 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-04-18 13:38:04.611560 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-04-18 13:38:04.611560 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-04-18 13:37:52.827573 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.615560 qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-04-18 13:38:04.679560 qwak_core-0.0.23/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-04-18 13:37:57.767567 qwak_core-0.0.23/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-04-18 13:38:04.679560 qwak_core-0.0.23/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-04-18 13:38:04.743560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-04-18 13:38:02.419563 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.743560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-04-18 13:38:04.743560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-04-18 13:38:02.555562 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.747560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-04-18 13:38:04.747560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-04-18 13:38:02.703562 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.747560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-04-18 13:38:04.747560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-04-18 13:38:02.843562 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.751560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-18 13:38:04.751560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-04-18 13:38:02.991562 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.751560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-04-18 13:38:04.751560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-04-18 13:38:03.147562 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-04-18 13:38:04.755560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-04-18 13:38:04.755560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-04-18 13:38:03.291562 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.755560 qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-04-18 13:38:04.707560 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-04-18 13:37:59.823565 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.707560 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-04-18 13:38:04.715560 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-04-18 13:38:00.255565 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.715560 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-04-18 13:38:04.711560 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-04-18 13:37:59.967565 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-04-18 13:38:04.711560 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-04-18 13:38:04.711560 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-04-18 13:38:00.111565 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.711560 qwak_core-0.0.23/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-04-18 13:38:04.695560 qwak_core-0.0.23/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-04-18 13:37:58.967566 qwak_core-0.0.23/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-04-18 13:38:04.695560 qwak_core-0.0.23/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-04-18 13:38:04.583560 qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-04-18 13:37:52.107573 qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-04-18 13:38:04.587560 qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-04-18 13:38:04.583560 qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-04-18 13:37:51.963574 qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.583560 qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-04-18 13:38:04.587560 qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-04-18 13:37:52.255573 qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-04-18 13:38:04.587560 qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-04-18 13:38:04.695560 qwak_core-0.0.23/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-04-18 13:37:58.647567 qwak_core-0.0.23/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-04-18 13:38:04.695560 qwak_core-0.0.23/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-04-18 13:38:04.707560 qwak_core-0.0.23/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-04-18 13:37:59.679566 qwak_core-0.0.23/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-04-18 13:38:04.707560 qwak_core-0.0.23/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-04-18 13:38:04.579560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-04-18 13:37:50.335575 qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.583560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-04-18 13:38:04.579560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-04-18 13:37:50.191575 qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-04-18 13:38:04.579560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-04-18 13:38:04.571560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-04-18 13:37:49.755576 qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.575560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-04-18 13:38:04.575560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-04-18 13:37:49.899576 qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.575560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-04-18 13:38:04.575560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-04-18 13:37:50.043576 qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-04-18 13:38:04.579560 qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-04-18 13:38:04.759560 qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-04-18 13:38:03.571561 qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-04-18 13:38:04.759560 qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-04-18 13:38:04.755560 qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-04-18 13:38:03.431562 qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.759560 qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-04-18 13:38:04.595560 qwak_core-0.0.23/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-04-18 13:37:51.375574 qwak_core-0.0.23/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.595560 qwak_core-0.0.23/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3001 2023-04-18 13:38:04.595560 qwak_core-0.0.23/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2574 2023-04-18 13:37:51.519574 qwak_core-0.0.23/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-18 13:38:04.595560 qwak_core-0.0.23/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2107 2023-04-18 13:38:05.519559 qwak_core-0.0.23/pyproject.toml
--rw-r--r--   0        0        0      447 2023-04-18 13:38:05.519559 qwak_core-0.0.23/qwak/__init__.py
--rw-r--r--   0        0        0     1168 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    31798 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5478 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0       77 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/feedback/__init__.py
--rw-r--r--   0        0        0     2710 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/feedback/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4255 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     2585 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     1927 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     2006 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2961 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1730 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    16848 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/inner/const.py
--rw-r--r--   0        0        0     1417 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     6729 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-04-18 13:37:22.339605 qwak_core-0.0.23/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5760 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2109 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0     2272 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/schema.py
--rw-r--r--   0        0        0     5609 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/schema_entities.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak/testing/fixtures.py
--rw-r--r--   0        0        0       46 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     1001 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4116 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13443 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-04-18 13:37:22.343605 qwak_core-0.0.23/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 qwak_core-0.0.23/setup.py
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.23/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-04-19 07:05:48.995262 qwak_core-0.0.24/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 07:06:30.751002 qwak_core-0.0.24/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-04-19 07:06:30.771002 qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-04-19 07:06:15.451100 qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.775002 qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-04-19 07:06:30.771002 qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-04-19 07:06:15.175102 qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.771002 qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-04-19 07:06:30.771002 qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-04-19 07:06:15.315101 qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.771002 qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-04-19 07:06:30.763002 qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-04-19 07:06:14.759104 qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-04-19 07:06:30.763002 qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-19 07:06:30.767002 qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-04-19 07:06:14.899103 qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.767002 qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-04-19 07:06:30.767002 qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-04-19 07:06:15.039102 qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.767002 qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-04-19 07:06:30.751002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-04-19 07:06:14.619105 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-04-19 07:06:30.755002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-04-19 07:06:30.755002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-04-19 07:06:15.591099 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.755002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-04-19 07:06:30.759002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-04-19 07:06:15.867097 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.759002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-04-19 07:06:30.759002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-04-19 07:06:16.007097 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-04-19 07:06:30.759002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-04-19 07:06:30.755002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-04-19 07:06:15.727098 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.755002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-04-19 07:06:30.763002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-04-19 07:06:16.147096 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.763002 qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-04-19 07:06:30.799002 qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-04-19 07:06:18.103083 qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.799002 qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-04-19 07:06:30.803002 qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-04-19 07:06:18.247083 qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-04-19 07:06:30.803002 qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-04-19 07:06:30.859001 qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-04-19 07:06:22.087059 qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.859001 qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-04-19 07:06:30.863001 qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-04-19 07:06:22.227058 qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-04-19 07:06:30.863001 qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-04-19 07:06:30.867001 qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-04-19 07:06:22.935054 qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-04-19 07:06:30.867001 qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-04-19 07:06:30.863001 qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-04-19 07:06:22.791055 qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.863001 qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-04-19 07:06:30.867001 qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-04-19 07:06:23.075053 qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.867001 qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-04-19 07:06:30.871001 qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-04-19 07:06:23.219052 qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-04-19 07:06:30.871001 qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-04-19 07:06:30.923001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-04-19 07:06:27.215027 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.927001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-04-19 07:06:30.919001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-04-19 07:06:26.935029 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.923001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-04-19 07:06:30.923001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-04-19 07:06:27.075028 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.923001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-04-19 07:06:30.915001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-04-19 07:06:26.655031 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-04-19 07:06:30.919001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-04-19 07:06:30.919001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-04-19 07:06:26.799030 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.919001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-04-19 07:06:30.931001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-04-19 07:06:27.627025 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.931001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-04-19 07:06:30.927001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-04-19 07:06:27.491026 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.931001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     3604 2023-04-19 07:06:30.927001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4212 2023-04-19 07:06:27.351026 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.927001 qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-04-19 07:06:30.963001 qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-04-19 07:06:30.219006 qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.967001 qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-04-19 07:06:30.959001 qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-04-19 07:06:29.923008 qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.963001 qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-04-19 07:06:30.963001 qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-04-19 07:06:30.075007 qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-04-19 07:06:30.963001 qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-04-19 07:06:30.895001 qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-04-19 07:06:24.659043 qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-04-19 07:06:30.895001 qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-04-19 07:06:30.891001 qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-04-19 07:06:24.515044 qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.891001 qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-04-19 07:06:30.883001 qwak_core-0.0.24/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-04-19 07:06:24.231046 qwak_core-0.0.24/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.883001 qwak_core-0.0.24/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-04-19 07:06:30.887001 qwak_core-0.0.24/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-04-19 07:06:24.371045 qwak_core-0.0.24/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.887001 qwak_core-0.0.24/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-04-19 07:06:30.887001 qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-04-19 07:06:24.799042 qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-04-19 07:06:30.887001 qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-04-19 07:06:30.891001 qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-04-19 07:06:25.111040 qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-04-19 07:06:30.891001 qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-04-19 07:06:30.899001 qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-04-19 07:06:25.403039 qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.899001 qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-04-19 07:06:30.903001 qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-19 07:06:25.539038 qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-19 07:06:30.903001 qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-04-19 07:06:30.879001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-04-19 07:06:23.807048 qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.879001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-04-19 07:06:30.879001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-04-19 07:06:23.947048 qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-04-19 07:06:30.879001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-04-19 07:06:30.875001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-04-19 07:06:23.515050 qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.875001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-04-19 07:06:30.871001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-04-19 07:06:23.371051 qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.871001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-04-19 07:06:30.875001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-04-19 07:06:23.667049 qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-04-19 07:06:30.875001 qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-04-19 07:06:30.791002 qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-04-19 07:06:17.403088 qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.791002 qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-19 07:06:30.791002 qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-04-19 07:06:17.543087 qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.791002 qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    15709 2023-04-19 07:06:30.795002 qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    16335 2023-04-19 07:06:17.683086 qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-04-19 07:06:30.795002 qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-04-19 07:06:30.843001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-04-19 07:06:21.239064 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.843001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-04-19 07:06:30.839002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-04-19 07:06:21.099065 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-04-19 07:06:30.843001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-04-19 07:06:30.827002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-04-19 07:06:19.979072 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.827002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-04-19 07:06:30.823002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-04-19 07:06:19.831073 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.823002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-04-19 07:06:30.819002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-04-19 07:06:19.387076 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.819002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-04-19 07:06:30.823002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-04-19 07:06:19.691074 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-04-19 07:06:30.823002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-04-19 07:06:30.827002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-04-19 07:06:20.119071 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.827002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-04-19 07:06:30.831002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-04-19 07:06:20.259070 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-04-19 07:06:30.831002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24876 2023-04-19 07:06:30.819002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    36861 2023-04-19 07:06:19.543075 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.819002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-04-19 07:06:30.831002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-04-19 07:06:20.395069 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.831002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-04-19 07:06:30.843001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-04-19 07:06:30.363005 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.847001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-04-19 07:06:30.847001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-04-19 07:06:30.507004 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-04-19 07:06:30.847001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-04-19 07:06:30.847001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-04-19 07:06:21.663062 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.851001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-04-19 07:06:30.851001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-04-19 07:06:21.803061 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-04-19 07:06:30.851001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-04-19 07:06:30.851001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-04-19 07:06:21.943060 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.855001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-04-19 07:06:30.855001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-04-19 07:06:22.511056 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.855001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-04-19 07:06:30.855001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-04-19 07:06:22.367057 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-04-19 07:06:30.855001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-04-19 07:06:30.859001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-04-19 07:06:22.651055 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.859001 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    13329 2023-04-19 07:06:30.835002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23039 2023-04-19 07:06:20.535069 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.835002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-04-19 07:06:30.835002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-04-19 07:06:20.675068 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.835002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-04-19 07:06:30.835002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-04-19 07:06:20.819067 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-04-19 07:06:30.839002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-04-19 07:06:30.839002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-04-19 07:06:20.959066 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.839002 qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-04-19 07:06:30.931001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-04-19 07:06:27.767024 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.931001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-04-19 07:06:30.935001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-04-19 07:06:27.907023 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-19 07:06:30.935001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-04-19 07:06:30.935001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-04-19 07:06:28.047022 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.935001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-04-19 07:06:30.939001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-04-19 07:06:28.199021 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-19 07:06:30.939001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-04-19 07:06:30.939001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-04-19 07:06:28.347020 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-04-19 07:06:30.939001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-04-19 07:06:30.943001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-04-19 07:06:28.483019 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.943001 qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-04-19 07:06:30.903001 qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-04-19 07:06:25.679037 qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.903001 qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-04-19 07:06:30.903001 qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-19 07:06:25.819036 qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-19 07:06:30.907001 qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-04-19 07:06:30.803002 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-04-19 07:06:18.815079 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.807002 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-19 07:06:30.807002 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-04-19 07:06:18.955078 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.811002 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-04-19 07:06:30.811002 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-04-19 07:06:19.095077 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-04-19 07:06:30.815002 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-04-19 07:06:30.815002 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-04-19 07:06:19.239076 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.815002 qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-04-19 07:06:30.883001 qwak_core-0.0.24/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-04-19 07:06:24.091047 qwak_core-0.0.24/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-04-19 07:06:30.883001 qwak_core-0.0.24/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-04-19 07:06:30.943001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-04-19 07:06:28.623018 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.943001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-04-19 07:06:30.947001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-04-19 07:06:28.763017 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.947001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-04-19 07:06:30.947001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-04-19 07:06:28.907016 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.947001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-04-19 07:06:30.951001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-04-19 07:06:29.051015 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.951001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-19 07:06:30.951001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-04-19 07:06:29.203014 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.951001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-04-19 07:06:30.955001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-04-19 07:06:29.359012 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-04-19 07:06:30.955001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-04-19 07:06:30.955001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-04-19 07:06:29.495011 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.955001 qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-04-19 07:06:30.907001 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-04-19 07:06:26.095034 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.911001 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-04-19 07:06:30.915001 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-04-19 07:06:26.511032 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.915001 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-04-19 07:06:30.911001 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-04-19 07:06:26.231033 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-04-19 07:06:30.911001 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-04-19 07:06:30.911001 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-04-19 07:06:26.375033 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.915001 qwak_core-0.0.24/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-04-19 07:06:30.899001 qwak_core-0.0.24/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-04-19 07:06:25.267039 qwak_core-0.0.24/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-04-19 07:06:30.899001 qwak_core-0.0.24/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-04-19 07:06:30.787002 qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-04-19 07:06:18.531081 qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-04-19 07:06:30.787002 qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-04-19 07:06:30.783002 qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-04-19 07:06:18.391082 qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.787002 qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-04-19 07:06:30.787002 qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-04-19 07:06:18.675080 qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-04-19 07:06:30.791002 qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-04-19 07:06:30.895001 qwak_core-0.0.24/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-04-19 07:06:24.951041 qwak_core-0.0.24/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-04-19 07:06:30.895001 qwak_core-0.0.24/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-04-19 07:06:30.907001 qwak_core-0.0.24/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-04-19 07:06:25.955035 qwak_core-0.0.24/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-04-19 07:06:30.907001 qwak_core-0.0.24/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-04-19 07:06:30.783002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-04-19 07:06:16.847091 qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.783002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-04-19 07:06:30.779002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-04-19 07:06:16.707092 qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-04-19 07:06:30.783002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-04-19 07:06:30.775002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-04-19 07:06:16.287095 qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.775002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-04-19 07:06:30.775002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-04-19 07:06:16.427094 qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.779002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-04-19 07:06:30.779002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-04-19 07:06:16.567093 qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-04-19 07:06:30.779002 qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-04-19 07:06:30.959001 qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-04-19 07:06:29.783009 qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-04-19 07:06:30.959001 qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-04-19 07:06:30.959001 qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-04-19 07:06:29.639010 qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.959001 qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-04-19 07:06:30.795002 qwak_core-0.0.24/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-04-19 07:06:17.823085 qwak_core-0.0.24/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.795002 qwak_core-0.0.24/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3001 2023-04-19 07:06:30.799002 qwak_core-0.0.24/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2574 2023-04-19 07:06:17.959084 qwak_core-0.0.24/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-19 07:06:30.799002 qwak_core-0.0.24/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2107 2023-04-19 07:06:32.106992 qwak_core-0.0.24/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-04-19 07:06:32.106992 qwak_core-0.0.24/qwak/__init__.py
+-rw-r--r--   0        0        0     1168 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    31798 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5478 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0       77 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-19 07:05:48.995262 qwak_core-0.0.24/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/feedback/__init__.py
+-rw-r--r--   0        0        0     2710 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/feedback/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4255 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     2585 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0     1201 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     1927 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     2006 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2961 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1730 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    16848 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/const.py
+-rw-r--r--   0        0        0     1417 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     6729 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5760 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2109 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0     2272 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/schema.py
+-rw-r--r--   0        0        0     5609 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0       46 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-04-19 07:05:48.999261 qwak_core-0.0.24/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     1001 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4116 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13443 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-04-19 07:05:49.003261 qwak_core-0.0.24/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 qwak_core-0.0.24/setup.py
+-rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.24/PKG-INFO
```

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.24/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.24/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/pyproject.toml` & `qwak_core-0.0.24/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.23"
+version = "0.0.24"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak"},
     {include = "_qwak_proto"},
```

### Comparing `qwak_core-0.0.23/qwak/automations/__init__.py` & `qwak_core-0.0.24/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/automations/automation_executions.py` & `qwak_core-0.0.24/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/automations/automations.py` & `qwak_core-0.0.24/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.24/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.24/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.24/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.24/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.24/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/alert_management/client.py` & `qwak_core-0.0.24/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/analytics/client.py` & `qwak_core-0.0.24/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/audience/client.py` & `qwak_core-0.0.24/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/automation_management/client.py` & `qwak_core-0.0.24/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.24/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.24/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.24/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.24/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/build_management/client.py` & `qwak_core-0.0.24/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.24/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.24/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/deployment/client.py` & `qwak_core-0.0.24/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.24/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.24/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.24/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/feedback/client.py` & `qwak_core-0.0.24/qwak/clients/feedback/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.24/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.24/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/logging_client/client.py` & `qwak_core-0.0.24/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/model_management/client.py` & `qwak_core-0.0.24/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/project/client.py` & `qwak_core-0.0.24/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/secret_service/client.py` & `qwak_core-0.0.24/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.24/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.24/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.24/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.24/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.24/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.24/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.24/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.24/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.24/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.24/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.24/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/const.py` & `qwak_core-0.0.24/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.24/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.24/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.24/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.24/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/singleton_meta.py` & `qwak_core-0.0.24/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/tool/auth.py` & `qwak_core-0.0.24/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.24/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.24/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.24/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.24/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/adapters/__init__.py` & `qwak_core-0.0.24/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.24/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.24/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.24/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.24/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.24/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/base.py` & `qwak_core-0.0.24/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/decorators/api.py` & `qwak_core-0.0.24/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.24/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/experiment_tracking.py` & `qwak_core-0.0.24/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/schema.py` & `qwak_core-0.0.24/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model/schema_entities.py` & `qwak_core-0.0.24/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.24/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.24/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.24/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.24/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.24/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.24/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/qwak_client/client.py` & `qwak_core-0.0.24/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.24/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/qwak_client/models/model.py` & `qwak_core-0.0.24/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.24/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.24/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.24/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/qwak_services_mock/services_mock.py` & `qwak_core-0.0.24/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.23/setup.py` & `qwak_core-0.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
  'protobuf>=3.10,<4',
  'python-jose',
  'requests',
  'typeguard>=2,<3']
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.23',
+    'version': '0.0.24',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.23/PKG-INFO` & `qwak_core-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.23
+Version: 0.0.24
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

