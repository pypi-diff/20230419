# Comparing `tmp/splight-lib-2.2.9.tar.gz` & `tmp/splight-lib-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-2.2.9.tar", last modified: Fri Apr 14 20:53:08 2023, max compression
+gzip compressed data, was "splight-lib-2.3.0.tar", last modified: Wed Apr 19 19:04:25 2023, max compression
```

## Comparing `splight-lib-2.2.9.tar` & `splight-lib-2.3.0.tar`

### file list

```diff
@@ -1,140 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.958515 splight-lib-2.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.000000 splight-lib-2.2.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 20:53:08.958515 splight-lib-2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 20:53:08.000000 splight-lib-2.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.934514 splight-lib-2.2.9/remote_splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.934514 splight-lib-2.2.9/remote_splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.934514 splight-lib-2.2.9/remote_splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/communication/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.934514 splight-lib-2.2.9/remote_splight_lib/database/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/database/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.934514 splight-lib-2.2.9/remote_splight_lib/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/datalake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.934514 splight-lib-2.2.9/remote_splight_lib/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-14 20:53:08.000000 splight-lib-2.2.9/remote_splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:53:08.958515 splight-lib-2.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 20:53:08.000000 splight-lib-2.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.934514 splight-lib-2.2.9/splight_abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.938515 splight-lib-2.2.9/splight_abstract/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/auth/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.938515 splight-lib-2.2.9/splight_abstract/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/cache/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.938515 splight-lib-2.2.9/splight_abstract/client/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/client/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.938515 splight-lib-2.2.9/splight_abstract/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/communication/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.938515 splight-lib-2.2.9/splight_abstract/database/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/database/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.938515 splight-lib-2.2.9/splight_abstract/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/datalake/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.942515 splight-lib-2.2.9/splight_abstract/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/deployment/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.942515 splight-lib-2.2.9/splight_abstract/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.942515 splight-lib-2.2.9/splight_abstract/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/hub/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.942515 splight-lib-2.2.9/splight_abstract/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/notification/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.942515 splight-lib-2.2.9/splight_abstract/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/remote/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.942515 splight-lib-2.2.9/splight_abstract/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_abstract/storage/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.942515 splight-lib-2.2.9/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.946514 splight-lib-2.2.9/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.946514 splight-lib-2.2.9/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.950514 splight-lib-2.2.9/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.950514 splight-lib-2.2.9/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.950514 splight-lib-2.2.9/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.950514 splight-lib-2.2.9/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/restclient/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.946514 splight-lib-2.2.9/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.958515 splight-lib-2.2.9/splight_models/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:53:08.958515 splight-lib-2.2.9/splight_models/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/communication/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/communication/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/datalake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/setpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-14 20:53:08.000000 splight-lib-2.2.9/splight_models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.831708 splight-lib-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.000000 splight-lib-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-19 19:04:25.831708 splight-lib-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 19:04:25.000000 splight-lib-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.811708 splight-lib-2.3.0/remote_splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.811708 splight-lib-2.3.0/remote_splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.811708 splight-lib-2.3.0/remote_splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/communication/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/remote_splight_lib/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/database/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/remote_splight_lib/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/datalake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/remote_splight_lib/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:04:25.831708 splight-lib-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-19 19:04:25.000000 splight-lib-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/splight_abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/splight_abstract/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/auth/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/splight_abstract/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/cache/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/client/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/communication/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/database/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/datalake/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/deployment/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/hub/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/notification/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/remote/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/storage/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23606 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.827708 splight-lib-2.3.0/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.831708 splight-lib-2.3.0/splight_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.831708 splight-lib-2.3.0/splight_models/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/communication/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/communication/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/datalake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/setpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/webhook.py
```

### Comparing `splight-lib-2.2.9/PKG-INFO` & `splight-lib-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.2.9
+Version: 2.3.0
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE.txt
 
 [![Lib upload](https://github.com/splightplatform/splight-lib/actions/workflows/libupload.yml/badge.svg)](https://github.com/splightplatform/splight-lib/actions/workflows/libupload.yml)
 
 ## How to install
 
 For development
 
-- `python setup.py develop`
+- `make install`
 
 For productive envs.
 
 - `python setup.py install`
 
 ## Tests
 
 ```
-pytest splight_lib/tests
+make test
 ```
```

### Comparing `splight-lib-2.2.9/remote_splight_lib/communication/client.py` & `splight-lib-2.3.0/remote_splight_lib/communication/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pysher
 import requests
 from furl import furl
 from retry import retry
 from typing import Callable, Dict
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 from splight_abstract.communication import (
     AbstractCommunicationClient,
     ClientNotReady,
 )
 import logging
 from splight_models.communication import CommunicationClientStatus, CommunicationContext, CommunicationEvent
 
 from remote_splight_lib.auth.auth import SplightAuthToken
 from remote_splight_lib.settings import settings
 from remote_splight_lib.communication.classmap import CLASSMAP
 
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 
 class CommunicationFactory:
 
     def __init__(self, model):
         self._model = model
```

### Comparing `splight-lib-2.2.9/remote_splight_lib/database/classmap.py` & `splight-lib-2.3.0/remote_splight_lib/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/remote_splight_lib/database/client.py` & `splight-lib-2.3.0/remote_splight_lib/database/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 from retry import retry
 from splight_abstract.remote import AbstractRemoteClient
 from splight_abstract.database import AbstractDatabaseClient
 from splight_models import File
 from remote_splight_lib.settings import settings
 from remote_splight_lib.exceptions import InvalidModel
 from remote_splight_lib.auth import SplightAuthToken
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 from splight_lib.encryption import EncryptionClient
 from typing import Dict, List, Type
 
 from furl import furl
 from pydantic import BaseModel
 from requests import Session
 from requests.exceptions import (
     ConnectionError,
     Timeout
 )
 from tempfile import NamedTemporaryFile
 
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 REQUEST_EXCEPTIONS = (ConnectionError, Timeout)
 
 
 class DatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
     """Splight API Database Client.
     Responsible for interacting with database resources using HTTP requests
     to the Splight API.
     """
 
-    def __init__(self, namespace: str = "default", **kwargs):
+    def __init__(self, namespace: str = "default"):
         super(DatabaseClient, self).__init__(namespace=namespace)
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         self._session = Session()
```

### Comparing `splight-lib-2.2.9/remote_splight_lib/datalake/client.py` & `splight-lib-2.3.0/remote_splight_lib/datalake/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 
 import pandas as pd
 import json
 from furl import furl
 from pydantic import BaseModel
 
 from remote_splight_lib.auth import SplightAuthToken
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 from remote_splight_lib.settings import settings
 from splight_abstract import AbstractRemoteClient, QuerySet
 from splight_abstract.datalake import AbstractDatalakeClient, validate_resource_type, validate_instance_type
 from splight_models import Query, DatalakeModel
 from retry import retry
 
 from splight_lib.restclient import (
     SplightRestClient,
     HTTPError,
     Timeout,
     ConnectError
 )
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 REQUEST_EXCEPTIONS = (HTTPError, Timeout, ConnectError)
 
 
 class DatalakeClient(AbstractDatalakeClient, AbstractRemoteClient):
 
     _PREFIX = "v2/engine/datalake"
 
-    def __init__(self, namespace: str = "default", **kwargs):
+    def __init__(self, namespace: str = "default"):
         super(DatalakeClient, self).__init__(namespace=namespace)
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         self._restclient = SplightRestClient()
```

### Comparing `splight-lib-2.2.9/remote_splight_lib/hub/client.py` & `splight-lib-2.3.0/remote_splight_lib/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/remote_splight_lib/settings.py` & `splight-lib-2.3.0/remote_splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/setup.py` & `splight-lib-2.3.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,43 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-
-with open('requirements.txt') as fp:
+with open("requirements.txt") as fp:
     install_requires = fp.readlines()
 
 dependency_links = [
     # External repoitories different from pypi
 ]
 
+test_requires = [
+    "pytest==7.1.2",
+    "mock==4.0.3",
+]
+
 setup(
-    name='splight-lib',
-    version='2.2.9',
-    author='Splight',
-    author_email='factory@splight-ae.com',
+    name="splight-lib",
+    version="2.3.0",
+    author="Splight",
+    author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
     zip_safe=False,
-    license='LICENSE.txt',
-    description='Library for public use. Splight',
-    long_description=open('README.md').read(),
+    license="LICENSE.txt",
+    description="Library for public use. Splight",
+    long_description=open("README.md").read(),
     install_requires=install_requires,
-    dependency_links=dependency_links
+    dependency_links=dependency_links,
+    extras_require={
+        "test": test_requires,
+        "dev": test_requires
+        + [
+            "flake8==6.0.0",
+            "ipython==8.12.0",
+            "ipdb==0.13.13",
+            "pre-commit==3.2.2",
+            "black==23.3.0",
+            "isort==5.12.0",
+        ],
+    },
 )
```

### Comparing `splight-lib-2.2.9/splight_abstract/auth/abstract.py` & `splight-lib-2.3.0/splight_abstract/auth/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/auth/exceptions.py` & `splight-lib-2.3.0/splight_abstract/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/cache/abstract.py` & `splight-lib-2.3.0/splight_abstract/cache/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from functools import wraps
 from typing import Callable, List
 from abc import abstractmethod
 from splight_abstract.client import AbstractClient
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 class AbstractCacheClient(AbstractClient):
 
     @abstractmethod
     def get(self, key):
         pass
```

### Comparing `splight-lib-2.2.9/splight_abstract/client/abstract.py` & `splight-lib-2.3.0/splight_abstract/client/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/client/filter.py` & `splight-lib-2.3.0/splight_abstract/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/client/hooks.py` & `splight-lib-2.3.0/splight_abstract/client/hooks.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/communication/abstract.py` & `splight-lib-2.3.0/splight_abstract/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/database/abstract.py` & `splight-lib-2.3.0/splight_abstract/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/datalake/abstract.py` & `splight-lib-2.3.0/splight_abstract/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/deployment/abstract.py` & `splight-lib-2.3.0/splight_abstract/deployment/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/endpoints/__init__.py` & `splight-lib-2.3.0/splight_abstract/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/hub/abstract.py` & `splight-lib-2.3.0/splight_abstract/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_abstract/storage/abstract.py` & `splight-lib-2.3.0/splight_abstract/storage/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/auth/mac_auth.py` & `splight-lib-2.3.0/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/client/database/classmap.py` & `splight-lib-2.3.0/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/client/database/local_client.py` & `splight-lib-2.3.0/splight_lib/client/database/local_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from typing import Dict, List, Type, Union
 from uuid import uuid4
 
 from splight_abstract.database import AbstractDatabaseClient
 from splight_lib.client.exceptions import InstanceNotFound
 from splight_lib.client.filter import value_filter_on_tuple
 from splight_models import SplightBaseModel
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 
 ResourceType = Type[SplightBaseModel]
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 
 class LocalDatabaseClient(AbstractDatabaseClient):
     """Database Client implementation for a local database that uses a
     JSON file.
     """
```

### Comparing `splight-lib-2.2.9/splight_lib/client/database/remote_client.py` & `splight-lib-2.3.0/splight_lib/client/database/remote_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 from tempfile import NamedTemporaryFile
 from typing import Dict, List, Type
 
 from furl import furl
 from pydantic import BaseModel
-from requests import Session
 
 from retry import retry
 
 from splight_abstract.database import AbstractDatabaseClient
 from splight_abstract.remote import AbstractRemoteClient
 from splight_lib.auth import SplightAuthToken
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 from splight_lib.client.database.classmap import CLASSMAP
 from splight_lib.client.exceptions import REQUEST_EXCEPTIONS, InvalidModel
 from splight_lib.client.settings import settings_remote as settings
+from splight_lib.restclient import SplightRestClient
 from splight_lib.encryption import EncryptionClient
 from splight_models import File
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 
 class RemoteDatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
     """Splight API Database Client.
     Responsible for interacting with database resources using HTTP requests
     to the Splight API.
     """
@@ -30,16 +30,16 @@
     def __init__(self, namespace: str = "default", *args, **kwargs):
         super().__init__(namespace=namespace)
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
-        self._session = Session()
-        self._session.headers.update(token.header)
+        self._restclient = SplightRestClient()
+        self._restclient.update_headers(token.header)
         logger.info("Remote database client initialized.", tags=LogTags.DATABASE)
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
     def save(self, instance: BaseModel) -> BaseModel:
         """Creates or updates a new resource depending on the model if
         it contains the id or not.
 
@@ -84,15 +84,15 @@
         ------
         InvalidModel thrown when the model name is not correct.
         """
         logger.debug("Deleting instance %s.", id, tags=LogTags.DATABASE)
         model_data = self._get_model_data(resource_type)
         path = model_data["path"]
         url = self._base_url / f"{path}/{id}/"
-        response = self._session.delete(url)
+        response = self._restclient.delete(url)
         response.raise_for_status()
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
     def _get(
         self,
         resource_type: Type,
         first: bool = False,
@@ -156,15 +156,15 @@
         ------
         InvalidModel thrown when the model name is not correct.
         """
         constructor = type(instance)
         model_data = self._get_model_data(constructor)
         path = model_data["path"]
         url = self._base_url / f"{path}/{instance.id}/download"
-        response = self._session.get(url)
+        response = self._restclient.get(url)
         response.raise_for_status()
         f = NamedTemporaryFile("wb+")
         f.write(response.content)
         f.seek(0)
         if decrypt and instance.encrypted:
             encryption_manager = EncryptionClient()
             encryption_manager.decrypt_file(path=f.name)
@@ -182,15 +182,15 @@
                 else None
             )
             kwargs["page"] = next_page
 
     def _list(self, path: str, **kwargs):
         url = self._base_url / f"{path}/"
         params = self._parse_params(**kwargs)
-        response = self._session.get(url, params=params)
+        response = self._restclient.get(url, params=params)
         response.raise_for_status()
         return response.json()
 
     @staticmethod
     def _get_model_data(constructor: Type):
         model_data = CLASSMAP.get(constructor)
         if not model_data:
@@ -199,21 +199,21 @@
 
     def _create(self, path: str, instance: BaseModel) -> Dict:
         url = self._base_url / f"{path}/"
         data = json.loads(instance.json(exclude_none=True))
         if isinstance(instance, File):
             with open(instance.file, "rb") as f:
                 file = {"file": f}
-                response = self._session.post(url, data=data, files=file)
+                response = self._restclient.post(url, data=data, files=file)
         else:
-            response = self._session.post(url, json=data)
+            response = self._restclient.post(url, json=data)
 
         response.raise_for_status()
         return response.json()
 
     def _update(self, path: str, resource_id: str, data: BaseModel) -> Dict:
         url = self._base_url / f"{path}/{resource_id}/"
-        response = self._session.put(
+        response = self._restclient.put(
             url, json=json.loads(data.json(exclude_none=True))
         )
         response.raise_for_status()
         return response.json()
```

### Comparing `splight-lib-2.2.9/splight_lib/client/datalake/local_client.py` & `splight-lib-2.3.0/splight_lib/client/datalake/local_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 import pandas as pd
 
 from splight_abstract.client import QuerySet
 from splight_abstract.datalake import AbstractDatalakeClient
 from splight_lib.client.file_handler import FixedLineNumberFileHandler
 from splight_lib.client.filter import value_filter
 from splight_models import DatalakeModel, Query
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 
 DLResource = Type[DatalakeModel]
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 
 class LocalDatalakeClient(AbstractDatalakeClient):
     """Datalake client implementation for a storing locally documents
     in different files.
     """
```

### Comparing `splight-lib-2.2.9/splight_lib/client/datalake/remote_client.py` & `splight-lib-2.3.0/splight_lib/client/datalake/remote_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     AbstractDatalakeClient,
     validate_instance_type,
     validate_resource_type,
 )
 from splight_lib.client.exceptions import SPLIGHT_REQUEST_EXCEPTIONS
 from splight_lib.client.settings import settings_remote as settings
 from splight_lib.restclient import SplightRestClient
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 from splight_models import DatalakeModel, Query
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 
 class RemoteDatalakeClient(AbstractDatalakeClient, AbstractRemoteClient):
 
     _PREFIX = "v2/engine/datalake"
 
     def __init__(self, namespace: str = "default", *args, **kwargs):
```

### Comparing `splight-lib-2.2.9/splight_lib/client/exceptions.py` & `splight-lib-2.3.0/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/client/file_handler.py` & `splight-lib-2.3.0/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/client/filter.py` & `splight-lib-2.3.0/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/client/settings.py` & `splight-lib-2.3.0/splight_lib/client/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/component/abstract.py` & `splight-lib-2.3.0/splight_lib/component/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from tempfile import NamedTemporaryFile
 from typing import Optional, Type, List, Dict, Tuple, Set, Any, Callable, Union
 from mergedeep import merge, Strategy as mergeStrategy
 from collections import defaultdict
 from pydantic import BaseModel, main
 from functools import cached_property
 from splight_lib.execution import ExecutionClient, Thread
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 from splight_lib.settings import setup as default_setup
 from splight_models import (
     CustomType,
     Deployment,
     DatalakeModel,
     Component,
     Command,
@@ -44,15 +44,15 @@
     SetPointResponseStatus,
     SetPointCreateEvent,
     SetPointUpdateEvent
 )
 import re
 
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 
 class SecretValueParser:
 
     def __init__(self, utils, *args, **kwargs):
         self.utils = utils
```

### Comparing `splight-lib-2.2.9/splight_lib/encryption.py` & `splight-lib-2.3.0/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/execution.py` & `splight-lib-2.3.0/splight_lib/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     Thread as DefaultThread,
     Event,
     Lock,
 )
 from subprocess import Popen as DefaultPopen
 from functools import wraps
 from splight_abstract.client.abstract import AbstractClient
-from splight_lib.logging import getLogger, LogTags
+from splight_lib.logging._internal import get_splight_logger, LogTags
 
 
-logger = getLogger(dev=True)
+logger = get_splight_logger()
 
 class Empty(object):
     pass
 
 
 class Task:
     """A periodic task for the scheduler."""
```

### Comparing `splight-lib-2.2.9/splight_lib/logging.py` & `splight-lib-2.3.0/splight_lib/logging/logging.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,158 +1,148 @@
-import logging
 import time
 import os
 import sys
-from concurrent_log_handler import ConcurrentRotatingFileHandler
 from typing import Dict, Optional
-from enum import auto
-from strenum import UppercaseStrEnum
-
-
-class LogTags(UppercaseStrEnum):
-    RUNTIME = auto()
-    BINDING = auto()
-    COMMUNICATION = auto()
-    INDEX = auto()
-    SECRET = auto()
-    HOOK = auto()
-    SETPOINT = auto()
-    COMMAND = auto()
-    PARAMETER = auto()
-    COMPONENT = auto() # TODO: not used yet.
-    DATABASE = auto()
-    DATALAKE = auto()
-    CACHE = auto()
+from logging import (
+    Formatter,
+    Logger,
+    NOTSET,
+    DEBUG,
+    INFO,
+    WARNING,
+    ERROR,
+    CRITICAL,
+    Handler,
+    StreamHandler,
+    root as rootLogger,
+)
 
 TAGS_KEY = "tags"
 
 
-class SplightFormatter(logging.Formatter):
-    DEFAULT_FMT: str = "%(levelname)s | %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
+class SplightFormatter(Formatter):
+    DEFAULT_FMT: str = (
+        "%(levelname)s | %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
+    )
 
     def format(self, record):
         fmt = self.DEFAULT_FMT
         try:
             if record.tags is not None:
                 fmt = " | ".join([fmt, "%(tags)s"])
         except AttributeError:
             pass  # tags aren't present
-        formatter = logging.Formatter(fmt=fmt)
+        formatter = Formatter(fmt=fmt)
         formatter.converter = time.gmtime
         return formatter.format(record)
 
 
-class BaseSplightLogger:
-
+class SplightLogger(Logger):
     def __init__(self, name: str = None) -> None:
+        # import ipdb; ipdb.set_trace()
         # this is to avoid adding handlers to root logger
         # and interfering with third party app logs
         self.name = name if name is not None else "splight"
-        self.logger = logging.getLogger(self.name)
-        self.logger.setLevel(self.log_level)
-
-        # hasHandlers returns True when self parent
-        # have a handler so, don"t use method
-        if not self.logger.handlers:
-            self.load_handlers()
-
-    def __repr__(self) -> str:
-        level = logging.getLevelName(self.logger.getEffectiveLevel())
-        return '<%s %s (%s)>' % (self.__class__.__name__, self.name, level)
-
-    @property
-    def log_level(self) -> int:
-        return int(os.getenv("LOG_LEVEL", logging.DEBUG))
+        level = int(os.getenv("LOG_LEVEL", INFO))
+        super().__init__(name, level)
+        # TODO: check what exactly do function.__code__.co_filename
+        # this attr is defined to decide which is the caller filename
+        self._srcfile = os.path.normcase(
+            standard_output_handler.__code__.co_filename
+        )
 
     @property
-    def formatter(self) -> logging.Formatter:
+    def formatter(self) -> Formatter:
         return SplightFormatter()
 
-    def load_handlers(self) -> None:
-        handler = logging.StreamHandler(sys.stdout)
-        handler.setFormatter(self.formatter)
-        handler.setLevel(self.log_level)
-        self.logger.addHandler(handler)
-        self.logger.propagate = False
-
     @staticmethod
     def _update_kwargs(kwargs: Dict) -> Dict:
+        """Format log method tags and save into `extra` logging argument."""
         tags = kwargs.pop(TAGS_KEY, None)
         if tags is not None:
             kwargs.update({"extra": {TAGS_KEY: tags}})
         return kwargs
 
+    def _log(
+        self,
+        level,
+        msg,
+        args,
+        exc_info=None,
+        extra=None,
+        stack_info=False,
+        stacklevel=1,
+    ):
+        """
+        This is a copy from logging._log, where it only changes the `_srcfile`
+        variable to use `self._scrfile` because we need to update it for current
+        file, i.e, splight_lib.logging.py to show the correct log caller file in
+        formatter.
+        """
+        sinfo = None
+        if self._srcfile:
+            # IronPython doesn't track Python frames, so findCaller raises an
+            # exception on some versions of IronPython. We trap it here so that
+            # IronPython can use logging.
+            try:
+                fn, lno, func, sinfo = self.findCaller(stack_info, stacklevel)
+            except ValueError:  # pragma: no cover
+                fn, lno, func = "(unknown file)", 0, "(unknown function)"
+        else:  # pragma: no cover
+            fn, lno, func = "(unknown file)", 0, "(unknown function)"
+        if exc_info:
+            if isinstance(exc_info, BaseException):
+                exc_info = (type(exc_info), exc_info, exc_info.__traceback__)
+            elif not isinstance(exc_info, tuple):
+                exc_info = sys.exc_info()
+        record = self.makeRecord(
+            self.name, level, fn, lno, msg, args, exc_info, func, extra, sinfo
+        )
+        self.handle(record)
+
+    def setLevel(self, level, update_handlers=True):
+        super().setLevel(level)
+        if update_handlers:
+            for h in self.handlers:
+                h.setLevel(level)
+        # Add logger.level to root logger
+        rootLogger.setLevel(level)
+
     def debug(self, msg: str, *args, **kwargs):
-        kwargs = self._update_kwargs(kwargs)
-        self.logger.debug(msg, *args, **kwargs)
+        if self.isEnabledFor(DEBUG):
+            kwargs = self._update_kwargs(kwargs)
+            self._log(DEBUG, msg, args, **kwargs)
 
     def info(self, msg: str, *args, **kwargs):
-        kwargs = self._update_kwargs(kwargs)
-        self.logger.info(msg, *args, **kwargs)
+        if self.isEnabledFor(INFO):
+            kwargs = self._update_kwargs(kwargs)
+            self._log(INFO, msg, args, **kwargs)
 
     def warning(self, msg: str, *args, **kwargs):
-        kwargs = self._update_kwargs(kwargs)
-        self.logger.warning(msg, *args, **kwargs)
+        if self.isEnabledFor(WARNING):
+            kwargs = self._update_kwargs(kwargs)
+            self._log(WARNING, msg, args, **kwargs)
 
     def error(self, msg: str, *args, **kwargs):
-        kwargs = self._update_kwargs(kwargs)
-        self.logger.error(msg, *args, **kwargs)
-
-    def exception(self, msg: str, *args, **kwargs):
-        kwargs = self._update_kwargs(kwargs)
-        self.logger.exception(msg, *args, **kwargs)
+        if self.isEnabledFor(ERROR):
+            kwargs = self._update_kwargs(kwargs)
+            self._log(ERROR, msg, args, **kwargs)
+
+    def exception(self, msg: str, *args, exc_info=True, **kwargs):
+        if self.isEnabledFor(ERROR):
+            kwargs = self._update_kwargs(kwargs)
+            self._log(ERROR, msg, args, exc_info=exc_info, **kwargs)
 
     def critical(self, msg: str, *args, **kwargs):
-        kwargs = self._update_kwargs(kwargs)
-        self.logger.critical(msg, *args, **kwargs)
+        if self.isEnabledFor(CRITICAL):
+            kwargs = self._update_kwargs(kwargs)
+            self._log(CRITICAL, msg, args, **kwargs)
 
 
-class SplightDevLogger(BaseSplightLogger):
-    def __init__(self, name: str = None) -> None:
-        name = name if name is not None else "splight-dev"
-        super().__init__(name)
-
-    def load_handlers(self) -> None:
-        filename = os.getenv("SPLIGHT_DEVELOPER_LOG_FILE", "/tmp/splight-dev.log")
-        max_bytes = int(os.getenv("SPLIGHT_DEVELOPER_MAX_BYTES", 5e+6))  # 5MB
-        backup_count = int(os.getenv("SPLIGHT_DEVELOPER_BACKUP_COUNT", 100))
-        handler = ConcurrentRotatingFileHandler(
-            filename=filename, maxBytes=max_bytes, backupCount=backup_count
-        )
-        handler.setFormatter(self.formatter)
-        handler.setLevel(self.log_level)
-
-        self.logger.addHandler(handler)
-        self.logger.propagate = False
-
-
-class ComponentLogger(BaseSplightLogger):
-
-    def __init__(self, name: str = None) -> None:
-        name = name if name is not None else "component"
-        super().__init__(name)
-
-    def load_handlers(self) -> None:
-        super().load_handlers()  # to load stdout handler
-        # adding file handler
-        filename = os.getenv("SPLIGHT_COMPONENT_LOG_FILE", "/tmp/components.log")
-        max_bytes = int(os.getenv("SPLIGHT_COMPONENT_MAX_BYTES", 5e+6))  # 5MB
-        backup_count = int(os.getenv("SPLIGHT_COMPONENT_BACKUP_COUNT", 100))
-        handler = ConcurrentRotatingFileHandler(
-            filename=filename, maxBytes=max_bytes, backupCount=backup_count
-        )
-        handler.setFormatter(self.formatter)
-
-        handler.setLevel(self.log_level)
-        self.logger.addHandler(handler)
-        self.logger.propagate = False
-
-
-def getLogger(name: Optional[str] = None, dev: bool = False):
-    if dev:
-        logger = SplightDevLogger(name)
-    else:
-        logger = ComponentLogger(name)
-    # Add handlers to root logger and his childrens
-    # force=True to force override
-    logging.basicConfig(handlers=logger.logger.handlers, force=True)
-    return logger
+def standard_output_handler(
+    formatter: Optional[Formatter] = SplightFormatter(),
+    log_level: Optional[str] = INFO,
+) -> Handler:
+    handler = StreamHandler(sys.stdout)
+    handler.setFormatter(formatter)
+    handler.setLevel(log_level)
+    return handler
```

### Comparing `splight-lib-2.2.9/splight_lib/restclient/client.py` & `splight-lib-2.3.0/splight_lib/restclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import httpx
 from typing import Optional, Callable, Any, Union, Mapping, List
 
-from splight_lib.restclient.cached import CachedObject
 from splight_lib.restclient.types import (
     AuthTypes,
     QueryParamTypes,
     HeaderTypes,
     CookieTypes,
     TimeoutTypes,
     DEFAULT_TIMEOUT_CONFIG,
@@ -58,15 +57,15 @@
         for attr in response.__dict__.keys():
             response_attr = getattr(response, attr)
             setattr(obj_cls, attr, response_attr)
 
         return obj_cls
 
 
-class SplightRestClient(CachedObject):
+class SplightRestClient:
     """A REST client for making HTTP requests.
 
     Currently, this client is based on httpx.Client.
 
     Class initialization parameters.
 
     1. Compatible with requests interface.
```

### Comparing `splight-lib-2.2.9/splight_lib/restclient/exceptions.py` & `splight-lib-2.3.0/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/restclient/types.py` & `splight-lib-2.3.0/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/settings.py` & `splight-lib-2.3.0/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib/webhook.py` & `splight-lib-2.3.0/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_lib.egg-info/PKG-INFO` & `splight-lib-2.3.0/splight_lib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.2.9
+Version: 2.3.0
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE.txt
 
 [![Lib upload](https://github.com/splightplatform/splight-lib/actions/workflows/libupload.yml/badge.svg)](https://github.com/splightplatform/splight-lib/actions/workflows/libupload.yml)
 
 ## How to install
 
 For development
 
-- `python setup.py develop`
+- `make install`
 
 For productive envs.
 
 - `python setup.py install`
 
 ## Tests
 
 ```
-pytest splight_lib/tests
+make test
 ```
```

### Comparing `splight-lib-2.2.9/splight_lib.egg-info/SOURCES.txt` & `splight-lib-2.3.0/splight_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 splight_abstract/remote/__init__.py
 splight_abstract/remote/abstract.py
 splight_abstract/storage/__init__.py
 splight_abstract/storage/abstract.py
 splight_lib/__init__.py
 splight_lib/encryption.py
 splight_lib/execution.py
-splight_lib/logging.py
 splight_lib/settings.py
 splight_lib/webhook.py
 splight_lib.egg-info/PKG-INFO
 splight_lib.egg-info/SOURCES.txt
 splight_lib.egg-info/dependency_links.txt
 splight_lib.egg-info/not-zip-safe
 splight_lib.egg-info/requires.txt
@@ -70,16 +69,19 @@
 splight_lib/client/database/local_client.py
 splight_lib/client/database/remote_client.py
 splight_lib/client/datalake/__init__.py
 splight_lib/client/datalake/local_client.py
 splight_lib/client/datalake/remote_client.py
 splight_lib/component/__init__.py
 splight_lib/component/abstract.py
+splight_lib/logging/__init__.py
+splight_lib/logging/_internal.py
+splight_lib/logging/component.py
+splight_lib/logging/logging.py
 splight_lib/restclient/__init__.py
-splight_lib/restclient/cached.py
 splight_lib/restclient/client.py
 splight_lib/restclient/exceptions.py
 splight_lib/restclient/types.py
 splight_models/__init__.py
 splight_models/alert.py
 splight_models/asset.py
 splight_models/attribute.py
```

### Comparing `splight-lib-2.2.9/splight_models/__init__.py` & `splight-lib-2.3.0/splight_models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/alert.py` & `splight-lib-2.3.0/splight_models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/blockchain.py` & `splight-lib-2.3.0/splight_models/blockchain.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/communication/context.py` & `splight-lib-2.3.0/splight_models/communication/context.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/communication/events.py` & `splight-lib-2.3.0/splight_models/communication/events.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/component.py` & `splight-lib-2.3.0/splight_models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/constants.py` & `splight-lib-2.3.0/splight_models/constants.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/datalake.py` & `splight-lib-2.3.0/splight_models/datalake.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/deployment.py` & `splight-lib-2.3.0/splight_models/deployment.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/exception.py` & `splight-lib-2.3.0/splight_models/exception.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/file.py` & `splight-lib-2.3.0/splight_models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/hub.py` & `splight-lib-2.3.0/splight_models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/notification.py` & `splight-lib-2.3.0/splight_models/notification.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/query.py` & `splight-lib-2.3.0/splight_models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/setpoint.py` & `splight-lib-2.3.0/splight_models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/user.py` & `splight-lib-2.3.0/splight_models/user.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/variable.py` & `splight-lib-2.3.0/splight_models/variable.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.9/splight_models/webhook.py` & `splight-lib-2.3.0/splight_models/webhook.py`

 * *Files identical despite different names*

