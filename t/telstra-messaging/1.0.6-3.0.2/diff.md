# Comparing `tmp/Telstra_Messaging-1.0.6.1.tar.gz` & `tmp/telstra_messaging-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Telstra_Messaging-1.0.6.tar", last modified: Mon Mar 25 04:50:41 2019, max compression
+gzip compressed data, was "telstra_messaging-3.0.2.tar", max compression
```

## Comparing `Telstra_Messaging-1.0.6.1.tar` & `telstra_messaging-3.0.2.tar`

### file list

```diff
@@ -1,74 +1,24 @@
-drwxr-xr-x   0 developersteve   (501) staff       (20)        0 2019-03-25 04:50:41.000000 Telstra_Messaging-1.0.6/
--rw-r--r--   0 developersteve   (501) staff       (20)      334 2019-03-25 04:50:41.000000 Telstra_Messaging-1.0.6/PKG-INFO
-drwxr-xr-x   0 developersteve   (501) staff       (20)        0 2019-03-25 04:50:41.000000 Telstra_Messaging-1.0.6/Telstra_Messaging.egg-info/
--rw-r--r--   0 developersteve   (501) staff       (20)      334 2019-03-25 04:50:40.000000 Telstra_Messaging-1.0.6/Telstra_Messaging.egg-info/PKG-INFO
--rw-r--r--   0 developersteve   (501) staff       (20)     2473 2019-03-25 04:50:40.000000 Telstra_Messaging-1.0.6/Telstra_Messaging.egg-info/SOURCES.txt
--rw-r--r--   0 developersteve   (501) staff       (20)       48 2019-03-25 04:50:40.000000 Telstra_Messaging-1.0.6/Telstra_Messaging.egg-info/requires.txt
--rw-r--r--   0 developersteve   (501) staff       (20)       23 2019-03-25 04:50:40.000000 Telstra_Messaging-1.0.6/Telstra_Messaging.egg-info/top_level.txt
--rw-r--r--   0 developersteve   (501) staff       (20)        1 2019-03-25 04:50:40.000000 Telstra_Messaging-1.0.6/Telstra_Messaging.egg-info/dependency_links.txt
-drwxr-xr-x   0 developersteve   (501) staff       (20)        0 2019-03-25 04:50:41.000000 Telstra_Messaging-1.0.6/test/
--rw-r--r--   0 developersteve   (501) staff       (20)     1159 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_provision_number_request.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1119 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_error_error_error62.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1095 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_send_sms_request.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1095 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_send_mms_request.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1584 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_messaging_api.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1213 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_authgeneratetokenpost_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1143 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_outbound_poll_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1179 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_send_mms_request_mms_content.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1135 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_delete_number_request.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1035 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_message.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1103 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_error_error_error.py
--rw-r--r--   0 developersteve   (501) staff       (20)        0 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/__init__.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1027 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_status.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1079 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_o_auth_request.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1167 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_provision_number_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1021 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_auth_api.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1069 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_message_type.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1077 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_authentication_api.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1167 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_get_subscription_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1185 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_outbound_poll_response_inner.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1135 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_message_sent_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1372 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_provisioning_api.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1087 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_o_auth_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1061 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_error_error.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1061 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_mms_content.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1135 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_inbound_poll_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     1145 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/test/test_error_error_error_error.py
-drwxr-xr-x   0 developersteve   (501) staff       (20)        0 2019-03-25 04:50:41.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/
--rw-r--r--   0 developersteve   (501) staff       (20)    17642 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/configuration.py
--rw-r--r--   0 developersteve   (501) staff       (20)    23294 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/rest.py
--rw-r--r--   0 developersteve   (501) staff       (20)    11783 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/__init__.py
-drwxr-xr-x   0 developersteve   (501) staff       (20)        0 2019-03-25 04:50:41.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/
--rw-r--r--   0 developersteve   (501) staff       (20)    17816 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/inbound_poll_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)    15198 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/get_subscription_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     2555 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/message_type.py
--rw-r--r--   0 developersteve   (501) staff       (20)     4049 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/error_error_error62.py
--rw-r--r--   0 developersteve   (501) staff       (20)     6251 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/outbound_poll_response_inner.py
--rw-r--r--   0 developersteve   (501) staff       (20)    14825 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/o_auth_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)    11402 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/__init__.py
--rw-r--r--   0 developersteve   (501) staff       (20)    16836 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/message.py
--rw-r--r--   0 developersteve   (501) staff       (20)    16383 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/message_sent_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     5776 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/send_mms_request_mms_content.py
--rw-r--r--   0 developersteve   (501) staff       (20)    16055 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/outbound_poll_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     3972 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/error_error.py
--rw-r--r--   0 developersteve   (501) staff       (20)     3993 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/error_error_error_error.py
--rw-r--r--   0 developersteve   (501) staff       (20)    13225 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/delete_number_request.py
--rw-r--r--   0 developersteve   (501) staff       (20)    15496 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/mms_content.py
--rw-r--r--   0 developersteve   (501) staff       (20)     5853 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/o_auth_request.py
--rw-r--r--   0 developersteve   (501) staff       (20)     3938 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/error_error_error.py
--rw-r--r--   0 developersteve   (501) staff       (20)    24659 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/send_sms_request.py
--rw-r--r--   0 developersteve   (501) staff       (20)    15479 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/provision_number_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)     5864 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/authgeneratetokenpost_response.py
--rw-r--r--   0 developersteve   (501) staff       (20)    15001 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/provision_number_request.py
--rw-r--r--   0 developersteve   (501) staff       (20)    12636 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/status.py
--rw-r--r--   0 developersteve   (501) staff       (20)    18580 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/models/send_mms_request.py
-drwxr-xr-x   0 developersteve   (501) staff       (20)        0 2019-03-25 04:50:41.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/api/
--rw-r--r--   0 developersteve   (501) staff       (20)    41801 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/api/messaging_api.py
--rw-r--r--   0 developersteve   (501) staff       (20)    16535 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/api/authentication_api.py
--rw-r--r--   0 developersteve   (501) staff       (20)    23720 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/api/provisioning_api.py
--rw-r--r--   0 developersteve   (501) staff       (20)      286 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/api/__init__.py
--rw-r--r--   0 developersteve   (501) staff       (20)     5596 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/api/auth_api.py
--rw-r--r--   0 developersteve   (501) staff       (20)    34525 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/Telstra_Messaging/api_client.py
--rw-r--r--   0 developersteve   (501) staff       (20)     3755 2019-03-25 04:28:39.000000 Telstra_Messaging-1.0.6/README.md
--rw-r--r--   0 developersteve   (501) staff       (20)    11082 2019-03-25 04:50:23.000000 Telstra_Messaging-1.0.6/setup.py
--rw-r--r--   0 developersteve   (501) staff       (20)       38 2019-03-25 04:50:41.000000 Telstra_Messaging-1.0.6/setup.cfg
+-rw-r--r--   0        0        0    11378 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/LICENSE
+-rw-r--r--   0        0        0    25497 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/README.md
+-rw-r--r--   0        0        0      888 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/__init__.py
+-rw-r--r--   0        0        0      762 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/exceptions.py
+-rw-r--r--   0        0        0     4682 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/free_trial_numbers.py
+-rw-r--r--   0        0        0     1063 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/health_check.py
+-rw-r--r--   0        0        0    31574 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/message.py
+-rw-r--r--   0        0        0     2847 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/oauth.py
+-rw-r--r--   0        0        0     8901 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/reports.py
+-rw-r--r--   0        0        0      903 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/types.py
+-rw-r--r--   0        0        0       38 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/callback_url.py
+-rw-r--r--   0        0        0     6152 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/config.py
+-rw-r--r--   0        0        0     1315 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/error_response.py
+-rw-r--r--   0        0        0     2043 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/free_trial_number.py
+-rw-r--r--   0        0        0      933 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/message_id.py
+-rw-r--r--   0        0        0      409 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/querystring.py
+-rw-r--r--   0        0        0     2961 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/reports_dates.py
+-rw-r--r--   0        0        0      929 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/schedule_send.py
+-rw-r--r--   0        0        0     1662 2023-04-18 23:01:43.960254 telstra_messaging-3.0.2/telstra/messaging/utils/virtual_number.py
+-rw-r--r--   0        0        0    16507 2023-04-18 23:01:43.964254 telstra_messaging-3.0.2/telstra/messaging/virtual_number.py
+-rw-r--r--   0        0        0    25995 1970-01-01 00:00:00.000000 telstra_messaging-3.0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

