# Comparing `tmp/panda-server-0.0.50.tar.gz` & `tmp/panda-server-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda-server-0.0.50.tar", last modified: Wed Mar 22 14:24:56 2023, max compression
+gzip compressed data, was "panda-server-0.0.51.tar", last modified: Wed Apr 19 15:31:41 2023, max compression
```

## Comparing `panda-server-0.0.50.tar` & `panda-server-0.0.51.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.118962 panda-server-0.0.50/
--rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-03-22 14:24:43.000000 panda-server-0.0.50/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-22 14:24:43.000000 panda-server-0.0.50/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-22 14:24:43.000000 panda-server-0.0.50/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-22 14:24:56.118962 panda-server-0.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-22 14:24:43.000000 panda-server-0.0.50/PandaPkgInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-22 14:24:43.000000 panda-server-0.0.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.086962 panda-server-0.0.50/panda_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-22 14:24:56.000000 panda-server-0.0.50/panda_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-03-22 14:24:56.000000 panda-server-0.0.50/panda_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:24:56.000000 panda-server-0.0.50/panda_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:24:55.000000 panda-server-0.0.50/panda_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-22 14:24:56.000000 panda-server-0.0.50/panda_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-22 14:24:56.000000 panda-server-0.0.50/panda_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.086962 panda-server-0.0.50/pandaserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.086962 panda-server-0.0.50/pandaserver/brokerage/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/brokerage/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.086962 panda-server-0.0.50/pandaserver/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/config/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/config/daemon_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/config/panda_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.090962 panda-server-0.0.50/pandaserver/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/configurator/Carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/configurator/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/configurator/aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.090962 panda-server-0.0.50/pandaserver/daemons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/master.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.090962 panda-server-0.0.50/pandaserver/daemons/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0 runner    (1001) docker     (123)    37494 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25064 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/daemons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.094962 panda-server-0.0.50/pandaserver/dataservice/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/Activator.py
--rw-r--r--   0 runner    (1001) docker     (123)    53932 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    39385 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/AdderSimplePlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/Closer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/CloserAtlasPlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/DDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/DDMHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/DataService.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/DataServiceUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/DynDataDistributer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/EventPicker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/Finisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16870 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/Notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/Setupper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113610 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/SetupperAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/SetupperDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/SetupperPluginBase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/eventLookupClientEI.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/dataservice/forkSetupper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.094962 panda-server-0.0.50/pandaserver/jobdispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58617 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16196 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/jobdispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.094962 panda-server-0.0.50/pandaserver/proxycache/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/proxycache/DBMSql.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/proxycache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/proxycache/panda_activeusers_query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/proxycache/panda_proxy_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.094962 panda-server-0.0.50/pandaserver/server/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/server/.gacl
--rwxr-xr-x   0 runner    (1001) docker     (123)    22396 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/server/panda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.098962 panda-server-0.0.50/pandaserver/srvcore/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/srvcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/srvcore/srv_msg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.102962 panda-server-0.0.50/pandaserver/taskbuffer/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/EiDBProxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7837 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25877 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)  1227603 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   137660 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19062 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/taskbuffer/workflow_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.110962 panda-server-0.0.50/pandaserver/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/SchemaChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.110962 panda-server-0.0.50/pandaserver/test/alice/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/banUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/boostPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/boostUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/callbackDDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/finishJob.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/finishTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/frontier_retagging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/getJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/killJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/killTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/killUser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.110962 panda-server-0.0.50/pandaserver/test/lsst/
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/reassignJobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/reassignSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/reassignTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/reassignWaiting.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/reloadInputDS.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/setPriority.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testEvgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testG4sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testG4sim17.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testReco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testSiteMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/test/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.110962 panda-server-0.0.50/pandaserver/userinterface/
--rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/userinterface/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)    89122 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/userinterface/UserIF.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/userinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.110962 panda-server-0.0.50/pandaserver/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/psnakemake_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.114962 panda-server-0.0.50/pandaserver/workflow/snakeparser/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35855 2023-03-22 14:24:43.000000 panda-server-0.0.50/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-22 14:24:56.118962 panda-server-0.0.50/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    13632 2023-03-22 14:24:43.000000 panda-server-0.0.50/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.118962 panda-server-0.0.50/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/conda_meta.yaml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.118962 panda-server-0.0.50/templates/init.d/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/init.d/panda_server.exe.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.118962 panda-server-0.0.50/templates/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/logrotate.d/panda_server.logrotate.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-add_main.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-add_sub.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-backupJobArch.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-boostUser.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-callback.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-configurator.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-copyArchive.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-datasetManager.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-esPreemption.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-evpPD2P.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-frontier_retagging.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-httpd.conf.rpmnew.template
--rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-network_configurator.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-pilot_streaming.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-priority.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-proxyCache.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-schedconfig_json.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-sw_tags.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-tmpwatch.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server-vomsrenew.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/panda_server.cfg.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/pandasrv.cron.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:24:56.118962 panda-server-0.0.50/templates/sysconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-22 14:24:43.000000 panda-server-0.0.50/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.009645 panda-server-0.0.51/
+-rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-04-19 15:31:28.000000 panda-server-0.0.51/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-19 15:31:28.000000 panda-server-0.0.51/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 15:31:28.000000 panda-server-0.0.51/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-19 15:31:41.009645 panda-server-0.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 15:31:28.000000 panda-server-0.0.51/PandaPkgInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 15:31:28.000000 panda-server-0.0.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.977645 panda-server-0.0.51/panda_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:28.000000 panda-server-0.0.51/pandaserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/brokerage/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/brokerage/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/config/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/config/panda_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/configurator/Carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/configurator/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/configurator/aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/master.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.985645 panda-server-0.0.51/pandaserver/daemons/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37494 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25064 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/dataservice/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Activator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39385 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderSimplePlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Closer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/CloserAtlasPlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DDMHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DataService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DataServiceUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DynDataDistributer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/EventPicker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Finisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16870 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Setupper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113610 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/SetupperAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/SetupperDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/SetupperPluginBase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/eventLookupClientEI.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/forkSetupper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/jobdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58936 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16316 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/proxycache/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/proxycache/DBMSql.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/proxycache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/proxycache/panda_activeusers_query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/proxycache/panda_proxy_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/server/.gacl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22396 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/server/panda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/srvcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/srv_msg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.997645 panda-server-0.0.51/pandaserver/taskbuffer/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/EiDBProxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1232383 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   137660 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19062 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/workflow_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/test/alice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/banUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/boostUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/callbackDDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/finishJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/finishTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/frontier_retagging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/getJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killUser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/test/lsst/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reassignJobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reassignSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/setPriority.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testG4sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testG4sim17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testReco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testSiteMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/userinterface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/userinterface/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89144 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/userinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/psnakemake_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.005645 panda-server-0.0.51/pandaserver/workflow/snakeparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-19 15:31:41.009645 panda-server-0.0.51/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13632 2023-04-19 15:31:29.000000 panda-server-0.0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.005645 panda-server-0.0.51/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/conda_meta.yaml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.009645 panda-server-0.0.51/templates/init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/init.d/panda_server.exe.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.009645 panda-server-0.0.51/templates/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/logrotate.d/panda_server.logrotate.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-add_main.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-add_sub.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-backupJobArch.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-boostUser.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-callback.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-configurator.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-copyArchive.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-datasetManager.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-esPreemption.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-evpPD2P.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-frontier_retagging.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-httpd.conf.rpmnew.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-network_configurator.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-pilot_streaming.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-priority.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-proxyCache.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-schedconfig_json.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-sw_tags.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-tmpwatch.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-vomsrenew.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server.cfg.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/pandasrv.cron.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.009645 panda-server-0.0.51/templates/sysconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/sysconfig/panda_server.sysconfig.rpmnew.template
```

### Comparing `panda-server-0.0.50/ChangeLog.txt` & `panda-server-0.0.51/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/LICENSE.txt` & `panda-server-0.0.51/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/panda_server.egg-info/SOURCES.txt` & `panda-server-0.0.51/panda_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/brokerage/SiteMapper.py` & `panda-server-0.0.51/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/brokerage/broker.py` & `panda-server-0.0.51/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/config/daemon_config.py` & `panda-server-0.0.51/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/config/panda_config.py` & `panda-server-0.0.51/pandaserver/config/panda_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/configurator/Carbon.py` & `panda-server-0.0.51/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/configurator/Configurator.py` & `panda-server-0.0.51/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/configurator/aux.py` & `panda-server-0.0.51/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/master.py` & `panda-server-0.0.51/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/add_main.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/add_main.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/add_sub.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/carbon.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/configurator.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/copyArchive.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/datasetManager.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/datasetManager.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/dummy_test.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/dummy_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/evpPD2P.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/metric_collector.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/pilotStreaming.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/task_evaluator.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/tmpwatch.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/scripts/worker_synchronization.py` & `panda-server-0.0.51/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/daemons/utils.py` & `panda-server-0.0.51/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/Activator.py` & `panda-server-0.0.51/pandaserver/dataservice/Activator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda-server-0.0.51/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -807,15 +807,15 @@
                             if tmpDsName.startswith('group') and self.job.workingGroup not in ['','NULL',None]:
                                 tmpDN = self.job.workingGroup
                             else:
                                 tmpDN = userInfo['nickname']
                             tmpMsg = "registerDatasetLocation for Rucio ds=%s site=%s id=%s" % (tmpDsName,tmpDQ2ID,tmpDN)
                             self.logger.debug(tmpMsg)
                             rucioAPI.registerDatasetLocation(tmpDsName,[tmpDQ2ID],owner=tmpDN,
-                                                             activity="User Subscriptions")
+                                                             activity="Analysis Output")
                     # set dataset status
                     for tmpName in subMap:
                         self.datasetMap[tmpName].status = 'running'
                 except (InsufficientAccountLimit, InvalidRSEExpression) as errType:
                     tmpMsg = "Rucio rejected to transfer files to {0} since {1}".format(','.join(userEPs),errType)
                     self.logger.error(tmpMsg)
                     self.job.ddmErrorCode = ErrorCode.EC_Adder
```

### Comparing `panda-server-0.0.50/pandaserver/dataservice/AdderGen.py` & `panda-server-0.0.51/pandaserver/dataservice/AdderGen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/AdderResult.py` & `panda-server-0.0.51/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/AdderSimplePlugin.py` & `panda-server-0.0.51/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/Closer.py` & `panda-server-0.0.51/pandaserver/dataservice/Closer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/CloserAtlasPlugin.py` & `panda-server-0.0.51/pandaserver/dataservice/CloserAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/DDM.py` & `panda-server-0.0.51/pandaserver/dataservice/DDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/DDMHandler.py` & `panda-server-0.0.51/pandaserver/dataservice/DDMHandler.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/DataService.py` & `panda-server-0.0.51/pandaserver/dataservice/DataService.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/DataServiceUtils.py` & `panda-server-0.0.51/pandaserver/dataservice/DataServiceUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,21 +200,24 @@
 
     # nonexistent site
     if not siteMapper.checkSite(siteName):
         return []
     # get siteSpec
     siteSpec = siteMapper.getSite(siteName)
     scope_site_input, scope_site_output = select_scope(siteSpec, prodSourceLabel, job_label)
+    runs_production = siteSpec.runs_production()
+    runs_analysis = siteSpec.runs_analysis()
     # loop over all sites
     retSites = []
     for tmpSiteName in siteMapper.siteSpecList:
         tmpSiteSpec = siteMapper.siteSpecList[tmpSiteName]
         scope_tmpSite_input, scope_tmpSite_output = select_scope(tmpSiteSpec, prodSourceLabel, job_label)
         # only same type
-        if siteSpec.type != tmpSiteSpec.type:
+        if (runs_production and not tmpSiteSpec.runs_production()) or \
+                (runs_analysis and not tmpSiteSpec.runs_analysis()):
             continue
         # only online sites
         if tmpSiteSpec.status != 'online':
             continue
         # same endpoint
         try:
             if not output_share and \
@@ -285,15 +288,15 @@
 
 
 # get activity for output
 def getActivityForOut(prodSourceLabel):
     if prodSourceLabel in ['managed']:
         activity = "Production Output"
     elif prodSourceLabel in ['user','panda']:
-        activity = "User Subscriptions"
+        activity = "Analysis Output"
     else:
         activity = "Functional Test"
     return activity
 
 
 def select_scope(site_spec, prodsourcelabel, job_label):
     """
```

### Comparing `panda-server-0.0.50/pandaserver/dataservice/DynDataDistributer.py` & `panda-server-0.0.51/pandaserver/dataservice/DynDataDistributer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/EventPicker.py` & `panda-server-0.0.51/pandaserver/dataservice/EventPicker.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                         tmpDQ2ID = tmpSiteSpec.ddm_output[scope_output]
                         tmpMsg = "%s ds=%s site=%s id=%s" % ('registerDatasetLocation for EventPicking ',
                                                              tmpUserDatasetName,
                                                              tmpDQ2ID,
                                                              None)
                         self.putLog(tmpMsg)
                         rucioAPI.registerDatasetLocation(tmpDS,[tmpDQ2ID],lifetime=14,owner=None,
-                                                         activity="User Subscriptions")
+                                                         activity="Analysis Output")
                         self.putLog('OK')
                     except Exception:
                         errType,errValue = sys.exc_info()[:2]
                         tmpStr = 'Failed to send transfer request : %s %s' % (errType,errValue)
                         tmpStr.strip()
                         tmpStr += traceback.format_exc()
                         self.endWithError(tmpStr)
```

### Comparing `panda-server-0.0.50/pandaserver/dataservice/Finisher.py` & `panda-server-0.0.51/pandaserver/dataservice/Finisher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/Notifier.py` & `panda-server-0.0.51/pandaserver/dataservice/Notifier.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/ProcessLimiter.py` & `panda-server-0.0.51/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda-server-0.0.51/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/Setupper.py` & `panda-server-0.0.51/pandaserver/dataservice/Setupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/SetupperAtlasPlugin.py` & `panda-server-0.0.51/pandaserver/dataservice/SetupperAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/SetupperDummyPlugin.py` & `panda-server-0.0.51/pandaserver/dataservice/SetupperDummyPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/SetupperPluginBase.py` & `panda-server-0.0.51/pandaserver/dataservice/SetupperPluginBase.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/eventLookupClientEI.py` & `panda-server-0.0.51/pandaserver/dataservice/eventLookupClientEI.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/dataservice/forkSetupper.py` & `panda-server-0.0.51/pandaserver/dataservice/forkSetupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda-server-0.0.51/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/jobdispatcher/JobDispatcher.py` & `panda-server-0.0.51/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -956,38 +956,38 @@
               timestamp=None, timeout=60, xml='', node=None, workdir=None, cpuConsumptionTime=None,
               cpuConsumptionUnit=None, remainingSpace=None, schedulerID=None, pilotID=None, siteName=None,
               messageLevel=None, pilotLog='', metaData='', cpuConversionFactor=None, exeErrorCode=None,
               exeErrorDiag=None, pilotTiming=None, computingElement=None, startTime=None, endTime=None, nEvents=None,
               nInputFiles=None, batchID=None, attemptNr=None, jobMetrics=None, stdout='', jobSubStatus=None,
               coreCount=None, maxRSS=None, maxVMEM=None, maxSWAP=None, maxPSS=None, avgRSS=None, avgVMEM=None,
               avgSWAP=None, avgPSS=None, totRCHAR=None, totWCHAR=None, totRBYTES=None, totWBYTES=None, rateRCHAR=None,
-              rateWCHAR=None, rateRBYTES=None, rateWBYTES=None, corruptedFiles=None, meanCoreCount=None, cpu_flags=''):
+              rateWCHAR=None, rateRBYTES=None, rateWBYTES=None, corruptedFiles=None, meanCoreCount=None, cpu_architecture_level=None):
     tmpLog = LogWrapper(_logger, 'updateJob PandaID={0} PID={1}'.format(jobId, os.getpid()))
     tmpLog.debug('start')
     # get DN
     realDN = _getDN(req)
     # get FQANs
     fqans = _getFQAN(req)
     # check production role
     prodManager = _checkRole(fqans, realDN, jobDispatcher, site=siteName, hostname=req.get_remote_host())
     # check token
     validToken = _checkToken(token, jobDispatcher)
     # accept json
     acceptJson = req.acceptJson()
 
     _logger.debug("updateJob({jobId},{state},{transExitCode},{pilotErrorCode},{pilotErrorDiag},{node},{workdir},"
-                  "cpuConsumptionTime={cpuConsumptionTime},{cpuConsumptionUnit},{remainingSpace},{schedulerID},{pilotID},"
-                  "{siteName},{messageLevel},{nEvents},{nInputFiles},{cpuConversionFactor},{exeErrorCode},"
-                  "{exeErrorDiag},{pilotTiming},{computingElement},{startTime},{endTime},{batchID},"
+                  "cpuConsumptionTime={cpuConsumptionTime},{cpuConsumptionUnit},{cpu_architecture_level},{remainingSpace},"
+                  "{schedulerID},{pilotID},{siteName},{messageLevel},{nEvents},{nInputFiles},{cpuConversionFactor},"
+                  "{exeErrorCode},{exeErrorDiag},{pilotTiming},{computingElement},{startTime},{endTime},{batchID},"
                   "attemptNr:{attemptNr},jobSubStatus:{jobSubStatus},core:{coreCount},DN:{realDN},role:{prodManager},"
                   "token:{token},val:{validToken},FQAN:{fqans},maxRSS={maxRSS},maxVMEM={maxVMEM},maxSWAP={maxSWAP},"
                   "maxPSS={maxPSS},avgRSS={avgRSS},avgVMEM={avgVMEM},avgSWAP={avgSWAP},avgPSS={avgPSS},"
                   "totRCHAR={totRCHAR},totWCHAR={totWCHAR},totRBYTES={totRBYTES},totWBYTES={totWBYTES},rateRCHAR={rateRCHAR},"
-                  "rateWCHAR={rateWCHAR},rateRBYTES={rateRBYTES},rateWBYTES={rateWBYTES},meanCoreCount={meanCoreCount},"
-                  "corruptedFiles={corruptedFiles}\n==cpu_flags==\n{cpu_flags}\n==XML==\n{xml}\n==LOG==\n{pilotLog}\n==Meta==\n{metaData}\n"
+                  "rateWCHAR={rateWCHAR},rateRBYTES={rateRBYTES},rateWBYTES={rateWBYTES},meanCoreCount={meanCoreCount},"                  
+                  "corruptedFiles={corruptedFiles}\n==XML==\n{xml}\n==LOG==\n{pilotLog}\n==Meta==\n{metaData}\n"
                   "==Metrics==\n{jobMetrics}\n==stdout==\n{stdout})".format(jobId=jobId, state=state, transExitCode=transExitCode,
                                                                             pilotErrorCode=pilotErrorCode, pilotErrorDiag=pilotErrorDiag,
                                                                             node=node, workdir=workdir,
                                                                             cpuConsumptionTime=cpuConsumptionTime,
                                                                             cpuConsumptionUnit=cpuConsumptionUnit,
                                                                             remainingSpace=remainingSpace, schedulerID=schedulerID,
                                                                             pilotID=pilotID, siteName=siteName, messageLevel=messageLevel,
@@ -1000,15 +1000,15 @@
                                                                             realDN=realDN, prodManager=prodManager, token=token,
                                                                             validToken=validToken, fqans=str(fqans), maxRSS=maxRSS,
                                                                             maxVMEM=maxVMEM, maxSWAP=maxSWAP, maxPSS=maxPSS, avgRSS=avgRSS,
                                                                             avgVMEM=avgVMEM, avgSWAP=avgSWAP, avgPSS=avgPSS, totRCHAR=totRCHAR,
                                                                             totWCHAR=totWCHAR, totRBYTES=totRBYTES, totWBYTES=totWBYTES,
                                                                             rateRCHAR=rateRCHAR, rateWCHAR=rateWCHAR, rateRBYTES=rateRBYTES,
                                                                             rateWBYTES=rateWBYTES, meanCoreCount=meanCoreCount,
-                                                                            corruptedFiles=corruptedFiles, cpu_flags=cpu_flags,
+                                                                            corruptedFiles=corruptedFiles, cpu_architecture_level=cpu_architecture_level,
                                                                             xml=xml, pilotLog=pilotLog[:1024],
                                                                             metaData=metaData[:1024], jobMetrics=jobMetrics,
                                                                             stdout=stdout))
     _pilotReqLogger.debug('method=updateJob,site=%s,node=%s,type=None' % (siteName, node))
     # invalid role
     if not prodManager:
         _logger.warning("updateJob(%s) : invalid role" % jobId)
@@ -1030,14 +1030,20 @@
         return Protocol.Response(Protocol.SC_Success).encode(acceptJson)
     # create parameter map
     param = {}
     if cpuConsumptionTime not in [None, '']:
         param['cpuConsumptionTime'] = cpuConsumptionTime
     if cpuConsumptionUnit is not None:
         param['cpuConsumptionUnit'] = cpuConsumptionUnit
+    if cpu_architecture_level:
+        try:
+            param['cpu_architecture_level'] = cpu_architecture_level[:20]
+        except Exception:
+            _logger.error("invalid cpu_architecture_level=%s for updateJob" % cpu_architecture_level)
+            pass
     if node is not None:
         param['modificationHost'] = node[:128]
     if transExitCode is not None:
         try:
             int(transExitCode)
             param['transExitCode'] = transExitCode
         except Exception:
```

### Comparing `panda-server-0.0.50/pandaserver/jobdispatcher/Protocol.py` & `panda-server-0.0.51/pandaserver/jobdispatcher/Protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,21 +279,23 @@
         self.data['maxWalltime'] = job.maxWalltime
         # looping check
         if job.is_no_looping_check():
             self.data['loopingCheck'] = False
         # debug mode
         if job.specialHandling is not None and 'debug' in job.specialHandling:
             self.data['debug'] = 'True'
-        # event service or job cloning
+        # event service or job cloning or fine-grained
         if EventServiceUtils.isJobCloningJob(job):
             self.data['cloneJob'] = EventServiceUtils.getJobCloningType(job)
         elif EventServiceUtils.isEventServiceJob(job) or EventServiceUtils.isJumboJob(job):
             self.data['eventService'] = 'True'
             # prod DBlock space token for pre-merging output
             self.data['prodDBlockTokenForOutput'] = strProdTokenForOutput[:-1]
+        elif EventServiceUtils.is_fine_grained_job(job):
+            self.data['eventService'] = 'True'
         # event service merge
         if isEventServiceMerge:
             self.data['eventServiceMerge'] = 'True'
             # write to file for ES merge
             writeToFileStr = ''
             try:
                 for outputName in job.metadata[0]:
```

### Comparing `panda-server-0.0.50/pandaserver/jobdispatcher/Watcher.py` & `panda-server-0.0.51/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/proxycache/DBMSql.py` & `panda-server-0.0.51/pandaserver/proxycache/DBMSql.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/proxycache/panda_activeusers_query.py` & `panda-server-0.0.51/pandaserver/proxycache/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/proxycache/panda_proxy_cache.py` & `panda-server-0.0.51/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/server/panda.py` & `panda-server-0.0.51/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/srvcore/CoreUtils.py` & `panda-server-0.0.51/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/srvcore/MailUtils.py` & `panda-server-0.0.51/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/srvcore/oidc_utils.py` & `panda-server-0.0.51/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/srvcore/srv_msg_utils.py` & `panda-server-0.0.51/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/CloudSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/ConBridge.py` & `panda-server-0.0.51/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/DBProxyPool.py` & `panda-server-0.0.51/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/DatasetSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/DdmSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/EiDBProxy.py` & `panda-server-0.0.51/pandaserver/taskbuffer/EiDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/ErrorCode.py` & `panda-server-0.0.51/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/EventServiceUtils.py` & `panda-server-0.0.51/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 # values for job.eventService
 esJobFlagNumber = 1
 esMergeJobFlagNumber = 2
 jobCloningFlagNumber = 3
 jumboJobFlagNumber = 4
 coJumboJobFlagNumber = 5
+fineGrainedFlagNumber = 6
 
 
 # values for event.is_jumbo
 eventTableIsJumbo = 1
 
 
 # siteid for waiting co-jumbo jobs
@@ -140,59 +141,47 @@
                 newSpecialHandling += '{0},'.format(tmpItem)
         newSpecialHandling = newSpecialHandling[:-1]
     except Exception:
         newSpecialHandling = specialHandling
     return eventServiceInfo,newSpecialHandling,esIndex
 
 
-
 # check if event service job
 def isEventServiceJob(job):
-    try:
-        if job.specialHandling is not None and esToken in job.specialHandling.split(','):
-            return True
-    except Exception:
-        pass
-    return False
-
+    # fine-grained job
+    if is_fine_grained_job(job):
+        return False
+    return isEventServiceSH(job.specialHandling)
 
 
 # check if event service merge job
 def isEventServiceMerge(job):
-    try:
-        if job.specialHandling is not None and esMergeToken in job.specialHandling.split(','):
-            return True
-    except Exception:
-        pass
-    return False
-
+    return isEventServiceMergeSH(job.specialHandling)
 
 
 # check if specialHandling for event service
 def isEventServiceSH(specialHandling):
     try:
         if specialHandling is not None and esToken in specialHandling.split(','):
             return True
     except Exception:
         pass
     return False
 
 
-
 # check if specialHandling for event service merge 
 def isEventServiceMergeSH(specialHandling):
     try:
         if specialHandling is not None and esMergeToken in specialHandling.split(','):
             return True
     except Exception:
         pass
     return False
 
 
-
 # set event service merge
 def setEventServiceMerge(job):
     try:
         # set ES flag
         job.eventService = esMergeJobFlagNumber
         # set gshare to express
         job.gshare = 'Express'
@@ -379,7 +368,17 @@
     try:
         if specialHandling is not None:
             if resurrectConsumersToken in specialHandling.split(','):
                 return True
     except Exception:
         pass
     return False
+
+
+# check if fine-grained job
+def is_fine_grained_job(job):
+    return job.eventService == fineGrainedFlagNumber
+
+
+# set fine-grained
+def set_fine_grained(job):
+    job.eventService = fineGrainedFlagNumber
```

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/FileSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/FileSpec.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             return self._owner.PandaID
         # others
         ret = object.__getattribute__(self, name)
         if ret is None:
             return "NULL"
         return ret
 
-    # override __setattr__ to collecte the changed attributes
+    # override __setattr__ to collect the changed attributes
     def __setattr__(self, name, value):
         oldVal = getattr(self, name)
         object.__setattr__(self, name, value)
         newVal = getattr(self, name)
         # collect changed attributes
         if oldVal != newVal:
             self._changedAttrs[name] = value
```

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/GlobalShares.py` & `panda-server-0.0.51/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/Initializer.py` & `panda-server-0.0.51/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/JobSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/JobSpec.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                    'coreCount', 'nInputDataFiles', 'inputFileType', 'inputFileProject', 'inputFileBytes',
                    'nOutputDataFiles', 'outputFileBytes', 'jobMetrics', 'workQueue_ID', 'jediTaskID',
                    'jobSubStatus', 'actualCoreCount', 'reqID', 'maxRSS', 'maxVMEM', 'maxSWAP', 'maxPSS',
                    'avgRSS', 'avgVMEM', 'avgSWAP', 'avgPSS', 'maxWalltime', 'nucleus', 'eventService',
                    'failedAttempt', 'hs06sec', 'gshare', 'hs06', 'totRCHAR', 'totWCHAR', 'totRBYTES',
                    'totWBYTES', 'rateRCHAR', 'rateWCHAR', 'rateRBYTES', 'rateWBYTES', 'resource_type',
                    'diskIO', 'memory_leak', 'memory_leak_x2', 'container_name', 'job_label',
-                   'gco2_regional', 'gco2_global'
+                   'gco2_regional', 'gco2_global', 'cpu_architecture_level'
                    )
     # slots
     __slots__ = _attributes + ('Files', '_changedAttrs')
     # attributes which have 0 by default
     _zeroAttrs = ('assignedPriority', 'currentPriority', 'attemptNr', 'maxAttempt', 'maxCpuCount', 'maxDiskCount',
                   'minRamCount', 'cpuConsumptionTime', 'pilotErrorCode', 'exeErrorCode', 'supErrorCode', 'ddmErrorCode',
                   'brokerageErrorCode', 'jobDispatcherErrorCode', 'taskBufferErrorCode', 'nEvents', 'relocationFlag',
```

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/JobUtils.py` & `panda-server-0.0.51/pandaserver/taskbuffer/JobUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/NucleusSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/OraDBProxy.py` & `panda-server-0.0.51/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1978,14 +1978,25 @@
                             job.jobStatus = 'closed'
                             job.jobSubStatus = 'jc_unlock'
                             job.taskBufferErrorCode = ErrorCode.EC_JobCloningUnlock
                             if retJC['win'] is not None:
                                 job.taskBufferErrorDiag = 'closed since another clone PandaID={0} got semaphore'.format(retJC['win'])
                             else:
                                 job.taskBufferErrorDiag = 'closed since failed to lock semaphore'
+                elif useJEDI and EventServiceUtils.is_fine_grained_job(job):
+                    # fine-grained
+                    n_done, n_remain = self.check_fine_grained_processing(job)
+                    if n_done > 0 or n_remain == 0:
+                        job.jobStatus = 'finished'
+                        if n_remain == 0:
+                            job.jobSubStatus = 'fg_done'
+                        else:
+                            job.jobSubStatus = 'fg_partial'
+                    else:
+                        job.jobSubStatus = 'fg_stumble'
                 # release unprocessed samples for HPO
                 if job.is_hpo_workflow():
                     self.release_unprocessed_events(job.jediTaskID, job.PandaID)
                 # delete from jobsDefined/Active
                 varMap = {}
                 varMap[':PandaID'] = job.PandaID
                 if fromJobsDefined:
@@ -12580,16 +12591,17 @@
             varMap[':jediTaskID'] = jobSpec.jediTaskID
             if not (jobSpec.isCancelled() and fileSpec.isUnMergedOutput()):
                 varMap[':attemptNr']  = fileSpec.attemptNr
             # set file status
             if fileSpec.type in ['input','pseudo_input']:
                 hasInput = True
                 updateAttemptNr = True
-                if jobSpec.jobStatus == 'finished' and not jobSpec.is_hpo_workflow() \
-                        and fileSpec.status != 'skipped':
+                if ((jobSpec.jobStatus == 'finished' and not EventServiceUtils.is_fine_grained_job(jobSpec)) or
+                        (jobSpec.jobSubStatus == 'fg_done' and EventServiceUtils.is_fine_grained_job(jobSpec))) and \
+                        not jobSpec.is_hpo_workflow() and fileSpec.status != 'skipped':
                     varMap[':status'] = 'finished'
                     if fileSpec.type in ['input','pseudo_input']:
                          updateNumEvents = True
                 else:
                     # set ready for next attempt
                     varMap[':status'] = 'ready'
                     if jobSpec.jobStatus == 'failed' and not jobSpec.is_hpo_workflow():
@@ -22184,14 +22196,18 @@
         method_name = comment.split(' ')[-2].split('.')[-1]
         tmpLog = LogWrapper(_logger, '{0}-{1}'.format(method_name, queue))
         tmpLog.debug('start')
         n_cores_running = 0
         workers_queued = {}
         n_cores_queued = 0
         harvester_ids_temp = list(worker_stats)
+        
+        # HIMEM resource types group
+        HIMEM = 'HIMEM'
+        HIMEM_RTS = ['SCORE_HIMEM', 'MCORE_HIMEM']
 
         # get the configuration for maximum workers of each type
         pq_data_des = self.get_config_for_pq(queue)
         resource_type_limits = {}
         queue_type = 'production'
         if not pq_data_des:
             tmpLog.debug('Error retrieving queue configuration from DB, limits can not be applied')
@@ -22210,42 +22226,62 @@
                 cores_queue = pq_data_des['corecount']
                 if not cores_queue:
                     cores_queue = 1
             except KeyError:
                 tmpLog.error('No corecount')
                 pass
 
-        # Filter central harvester instances that support UPS model
+        # Retrieve the assigned harvester instance and submit UPS commands only to this instance. We have had multiple
+        # cases of test instances submitting to large queues in classic pull mode and not following commands.
+        try:
+            assigned_harvester_id = pq_data_des['harvester']
+        except KeyErrorException:
+            assigned_harvester_id = None
+
+        
         harvester_ids = []
-        for harvester_id in harvester_ids_temp:
-            if 'ACT' not in harvester_id and 'test_fbarreir' not in harvester_id and 'cern_cloud' not in harvester_id:
-                harvester_ids.append(harvester_id)
+        # If the assigned instance is working, use it for the statistics
+        if assigned_harvester_id in harvester_ids_temp:
+            harvester_ids = [assigned_harvester_id]
+
+        # Filter central harvester instances that support UPS model
+        else:
+            for harvester_id in harvester_ids_temp:
+                if 'ACT' not in harvester_id and 'test_fbarreir' not in harvester_id and 'cern_cloud' not in harvester_id:
+                    harvester_ids.append(harvester_id)
 
         for harvester_id in harvester_ids:
             for job_type in worker_stats[harvester_id]:
                 workers_queued.setdefault(job_type, {})
                 for resource_type in worker_stats[harvester_id][job_type]:
                     core_factor = JobUtils.translate_resourcetype_to_cores(resource_type, cores_queue)
                     try:
                         n_cores_running = n_cores_running + worker_stats[harvester_id][job_type][resource_type]['running'] * core_factor
 
+                        # This limit is in #JOBS or #WORKERS
                         if resource_type in resource_type_limits:
                             resource_type_limits[resource_type] = resource_type_limits[resource_type] - worker_stats[harvester_id][job_type][resource_type]['running']
                             tmpLog.debug('Limit for rt {0} down to {1}'.format(resource_type, resource_type_limits[resource_type]))
+                        
+                        # This limit is in #CORES, since it mixes single and multi core jobs
+                        if resource_type in HIMEM_RTS and HIMEM in resource_type_limits:
+                            resource_type_limits[HIMEM] = resource_type_limits[HIMEM] - worker_stats[harvester_id][job_type][resource_type]['running'] * core_factor
+                            tmpLog.debug('Limit for rt group {0} down to {1}'.format(HIMEM, resource_type_limits[HIMEM]))
+                            
                     except KeyError:
                         pass
 
                     try:  # submitted
                         workers_queued[job_type].setdefault(resource_type, 0)
                         workers_queued[job_type][resource_type] = workers_queued[job_type][resource_type] + worker_stats[harvester_id][job_type][resource_type]['submitted']
                         n_cores_queued = n_cores_queued + worker_stats[harvester_id][job_type][resource_type]['submitted'] * core_factor
                     except KeyError:
                         pass
 
-                    try: # ready
+                    try:  # ready
                         workers_queued[job_type].setdefault(resource_type, 0)
                         workers_queued[job_type][resource_type] = workers_queued[job_type][resource_type] + worker_stats[harvester_id][job_type][resource_type]['ready']
                         n_cores_queued = n_cores_queued + worker_stats[harvester_id][job_type][resource_type]['ready'] * core_factor
                     except KeyError:
                         pass
 
         tmpLog.debug('Queue {0} queued worker overview: {1}'.format(queue, workers_queued))
@@ -22265,15 +22301,15 @@
         n_cores_to_submit = max(n_cores_target - n_cores_queued, 5 * cores_queue)
         tmpLog.debug('IN CORES: nrunning {0}, ntarget {1}, nqueued {2}. We need to process {3} cores'
                      .format(n_cores_running, n_cores_target, n_cores_queued, n_cores_to_submit))
 
         # Get the sorted global shares
         sorted_shares = self.get_sorted_leaves()
 
-        # Run over the activated jobs by gshare&priority and substract them from the queued
+        # Run over the activated jobs by gshare & priority, and substract them from the queued
         # A negative value for queued will mean more pilots of that resource type are missing
         for share in sorted_shares:
             var_map = {':queue': queue, ':gshare': share.name}
             sql = """
                   SELECT gshare, prodsourcelabel, resource_type FROM {0}.jobsactive4
                   WHERE jobstatus = 'activated'
                      AND computingsite=:queue
@@ -22284,19 +22320,24 @@
             activated_jobs = self.cur.fetchall()
             tmpLog.debug('Processing share: {0}. Got {1} activated jobs'.format(share.name, len(activated_jobs)))
             for gshare, prodsourcelabel, resource_type in activated_jobs:
                 core_factor = JobUtils.translate_resourcetype_to_cores(resource_type, cores_queue)
 
                 # translate prodsourcelabel to a subset of job types, typically 'user' and 'managed'
                 job_type = JobUtils.translate_prodsourcelabel_to_jobtype(queue_type, prodsourcelabel)
-
                 # if we reached the limit for the resource type, skip the job
                 if resource_type in resource_type_limits and resource_type_limits[resource_type] <= 0:
                     # tmpLog.debug('Reached resource type limit for {0}'.format(resource_type))
                     continue
+                
+                # if we reached the limit for the HIMEM resource type group, skip the job
+                if resource_type in HIMEM_RTS and HIMEM in resource_type_limits and resource_type_limits[HIMEM] <= 0:
+                    # tmpLog.debug('Reached resource type limit for {0}'.format(resource_type))
+                    continue
+
                 workers_queued.setdefault(job_type, {})
                 workers_queued[job_type].setdefault(resource_type, 0)
                 workers_queued[job_type][resource_type] = workers_queued[job_type][resource_type] - 1
                 if workers_queued[job_type][resource_type] <= 0:
                     # we've gone over the jobs that already have a queued worker, now we go for new workers
                     n_cores_to_submit = n_cores_to_submit - core_factor
 
@@ -25269,7 +25310,51 @@
 
         except Exception:
             self._rollback()
             type, value, tb = sys.exc_info()
             tmp_log.error("{} {}".format(type, value))
             tmp_log.error(format(traceback.format_exc()))
             return -1, None
+
+    # check fine-grained job
+    def check_fine_grained_processing(self, job_spec):
+        comment = ' /* DBProxy.check_fine_grained_processing */'
+        methodName = comment.split(' ')[-2].split('.')[-1]
+        methodName += ' < jediTaskID={} PandaID={} >'.format(job_spec.jediTaskID, job_spec.PandaID)
+        try:
+            # get configs
+            tmpLog = LogWrapper(_logger, methodName)
+            # sql to release events
+            sqlW  = "UPDATE {0}.JEDI_Events ".format(panda_config.schemaJEDI)
+            sqlW += "SET PandaID=:jobsetID,status=:newEventStatus "
+            sqlW += "WHERE jediTaskID=:jediTaskID AND PandaID=:PandaID AND status<>:eventStatus "
+            # sql to count successful events
+            sqlC  = "SELECT COUNT(*) FROM {0}.JEDI_Events ".format(panda_config.schemaJEDI)
+            sqlC += "WHERE jediTaskID=:jediTaskID AND PandaID=:PandaID AND status=:eventStatus "
+            # sql to count remaining events
+            sqlU  = "SELECT COUNT(*) FROM {0}.JEDI_Events ".format(panda_config.schemaJEDI)
+            sqlU += "WHERE jediTaskID=:jediTaskID AND PandaID=:jobsetID "
+            # release
+            varMap = {':jediTaskID': job_spec.jediTaskID,
+                      ':PandaID': job_spec.PandaID,
+                      ':jobsetID': job_spec.jobsetID,
+                      ':eventStatus': EventServiceUtils.ST_finished,
+                      ':newEventStatus': EventServiceUtils.ST_ready}
+            self.cur.execute(sqlW + comment, varMap)
+            n_release = self.cur.rowcount
+            # count successful events
+            varMap = {':jediTaskID': job_spec.jediTaskID,
+                      ':PandaID': job_spec.PandaID,
+                      ':eventStatus': EventServiceUtils.ST_finished}
+            self.cur.execute(sqlC + comment, varMap)
+            n_done, = self.cur.fetchone()
+            # count remaining events
+            varMap = {':jediTaskID': job_spec.jediTaskID,
+                      ':jobsetID': job_spec.jobsetID}
+            self.cur.execute(sqlU + comment, varMap)
+            n_remain, = self.cur.fetchone()
+            tmpLog.debug("done={} release/remain={}/{}".format(n_done, n_release, n_remain))
+            return n_done, n_remain
+        except Exception:
+            # error
+            self.dumpErrorMessage(_logger, methodName)
+            raise RuntimeError(methodName + ' failed')
```

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/PrioUtil.py` & `panda-server-0.0.51/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/ProcessGroups.py` & `panda-server-0.0.51/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/ResourceSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/SQLDumper.py` & `panda-server-0.0.51/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/SiteSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/TaskBuffer.py` & `panda-server-0.0.51/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda-server-0.0.51/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/Utils.py` & `panda-server-0.0.51/pandaserver/taskbuffer/Utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/WorkerSpec.py` & `panda-server-0.0.51/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/WrappedCursor.py` & `panda-server-0.0.51/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/WrappedPickle.py` & `panda-server-0.0.51/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import decimal
 from io import BytesIO
 try:
     # python 2
     import cPickle as pickle
     from copy_reg import _reconstructor as map__reconstructor
 except ImportError:
     # python 3
@@ -19,14 +20,28 @@
         def __setattr__(self, key, value):
             if key == 'find_global':
                 pickle.Unpickler.__setattr__(self, 'find_class', value)
             else:
                 pickle.Unpickler.__setattr__(self, key, value)
 
 
+# conversion for unserializable values
+def conversion_func(item):
+    if isinstance(item, list):
+        return [conversion_func(i) for i in item]
+    if isinstance(item, dict):
+        return {k: conversion_func(item[k]) for k in item}
+    if isinstance(item, decimal.Decimal):
+        if item == item.to_integral_value():
+            item = int(item)
+        else:
+            item = float(item)
+    return item
+
+
 # wrapper to avoid de-serializing unsafe objects
 class WrappedPickle(object):
     # allowed modules and classes
     allowedModClass = {
         'copy_reg'            : ['_reconstructor'],
         '__builtin__'         : ['object'],
         'datetime'            : ['datetime'],
@@ -72,9 +87,11 @@
             pickle_string = pickle_string.encode()
         pickle_obj = Common_Unpickler(BytesIO(pickle_string))
         pickle_obj.find_global = cls.find_class
         return pickle_obj.load()
 
     # dumps
     @classmethod
-    def dumps(cls, obj):
+    def dumps(cls, obj, convert_to_safe=False):
+        if convert_to_safe:
+            obj = conversion_func(obj)
         return pickle.dumps(obj, protocol=0)
```

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/retryModule.py` & `panda-server-0.0.51/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/taskbuffer/workflow_processor.py` & `panda-server-0.0.51/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/SchemaChecker.py` & `panda-server-0.0.51/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda-server-0.0.51/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda-server-0.0.51/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/banUser.py` & `panda-server-0.0.51/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/boostPrio.py` & `panda-server-0.0.51/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/boostUser.py` & `panda-server-0.0.51/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/callbackDDM.py` & `panda-server-0.0.51/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/finishJob.py` & `panda-server-0.0.51/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/frontier_retagging.py` & `panda-server-0.0.51/pandaserver/test/frontier_retagging.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/getJobs.py` & `panda-server-0.0.51/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/killJob.py` & `panda-server-0.0.51/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/killJobLowPrio.py` & `panda-server-0.0.51/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/killJobsInTask.py` & `panda-server-0.0.51/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/killProdJobs.py` & `panda-server-0.0.51/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/killTask.py` & `panda-server-0.0.51/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/killUser.py` & `panda-server-0.0.51/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/lsst/lsstSubmit.py` & `panda-server-0.0.51/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda-server-0.0.51/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda-server-0.0.51/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/reassignSite.py` & `panda-server-0.0.51/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/reassignTask.py` & `panda-server-0.0.51/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/reassignWaiting.py` & `panda-server-0.0.51/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/reloadInputDS.py` & `panda-server-0.0.51/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/sendCommandToJob.py` & `panda-server-0.0.51/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/setDebugMode.py` & `panda-server-0.0.51/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/setPriority.py` & `panda-server-0.0.51/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testEvgen.py` & `panda-server-0.0.51/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testEvgen17.py` & `panda-server-0.0.51/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testG4sim.py` & `panda-server-0.0.51/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testG4sim17.py` & `panda-server-0.0.51/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda-server-0.0.51/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testGlobalShares.py` & `panda-server-0.0.51/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testJobFlowATLAS.py` & `panda-server-0.0.51/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testReco.py` & `panda-server-0.0.51/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testSimulReco14.py` & `panda-server-0.0.51/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testSiteMap.py` & `panda-server-0.0.51/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/test/testutils.py` & `panda-server-0.0.51/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/userinterface/Client.py` & `panda-server-0.0.51/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/userinterface/UserIF.py` & `panda-server-0.0.51/pandaserver/userinterface/UserIF.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
     # get job statistics per site
     def getJobStatisticsPerSite(self,predefined=False,workingGroup='',countryGroup='',jobType='',
                                 minPriority=None,readArchived=True):
         # get job statistics
         ret = self.taskBuffer.getJobStatistics(readArchived,predefined,workingGroup,countryGroup,jobType,
                                                minPriority=minPriority)
         # serialize
-        return WrappedPickle.dumps(ret)
+        return WrappedPickle.dumps(ret, convert_to_safe=True)
 
 
     # get job statistics per site and resource
     def getJobStatisticsPerSiteResource(self, timeWindow):
         # get job statistics
         ret = self.taskBuffer.getJobStatisticsPerSiteResource(timeWindow)
         # serialize
```

### Comparing `panda-server-0.0.50/pandaserver/workflow/pcwl_test.py` & `panda-server-0.0.51/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/workflow/pcwl_utils.py` & `panda-server-0.0.51/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/workflow/psnakemake_test.py` & `panda-server-0.0.51/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/workflow/snakeparser/extensions.py` & `panda-server-0.0.51/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/workflow/snakeparser/log.py` & `panda-server-0.0.51/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/workflow/snakeparser/parser.py` & `panda-server-0.0.51/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/workflow/snakeparser/utils.py` & `panda-server-0.0.51/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/pandaserver/workflow/workflow_utils.py` & `panda-server-0.0.51/pandaserver/workflow/workflow_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
     # short description
     def short_desc(self):
         return "ID:{} Name:{} Type:{}".format(self.id, self.name, self.type)
 
     # resolve workload-specific parameters
     def resolve_params(self, task_template=None, id_map=None, workflow=None):
-        if self.type == 'prun':
+        if self.type in ['prun', 'junction', 'reana']:
             dict_inputs = self.convert_dict_inputs()
             if 'opt_secondaryDSs' in dict_inputs:
                 # look for secondaryDsTypes if missing
                 if 'opt_secondaryDsTypes' not in dict_inputs:
                     dict_inputs['opt_secondaryDsTypes'] = []
                     for ds_name in dict_inputs['opt_secondaryDSs']:
                         for pid in self.parents:
```

### Comparing `panda-server-0.0.50/setup.py` & `panda-server-0.0.51/setup.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/conda_meta.yaml.template` & `panda-server-0.0.51/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/init.d/panda_daemon.exe.template` & `panda-server-0.0.51/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/init.d/panda_httpd.exe.template` & `panda-server-0.0.51/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/init.d/panda_server.exe.template` & `panda-server-0.0.51/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/logrotate.d/panda_server.logrotate.template` & `panda-server-0.0.51/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda-server-0.0.51/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/panda_server-httpd.conf.rpmnew.template` & `panda-server-0.0.51/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/panda_server-makeSlsXml.exe.template` & `panda-server-0.0.51/templates/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/panda_server-vomsrenew.exe.template` & `panda-server-0.0.51/templates/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/panda_server.cfg.rpmnew.template` & `panda-server-0.0.51/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/pandasrv.cron.template` & `panda-server-0.0.51/templates/pandasrv.cron.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.50/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda-server-0.0.51/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files identical despite different names*

