# Comparing `tmp/opentera-1.2.0.tar.gz` & `tmp/opentera-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentera-1.2.0.tar", last modified: Tue Mar  7 18:26:30 2023, max compression
+gzip compressed data, was "opentera-1.2.1.tar", last modified: Wed Apr 19 13:15:57 2023, max compression
```

## Comparing `opentera-1.2.0.tar` & `opentera-1.2.1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.807885 opentera-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-07 18:25:04.000000 opentera-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-07 18:25:04.000000 opentera-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-07 18:26:30.807885 opentera-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-07 18:25:04.000000 opentera-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.791884 opentera-1.2.0/opentera/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-07 18:25:35.000000 opentera-1.2.0/opentera/OpenTeraServerVersion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.795884 opentera-1.2.0/opentera/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/config/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.795884 opentera-1.2.0/opentera/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/crypto/crypto_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.795884 opentera-1.2.0/opentera/db/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12396 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/SoftDeleteMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/SoftDeleteQueryRewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/SoftInsertMixin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.799884 opentera-1.2.0/opentera/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraAsset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraDevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraDeviceParticipant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraDeviceProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraDeviceSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraDeviceSubType.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraDeviceType.py
--rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraParticipant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraParticipantGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraServerSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraService.py
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraServiceAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraServiceConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraServiceConfigSpecific.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraServiceProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraServiceRole.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraServiceSite.py
--rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraSession.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraSessionDevices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraSessionEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraSessionParticipants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraSessionType.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraSessionTypeProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraSessionTypeSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraSessionUsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraTestType.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraTestTypeProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraTestTypeSite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13864 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraUser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraUserGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraUserPreference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/TeraUserUserGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/db/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.799884 opentera-1.2.0/opentera/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.803884 opentera-1.2.0/opentera/forms/
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraDeviceForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraDeviceSubTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraDeviceTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraParticipantForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraParticipantGroupForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraProjectForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraServiceConfigForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraServiceForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraSessionForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraSessionTypeConfigForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraSessionTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraSiteForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraTestTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraUserForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraUserGroupForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/TeraVersionsForm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.803884 opentera-1.2.0/opentera/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/logging/LoggingClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.803884 opentera-1.2.0/opentera/messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:05.000000 opentera-1.2.0/opentera/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.803884 opentera-1.2.0/opentera/messages/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/CreateSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/DatabaseEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/DeviceEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/JoinSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/JoinSessionReplyEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/LeaveSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/LogEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/LoginEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/ParticipantEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/RPCMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/Result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/ServerCommand_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/StopSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/TeraEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-07 18:26:24.000000 opentera-1.2.0/opentera/messages/python/TeraMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-07 18:26:24.000000 opentera-1.2.0/opentera/messages/python/TeraModuleMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-07 18:26:24.000000 opentera-1.2.0/opentera/messages/python/UserEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-07 18:26:23.000000 opentera-1.2.0/opentera/messages/python/UserRegisterToEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-07 18:25:05.000000 opentera-1.2.0/opentera/messages/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.803884 opentera-1.2.0/opentera/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/modules/BaseModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.803884 opentera-1.2.0/opentera/redis/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5734 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/redis/RedisClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2896 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/redis/RedisProtocolFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/redis/RedisRPCClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/redis/RedisVars.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.807885 opentera-1.2.0/opentera/services/
--rw-r--r--   0 runner    (1001) docker     (123)    38390 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/BaseWebRTCService.py
--rw-r--r--   0 runner    (1001) docker     (123)    17543 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/ServiceAccessManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/ServiceConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/ServiceOpenTera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/ServiceOpenTeraWithAssets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/ServiceOpenTeraWithTests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/TeraDeviceClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/TeraParticipantClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/TeraServiceClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/TeraUserClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.807885 opentera-1.2.0/opentera/services/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/modules/WebRTCModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/services/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.807885 opentera-1.2.0/opentera/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/utils/Metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/utils/TeraVersions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/utils/UserAgentParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.807885 opentera-1.2.0/opentera/utils/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/utils/assets/AssetFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/utils/assets/AssetVideoFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/utils/assets/BaseAsset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:25:04.000000 opentera-1.2.0/opentera/utils/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.795884 opentera-1.2.0/opentera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-07 18:26:30.000000 opentera-1.2.0/opentera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-03-07 18:26:30.000000 opentera-1.2.0/opentera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 18:26:30.000000 opentera-1.2.0/opentera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-07 18:26:30.000000 opentera-1.2.0/opentera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-07 18:26:30.000000 opentera-1.2.0/opentera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 18:26:30.807885 opentera-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-07 18:25:04.000000 opentera-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.791884 opentera-1.2.0/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.791884 opentera-1.2.0/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.807885 opentera-1.2.0/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-07 18:26:26.000000 opentera-1.2.0/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    71383 2023-03-07 18:25:04.000000 opentera-1.2.0/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.791884 opentera-1.2.0/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:26:30.807885 opentera-1.2.0/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    37867 2023-03-07 18:26:26.000000 opentera-1.2.0/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    88110 2023-03-07 18:25:04.000000 opentera-1.2.0/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.833879 opentera-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-19 13:14:34.000000 opentera-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 13:14:34.000000 opentera-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-19 13:15:57.833879 opentera-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 13:14:34.000000 opentera-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 13:15:02.000000 opentera-1.2.1/opentera/OpenTeraServerVersion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/config/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/crypto/crypto_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera/db/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12396 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/SoftDeleteMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/SoftDeleteQueryRewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/SoftInsertMixin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.821878 opentera-1.2.1/opentera/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraAsset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceParticipant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceSubType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceType.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraParticipant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraParticipantGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServerSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceConfigSpecific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceRole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionDevices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionParticipants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionTypeProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionTypeSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionUsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraTestType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraTestTypeProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraTestTypeSite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13864 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraUserGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraUserPreference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraUserUserGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.821878 opentera-1.2.1/opentera/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.825878 opentera-1.2.1/opentera/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraDeviceForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraDeviceSubTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraDeviceTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraParticipantForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraParticipantGroupForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraProjectForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraServiceConfigForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraServiceForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraSessionForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraSessionTypeConfigForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraSessionTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraSiteForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraTestTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraUserForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraUserGroupForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraVersionsForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.825878 opentera-1.2.1/opentera/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/logging/LoggingClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.825878 opentera-1.2.1/opentera/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:35.000000 opentera-1.2.1/opentera/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/messages/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/CreateSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/DatabaseEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/DeviceEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/JoinSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/JoinSessionReplyEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/LeaveSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/LogEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/LoginEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/ParticipantEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/RPCMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/Result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/ServerCommand_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/StopSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/TeraEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/TeraMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-19 13:15:51.000000 opentera-1.2.1/opentera/messages/python/TeraModuleMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-19 13:15:51.000000 opentera-1.2.1/opentera/messages/python/UserEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/UserRegisterToEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-19 13:14:35.000000 opentera-1.2.1/opentera/messages/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/modules/BaseModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/redis/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5734 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/RedisClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2896 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/RedisProtocolFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/RedisRPCClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/RedisVars.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/services/
+-rw-r--r--   0 runner    (1001) docker     (123)    38393 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/BaseWebRTCService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17543 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceAccessManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceOpenTera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceOpenTeraWithAssets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceOpenTeraWithTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/TeraDeviceClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/TeraParticipantClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/TeraServiceClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/TeraUserClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/services/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/modules/WebRTCModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/TeraVersions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/UserAgentParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/utils/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/assets/AssetFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/assets/AssetVideoFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/assets/BaseAsset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:15:57.833879 opentera-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-19 13:14:34.000000 opentera-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.813878 opentera-1.2.1/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.813878 opentera-1.2.1/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.833879 opentera-1.2.1/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-19 13:15:53.000000 opentera-1.2.1/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    71383 2023-04-19 13:14:34.000000 opentera-1.2.1/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.813878 opentera-1.2.1/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.833879 opentera-1.2.1/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    37867 2023-04-19 13:15:53.000000 opentera-1.2.1/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    88110 2023-04-19 13:14:34.000000 opentera-1.2.1/translations/fr/LC_MESSAGES/messages.po
```

### Comparing `opentera-1.2.0/LICENSE` & `opentera-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/PKG-INFO` & `opentera-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: opentera
-Version: 1.2.0
+Version: 1.2.1
 Summary: OpenTera base package
 Home-page: https://github.com/introlab/opentera
 Author: Dominic Létourneau, Simon Brière
 Author-email: dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OpenTera
 
 Python package for OpenTera micro-service architecture. 
 External microservices can use this package as a base.
```

### Comparing `opentera-1.2.0/README.md` & `opentera-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/config/ConfigManager.py` & `opentera-1.2.1/opentera/config/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/crypto/crypto_utils.py` & `opentera-1.2.1/opentera/crypto/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/Base.py` & `opentera-1.2.1/opentera/db/Base.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/SoftDeleteMixin.py` & `opentera-1.2.1/opentera/db/SoftDeleteMixin.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/SoftDeleteQueryRewriter.py` & `opentera-1.2.1/opentera/db/SoftDeleteQueryRewriter.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/SoftInsertMixin.py` & `opentera-1.2.1/opentera/db/SoftInsertMixin.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraAsset.py` & `opentera-1.2.1/opentera/db/models/TeraAsset.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraDevice.py` & `opentera-1.2.1/opentera/db/models/TeraDevice.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraDeviceParticipant.py` & `opentera-1.2.1/opentera/db/models/TeraDeviceParticipant.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraDeviceProject.py` & `opentera-1.2.1/opentera/db/models/TeraDeviceProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraDeviceSite.py` & `opentera-1.2.1/opentera/db/models/TeraDeviceSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraDeviceSubType.py` & `opentera-1.2.1/opentera/db/models/TeraDeviceSubType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraDeviceType.py` & `opentera-1.2.1/opentera/db/models/TeraDeviceType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraParticipant.py` & `opentera-1.2.1/opentera/db/models/TeraParticipant.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraParticipantGroup.py` & `opentera-1.2.1/opentera/db/models/TeraParticipantGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraProject.py` & `opentera-1.2.1/opentera/db/models/TeraProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraServerSettings.py` & `opentera-1.2.1/opentera/db/models/TeraServerSettings.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraService.py` & `opentera-1.2.1/opentera/db/models/TeraService.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,14 +191,15 @@
         new_service.service_clientendpoint = '/rehab'
         new_service.service_endpoint_participant = '/participant'
         # Not yet implemented...
         # new_service.service_endpoint_user = '/user'
         # new_service.service_endpoint_device = '/device'
         new_service.service_enabled = True
         new_service.service_editable_config = True
+        new_service.service_system = True
         TeraService.db().session.add(new_service)
 
         new_service = TeraService()
         new_service.service_uuid = str(uuid.uuid4())
         new_service.service_key = 'RobotTeleOperationService'
         new_service.service_name = 'Robot Teleoperation Service'
         new_service.service_hostname = '127.0.0.1'
```

### Comparing `opentera-1.2.0/opentera/db/models/TeraServiceAccess.py` & `opentera-1.2.1/opentera/db/models/TeraServiceAccess.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraServiceConfig.py` & `opentera-1.2.1/opentera/db/models/TeraServiceConfig.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraServiceConfigSpecific.py` & `opentera-1.2.1/opentera/db/models/TeraServiceConfigSpecific.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraServiceProject.py` & `opentera-1.2.1/opentera/db/models/TeraServiceProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraServiceRole.py` & `opentera-1.2.1/opentera/db/models/TeraServiceRole.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraServiceSite.py` & `opentera-1.2.1/opentera/db/models/TeraServiceSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraSession.py` & `opentera-1.2.1/opentera/db/models/TeraSession.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraSessionDevices.py` & `opentera-1.2.1/opentera/db/models/TeraSessionDevices.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraSessionEvent.py` & `opentera-1.2.1/opentera/db/models/TeraSessionEvent.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraSessionParticipants.py` & `opentera-1.2.1/opentera/db/models/TeraSessionParticipants.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraSessionType.py` & `opentera-1.2.1/opentera/db/models/TeraSessionType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraSessionTypeProject.py` & `opentera-1.2.1/opentera/db/models/TeraSessionTypeProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraSessionTypeSite.py` & `opentera-1.2.1/opentera/db/models/TeraSessionTypeSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraSessionUsers.py` & `opentera-1.2.1/opentera/db/models/TeraSessionUsers.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraSite.py` & `opentera-1.2.1/opentera/db/models/TeraSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraTest.py` & `opentera-1.2.1/opentera/db/models/TeraTest.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraTestType.py` & `opentera-1.2.1/opentera/db/models/TeraTestType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraTestTypeProject.py` & `opentera-1.2.1/opentera/db/models/TeraTestTypeProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraTestTypeSite.py` & `opentera-1.2.1/opentera/db/models/TeraTestTypeSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraUser.py` & `opentera-1.2.1/opentera/db/models/TeraUser.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraUserGroup.py` & `opentera-1.2.1/opentera/db/models/TeraUserGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraUserPreference.py` & `opentera-1.2.1/opentera/db/models/TeraUserPreference.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/TeraUserUserGroup.py` & `opentera-1.2.1/opentera/db/models/TeraUserUserGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/db/models/__init__.py` & `opentera-1.2.1/opentera/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraDeviceForm.py` & `opentera-1.2.1/opentera/forms/TeraDeviceForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraDeviceSubTypeForm.py` & `opentera-1.2.1/opentera/forms/TeraDeviceSubTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraDeviceTypeForm.py` & `opentera-1.2.1/opentera/forms/TeraDeviceTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraForm.py` & `opentera-1.2.1/opentera/forms/TeraForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraParticipantForm.py` & `opentera-1.2.1/opentera/forms/TeraParticipantForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraParticipantGroupForm.py` & `opentera-1.2.1/opentera/forms/TeraParticipantGroupForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraProjectForm.py` & `opentera-1.2.1/opentera/forms/TeraProjectForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraServiceConfigForm.py` & `opentera-1.2.1/opentera/forms/TeraServiceConfigForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraServiceForm.py` & `opentera-1.2.1/opentera/forms/TeraServiceForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraSessionForm.py` & `opentera-1.2.1/opentera/forms/TeraSessionForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraSessionTypeForm.py` & `opentera-1.2.1/opentera/forms/TeraSessionTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraSiteForm.py` & `opentera-1.2.1/opentera/forms/TeraSiteForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraTestTypeForm.py` & `opentera-1.2.1/opentera/forms/TeraTestTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraUserForm.py` & `opentera-1.2.1/opentera/forms/TeraUserForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraUserGroupForm.py` & `opentera-1.2.1/opentera/forms/TeraUserGroupForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/forms/TeraVersionsForm.py` & `opentera-1.2.1/opentera/forms/TeraVersionsForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/logging/LoggingClient.py` & `opentera-1.2.1/opentera/logging/LoggingClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/CreateSession_pb2.py` & `opentera-1.2.1/opentera/messages/python/CreateSession_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/DatabaseEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/DatabaseEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/DeviceEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/DeviceEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/JoinSessionEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/JoinSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/JoinSessionReplyEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/JoinSessionReplyEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/LeaveSessionEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/LeaveSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/LogEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/LogEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/LoginEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/LoginEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/ParticipantEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/ParticipantEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/RPCMessage_pb2.py` & `opentera-1.2.1/opentera/messages/python/RPCMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/Result_pb2.py` & `opentera-1.2.1/opentera/messages/python/Result_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/ServerCommand_pb2.py` & `opentera-1.2.1/opentera/messages/python/ServerCommand_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/StopSessionEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/StopSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/TeraEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/TeraEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/TeraMessage_pb2.py` & `opentera-1.2.1/opentera/messages/python/TeraMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/TeraModuleMessage_pb2.py` & `opentera-1.2.1/opentera/messages/python/TeraModuleMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/UserEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/UserEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/UserRegisterToEvent_pb2.py` & `opentera-1.2.1/opentera/messages/python/UserRegisterToEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/messages/python/__init__.py` & `opentera-1.2.1/opentera/messages/python/__init__.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/modules/BaseModule.py` & `opentera-1.2.1/opentera/modules/BaseModule.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/redis/RedisClient.py` & `opentera-1.2.1/opentera/redis/RedisClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/redis/RedisProtocolFactory.py` & `opentera-1.2.1/opentera/redis/RedisProtocolFactory.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/redis/RedisRPCClient.py` & `opentera-1.2.1/opentera/redis/RedisRPCClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 rpc_args.append(val)
             else:
                 print('Invalid arg:', arg)
 
         # Set args
         message.args.extend(rpc_args)
 
-        # Will answer on the replay_to field
+        # Will answer on the reply_to field
         p.subscribe(message.reply_to)
         # First message is for subscribe result
         message1 = p.get_message(timeout=self.timeout)
 
         # Publish request
         self.client.publish(topic, message.SerializeToString())
```

### Comparing `opentera-1.2.0/opentera/redis/RedisVars.py` & `opentera-1.2.1/opentera/redis/RedisVars.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/services/BaseWebRTCService.py` & `opentera-1.2.1/opentera/services/BaseWebRTCService.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,16 @@
         # Should send invitations
         session_info = self.get_session_info_from_key(session_key)
 
         if session_info:
             self.send_join_message(session_info=session_info)
 
     def setup_rpc_interface(self):
-        # TODO Update rpc interface
+        super().setup_rpc_interface()
+
         self.rpc_api['session_manage'] = {'args': ['str:json_info'],
                                           'returns': 'dict',
                                           'callback': self.session_manage}
 
         self.rpc_api['participant_info'] = {'args': ['str:participant_uuid'],
                                             'returns': 'dict',
                                             'callback': self.participant_info}
```

### Comparing `opentera-1.2.0/opentera/services/ServiceAccessManager.py` & `opentera-1.2.1/opentera/services/ServiceAccessManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/services/ServiceConfigManager.py` & `opentera-1.2.1/opentera/services/ServiceConfigManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/services/ServiceOpenTera.py` & `opentera-1.2.1/opentera/services/ServiceOpenTera.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,16 +64,17 @@
         # Build standard interface
         self.build_interface()
 
         # Register to system events
         self.register_to_events()
 
     def setup_rpc_interface(self):
-        # Should be implemented in derived classes
-        pass
+        self.rpc_api['session_type_config'] = {'args': ['int:id_session_type'],
+                                               'returns': 'dict',
+                                               'callback': self.get_session_type_config_form}
 
     def register_to_events(self):
         # Should be implemented in derived classes
         yield None
 
     def notify_service_messages(self, pattern, channel, message):
         pass
@@ -201,7 +202,11 @@
         tera_message = messages.TeraModuleMessage()
         tera_message.head.version = 1
         tera_message.head.time = datetime.datetime.now().timestamp()
         tera_message.head.seq = seq
         tera_message.head.source = src
         tera_message.head.dest = dest
         return tera_message
+
+    def get_session_type_config_form(self, id_session_type: int) -> dict:
+        # Default session type config form for services
+        return {}
```

### Comparing `opentera-1.2.0/opentera/services/ServiceOpenTeraWithAssets.py` & `opentera-1.2.1/opentera/services/ServiceOpenTeraWithAssets.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/services/ServiceOpenTeraWithTests.py` & `opentera-1.2.1/opentera/services/ServiceOpenTeraWithTests.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/services/TeraDeviceClient.py` & `opentera-1.2.1/opentera/services/TeraDeviceClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,19 @@
         self.__id_device = token_dict['id_device']
         self.__device_token = token
 
         # A little trick here to get the right URL for the server if we are using a proxy
         backend_hostname = config_man.backend_config["hostname"]
         backend_port = str(config_man.backend_config["port"])
 
-        if 'X-Externalhost' in request.headers:
-            backend_hostname = request.headers['X-Externalhost']
+        # if 'X-Externalhost' in request.headers:
+        #    backend_hostname = request.headers['X-Externalhost']
 
-        if 'X-Externalport' in request.headers:
-            backend_port = request.headers['X-Externalport']
+        #if 'X-Externalport' in request.headers:
+        #    backend_port = request.headers['X-Externalport']
 
         self.__backend_url = 'https://' + backend_hostname + ':' + backend_port
 
 
     @property
     def device_uuid(self):
         return self.__device_uuid
```

### Comparing `opentera-1.2.0/opentera/services/TeraParticipantClient.py` & `opentera-1.2.1/opentera/services/TeraParticipantClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         self.__id_participant = token_dict['id_participant']
         self.__participant_token = token
 
         # A little trick here to get the right URL for the server if we are using a proxy
         backend_hostname = config_man.backend_config["hostname"]
         backend_port = str(config_man.backend_config["port"])
 
-        if 'X-Externalhost' in request.headers:
-            backend_hostname = request.headers['X-Externalhost']
+        #if 'X-Externalhost' in request.headers:
+        #    backend_hostname = request.headers['X-Externalhost']
 
-        if 'X-Externalport' in request.headers:
-            backend_port = request.headers['X-Externalport']
+        #if 'X-Externalport' in request.headers:
+        #    backend_port = request.headers['X-Externalport']
 
         self.__backend_url = 'https://' + backend_hostname + ':' + backend_port
         self.__config_man = config_man
         self.__rpc_client = RedisRPCClient(config_man.redis_config)
 
     @property
     def participant_uuid(self):
```

### Comparing `opentera-1.2.0/opentera/services/TeraServiceClient.py` & `opentera-1.2.1/opentera/services/TeraServiceClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,19 @@
         self.__service_uuid = token_dict['service_uuid']
         self.__service_token = token
 
         # A little trick here to get the right URL for the server if we are using a proxy
         backend_hostname = config_man.backend_config["hostname"]
         backend_port = str(config_man.backend_config["port"])
 
-        if 'X-Externalhost' in request.headers:
-            backend_hostname = request.headers['X-Externalhost']
+        #if 'X-Externalhost' in request.headers:
+        #    backend_hostname = request.headers['X-Externalhost']
 
-        if 'X-Externalport' in request.headers:
-            backend_port = request.headers['X-Externalport']
+        #if 'X-Externalport' in request.headers:
+        #    backend_port = request.headers['X-Externalport']
 
         self.__backend_url = 'https://' + backend_hostname + ':' + backend_port
 
     @property
     def service_uuid(self):
         return self.__service_uuid
```

### Comparing `opentera-1.2.0/opentera/services/TeraUserClient.py` & `opentera-1.2.1/opentera/services/TeraUserClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         self.__user_token = token
         self.__user_superadmin = token_dict['user_superadmin']
 
         # A little trick here to get the right URL for the server if we are using a proxy
         backend_hostname = config_man.backend_config["hostname"]
         backend_port = str(config_man.backend_config["port"])
 
-        if 'X-Externalhost' in request.headers:
-            backend_hostname = request.headers['X-Externalhost']
+        # if 'X-Externalhost' in request.headers:
+        #   backend_hostname = request.headers['X-Externalhost']
 
-        if 'X-Externalport' in request.headers:
-            backend_port = request.headers['X-Externalport']
+        #if 'X-Externalport' in request.headers:
+        #    backend_port = request.headers['X-Externalport']
 
         self.__backend_url = 'https://' + backend_hostname + ':' + backend_port
 
     @property
     def user_uuid(self):
         return self.__user_uuid
```

### Comparing `opentera-1.2.0/opentera/services/modules/WebRTCModule.py` & `opentera-1.2.1/opentera/services/modules/WebRTCModule.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,15 +146,20 @@
         return port
 
     def launch_node(self, port, key, owner, session_info):
         executable_args = [self.config.webrtc_config['executable'],
                            self.config.webrtc_config['script'],
                            '--port=' + str(port),
                            '--key=' + str(key),
-                           '--debug=' + str(1)]
+                           '--debug=' + str(1), 
+                           '--redis_hostname=' + str(self.config.redis_config['hostname']), 
+                           '--redis_port=' + str(self.config.redis_config['port']),
+                           '--redis_db=' + str(self.config.redis_config['db']),
+                           '--redis_username=' + str(self.config.redis_config['username']),
+                           '--redis_password=' + str(self.config.redis_config['password'])]
 
         # stdout=os.subprocess.PIPE, stderr=os.subprocess.PIPE)
         try:
             process = subprocess.Popen(executable_args,
                                        cwd=os.path.realpath(self.config.webrtc_config['working_directory']))
 
             # One more process
```

### Comparing `opentera-1.2.0/opentera/utils/Metrics.py` & `opentera-1.2.1/opentera/utils/Metrics.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/utils/TeraVersions.py` & `opentera-1.2.1/opentera/utils/TeraVersions.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/utils/UserAgentParser.py` & `opentera-1.2.1/opentera/utils/UserAgentParser.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera/utils/assets/BaseAsset.py` & `opentera-1.2.1/opentera/utils/assets/BaseAsset.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera.egg-info/PKG-INFO` & `opentera-1.2.1/opentera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: opentera
-Version: 1.2.0
+Version: 1.2.1
 Summary: OpenTera base package
 Home-page: https://github.com/introlab/opentera
 Author: Dominic Létourneau, Simon Brière
 Author-email: dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OpenTera
 
 Python package for OpenTera micro-service architecture. 
 External microservices can use this package as a base.
```

### Comparing `opentera-1.2.0/opentera.egg-info/SOURCES.txt` & `opentera-1.2.1/opentera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/opentera.egg-info/requires.txt` & `opentera-1.2.1/opentera.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `opentera-1.2.0/setup.py` & `opentera-1.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 with open("env/requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.readlines()
     requirements.append('protobuf==3.20.3')
 
 setuptools.setup(
     name="opentera",
-    version="1.2.0",
+    version="1.2.1",
     author="Dominic Létourneau, Simon Brière",
     author_email="dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca",
     description="OpenTera base package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/introlab/opentera",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.10',
 )
```

### Comparing `opentera-1.2.0/translations/en/LC_MESSAGES/messages.po` & `opentera-1.2.1/translations/en/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2019.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-07 08:35-0500\n"
+"POT-Creation-Date: 2023-03-21 09:06-0400\n"
 "PO-Revision-Date: 2021-01-25 13:01-0500\n"
 "Last-Translator: \n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 #: modules/FlaskModule/API/device/DeviceLogin.py:82
 msgid "Unable to get online devices."
 msgstr ""
 
 #: modules/FlaskModule/API/device/DeviceLogin.py:98
 msgid "Device already logged in."
@@ -76,17 +76,17 @@
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:84
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:107
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:159
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:350
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:353
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:198
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:269
-#: modules/FlaskModule/API/user/UserQueryProjects.py:144
-#: modules/FlaskModule/API/user/UserQueryProjects.py:149
-#: modules/FlaskModule/API/user/UserQueryProjects.py:251
+#: modules/FlaskModule/API/user/UserQueryProjects.py:145
+#: modules/FlaskModule/API/user/UserQueryProjects.py:150
+#: modules/FlaskModule/API/user/UserQueryProjects.py:258
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:112
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:117
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:121
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:129
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:208
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:212
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:216
@@ -171,17 +171,17 @@
 #: modules/FlaskModule/API/user/UserQueryDevices.py:343
 #: modules/FlaskModule/API/user/UserQueryDevices.py:460
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:120
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:135
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:178
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:239
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:280
-#: modules/FlaskModule/API/user/UserQueryProjects.py:189
-#: modules/FlaskModule/API/user/UserQueryProjects.py:204
-#: modules/FlaskModule/API/user/UserQueryProjects.py:269
+#: modules/FlaskModule/API/user/UserQueryProjects.py:190
+#: modules/FlaskModule/API/user/UserQueryProjects.py:205
+#: modules/FlaskModule/API/user/UserQueryProjects.py:276
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:151
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:163
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:185
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:231
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:208
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:264
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:287
@@ -235,15 +235,15 @@
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:82
 #: modules/FlaskModule/API/service/ServiceQueryProjects.py:56
 #: modules/FlaskModule/API/service/ServiceQueryServices.py:76
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:62
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:122
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:109
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:86
-#: modules/FlaskModule/API/user/UserQueryProjects.py:109
+#: modules/FlaskModule/API/user/UserQueryProjects.py:110
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:80
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:123
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:112
 #: modules/FlaskModule/API/user/UserQueryServices.py:104
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:62
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:101
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:79
@@ -720,15 +720,15 @@
 "Can't delete device from project. Please remove all participants "
 "associated with the device or all sessions in the project referring to "
 "the device before deleting."
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:180
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:192
-#: modules/FlaskModule/API/user/UserQueryProjects.py:131
+#: modules/FlaskModule/API/user/UserQueryProjects.py:132
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:179
 msgid "Missing id_project"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:182
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:157
 msgid "Missing devices"
@@ -1041,31 +1041,31 @@
 msgid "Invalid role name or id for that project"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:265
 msgid "No project access to delete."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:125
+#: modules/FlaskModule/API/user/UserQueryProjects.py:126
 msgid "Missing project"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:133
+#: modules/FlaskModule/API/user/UserQueryProjects.py:134
 msgid "Missing id_site arguments"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:162
+#: modules/FlaskModule/API/user/UserQueryProjects.py:163
 msgid "No access to a session type for at least one of it"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:174
+#: modules/FlaskModule/API/user/UserQueryProjects.py:175
 msgid "At least one session type is not associated to the project site"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:262
+#: modules/FlaskModule/API/user/UserQueryProjects.py:269
 msgid ""
 "Can't delete project: please delete all participants with sessions before"
 " deleting."
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:99
 msgid "Missing service_access"
```

### Comparing `opentera-1.2.0/translations/fr/LC_MESSAGES/messages.mo` & `opentera-1.2.1/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-07 08:35-0500\n"
+"POT-Creation-Date: 2023-03-21 09:06-0400\n"
 "PO-Revision-Date: 2023-03-07 08:35-0500\n"
 "Last-Translator: \n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `opentera-1.2.0/translations/fr/LC_MESSAGES/messages.po` & `opentera-1.2.1/translations/fr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-07 08:35-0500\n"
+"POT-Creation-Date: 2023-03-21 09:06-0400\n"
 "PO-Revision-Date: 2023-03-07 08:35-0500\n"
 "Last-Translator: \n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 #: modules/FlaskModule/API/device/DeviceLogin.py:82
 msgid "Unable to get online devices."
 msgstr "Impossible d'obtenir les appareils connectés."
 
 #: modules/FlaskModule/API/device/DeviceLogin.py:98
 msgid "Device already logged in."
@@ -76,17 +76,17 @@
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:84
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:107
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:159
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:350
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:353
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:198
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:269
-#: modules/FlaskModule/API/user/UserQueryProjects.py:144
-#: modules/FlaskModule/API/user/UserQueryProjects.py:149
-#: modules/FlaskModule/API/user/UserQueryProjects.py:251
+#: modules/FlaskModule/API/user/UserQueryProjects.py:145
+#: modules/FlaskModule/API/user/UserQueryProjects.py:150
+#: modules/FlaskModule/API/user/UserQueryProjects.py:258
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:112
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:117
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:121
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:129
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:208
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:212
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:216
@@ -171,17 +171,17 @@
 #: modules/FlaskModule/API/user/UserQueryDevices.py:343
 #: modules/FlaskModule/API/user/UserQueryDevices.py:460
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:120
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:135
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:178
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:239
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:280
-#: modules/FlaskModule/API/user/UserQueryProjects.py:189
-#: modules/FlaskModule/API/user/UserQueryProjects.py:204
-#: modules/FlaskModule/API/user/UserQueryProjects.py:269
+#: modules/FlaskModule/API/user/UserQueryProjects.py:190
+#: modules/FlaskModule/API/user/UserQueryProjects.py:205
+#: modules/FlaskModule/API/user/UserQueryProjects.py:276
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:151
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:163
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:185
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:231
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:208
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:264
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:287
@@ -235,15 +235,15 @@
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:82
 #: modules/FlaskModule/API/service/ServiceQueryProjects.py:56
 #: modules/FlaskModule/API/service/ServiceQueryServices.py:76
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:62
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:122
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:109
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:86
-#: modules/FlaskModule/API/user/UserQueryProjects.py:109
+#: modules/FlaskModule/API/user/UserQueryProjects.py:110
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:80
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:123
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:112
 #: modules/FlaskModule/API/user/UserQueryServices.py:104
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:62
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:101
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:79
@@ -729,15 +729,15 @@
 msgstr ""
 "Impossible de retirer l'appareil du projet: veuillez retirer tous les "
 "participants associés à cet appareil et/ou toutes les séances de ce "
 "projet impliquant cet appareil."
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:180
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:192
-#: modules/FlaskModule/API/user/UserQueryProjects.py:131
+#: modules/FlaskModule/API/user/UserQueryProjects.py:132
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:179
 msgid "Missing id_project"
 msgstr "Champ manquant : id_project"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:182
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:157
 msgid "Missing devices"
@@ -1085,31 +1085,31 @@
 msgid "Invalid role name or id for that project"
 msgstr "Nom du rôle ou ID invalide pour ce projet"
 
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:265
 msgid "No project access to delete."
 msgstr "Aucun accès au projet pour supprimer."
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:125
+#: modules/FlaskModule/API/user/UserQueryProjects.py:126
 msgid "Missing project"
 msgstr "Projet manquant"
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:133
+#: modules/FlaskModule/API/user/UserQueryProjects.py:134
 msgid "Missing id_site arguments"
 msgstr "Champ id_site manquant"
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:162
+#: modules/FlaskModule/API/user/UserQueryProjects.py:163
 msgid "No access to a session type for at least one of it"
 msgstr "Pas d'accès à ce type de session pour au moins un projet"
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:174
+#: modules/FlaskModule/API/user/UserQueryProjects.py:175
 msgid "At least one session type is not associated to the project site"
 msgstr "Au moins un type de séance n’est pas associé au site du projet"
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:262
+#: modules/FlaskModule/API/user/UserQueryProjects.py:269
 msgid ""
 "Can't delete project: please delete all participants with sessions before"
 " deleting."
 msgstr ""
 "Impossible de supprimer le projet: veuillez supprimer tous les "
 "participants ayant des séances au préalable."
```

