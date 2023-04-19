# Comparing `tmp/pip_services3_rpc-3.3.3.tar.gz` & `tmp/pip_services3_rpc-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pip_services3_rpc-3.3.3.tar", last modified: Sun Apr 17 15:52:15 2022, max compression
+gzip compressed data, was "pip_services3_rpc-3.3.4.tar", last modified: Wed Apr 19 00:39:06 2023, max compression
```

## Comparing `pip_services3_rpc-3.3.3.tar` & `pip_services3_rpc-3.3.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/
--rw-r--r--   0 runner    (1001) docker     (116)      291 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/
--rw-r--r--   0 runner    (1001) docker     (116)    16490 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/RestService.py
--rw-r--r--   0 runner    (1001) docker     (116)     4405 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/HttpRequestDetector.py
--rw-r--r--   0 runner    (1001) docker     (116)     1455 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/RestQueryParams.py
--rw-r--r--   0 runner    (1001) docker     (116)      528 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/HeartBeatOperations.py
--rw-r--r--   0 runner    (1001) docker     (116)     3493 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/AboutOperations.py
--rw-r--r--   0 runner    (1001) docker     (116)     1506 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/SSLCherryPyServer.py
--rw-r--r--   0 runner    (1001) docker     (116)     2704 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/StatusOperations.py
--rw-r--r--   0 runner    (1001) docker     (116)     4782 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/HttpResponseSender.py
--rw-r--r--   0 runner    (1001) docker     (116)     5387 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/CommandableHttpService.py
--rw-r--r--   0 runner    (1001) docker     (116)     5535 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/RestOperations.py
--rw-r--r--   0 runner    (1001) docker     (116)     3465 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/HeartbeatRestService.py
--rw-r--r--   0 runner    (1001) docker     (116)      520 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/IRegisterable.py
--rw-r--r--   0 runner    (1001) docker     (116)     2046 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/InstrumentTiming.py
--rw-r--r--   0 runner    (1001) docker     (116)     1509 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8523 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/CommandableSwaggerDocument.py
--rw-r--r--   0 runner    (1001) docker     (116)     5982 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/StatusRestService.py
--rw-r--r--   0 runner    (1001) docker     (116)    17870 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/HttpEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)      292 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/services/ISwaggerService.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/test/
--rw-r--r--   0 runner    (1001) docker     (116)      968 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/test/TestCommandableHttpClient.py
--rw-r--r--   0 runner    (1001) docker     (116)      192 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1028 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/test/TestRestClient.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/clients/
--rw-r--r--   0 runner    (1001) docker     (116)    15115 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/clients/RestClient.py
--rw-r--r--   0 runner    (1001) docker     (116)     6625 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/clients/DirectClient.py
--rw-r--r--   0 runner    (1001) docker     (116)     4015 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/clients/CommandableHttpClient.py
--rw-r--r--   0 runner    (1001) docker     (116)      491 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/connect/
--rw-r--r--   0 runner    (1001) docker     (116)     9001 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/connect/HttpConnectionResolver.py
--rw-r--r--   0 runner    (1001) docker     (116)      385 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/auth/
--rw-r--r--   0 runner    (1001) docker     (116)      685 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/auth/BasicAuthorizer.py
--rw-r--r--   0 runner    (1001) docker     (116)      226 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1367 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/auth/RoleAuthorizer.py
--rw-r--r--   0 runner    (1001) docker     (116)     2070 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/auth/OwnerAuthorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/build/
--rw-r--r--   0 runner    (1001) docker     (116)      371 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1246 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/pip_services3_rpc/build/DefaultRpcFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/pip_services3_rpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1304 2022-04-17 15:52:14.000000 pip_services3_rpc-3.3.3/pip_services3_rpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      180 2022-04-17 15:52:14.000000 pip_services3_rpc-3.3.3/pip_services3_rpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-17 15:52:14.000000 pip_services3_rpc-3.3.3/pip_services3_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-04-17 15:52:14.000000 pip_services3_rpc-3.3.3/pip_services3_rpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2640 2022-04-17 15:52:14.000000 pip_services3_rpc-3.3.3/pip_services3_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-17 15:52:14.000000 pip_services3_rpc-3.3.3/pip_services3_rpc.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)     1304 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       54 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2368 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      168 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4312 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)     1860 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/test/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/test/services/
--rw-r--r--   0 runner    (1001) docker     (116)     2353 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/DummyRestOperations.py
--rw-r--r--   0 runner    (1001) docker     (116)     5528 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/test_DummyRestService.py
--rw-r--r--   0 runner    (1001) docker     (116)     3004 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/test_DummyCredentialsRestService.py
--rw-r--r--   0 runner    (1001) docker     (116)     5380 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/test_DummyCommandableHttpService.py
--rw-r--r--   0 runner    (1001) docker     (116)     1255 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/test_HeartbeatRestService.py
--rw-r--r--   0 runner    (1001) docker     (116)      520 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2408 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/test_HttpEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)      864 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/DummyCommandableHttpService.py
--rw-r--r--   0 runner    (1001) docker     (116)     5202 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/DummyRestService.py
--rw-r--r--   0 runner    (1001) docker     (116)     1807 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/test_StatusRestService.py
--rw-r--r--   0 runner    (1001) docker     (116)     4097 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/services/test_DummyOperations.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/test/clients/
--rw-r--r--   0 runner    (1001) docker     (116)     2681 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/clients/DummyCommandableHttpClient.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/clients/test_DummyCommandableHttpClient.py
--rw-r--r--   0 runner    (1001) docker     (116)     2978 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/clients/DummyDirectClient.py
--rw-r--r--   0 runner    (1001) docker     (116)     4046 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/clients/DummyRestClient.py
--rw-r--r--   0 runner    (1001) docker     (116)     1816 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/clients/test_DummyRestClient.py
--rw-r--r--   0 runner    (1001) docker     (116)      929 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2182 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/clients/DummyClientFixture.py
--rw-r--r--   0 runner    (1001) docker     (116)     1345 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/clients/IDummyClient.py
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/clients/test_DummyDirectClient.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-17 15:52:15.000000 pip_services3_rpc-3.3.3/test/connect/
--rw-r--r--   0 runner    (1001) docker     (116)     6083 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/connect/test_HttpConnectionResolver.py
--rw-r--r--   0 runner    (1001) docker     (116)      395 2022-04-17 15:51:01.000000 pip_services3_rpc-3.3.3/test/connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.076429 pip_services3_rpc-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 00:39:06.076429 pip_services3_rpc-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.064428 pip_services3_rpc-3.3.4/pip_services3_rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.068429 pip_services3_rpc-3.3.4/pip_services3_rpc/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/auth/BasicAuthorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/auth/OwnerAuthorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/auth/RoleAuthorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.068429 pip_services3_rpc-3.3.4/pip_services3_rpc/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/build/DefaultRpcFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.068429 pip_services3_rpc-3.3.4/pip_services3_rpc/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/clients/CommandableHttpClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/clients/DirectClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/clients/RestClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.068429 pip_services3_rpc-3.3.4/pip_services3_rpc/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/connect/HttpConnectionResolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.072429 pip_services3_rpc-3.3.4/pip_services3_rpc/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/AboutOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/CommandableHttpService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/CommandableSwaggerDocument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/HeartBeatOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/HeartbeatRestService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/HttpEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/HttpRequestDetector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/HttpResponseSender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/IRegisterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/ISwaggerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/InstrumentTiming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/RestOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/RestQueryParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16490 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/RestService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/SSLCherryPyServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/StatusOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/StatusRestService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.072429 pip_services3_rpc-3.3.4/pip_services3_rpc/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/test/TestCommandableHttpClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/test/TestRestClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/pip_services3_rpc/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.068429 pip_services3_rpc-3.3.4/pip_services3_rpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 00:39:06.000000 pip_services3_rpc-3.3.4/pip_services3_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-19 00:39:06.000000 pip_services3_rpc-3.3.4/pip_services3_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:39:06.000000 pip_services3_rpc-3.3.4/pip_services3_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-19 00:39:06.000000 pip_services3_rpc-3.3.4/pip_services3_rpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 00:39:06.000000 pip_services3_rpc-3.3.4/pip_services3_rpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:39:06.000000 pip_services3_rpc-3.3.4/pip_services3_rpc.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 00:39:06.076429 pip_services3_rpc-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.064428 pip_services3_rpc-3.3.4/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.076429 pip_services3_rpc-3.3.4/test/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/clients/DummyClientFixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/clients/DummyCommandableHttpClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/clients/DummyDirectClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/clients/DummyRestClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/clients/IDummyClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/clients/test_DummyCommandableHttpClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/clients/test_DummyDirectClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/clients/test_DummyRestClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.076429 pip_services3_rpc-3.3.4/test/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/connect/test_HttpConnectionResolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:39:06.076429 pip_services3_rpc-3.3.4/test/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/DummyCommandableHttpService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/DummyRestOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/DummyRestService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/test_DummyCommandableHttpService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/test_DummyCredentialsRestService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/test_DummyOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/test_DummyRestService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/test_HeartbeatRestService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/test_HttpEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-19 00:38:26.000000 pip_services3_rpc-3.3.4/test/services/test_StatusRestService.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/RestService.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/RestService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/HttpRequestDetector.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/HttpRequestDetector.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,17 +92,19 @@
                 ip = json_data['connection']['remoteAddress']
             except KeyError:
                 try:
                     ip = json_data['connection']['socket']['remoteAddress']
                 except KeyError:
                     pass
 
-        if ip is None:
+        if ip is None and json_data is not None:
             try:
-                ip = json_data['socket']['remoteAddress']
+                socket = json_data.get('socket')
+                if socket:
+                    ip = socket.get('remoteAddress')
             except KeyError:
                 pass
 
         if ip is not None:
             ip = str(ip)
             index = ip.find(':')
             if index > 0:
```

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/RestQueryParams.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/RestQueryParams.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/HeartBeatOperations.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/HeartBeatOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/AboutOperations.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/AboutOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/SSLCherryPyServer.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/SSLCherryPyServer.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/StatusOperations.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/StatusOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/HttpResponseSender.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/HttpResponseSender.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/CommandableHttpService.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/CommandableHttpService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/RestOperations.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/RestOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/HeartbeatRestService.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/HeartbeatRestService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/IRegisterable.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/IRegisterable.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/InstrumentTiming.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/InstrumentTiming.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/__init__.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/CommandableSwaggerDocument.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/CommandableSwaggerDocument.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/StatusRestService.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/StatusRestService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/services/HttpEndpoint.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/services/HttpEndpoint.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/test/TestCommandableHttpClient.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/test/TestCommandableHttpClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/test/TestRestClient.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/test/TestRestClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/clients/RestClient.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/clients/RestClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/clients/DirectClient.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/clients/DirectClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/clients/CommandableHttpClient.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/clients/CommandableHttpClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/connect/HttpConnectionResolver.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/connect/HttpConnectionResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/auth/BasicAuthorizer.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/auth/BasicAuthorizer.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/auth/RoleAuthorizer.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/auth/RoleAuthorizer.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/auth/OwnerAuthorizer.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/auth/OwnerAuthorizer.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc/build/DefaultRpcFactory.py` & `pip_services3_rpc-3.3.4/pip_services3_rpc/build/DefaultRpcFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc.egg-info/PKG-INFO` & `pip_services3_rpc-3.3.4/pip_services3_rpc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: pip-services3-rpc
-Version: 3.3.3
+Version: 3.3.4
 Summary: Communication components for Pip.Services in Python
 Home-page: http://github.com/pip-services3-python/pip-services3-rpc-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
-Description: 
-        Pip.Services Rpc
-        ----------------------
-        
-        Pip.Services is an open-source library of basic microservices.
-        pip_services3_rpc provides synchronous and asynchronous communication components.
-        
-        Links
-        `````
-        
-        * `website <http://github.com/pip-services-python/>`_
-        * `development version <http://github.com/pip-services3-python/pip-services3-rpc-python>`
-        
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+Pip.Services Rpc
+----------------------
+
+Pip.Services is an open-source library of basic microservices.
+pip_services3_rpc provides synchronous and asynchronous communication components.
+
+Links
+`````
+
+* `website <http://github.com/pip-services-python/>`_
+* `development version <http://github.com/pip-services3-python/pip-services3-rpc-python>`
+
+
+
```

### Comparing `pip_services3_rpc-3.3.3/pip_services3_rpc.egg-info/SOURCES.txt` & `pip_services3_rpc-3.3.4/pip_services3_rpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/PKG-INFO` & `pip_services3_rpc-3.3.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,60 @@
-Metadata-Version: 2.1
-Name: pip_services3_rpc
-Version: 3.3.3
-Summary: Communication components for Pip.Services in Python
-Home-page: http://github.com/pip-services3-python/pip-services3-rpc-python
-Author: Conceptual Vision Consulting LLC
-Author-email: seroukhov@gmail.com
-License: MIT
-Description: 
-        Pip.Services Rpc
-        ----------------------
-        
-        Pip.Services is an open-source library of basic microservices.
-        pip_services3_rpc provides synchronous and asynchronous communication components.
-        
-        Links
-        `````
-        
-        * `website <http://github.com/pip-services-python/>`_
-        * `development version <http://github.com/pip-services3-python/pip-services3-rpc-python>`
-        
-        
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
+"""
+Pip.Services Rpc
+----------------------
+
+Pip.Services is an open-source library of basic microservices.
+pip_services3_rpc provides synchronous and asynchronous communication components.
+
+Links
+`````
+
+* `website <http://github.com/pip-services-python/>`_
+* `development version <http://github.com/pip-services3-python/pip-services3-rpc-python>`
+
+"""
+
+from setuptools import find_packages
+from setuptools import setup
+
+try:
+    readme = open('readme.md').read()
+except:
+    readme = __doc__
+
+setup(
+    name='pip_services3_rpc',
+    version='3.3.4',
+    url='http://github.com/pip-services3-python/pip-services3-rpc-python',
+    license='MIT',
+    author='Conceptual Vision Consulting LLC',
+    author_email='seroukhov@gmail.com',
+    description='Communication components for Pip.Services in Python',
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    packages=find_packages(exclude=['config', 'data', 'test']),
+    include_package_data=True,
+    zip_safe=True,
+    platforms='any',
+    install_requires=[
+        'pytz',
+        'bottle >= 0.12.19, < 0.13',
+        'requests >= 2.27.1, < 3.0',
+        'cheroot >= 8.6.0, < 9.0',
+        'beaker >= 1.11.0, < 2.0',
+        'psutil >= 5.9.0, < 6.0',
+        'pip-services3-commons >= 3.3.14, < 4.0',
+        'pip-services3-components >= 3.5.9, < 4.0'
+    ],
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Topic :: Software Development :: Libraries :: Python Modules'
+    ]
+)
```

### Comparing `pip_services3_rpc-3.3.3/README.md` & `pip_services3_rpc-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/LICENSE` & `pip_services3_rpc-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/CHANGELOG.md` & `pip_services3_rpc-3.3.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # <img src="https://uploads-ssl.webflow.com/5ea5d3315186cf5ec60c3ee4/5edf1c94ce4c859f2b188094_logo.svg" alt="Pip.Services Logo" width="200"> <br/> Remote Procedure Calls for Python Changelog
 
+## <a name="3.3.4"></a> 3.3.4 (2023-04-19)
+### Bug Fixes
+- Fixed HttpRequestDetector.detect_address
+
 ## <a name="3.3.3"></a> 3.3.3 (2022-04-17)
 
 ### Bug Fixes
 * Fixed error processing for CommandableHttpClient
 * Improve body Schema validation for requests
 * Make server process as deamon
```

### Comparing `pip_services3_rpc-3.3.3/test/services/DummyRestOperations.py` & `pip_services3_rpc-3.3.4/test/services/DummyRestOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/test_DummyRestService.py` & `pip_services3_rpc-3.3.4/test/services/test_DummyRestService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/test_DummyCredentialsRestService.py` & `pip_services3_rpc-3.3.4/test/services/test_DummyCredentialsRestService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/test_DummyCommandableHttpService.py` & `pip_services3_rpc-3.3.4/test/services/test_DummyCommandableHttpService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/test_HeartbeatRestService.py` & `pip_services3_rpc-3.3.4/test/services/test_HeartbeatRestService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/__init__.py` & `pip_services3_rpc-3.3.4/test/services/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/test_HttpEndpoint.py` & `pip_services3_rpc-3.3.4/test/services/test_HttpEndpoint.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/DummyCommandableHttpService.py` & `pip_services3_rpc-3.3.4/test/services/DummyCommandableHttpService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/DummyRestService.py` & `pip_services3_rpc-3.3.4/test/services/DummyRestService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/test_StatusRestService.py` & `pip_services3_rpc-3.3.4/test/services/test_StatusRestService.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/services/test_DummyOperations.py` & `pip_services3_rpc-3.3.4/test/services/test_DummyOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/clients/DummyCommandableHttpClient.py` & `pip_services3_rpc-3.3.4/test/clients/DummyCommandableHttpClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/clients/test_DummyCommandableHttpClient.py` & `pip_services3_rpc-3.3.4/test/clients/test_DummyCommandableHttpClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/clients/DummyDirectClient.py` & `pip_services3_rpc-3.3.4/test/clients/DummyDirectClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/clients/DummyRestClient.py` & `pip_services3_rpc-3.3.4/test/clients/DummyRestClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/clients/test_DummyRestClient.py` & `pip_services3_rpc-3.3.4/test/clients/test_DummyRestClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/clients/__init__.py` & `pip_services3_rpc-3.3.4/test/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/clients/DummyClientFixture.py` & `pip_services3_rpc-3.3.4/test/clients/DummyClientFixture.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/clients/IDummyClient.py` & `pip_services3_rpc-3.3.4/test/clients/IDummyClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/clients/test_DummyDirectClient.py` & `pip_services3_rpc-3.3.4/test/clients/test_DummyDirectClient.py`

 * *Files identical despite different names*

### Comparing `pip_services3_rpc-3.3.3/test/connect/test_HttpConnectionResolver.py` & `pip_services3_rpc-3.3.4/test/connect/test_HttpConnectionResolver.py`

 * *Files identical despite different names*

