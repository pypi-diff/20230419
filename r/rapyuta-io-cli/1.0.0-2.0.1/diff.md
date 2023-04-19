# Comparing `tmp/rapyuta-io-cli-1.0.0.tar.gz` & `tmp/rapyuta-io-cli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta-io-cli-1.0.0.tar", last modified: Tue Feb  7 11:52:41 2023, max compression
+gzip compressed data, was "rapyuta-io-cli-2.0.1.tar", last modified: Wed Apr 19 11:05:21 2023, max compression
```

## Comparing `rapyuta-io-cli-1.0.0.tar` & `rapyuta-io-cli-2.0.1.tar`

### file list

```diff
@@ -1,202 +1,222 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.972673 rapyuta-io-cli-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-02-07 11:52:41.972673 rapyuta-io-cli-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4517 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-07 11:52:41.000000 rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/apply/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)    15249 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/resolver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/template.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/apply/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/auth/
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/staging.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/build/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/import_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/trigger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    39586 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/build/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/chart/
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     2899 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/search.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/chart/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/completion/
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.956673 rapyuta-io-cli-1.0.0/riocli/config/
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/deployment/
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    12936 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/model.py
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    88023 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/deployment/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/device/
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     6340 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/label.py
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/metric.py
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/onboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/device/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/device_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/forward.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/rapyuta_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/scp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    22851 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/device/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/disk/
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    12046 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/disk/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.960673 rapyuta-io-cli-1.0.0/riocli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/managedservice/
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/list_providers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3977 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    11814 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/managedservice/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/marketplace/
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3365 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/marketplace/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/model/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/network/
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4450 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/native_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/routed_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    21111 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/network/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/package/
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     9327 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/util.py
--rw-r--r--   0 runner    (1001) docker     (122)   159487 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/package/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.964673 rapyuta-io-cli-1.0.0/riocli/parameter/
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/upload.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/parameter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/project/
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    18238 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/project/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/rosbag/
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/rosbag/blob.py
--rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/rosbag/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/rosbag/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/secret/
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/docker_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/import_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2822 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/source_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    32016 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/secret/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/shell/
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/shell/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/static_route/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/open.py
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     8849 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/static_route/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/usergroup/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/usergroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/usergroup/list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 11:52:41.968673 rapyuta-io-cli-1.0.0/riocli/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3342 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/selector.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/riocli/utils/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-07 11:52:41.972673 rapyuta-io-cli-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-02-07 11:52:31.000000 rapyuta-io-cli-1.0.0/setup.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)    11357 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/LICENSE
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2736 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/PKG-INFO
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2453 2023-04-04 05:52:38.000000 rapyuta-io-cli-2.0.1/README.md
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.171484 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2736 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     5457 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)        1 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)       45 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      438 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/requires.txt
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)        7 2023-04-19 11:05:21.000000 rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/top_level.txt
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.171484 rapyuta-io-cli-2.0.1/riocli/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      728 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      675 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/__main__.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.171484 rapyuta-io-cli-2.0.1/riocli/apply/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3798 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/apply/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1446 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/explain.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/apply/manifests/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      451 2022-12-20 12:13:39.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/04-build-catkin.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      524 2022-12-20 12:13:39.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/05-build-docker.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      348 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/06-build-docker-ros.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      206 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/07-device-preinstalled.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      194 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/08-device-docker.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      895 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/09-cloud-routed-network.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      246 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/10-device-routed-network.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      212 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/11-cloud-native-network.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      246 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/12-device-native-network.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      696 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/13-device-package-with-rosbag.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      910 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/14-cloud-package-with-rosbag.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      530 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/15-device-deployment-no-override-options.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      773 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/16-device-deployment-with-override-options.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      582 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/17-device-deployment-with-on-demand-options.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      915 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/deployment.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      273 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/device-with-both-runtimes.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      121 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/disk.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      171 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/managedservice.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1188 2023-04-10 10:43:41.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/package.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      133 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/project.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      802 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/secret.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      102 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/manifests/static-route.yaml
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)    15225 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/apply/parse.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     8142 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/apply/resolver.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1697 2022-12-20 12:13:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/template.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1938 2022-12-20 12:13:40.000000 rapyuta-io-cli-2.0.1/riocli/apply/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/auth/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1386 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/auth/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2524 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/auth/login.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1015 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/auth/logout.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1130 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/auth/refresh_token.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2567 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/auth/staging.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      911 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/auth/status.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1320 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/auth/token.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2309 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/auth/util.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2723 2023-04-19 11:03:19.000000 rapyuta-io-cli-2.0.1/riocli/bootstrap.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/build/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1415 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/build/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3513 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/create.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1394 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3644 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/import_build.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     4889 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1767 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1807 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/logs.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3191 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/build/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1667 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/build/trigger.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1884 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/build/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/chart/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1295 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2342 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/apply.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3182 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/chart.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2138 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1069 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/info.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1328 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1208 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/search.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2303 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/chart/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/completion/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1361 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/completion/__init__.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.175485 rapyuta-io-cli-2.0.1/riocli/config/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1100 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/config/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3519 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/config/config.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/deployment/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1544 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/deployment/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1487 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     4423 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/deployment/errors.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2820 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2278 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2352 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/logs.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)    14700 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/deployment/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      887 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/deployment/run.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2495 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/ssh.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1113 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/deployment/status.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     5648 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/deployment/util.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1821 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/deployment/wait.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/device/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1903 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/device/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     4447 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/config.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2824 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/create.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1404 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1645 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/device/deployment.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1313 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/execute.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     6340 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/files.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1585 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     4083 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/label.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1407 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3301 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/metric.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2739 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/device/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1268 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/device/onboard.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/device/tools/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1313 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2517 2023-04-16 11:13:46.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/device_init.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1626 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/forward.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1461 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/rapyuta_logs.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1735 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/scp.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3281 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/service.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3141 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/ssh.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2669 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/tools/util.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3736 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/topic.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3878 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/device/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/disk/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1101 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/disk/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1553 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/disk/create.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1414 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/disk/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1414 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/disk/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3100 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/disk/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2821 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/disk/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/exceptions/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      892 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/exceptions/__init__.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/managedservice/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1326 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1283 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1398 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1316 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/list_providers.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2037 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3977 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/managedservice/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.179484 rapyuta-io-cli-2.0.1/riocli/marketplace/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1172 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1569 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     4032 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/install.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1597 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3365 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/marketplace/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/model/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)       36 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/model/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     5810 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/model/base.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/network/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1296 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/network/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2086 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/network/create.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1916 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1500 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2430 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1959 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/logs.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     4062 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/network/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2676 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/network/native_network.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3184 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/network/routed_network.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     6168 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/network/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/package/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1332 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/package/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1472 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/package/create.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1554 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/package/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1390 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/package/deployment.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2347 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/package/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2447 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/package/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     9441 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/package/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2204 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/package/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/parameter/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1628 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2969 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/parameter/apply.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1483 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3560 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/diff.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2151 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/download.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1187 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2076 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/upload.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2587 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/parameter/utils.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/project/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1296 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1642 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/create.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1413 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2076 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1806 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1814 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/project/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1231 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/project/select.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3816 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/project/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.183485 rapyuta-io-cli-2.0.1/riocli/rosbag/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1019 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/rosbag/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     4323 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/rosbag/blob.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)    11554 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/rosbag/job.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      162 2022-12-20 12:13:40.000000 rapyuta-io-cli-2.0.1/riocli/rosbag/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/secret/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1298 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/secret/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2436 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/create.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1406 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1503 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/docker_secret.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3442 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/import_secret.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1649 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1965 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3023 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/secret/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2779 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/secret/source_secret.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2031 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/secret/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/shell/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2040 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/shell/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      719 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/shell/prompt.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/static_route/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1415 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/static_route/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1148 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/static_route/create.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1478 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/static_route/delete.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1977 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/static_route/inspect.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1028 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/static_route/list.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1889 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/static_route/model.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1158 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/static_route/open.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2418 2023-02-10 09:00:02.000000 rapyuta-io-cli-2.0.1/riocli/static_route/util.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/usergroup/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)        0 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/usergroup/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)        0 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/usergroup/list.py
+drwxrwxr-x   0 pallab    (1000) pallab    (1000)        0 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/riocli/utils/
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     3381 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/utils/__init__.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)      944 2022-11-28 16:39:40.000000 rapyuta-io-cli-2.0.1/riocli/utils/context.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     2378 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/utils/execute.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1357 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/utils/mermaid.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1607 2023-04-16 12:13:07.000000 rapyuta-io-cli-2.0.1/riocli/utils/selector.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1602 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/utils/spinner.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1929 2023-04-16 11:39:39.000000 rapyuta-io-cli-2.0.1/riocli/utils/ssh_tunnel.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1094 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/riocli/utils/validate.py
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)       38 2023-04-19 11:05:21.187485 rapyuta-io-cli-2.0.1/setup.cfg
+-rw-rw-r--   0 pallab    (1000) pallab    (1000)     1627 2023-04-19 10:59:34.000000 rapyuta-io-cli-2.0.1/setup.py
```

### Comparing `rapyuta-io-cli-1.0.0/PKG-INFO` & `rapyuta-io-cli-2.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,105 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 1.0.0
+Version: 2.0.1
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
-License: UNKNOWN
-Description: # Rapyuta CLI
-        
-        Rapyuta CLI exposes features of Rapyuta.io platform on the command-line.
-        
-        The application is written in Python 3 and it is distributed through PyPI for
-        Python 3 environments.
-        
-        For Reference on directory structure please refer Please have a look at the
-        corresponding article:
-        http://gehrcke.de/2014/02/distributing-a-python-command-line-application/
-        
-        ## Install
-        
-        Rio CLI is available on PyPI index and can be installed directly by running the
-        following command.
-        
-        ``` bash
-        pip install rapyuta-io-cli
-        ```
-        
-        
-        On Unix-like systems it places the `rio` executable in the user's PATH. On
-        Windows it places the `rio.exe` in the centralized `Scripts` directory
-        which should be in the user's PATH.
-        
-        To install the CLI from source, you can use the `setup.py` script directly.
-        Clone the repository and from the root of the directory, run the following
-        command.
-        
-        ``` bash
-        python setup.py install
-        ```
-        
-        ## Getting Started
-        
-        To begin using the CLI, it must be authenticated with the Platform.
-        
-        ``` bash
-        rio auth login
-        ```
-        
-        The Email and Password can either be given through flags (for scripting
-        purposes) or interactively through the Prompts.
-        
-        NOTE: Entering password as a Flag is not recommended because it leaves the
-        Traces.
-        
-        ## Development
-        
-        Rio CLI project uses [Pipenv](https://pipenv.pypa.io/en/latest/) for
-        development. It needs to be installed to setup the development environment.
-        
-        ``` bash
-        pip install pipenv
-        ```
-        
-        Once Pipenv is installed, a Python virtual environment can be quickly
-        bootstrapped by running the following commands in the root of the repository.
-        
-        ``` bash
-        pipenv install --dev
-        ```
-        
-        This will create a virtual environment in the Pipenv's preconfigured location
-        (if one doesn't already exists). It will also install all the dependencies and
-        `riocli` package in the location.
-        
-        To run the CLI (or any command) under the context of Pipenv's virtual
-        environment, prepend the commands with `pipenv run`
-         
-        ```bash
-        pipenv run rio
-        ```
-        
-        To run the RIO CLI from the source directly, you can use `riocli` module
-        directly.
-        
-        ``` bash
-        pipenv run python -m riocli
-        ```
-        
-        New dependencies can be installed directly using `pipenv`. This modifies the
-        `Pipfile` and `Pipfile.lock`.
-        
-        ``` bash
-        pipenv install {dependency}
-        ```
-        
-        But using the `pipenv` directly doesn't sync the dependencies in the
-        `setup.py` file. For this, the project uses a utility called `pipenv-setup`
-        which allows us to sync the dependencies.
-        
-        ``` bash
-        pipenv run pipenv-setup sync
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Rapyuta CLI
+
+Rapyuta CLI exposes features of Rapyuta.io platform on the command-line.
+
+The application is written in Python 3 and it is distributed through PyPI for
+Python 3 environments.
+
+For Reference on directory structure please refer Please have a look at the
+corresponding article:
+http://gehrcke.de/2014/02/distributing-a-python-command-line-application/
+
+## Install
+
+Rio CLI is available on PyPI index and can be installed directly by running the
+following command.
+
+``` bash
+pip install rapyuta-io-cli
+```
+
+
+On Unix-like systems it places the `rio` executable in the user's PATH. On
+Windows it places the `rio.exe` in the centralized `Scripts` directory
+which should be in the user's PATH.
+
+To install the CLI from source, you can use the `setup.py` script directly.
+Clone the repository and from the root of the directory, run the following
+command.
+
+``` bash
+python setup.py install
+```
+
+## Getting Started
+
+To begin using the CLI, it must be authenticated with the Platform.
+
+``` bash
+rio auth login
+```
+
+The Email and Password can either be given through flags (for scripting
+purposes) or interactively through the Prompts.
+
+NOTE: Entering password as a Flag is not recommended because it leaves the
+Traces.
+
+## Development
+
+Rio CLI project uses [Pipenv](https://pipenv.pypa.io/en/latest/) for
+development. It needs to be installed to setup the development environment.
+
+``` bash
+pip install pipenv
+```
+
+Once Pipenv is installed, a Python virtual environment can be quickly
+bootstrapped by running the following commands in the root of the repository.
+
+``` bash
+pipenv install --dev
+```
+
+This will create a virtual environment in the Pipenv's preconfigured location
+(if one doesn't already exists). It will also install all the dependencies and
+`riocli` package in the location.
+
+To run the CLI (or any command) under the context of Pipenv's virtual
+environment, prepend the commands with `pipenv run`
+ 
+```bash
+pipenv run rio
+```
+
+To run the RIO CLI from the source directly, you can use `riocli` module
+directly.
+
+``` bash
+pipenv run python -m riocli
+```
+
+New dependencies can be installed directly using `pipenv`. This modifies the
+`Pipfile` and `Pipfile.lock`.
+
+``` bash
+pipenv install {dependency}
+```
+
+But using the `pipenv` directly doesn't sync the dependencies in the
+`setup.py` file. For this, the project uses a utility called `pipenv-setup`
+which allows us to sync the dependencies.
+
+``` bash
+pipenv run pipenv-setup sync
+```
```

### Comparing `rapyuta-io-cli-1.0.0/README.md` & `rapyuta-io-cli-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/rapyuta_io_cli.egg-info/PKG-INFO` & `rapyuta-io-cli-2.0.1/rapyuta_io_cli.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,105 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 1.0.0
+Version: 2.0.1
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
-License: UNKNOWN
-Description: # Rapyuta CLI
-        
-        Rapyuta CLI exposes features of Rapyuta.io platform on the command-line.
-        
-        The application is written in Python 3 and it is distributed through PyPI for
-        Python 3 environments.
-        
-        For Reference on directory structure please refer Please have a look at the
-        corresponding article:
-        http://gehrcke.de/2014/02/distributing-a-python-command-line-application/
-        
-        ## Install
-        
-        Rio CLI is available on PyPI index and can be installed directly by running the
-        following command.
-        
-        ``` bash
-        pip install rapyuta-io-cli
-        ```
-        
-        
-        On Unix-like systems it places the `rio` executable in the user's PATH. On
-        Windows it places the `rio.exe` in the centralized `Scripts` directory
-        which should be in the user's PATH.
-        
-        To install the CLI from source, you can use the `setup.py` script directly.
-        Clone the repository and from the root of the directory, run the following
-        command.
-        
-        ``` bash
-        python setup.py install
-        ```
-        
-        ## Getting Started
-        
-        To begin using the CLI, it must be authenticated with the Platform.
-        
-        ``` bash
-        rio auth login
-        ```
-        
-        The Email and Password can either be given through flags (for scripting
-        purposes) or interactively through the Prompts.
-        
-        NOTE: Entering password as a Flag is not recommended because it leaves the
-        Traces.
-        
-        ## Development
-        
-        Rio CLI project uses [Pipenv](https://pipenv.pypa.io/en/latest/) for
-        development. It needs to be installed to setup the development environment.
-        
-        ``` bash
-        pip install pipenv
-        ```
-        
-        Once Pipenv is installed, a Python virtual environment can be quickly
-        bootstrapped by running the following commands in the root of the repository.
-        
-        ``` bash
-        pipenv install --dev
-        ```
-        
-        This will create a virtual environment in the Pipenv's preconfigured location
-        (if one doesn't already exists). It will also install all the dependencies and
-        `riocli` package in the location.
-        
-        To run the CLI (or any command) under the context of Pipenv's virtual
-        environment, prepend the commands with `pipenv run`
-         
-        ```bash
-        pipenv run rio
-        ```
-        
-        To run the RIO CLI from the source directly, you can use `riocli` module
-        directly.
-        
-        ``` bash
-        pipenv run python -m riocli
-        ```
-        
-        New dependencies can be installed directly using `pipenv`. This modifies the
-        `Pipfile` and `Pipfile.lock`.
-        
-        ``` bash
-        pipenv install {dependency}
-        ```
-        
-        But using the `pipenv` directly doesn't sync the dependencies in the
-        `setup.py` file. For this, the project uses a utility called `pipenv-setup`
-        which allows us to sync the dependencies.
-        
-        ``` bash
-        pipenv run pipenv-setup sync
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Rapyuta CLI
+
+Rapyuta CLI exposes features of Rapyuta.io platform on the command-line.
+
+The application is written in Python 3 and it is distributed through PyPI for
+Python 3 environments.
+
+For Reference on directory structure please refer Please have a look at the
+corresponding article:
+http://gehrcke.de/2014/02/distributing-a-python-command-line-application/
+
+## Install
+
+Rio CLI is available on PyPI index and can be installed directly by running the
+following command.
+
+``` bash
+pip install rapyuta-io-cli
+```
+
+
+On Unix-like systems it places the `rio` executable in the user's PATH. On
+Windows it places the `rio.exe` in the centralized `Scripts` directory
+which should be in the user's PATH.
+
+To install the CLI from source, you can use the `setup.py` script directly.
+Clone the repository and from the root of the directory, run the following
+command.
+
+``` bash
+python setup.py install
+```
+
+## Getting Started
+
+To begin using the CLI, it must be authenticated with the Platform.
+
+``` bash
+rio auth login
+```
+
+The Email and Password can either be given through flags (for scripting
+purposes) or interactively through the Prompts.
+
+NOTE: Entering password as a Flag is not recommended because it leaves the
+Traces.
+
+## Development
+
+Rio CLI project uses [Pipenv](https://pipenv.pypa.io/en/latest/) for
+development. It needs to be installed to setup the development environment.
+
+``` bash
+pip install pipenv
+```
+
+Once Pipenv is installed, a Python virtual environment can be quickly
+bootstrapped by running the following commands in the root of the repository.
+
+``` bash
+pipenv install --dev
+```
+
+This will create a virtual environment in the Pipenv's preconfigured location
+(if one doesn't already exists). It will also install all the dependencies and
+`riocli` package in the location.
+
+To run the CLI (or any command) under the context of Pipenv's virtual
+environment, prepend the commands with `pipenv run`
+ 
+```bash
+pipenv run rio
+```
+
+To run the RIO CLI from the source directly, you can use `riocli` module
+directly.
+
+``` bash
+pipenv run python -m riocli
+```
+
+New dependencies can be installed directly using `pipenv`. This modifies the
+`Pipfile` and `Pipfile.lock`.
+
+``` bash
+pipenv install {dependency}
+```
+
+But using the `pipenv` directly doesn't sync the dependencies in the
+`setup.py` file. For this, the project uses a utility called `pipenv-setup`
+which allows us to sync the dependencies.
+
+``` bash
+pipenv run pipenv-setup sync
+```
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/__main__.py` & `rapyuta-io-cli-2.0.1/riocli/__main__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/apply/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     click.secho("----- Files Processed ----", fg="yellow")
     for file in glob_files:
         click.secho(file, fg="yellow")
 
     rc = Applier(glob_files, abs_values, abs_secrets)
     rc.parse_dependencies()
 
-    if not silent:
+    if not silent and not dryrun:
         click.confirm("Do you want to proceed?", default=True, abort=True)
 
     rc.apply(dryrun=dryrun, workers=workers)
 
 
 @click.command(
     'delete',
@@ -86,11 +86,11 @@
     if len(glob_files) == 0:
         click.secho('no files specified', fg='red')
         raise SystemExit(1)
 
     rc = Applier(glob_files, abs_values, abs_secrets)
     rc.parse_dependencies(check_missing=False, delete=True)
 
-    if not silent:
+    if not silent and not dryrun:
         click.confirm("Do you want to proceed?", default=True, abort=True)
 
     rc.delete(dryrun=dryrun)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/explain.py` & `rapyuta-io-cli-2.0.1/riocli/apply/explain.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/parse.py` & `rapyuta-io-cli-2.0.1/riocli/apply/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,46 +85,48 @@
                                 or self.DEFAULT_MAX_WORKERS)
         if kwargs['workers'] == 1:
             return self.apply_sync(*args, **kwargs)
 
         return self.apply_async(*args, **kwargs)
 
     def apply_async(self, *args, **kwargs):
-        WORKERS = int(kwargs.get('workers') or self.DEFAULT_MAX_WORKERS)
+        workers = int(kwargs.get('workers') or self.DEFAULT_MAX_WORKERS)
         task_queue = queue.Queue()
         done_queue = queue.Queue()
 
         def worker():
             while True:
-                obj = task_queue.get()
-                if obj in self.resolved_objects and 'manifest' in self.resolved_objects[obj]:
-                    # click.secho("obj {} is being aplied".format(obj))
+                o = task_queue.get()
+                if o in self.resolved_objects and 'manifest' in self.resolved_objects[o]:
                     try:
-                        self._apply_manifest(obj, *args, **kwargs)
+                        self._apply_manifest(o, *args, **kwargs)
                     except Exception as ex:
                         click.secho(
-                            '[Err] Object "{}" apply failed. Apply will not progress further.'.format(obj, str(ex)))
-                        raise ex
+                            '[Err] Object "{}" apply failed. Apply will not progress further.'.format(o, str(ex)))
+                        done_queue.put(ex)
+                        continue
 
                 task_queue.task_done()
-                done_queue.put(obj)
+                done_queue.put(o)
 
         worker_list = []
-        for worker_id in range(0, WORKERS):
+        for worker_id in range(workers):
             worker_list.append(threading.Thread(target=worker, daemon=True))
             worker_list[worker_id].start()
 
         self.graph.prepare()
         while self.graph.is_active():
             for obj in self.graph.get_ready():
-                # if obj in self.resolved_objects and 'manifest' in self.resolved_objects[obj]:
                 task_queue.put(obj)
 
             done_obj = done_queue.get()
-            self.graph.done(done_obj)
+            if not isinstance(done_obj, Exception):
+                self.graph.done(done_obj)
+            else:
+                raise Exception(done_obj)
 
         task_queue.join()
 
     def apply_sync(self, *args, **kwargs):
         self.graph.prepare()
         while self.graph.is_active():
             for obj in self.graph.get_ready():
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/resolver.py` & `rapyuta-io-cli-2.0.1/riocli/apply/resolver.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/template.py` & `rapyuta-io-cli-2.0.1/riocli/apply/template.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/apply/util.py` & `rapyuta-io-cli-2.0.1/riocli/apply/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/login.py` & `rapyuta-io-cli-2.0.1/riocli/auth/login.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/logout.py` & `rapyuta-io-cli-2.0.1/riocli/auth/logout.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/refresh_token.py` & `rapyuta-io-cli-2.0.1/riocli/auth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/staging.py` & `rapyuta-io-cli-2.0.1/riocli/auth/staging.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/status.py` & `rapyuta-io-cli-2.0.1/riocli/auth/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/token.py` & `rapyuta-io-cli-2.0.1/riocli/auth/token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/auth/util.py` & `rapyuta-io-cli-2.0.1/riocli/auth/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/bootstrap.py` & `rapyuta-io-cli-2.0.1/riocli/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.0.0"
+__version__ = "2.0.1"
 
 import click
 import rapyuta_io.version
 from click import Context
 from click_help_colors import HelpColorsGroup
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/build/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/create.py` & `rapyuta-io-cli-2.0.1/riocli/build/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/delete.py` & `rapyuta-io-cli-2.0.1/riocli/build/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/import_build.py` & `rapyuta-io-cli-2.0.1/riocli/build/import_build.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/build/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/list.py` & `rapyuta-io-cli-2.0.1/riocli/build/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/logs.py` & `rapyuta-io-cli-2.0.1/riocli/build/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/model.py` & `rapyuta-io-cli-2.0.1/riocli/build/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 from rapyuta_io import Build as v1Build, Client, BuildOptions, CatkinOption
 
-from riocli.build.validation import validate
 from riocli.model import Model
+from riocli.utils.validate import validate_manifest, load_schema
 
 
 class Build(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
-        guid, obj = self.rc.find_depends({"kind": "build", "nameOrGUID": self.metadata.name})
+        guid, obj = self.rc.find_depends(
+            {"kind": "build", "nameOrGUID": self.metadata.name})
         if not guid:
             return False
 
         return obj
 
     def create_object(self, client: Client) -> v1Build:
         build = client.create_build(build=self.to_v1())
@@ -65,9 +66,13 @@
         )
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
-    def validate(data) -> None:
-        validate(data)
+    def validate(data):
+        """
+        Validates if build data is matching with its corresponding schema
+        """
+        schema = load_schema('build')
+        validate_manifest(instance=data, schema=schema)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/trigger.py` & `rapyuta-io-cli-2.0.1/riocli/build/trigger.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/build/util.py` & `rapyuta-io-cli-2.0.1/riocli/build/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/chart/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
 from riocli.chart.apply import apply_chart
 from riocli.chart.delete import delete_chart
-from riocli.chart.search import list_charts, search_chart, info_chart
+from riocli.chart.info import info_chart
+from riocli.chart.list import list_charts
+from riocli.chart.search import search_chart
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
     help_headers_color='yellow',
     help_options_color='green',
 )
 def chart() -> None:
     """
-    Rapyuta Charts is a way to package the complete Application for Rapyuta.io Platform.
+    Rapyuta Charts is a way to package the complete Application for
+    Rapyuta.io Platform.
     """
     pass
 
 
 chart.add_command(search_chart)
 chart.add_command(info_chart)
 chart.add_command(apply_chart)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/apply.py` & `rapyuta-io-cli-2.0.1/riocli/chart/apply.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,22 +22,41 @@
 @click.command(
     'apply',
     cls=HelpColorsCommand,
     help_headers_color='yellow',
     help_options_color='green',
     help='Apply a new Rapyuta Chart in the Project',
 )
-@click.option('--dryrun', '-d', is_flag=True, default=False, help='dry run the yaml files without applying any change')
+@click.option('--dryrun', '-d', is_flag=True, default=False,
+              help='dry run the yaml files without applying any change')
+@click.option('-f', '--force', '--silent', 'silent', is_flag=True,
+              type=click.BOOL, default=False,
+              help="Skip confirmation")
 @click.option('--values', '-v',
-              help="path to values yaml file. key/values specified in the values file can be used as variables in template yamls")
+              help="Path to values yaml file. key/values specified in the "
+                   "values file can be used as variables in template yamls")
 @click.option('--secrets', '-s',
-              help="secret files are sops encoded value files. rio-cli expects sops to be authorized for decoding files on this computer")
-@click.option('--workers', '-w', help="number of parallel workers while running apply command. defaults to 6.")
+              help="Secret files are sops encoded value files. rio-cli "
+                   "expects sops to be authorized for decoding files on "
+                   "this computer")
+@click.option('--workers', '-w',
+              help="number of parallel workers while running apply command. "
+                   "defaults to 6.")
 @click.argument('chart', type=str)
-def apply_chart(chart: str, values: str, secrets: str, dryrun: bool, workers: int = 6) -> None:
+def apply_chart(
+        chart: str,
+        values: str,
+        secrets: str,
+        dryrun: bool,
+        workers: int = 6,
+        silent: bool = False) -> None:
+    """Install a chart from the rapyuta-charts repository."""
     versions = find_chart(chart)
     if len(versions) > 1:
-        click.secho('More than one charts are available, please specify the version!', fg='red')
+        click.secho(
+            'More than one charts are available, please specify the version!',
+            fg='red')
 
     chart = Chart(**versions[0])
-    chart.apply_chart(values, secrets, dryrun, workers)
+    chart.apply_chart(values, secrets, dryrun=dryrun, workers=workers,
+                      silent=silent)
     chart.cleanup()
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/chart.py` & `rapyuta-io-cli-2.0.1/riocli/chart/chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,54 +24,69 @@
 
 class Chart(Munch):
     def __init__(self, *args, **kwargs):
         super(Chart, self).__init__(*args, **kwargs)
         self.tmp_dir = None
         self.downloaded = False
 
-    def apply_chart(self, values: str = None, secrets: str = None, dryrun: bool = None, workers: int = 6):
+    def apply_chart(
+            self,
+            values: str = None,
+            secrets: str = None,
+            dryrun: bool = None,
+            workers: int = 6,
+            silent: bool = False):
         if not self.downloaded:
             self.download_chart()
 
         templates_dir = Path(self.tmp_dir.name, self.name, 'templates')
         if not values:
-            values = Path(self.tmp_dir.name, self.name, 'values.yaml').as_posix()
+            values = Path(self.tmp_dir.name, self.name,
+                          'values.yaml').as_posix()
 
-        apply.callback(values=values, files=[templates_dir], secrets=secrets, dryrun=dryrun, workers=workers)
+        apply.callback(values=values, files=[templates_dir], secrets=secrets,
+                       dryrun=dryrun, workers=workers, silent=silent)
 
-    def delete_chart(self, values: str = None, secrets: str = None, dryrun: bool = None):
+    def delete_chart(
+            self,
+            values: str = None,
+            secrets: str = None,
+            dryrun: bool = None,
+            silent: bool = False):
         if not self.downloaded:
             self.download_chart()
 
         templates_dir = Path(self.tmp_dir.name, self.name, 'templates')
         if not values:
-            values = Path(self.tmp_dir.name, self.name, 'values.yaml').as_posix()
+            values = Path(self.tmp_dir.name, self.name,
+                          'values.yaml').as_posix()
 
-        delete.callback(values=values, files=[templates_dir], secrets=secrets, dryrun=dryrun)
+        delete.callback(values=values, files=[templates_dir], secrets=secrets,
+                        dryrun=dryrun, silent=silent)
 
     def download_chart(self):
         self._create_temp_directory()
-        click.secho('Downloading {}:{} chart in {}'.format(self.name, self.version, self.tmp_dir.name), fg='yellow')
+        click.secho('Downloading {}:{} chart in {}'.format(
+            self.name, self.version, self.tmp_dir.name), fg='cyan')
         chart_filepath = Path(self.tmp_dir.name, self._chart_filename())
 
         with open(chart_filepath, 'wb') as f:
             resp = requests.get(self.urls[0])
             f.write(resp.content)
 
         self.extract_chart()
         self.downloaded = True
 
     def extract_chart(self):
         try:
             chart_filepath = Path(self.tmp_dir.name, self._chart_filename())
-            chart_tarball = tarfile.open(chart_filepath)
-            chart_tarball.extractall(path=self.tmp_dir.name)
-        finally:
-            if chart_tarball:
-                chart_tarball.close()
+            with tarfile.open(chart_filepath) as tarball:
+                tarball.extractall(path=self.tmp_dir.name)
+        except Exception as e:
+            raise e
 
     def cleanup(self):
         if self.tmp_dir:
             self.tmp_dir.cleanup()
 
     def _chart_filename(self):
         return self.urls[0].split('/')[-1]
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/delete.py` & `rapyuta-io-cli-2.0.1/riocli/chart/search.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,32 +7,28 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 import click
 from click_help_colors import HelpColorsCommand
 
-from riocli.chart.chart import Chart
-from riocli.chart.util import find_chart
+from riocli.chart.util import find_chart, print_chart_entries
 
 
 @click.command(
-    'delete',
+    'search',
     cls=HelpColorsCommand,
     help_headers_color='yellow',
     help_options_color='green',
-    help='Delete the Rapyuta Chart from the Project',
+    help='Search for available charts in the repository',
 )
-@click.option('--values')
-@click.option('--dryrun', '-d', is_flag=True, default=False, help='Perform dry-run for applying the chart')
+@click.option('-w', '--wide', is_flag=True, default=False,
+              help='Print more details')
 @click.argument('chart', type=str)
-def delete_chart(chart: str, values: str, dryrun: bool) -> None:
+def search_chart(chart: str, wide: bool = False) -> None:
+    """Search for a chart in the chart repo."""
     versions = find_chart(chart)
-    if len(versions) > 1:
-        click.secho('More than one charts are available, please specify the version!', fg='red')
-
-    chart = Chart(**versions[0])
-    chart.delete_chart(values, dryrun)
-    chart.cleanup()
+    print_chart_entries(versions, wide=wide)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/search.py` & `rapyuta-io-cli-2.0.1/riocli/chart/list.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,69 +7,34 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import typing
 
 import click
 from click_help_colors import HelpColorsCommand
 from munch import munchify
-from yaml import safe_dump_all
 
-from riocli.chart.util import find_chart, fetch_index
-from riocli.utils import tabulate_data
-
-
-@click.command(
-    'info',
-    cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
-    help='Describe the available chart with versions',
-)
-@click.argument('chart', type=str)
-def info_chart(chart: str) -> None:
-    versions = find_chart(chart)
-    click.echo(safe_dump_all(versions))
-
-
-@click.command(
-    'search',
-    cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
-    help='Search for available charts in the repository',
-)
-@click.argument('chart', type=str)
-def search_chart(chart: str) -> None:
-    versions = find_chart(chart)
-    _display_entries(versions)
+from riocli.chart.util import fetch_index, print_chart_entries
 
 
 @click.command(
     'list',
     cls=HelpColorsCommand,
     help_headers_color='yellow',
     help_options_color='green',
 )
-def list_charts() -> None:
+@click.option('-w', '--wide', is_flag=True, default=False,
+              help='Print more details')
+def list_charts(wide: bool = False) -> None:
+    """List all available charts."""
     index = fetch_index()
     if 'entries' not in index:
         raise Exception('No entries found!')
     entries = []
     for name, chart in index['entries'].items():
         for version in chart:
             entries.append(version)
 
-    _display_entries(munchify(entries))
-
-
-def _display_entries(entries: typing.List) -> None:
-    headers = ['Name', 'Version', 'Created At', 'Description']
-
-    data = [[e.get('name'), e.get('version'), e.get('created'), e.get('description')]
-            for e in entries]
-
-    tabulate_data(data, headers)
+    print_chart_entries(munchify(entries), wide=wide)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/chart/util.py` & `rapyuta-io-cli-2.0.1/riocli/chart/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import typing
 
 import requests
 from yaml import safe_load
 
-DEFAULT_REPOSITORY = 'https://rapyuta-robotics.github.io/rapyuta-charts/incubator/index.yaml'
+from riocli.utils import tabulate_data
+
+DEFAULT_REPOSITORY = 'https://rapyuta-robotics.github.io/rapyuta-charts/incubator/index.yaml'  # noqa
 
 
 def find_chart(chart: str) -> typing.List:
+    """Finds a chart in the upstream index."""
     chart, ver = parse_chart(chart)
 
     index = fetch_index()
     if 'entries' not in index:
         raise Exception('No entries found!')
 
     if chart not in index['entries']:
@@ -20,14 +23,15 @@
     if ver:
         versions = _find_version(entries=versions, version=ver)
 
     return versions
 
 
 def fetch_index(repository=DEFAULT_REPOSITORY) -> typing.Dict:
+    """Fetches the upstream chart index."""
     response = requests.get(repository)
     if not response.ok:
         raise Exception('Fetching index failed: %s'.format(repository))
 
     index = safe_load(response.text)
     return index
 
@@ -57,7 +61,26 @@
     return chart, ver
 
 
 def _find_version(entries: typing.List, version: str):
     for entry in entries:
         if entry.get('version') == version:
             return [entry]
+
+
+def print_chart_entries(entries: typing.List, wide: bool = False) -> None:
+    """Prints charts in a tabular format."""
+    entries = sorted(entries, key=lambda x: x.get('name').lower())
+
+    headers = ['Name', 'Version', 'Created At']
+    if wide:
+        headers.append('Description')
+
+    data = []
+    for entry in entries:
+        row = [entry.get('name'), entry.get('version'), entry.get('created')]
+        if wide:
+            row.append(entry.get('description'))
+
+        data.append(row)
+
+    tabulate_data(data, headers)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/completion/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/config/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/config/config.py` & `rapyuta-io-cli-2.0.1/riocli/config/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/delete.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/list.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/logs.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/model.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,36 +13,41 @@
 # limitations under the License.
 import os
 import typing
 
 import click
 from rapyuta_io import Client
 from rapyuta_io.clients.catalog_client import Package
+from rapyuta_io.clients.deployment import DeploymentNotRunningException
 from rapyuta_io.clients.native_network import NativeNetwork
-from rapyuta_io.clients.package import ProvisionConfiguration, RestartPolicy, ExecutableMount
-from rapyuta_io.clients.rosbag import ROSBagJob, ROSBagOptions, ROSBagCompression, UploadOptions, \
-    ROSBagOnDemandUploadOptions, ROSBagTimeRange, ROSBagUploadTypes, OverrideOptions, TopicOverrideInfo
+from rapyuta_io.clients.package import ProvisionConfiguration, RestartPolicy, \
+    ExecutableMount
+from rapyuta_io.clients.rosbag import ROSBagJob, ROSBagOptions, \
+    ROSBagCompression, UploadOptions, \
+    ROSBagOnDemandUploadOptions, ROSBagTimeRange, ROSBagUploadTypes, \
+    OverrideOptions, TopicOverrideInfo
 from rapyuta_io.clients.routed_network import RoutedNetwork
 
+from riocli.deployment.errors import ERRORS
 from riocli.deployment.util import add_mount_volume_provision_config
-from riocli.deployment.validation import validate
 from riocli.model import Model
 from riocli.package.util import find_package_guid
 from riocli.static_route.util import find_static_route_guid
+from riocli.utils.validate import validate_manifest, load_schema
 
 
 class Deployment(Model):
     RESTART_POLICY = {
         'always': RestartPolicy.Always,
         'never': RestartPolicy.Never,
         'onfailure': RestartPolicy.OnFailure
     }
 
     def find_object(self, client: Client) -> typing.Any:
-        guid, obj = self.rc.find_depends({"kind": "deployment", "nameOrGUID": self.metadata.name})
+        guid, obj = self.rc.find_depends({'kind': 'deployment', 'nameOrGUID': self.metadata.name})
         if not guid:
             return False
 
         return obj
 
     def create_object(self, client: Client) -> typing.Any:
         pkg_guid, pkg = self.rc.find_depends(self.metadata.depends, self.metadata.depends.version)
@@ -55,18 +60,18 @@
         internal_component = default_plan['internalComponents'][0]
 
         __planId = default_plan['planId']
         __componentName = internal_component.componentName
         runtime = internal_component['runtime']
 
         if 'runtime' in self.spec and runtime != self.spec.runtime:
-            click.secho('>> runtime mismatch => ' + \
+            click.secho('>> runtime mismatch => ' +
                         'deployment:{}.runtime !== package:{}.runtime '.format(
                             self.metadata.name, pkg['packageName']
-                        ), fg="red"
+                        ), fg='red'
                         )
             return
 
         provision_config = pkg.get_provision_configuration(__planId)
 
         # add label
         if 'labels' in self.metadata:
@@ -88,19 +93,19 @@
 
         # Add Network
         if 'rosNetworks' in self.spec:
             for network_depends in self.spec.rosNetworks:
                 network_guid, network_obj = self.rc.find_depends(network_depends.depends)
 
                 if type(network_obj) == RoutedNetwork:
-                    provision_config.add_routed_network(network_obj,
-                                                        network_interface=network_depends.get('interface', None))
+                    provision_config.add_routed_network(
+                        network_obj, network_interface=network_depends.get('interface', None))
                 if type(network_obj) == NativeNetwork:
-                    provision_config.add_native_network(network_obj,
-                                                        network_interface=network_depends.get('interface', None))
+                    provision_config.add_native_network(
+                        network_obj, network_interface=network_depends.get('interface', None))
 
         if 'rosBagJobs' in self.spec:
             for req_job in self.spec.rosBagJobs:
                 provision_config.add_rosbag_job(__componentName, self._form_rosbag_job(req_job))
 
         if self.spec.runtime == 'cloud':
             if 'staticRoutes' in self.spec:
@@ -114,59 +119,70 @@
             if 'volumes' in self.spec:
                 disk_mounts = {}
                 for vol in self.spec.volumes:
                     disk_guid, disk = self.rc.find_depends(vol.depends)
                     if disk_guid not in disk_mounts:
                         disk_mounts[disk_guid] = []
 
-                    disk_mounts[disk_guid].append(ExecutableMount(vol.execName, vol.mountPath, vol.subPath))
+                    disk_mounts[disk_guid].append(
+                        ExecutableMount(vol.execName, vol.mountPath, vol.subPath))
 
                 for disk_guid in disk_mounts.keys():
                     disk = client.get_volume_instance(disk_guid)
                     provision_config.mount_volume(__componentName, volume=disk,
                                                   executable_mounts=disk_mounts[disk_guid])
 
             # TODO: Managed Services is currently limited to `cloud` deployments
             # since we don't expose `elasticsearch` outside Openshift. This may
             # change in the future.
             if 'managedServices' in self.spec:
                 managed_services = []
                 for managed_service in self.spec.managedServices:
                     managed_services.append({
-                        "instance": managed_service.depends.nameOrGUID,
+                        'instance': managed_service.depends.nameOrGUID,
                     })
-                provision_config.context["managedServices"] = managed_services
+                provision_config.context['managedServices'] = managed_services
 
         if self.spec.runtime == 'device':
             device_guid, device = self.rc.find_depends(self.spec.device.depends)
             if device is None and device_guid:
                 device = client.get_device(device_guid)
-            provision_config.add_device(__componentName, device=device)
+            provision_config.add_device(__componentName, device=device, set_component_alias=False)
 
             if 'restart' in self.spec:
-                provision_config.add_restart_policy(__componentName, self.RESTART_POLICY[self.spec.restart.lower()])
+                provision_config.add_restart_policy(
+                    __componentName, self.RESTART_POLICY[self.spec.restart.lower()])
 
             # Add Network
             # if self.spec.rosNetworks:
             # for network in self.spec.rosNetworks:
             # network_type =
 
             # Add Disk
             exec_mounts = []
             if 'volumes' in self.spec:
                 for vol in self.spec.volumes:
                     exec_mounts.append(ExecutableMount(vol.execName, vol.mountPath, vol.subPath))
             if len(exec_mounts) > 0:
-                provision_config = add_mount_volume_provision_config(provision_config, __componentName, device,
-                                                                     exec_mounts)
+                provision_config = add_mount_volume_provision_config(
+                    provision_config, __componentName, device, exec_mounts)
+
+        provision_config.set_component_alias(__componentName, self.metadata.name)
 
         if os.environ.get('DEBUG'):
             print(provision_config)
         deployment = pkg.provision(self.metadata.name, provision_config)
-        deployment.poll_deployment_till_ready()
+
+        try:
+            deployment.poll_deployment_till_ready()
+        except DeploymentNotRunningException as e:
+            raise Exception(process_deployment_errors(e)) from e
+        except Exception as e:
+            raise e
+
         deployment.get_status()
         return deployment
 
     def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
         if 'depends' in self.spec:
             pass
         pass
@@ -174,18 +190,14 @@
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
         obj.deprovision()
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
-    @staticmethod
-    def validate(data):
-        validate(data)
-
     def _get_package(self, client: Client) -> Package:
         name = self.metadata.depends.nameOrGUID
         if name.startswith('pkg-') or name.startswith('io-'):
             guid = name
         else:
             guid = find_package_guid(client, name, self.metadata.depends.version)
 
@@ -223,15 +235,16 @@
         for route in self.spec.staticRoutes:
             name = route.depends.nameOrGUID
             if name.startswith('staticroute-'):
                 guid = name
             else:
                 guid = find_static_route_guid(client, name)
             static_route = client.get_static_route(route_guid=guid)
-            prov_config.add_static_route(component_name=component, endpoint_name=route.name, static_route=static_route)
+            prov_config.add_static_route(
+                component_name=component, endpoint_name=route.name, static_route=static_route)
 
     def _form_rosbag_job(self, req_job):
         rosbag_job_kw_args = {
             'name': req_job.name,
             'rosbag_options': ROSBagOptions(
                 all_topics=req_job.recordOptions.get('allTopics'),
                 topics=req_job.recordOptions.get('topics'),
@@ -248,15 +261,16 @@
                 max_split_duration=req_job.recordOptions.get('maxSplitDuration')
             )}
 
         if 'uploadOptions' in req_job:
             rosbag_job_kw_args['upload_options'] = self._form_rosbag_upload_options(req_job.uploadOptions)
 
         if 'overrideOptions' in req_job:
-            rosbag_job_kw_args['override_options'] = self._form_rosbag_override_options(req_job.overrideOptions)
+            rosbag_job_kw_args['override_options'] = self._form_rosbag_override_options(
+                req_job.overrideOptions)
 
         return ROSBagJob(**rosbag_job_kw_args)
 
     @staticmethod
     def _form_rosbag_upload_options(upload_options):
         upload_options_kw_args = {
             'max_upload_rate': upload_options.maxUploadRate,
@@ -299,7 +313,46 @@
 
             override_options_kw_args['topic_override_info'] = override_infos
 
         if 'excludeTopics' in override_options:
             override_options_kw_args['exclude_topics'] = override_options.excludeTopics
 
         return OverrideOptions(**override_options_kw_args)
+
+    @staticmethod
+    def validate(data):
+        """
+        Validates if deployment data is matching with its corresponding schema
+        """
+        schema = load_schema('deployment')
+        validate_manifest(instance=data, schema=schema)
+
+
+def process_deployment_errors(e: DeploymentNotRunningException):
+    errors = e.deployment_status.errors
+    err_fmt = '[{}] {}\nAction: {}'
+    support_action = ('Report the issue together with the relevant'
+                      ' details to the support team')
+
+    action, description = '', ''
+    msgs = []
+    for code in errors:
+        if code in ERRORS:
+            description = ERRORS[code]['description']
+            action = ERRORS[code]['action']
+        elif code.startswith('DEP_E2'):
+            description = 'Internal rapyuta.io error in the components deployed on cloud'
+            action = support_action
+        elif code.startswith('DEP_E3'):
+            description = 'Internal rapyuta.io error in the components deployed on a device'
+            action = support_action
+        elif code.startswith('DEP_E4'):
+            description = 'Internal rapyuta.io error'
+            action = support_action
+
+        code = click.style(code, fg='yellow')
+        description = click.style(description, fg='red')
+        action = click.style(action, fg='green')
+
+        msgs.append(err_fmt.format(code, description, action))
+
+    return '\n'.join(msgs)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/run.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/run.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/ssh.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/status.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/util.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/deployment/wait.py` & `rapyuta-io-cli-2.0.1/riocli/deployment/wait.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/device/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/config.py` & `rapyuta-io-cli-2.0.1/riocli/device/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/create.py` & `rapyuta-io-cli-2.0.1/riocli/device/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/delete.py` & `rapyuta-io-cli-2.0.1/riocli/device/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/deployment.py` & `rapyuta-io-cli-2.0.1/riocli/device/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/execute.py` & `rapyuta-io-cli-2.0.1/riocli/device/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/files.py` & `rapyuta-io-cli-2.0.1/riocli/device/files.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/device/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/label.py` & `rapyuta-io-cli-2.0.1/riocli/device/label.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/list.py` & `rapyuta-io-cli-2.0.1/riocli/device/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/metric.py` & `rapyuta-io-cli-2.0.1/riocli/device/metric.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/model.py` & `rapyuta-io-cli-2.0.1/riocli/device/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 from rapyuta_io import Client
 from rapyuta_io.clients.device import Device as v1Device, DevicePythonVersion
 
-from riocli.device.validation import validate
 from riocli.model import Model
+from riocli.utils.validate import validate_manifest, load_schema
 
 
 class Device(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
-        guid, obj = self.rc.find_depends({"kind": "device", "nameOrGUID": self.metadata.name})
+        guid, obj = self.rc.find_depends(
+            {"kind": "device", "nameOrGUID": self.metadata.name})
         if not guid:
             return False
 
         return obj
 
     def create_object(self, client: Client) -> v1Device:
         device = client.create_device(self.to_v1())
@@ -61,9 +62,13 @@
                         rosbag_mount_path=rosbag_mount_path, ros_workspace=ros_workspace)
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
-    def validate(data) -> None:
-        validate(data)
+    def validate(data):
+        """
+        Validates if device data is matching with its corresponding schema
+        """
+        schema = load_schema('device')
+        validate_manifest(instance=data, schema=schema)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/onboard.py` & `rapyuta-io-cli-2.0.1/riocli/device/onboard.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/device/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/device_init.py` & `rapyuta-io-cli-2.0.1/riocli/device/tools/device_init.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/forward.py` & `rapyuta-io-cli-2.0.1/riocli/device/tools/forward.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/rapyuta_logs.py` & `rapyuta-io-cli-2.0.1/riocli/device/tools/rapyuta_logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/scp.py` & `rapyuta-io-cli-2.0.1/riocli/device/tools/scp.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/service.py` & `rapyuta-io-cli-2.0.1/riocli/device/tools/service.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/ssh.py` & `rapyuta-io-cli-2.0.1/riocli/device/tools/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/tools/util.py` & `rapyuta-io-cli-2.0.1/riocli/device/tools/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/topic.py` & `rapyuta-io-cli-2.0.1/riocli/device/topic.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/device/util.py` & `rapyuta-io-cli-2.0.1/riocli/device/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/create.py` & `rapyuta-io-cli-2.0.1/riocli/disk/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/delete.py` & `rapyuta-io-cli-2.0.1/riocli/disk/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/list.py` & `rapyuta-io-cli-2.0.1/riocli/disk/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/model.py` & `rapyuta-io-cli-2.0.1/riocli/disk/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import click_spinner
 from munch import munchify
 from rapyuta_io import Client
 from rapyuta_io.utils.rest_client import HttpMethod
 
 from riocli.disk.util import _api_call
 from riocli.model import Model
+from riocli.utils.validate import load_schema, validate_manifest
 
 
 class Disk(Model):
     def find_object(self, client: Client) -> typing.Any:
         _, disk = self.rc.find_depends({'kind': 'disk', 'nameOrGUID': self.metadata.name})
         if not disk:
             return False
@@ -73,9 +74,10 @@
                 continue
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
-    def validate(d):
-        pass
+    def validate(data):
+        schema = load_schema('disk')
+        validate_manifest(data, schema)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/disk/util.py` & `rapyuta-io-cli-2.0.1/riocli/disk/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/exceptions/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/managedservice/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/managedservice/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/list.py` & `rapyuta-io-cli-2.0.1/riocli/managedservice/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/list_providers.py` & `rapyuta-io-cli-2.0.1/riocli/managedservice/list_providers.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/model.py` & `rapyuta-io-cli-2.0.1/riocli/managedservice/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 import typing
 
 from munch import munchify
 from rapyuta_io import Client
 
 from riocli.managedservice.util import ManagedServicesClient
-from riocli.managedservice.validation import validate
 from riocli.model import Model
+from riocli.utils.validate import load_schema, validate_manifest
 
 
 class ManagedService(Model):
     def find_object(self, client: Client) -> typing.Any:
         name = self.metadata.name
         client = ManagedServicesClient()
 
@@ -50,9 +50,13 @@
         return client.list_instances()
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
-    def validate(d):
-        validate(d)
+    def validate(data):
+        """
+        Validates if managedservice data is matching with its corresponding schema
+        """
+        schema = load_schema('managedservice')
+        validate_manifest(instance=data, schema=schema)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/managedservice/util.py` & `rapyuta-io-cli-2.0.1/riocli/managedservice/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/marketplace/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/install.py` & `rapyuta-io-cli-2.0.1/riocli/marketplace/install.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/list.py` & `rapyuta-io-cli-2.0.1/riocli/marketplace/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/marketplace/util.py` & `rapyuta-io-cli-2.0.1/riocli/marketplace/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/model/base.py` & `rapyuta-io-cli-2.0.1/riocli/model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 from abc import ABC, abstractmethod
 from datetime import datetime
 from shutil import get_terminal_size
+import yaml
+import os
 
 import click
 from munch import Munch, munchify
 from rapyuta_io import Client
+from pathlib import Path
 
 from riocli.project.util import find_project_guid
 
 prompt = ">> {}{}{} [{}]"  # >> msg  spacer  rigth_msg time
 
 DELETE_POLICY_LABEL = 'rapyuta.io/deletionPolicy'
 
+schema_dir = Path('jsonschema')
 
 def message_with_prompt(msg, right_msg="", fg='white', with_time=True):
     columns, _ = get_terminal_size()
     time = datetime.now().isoformat('T')
     spacer = ' ' * (int(columns) - len(msg + right_msg + time) - 12)
     msg = prompt.format(msg, spacer, right_msg, time)
     click.secho(msg, fg=fg)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/network/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/create.py` & `rapyuta-io-cli-2.0.1/riocli/network/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 @click.command('create')
 @click.argument('name', type=str)
 @click.option('--network', help='Type of Network',
               type=click.Choice(['routed', 'native']), default='routed')
 @click.option('--ros', help='Version of ROS',
               type=click.Choice(['kinetic', 'melodic', 'noetic']), default='melodic')
 @click.option('--device', 'device_name', help='Device ID of the Device where Network will run (device only)')
-@click.option('--limit', help='Resource Limit for Network (cloud only) '
-                              '[x_small is only available for Native Network]',
-              type=click.Choice(['x_small', 'small', 'medium', 'large']), default='small')
+@click.option('--cpu', help='cpu limit for Network (cloud only) ', type=float)
+@click.option('--memory', help='memory limit for Network (cloud only) ', type=int)
 @click.option('--network-interface', '-nic', type=str,
               help='Network Interface on which Network will listen (device only)')
 @click.option('--restart-policy', help='Restart policy for the Network (device only)',
               type=click.Choice(['always', 'no', 'on-failure']), default='always')
 @device_name_to_guid
 def create_network(name: str, network: str, **kwargs: typing.Any) -> None:
     """
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/delete.py` & `rapyuta-io-cli-2.0.1/riocli/network/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/network/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/list.py` & `rapyuta-io-cli-2.0.1/riocli/network/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/logs.py` & `rapyuta-io-cli-2.0.1/riocli/network/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/model.py` & `rapyuta-io-cli-2.0.1/riocli/network/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,52 +11,42 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 from typing import Union, Any, Dict
 
 from rapyuta_io import Client
-from rapyuta_io.clients.native_network import NativeNetwork, NativeNetworkLimits, Parameters as NativeNetworkParameters
-from rapyuta_io.clients.routed_network import RoutedNetwork, RoutedNetworkLimits, Parameters as RoutedNetworkParameters
+from rapyuta_io.clients.native_network import NativeNetwork, Parameters as NativeNetworkParameters
+from rapyuta_io.clients.routed_network import RoutedNetwork, Parameters as RoutedNetworkParameters
 
 from riocli.model import Model
 from riocli.network.util import find_network_name, NetworkNotFound
-from riocli.network.validation import validate
+from riocli.utils.validate import validate_manifest, load_schema
 
 
 class Network(Model):
-    _RoutedNetworkLimits = {
-        'small': RoutedNetworkLimits.SMALL,
-        'medium': RoutedNetworkLimits.MEDIUM,
-        'large': RoutedNetworkLimits.LARGE,
-    }
-
-    _NativeNetworkLimits = {
-        'xSmall': NativeNetworkLimits.X_SMALL,
-        'small': NativeNetworkLimits.SMALL,
-        'medium': NativeNetworkLimits.MEDIUM,
-        'large': NativeNetworkLimits.LARGE,
-
-    }
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
         try:
             network, _ = find_network_name(client, self.metadata.name, self.spec.type, is_resolve_conflict=False)
             return network
         except NetworkNotFound:
             return False
 
     def create_object(self, client: Client) -> Union[NativeNetwork, RoutedNetwork]:
         if self.spec.type == 'routed':
-            return self._create_routed_network(client)
+            network = self._create_routed_network(client)
+            network.poll_routed_network_till_ready()
+            return network
 
         network = client.create_native_network(self.to_v1(client))
+        network.poll_native_network_till_ready()
         return network
 
     def update_object(self, client: Client, obj: Union[RoutedNetwork, NativeNetwork]) -> Any:
         # try:
         #     obj.delete()
         #     self.create_object(client)
         # except Exception as e:
@@ -67,17 +57,14 @@
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
         obj.delete()
 
     @classmethod
     def pre_process(cls, client: Client, d: Dict) -> None:
         pass
 
-    @staticmethod
-    def validate(data) -> None:
-        validate(data)
 
     def to_v1(self, client: Client) -> NativeNetwork:
         if self.spec.runtime == 'cloud':
             limits = self._get_limits()
             parameters = NativeNetworkParameters(limits=limits)
         else:
             device = client.get_device(self.spec.deviceGUID)
@@ -101,12 +88,14 @@
 
     def _create_device_routed_network(self, client: Client) -> RoutedNetwork:
         device = client.get_device(self.spec.deviceGUID)
         return client.create_device_routed_network(name=self.metadata.name, ros_distro=self.spec.rosDistro, shared=True,
                                                    device=device,
                                                    network_interface=self.spec.networkInterface)
 
-    def _get_limits(self) -> Union[RoutedNetworkLimits, NativeNetworkLimits]:
-        if self.spec.type == 'routed':
-            return self._RoutedNetworkLimits[self.spec.resourceLimits]
-        else:
-            return self._NativeNetworkLimits[self.spec.resourceLimits]
+    @staticmethod
+    def validate(data):
+        """
+        Validates if network data is matching with its corresponding schema
+        """
+        schema = load_schema('network')
+        validate_manifest(instance=data, schema=schema)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/native_network.py` & `rapyuta-io-cli-2.0.1/riocli/network/native_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 import click
 from click_spinner import spinner
-from rapyuta_io.clients.native_network import NativeNetwork, Parameters, NativeNetworkLimits
+from rapyuta_io.clients.native_network import NativeNetwork, Parameters
 from rapyuta_io.clients.package import Runtime, ROSDistro
-
+from rapyuta_io.clients.common_models import Limits
 from riocli.config import new_client
 
 
 def create_native_network(name: str, ros: str, device_guid: str = None, network_interface: str = None,
-                          limit: str = None, restart_policy: str = None, **kwargs: typing.Any) -> None:
+                          cpu: float = 0, memory: int = 0, restart_policy: str = None, **kwargs: typing.Any) -> None:
     client = new_client()
 
     ros_distro = ROSDistro(ros)
     runtime = Runtime.CLOUD
 
-    if limit is not None:
-        limit = getattr(NativeNetworkLimits, limit.upper())
+    limit = None
+    if cpu or memory:
+        if device_guid:
+            raise Exception('Native network for device does not support cpu or memory')
+        limit = Limits(cpu, memory)
 
     device = None
     if device_guid:
         runtime = Runtime.DEVICE
         device = client.get_device(device_id=device_guid)
 
     parameters = Parameters(limits=limit, device=device, network_interface=network_interface,
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/routed_network.py` & `rapyuta-io-cli-2.0.1/riocli/network/routed_network.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,37 +13,44 @@
 # limitations under the License.
 import typing
 
 import click
 from click_spinner import spinner
 from rapyuta_io import ROSDistro
 from rapyuta_io.clients.package import RestartPolicy
-from rapyuta_io.clients.routed_network import RoutedNetworkLimits, Parameters
-
+from rapyuta_io.clients.routed_network import Parameters
+from rapyuta_io.clients.common_models import Limits
 from riocli.config import new_client
 
 
 def create_routed_network(name: str, ros: str, device_guid: str = None, network_interface: str = None,
-                          limit: str = None, restart_policy: str = None, **kwargs: typing.Any) -> None:
+                          cpu: float = 0, memory: int = 0, restart_policy: str = None, **kwargs: typing.Any) -> None:
     client = new_client()
     ros_distro = ROSDistro(ros)
-    limit = getattr(RoutedNetworkLimits, limit.upper())
+
+    limit = None
+    if cpu or memory:
+        if device_guid:
+            raise Exception('Routed network for device does not support cpu or memory')
+        limit = Limits(cpu, memory)
+
     if restart_policy:
         restart_policy = RestartPolicy(restart_policy)
 
     with spinner():
         if device_guid:
             device = client.get_device(device_id=device_guid)
             client.create_device_routed_network(name=name, ros_distro=ros_distro, shared=False,
                                                 device=device,
                                                 network_interface=network_interface,
                                                 restart_policy=restart_policy)
         else:
+            parameters = None if not limit else Parameters(limit)
             client.create_cloud_routed_network(name, ros_distro=ros_distro, shared=False,
-                                               parameters=Parameters(limit))
+                                               parameters=parameters)
 
     click.secho('Routed Network created successfully!', fg='green')
 
 
 def inspect_routed_network(network_guid: str) -> dict:
     client = new_client()
     network = client.get_routed_network(network_guid)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/network/util.py` & `rapyuta-io-cli-2.0.1/riocli/network/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/create.py` & `rapyuta-io-cli-2.0.1/riocli/package/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/delete.py` & `rapyuta-io-cli-2.0.1/riocli/package/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/deployment.py` & `rapyuta-io-cli-2.0.1/riocli/package/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/package/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/list.py` & `rapyuta-io-cli-2.0.1/riocli/package/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/model.py` & `rapyuta-io-cli-2.0.1/riocli/package/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 import typing
 
 from munch import munchify
 from rapyuta_io import Client
 from rapyuta_io.clients.package import RestartPolicy
 
 from riocli.model import Model
-# from riocli.package.util import find_project_guid, ProjectNotFound
-from riocli.package.validation import validate
+from riocli.utils.validate import validate_manifest, load_schema
 
 
 class Package(Model):
     RESTART_POLICY = {
         'always': RestartPolicy.Always,
         'never': RestartPolicy.Never,
         'onfailure': RestartPolicy.OnFailure
@@ -241,9 +240,13 @@
                 "port": endpoint.port, "targetPort": endpoint.targetPort, "proto": proto.upper()}
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
-    def validate(data) -> None:
-        validate(data)
+    def validate(data):
+        """
+        Validates if package data is matching with its corresponding schema
+        """
+        schema = load_schema('package')
+        validate_manifest(instance=data, schema=schema)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/package/util.py` & `rapyuta-io-cli-2.0.1/riocli/package/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/parameter/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/parameter/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,48 @@
-# Copyright 2021 Rapyuta Robotics
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import click
-from click_help_colors import HelpColorsGroup
-
-from riocli.parameter.apply import apply_configurations
-from riocli.parameter.diff import diff_configurations
-from riocli.parameter.download import download_configurations
-from riocli.parameter.upload import upload_configurations
-
-
-# from riocli.parameter.diff import diff_configurations
-# from riocli.parameter.download import download_configurations
-
-
-@click.group(
-    invoke_without_command=False,
-    cls=HelpColorsGroup,
-    help_headers_color='yellow',
-    help_options_color='green',
-)
-def parameter() -> None:
-    """
-    Define groups of executables to deploy together
-    """
-    pass
-
-
-parameter.add_command(upload_configurations)
-parameter.add_command(download_configurations)
-parameter.add_command(diff_configurations)
-parameter.add_command(apply_configurations)
+# Copyright 2023 Rapyuta Robotics
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import click
+from click_help_colors import HelpColorsGroup
+
+from riocli.parameter.apply import apply_configurations
+from riocli.parameter.delete import delete_configurations
+from riocli.parameter.diff import diff_configurations
+from riocli.parameter.download import download_configurations
+from riocli.parameter.list import list_configuration_trees
+from riocli.parameter.upload import upload_configurations
+
+
+# from riocli.parameter.diff import diff_configurations
+# from riocli.parameter.download import download_configurations
+
+
+@click.group(
+    invoke_without_command=False,
+    cls=HelpColorsGroup,
+    help_headers_color='yellow',
+    help_options_color='green',
+)
+def parameter() -> None:
+    """
+    Define groups of executables to deploy together
+    """
+    pass
+
+
+parameter.add_command(upload_configurations)
+parameter.add_command(download_configurations)
+parameter.add_command(diff_configurations)
+parameter.add_command(apply_configurations)
+parameter.add_command(list_configuration_trees)
+parameter.add_command(delete_configurations)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/parameter/apply.py` & `rapyuta-io-cli-2.0.1/riocli/parameter/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/parameter/delete.py` & `rapyuta-io-cli-2.0.1/riocli/static_route/create.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 import click
+from click_spinner import spinner
 
 from riocli.config import new_client
 
 
-@click.command('delete')
-@click.option('--tree-names', type=click.STRING, multiple=True, default=None,
-              help='Directory names to upload')
-def delete_configurations(tree_names: str = None) -> None:
+@click.command('create')
+@click.argument('prefix', type=str)
+def create_static_route(prefix: str) -> None:
     """
-    Upload a set of configurations to IO.
-
-    Compile the IO configurations from the paths provided. Output to a temporary directory. Upload the directory.
+    Creates a new instance of static route
     """
     try:
         client = new_client()
-        pass
-    except IOError as e:
-        click.secho(str(e.__traceback__), fg='red')
+        with spinner():
+            route = client.create_static_route(prefix)
+        click.secho("Static Route created successfully for URL {}".format(route.urlString), fg='green')
+    except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/parameter/download.py` & `rapyuta-io-cli-2.0.1/riocli/parameter/download.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,58 @@
-# Copyright 2021 Rapyuta Robotics
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-# -----------------------------------------------------------------------------
-#
-# Configurations
-# Args
-#    path,  tree_names,  delete_existing=True|False
-# -----------------------------------------------------------------------------
-
-from tempfile import mkdtemp
-from typing import Tuple
-from xmlrpc.client import Boolean
-
-import click
-from rapyuta_io.utils.error import APIError, InternalServerError
-
-from riocli.config import new_client
-
-
-@click.command('download')
-@click.option('--path', type=click.Path(dir_okay=True, file_okay=False, writable=True, exists=True, resolve_path=True),
-              default=["."],
-              help='Root Path for the Parameters to be download')
-@click.option('--tree-names', type=click.STRING, multiple=True, default=None,
-              help='Tree names to fetch')
-@click.option('--delete-existing', is_flag=True,
-              help='Overwrite existing parameter tree')
-def download_configurations(path: click.Path, tree_names: Tuple = None, delete_existing: Boolean = False) -> None:
-    """
-    Download the configurations
-    """
-    if path is None:
-        path = mkdtemp()  # Temporary directory to hold the configurations
-
-    tree_names = list(tree_names)
-
-    try:
-        client = new_client()
-
-        client.download_configurations(str(path), tree_names=tree_names, delete_existing_trees=delete_existing)
-
-    except (APIError, InternalServerError) as e:
-        click.secho(f"failed API request {str(e)}", fg='red')
-        raise SystemExit(1)
-    except (IOError, OSError) as e:
-        click.secho(f"failed file/directory creation {str(e)}", fg='red')
-        raise SystemExit(1)
-
-    click.secho("Downloaded IO configurations to '{}'".format(path), fg='green')
-    return path
+# Copyright 2023 Rapyuta Robotics
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import typing
+from tempfile import mkdtemp
+from xmlrpc.client import Boolean
+
+import click
+from click_spinner import spinner
+
+from riocli.config import new_client
+from riocli.parameter.utils import display_trees
+
+
+# -----------------------------------------------------------------------------
+#
+# Configurations
+# Args
+#    path,  tree_names,  delete_existing=True|False
+# -----------------------------------------------------------------------------
+
+
+@click.command('download')
+@click.option('--tree-names', type=click.STRING, multiple=True, default=None, help='Tree names to fetch')
+@click.option('--overwrite', '--delete-existing', 'delete_existing', is_flag=True,
+              help='Overwrite existing parameter tree')
+@click.argument('path', type=click.Path(exists=True), required=False)
+def download_configurations(path: str, tree_names: typing.Tuple[str] = None, delete_existing: Boolean = False) -> None:
+    """
+    Download the Configuration Parameter trees.
+    """
+    if path is None:
+        # Not using the Context Manager because we need to persist the Temporary directory.
+        path = mkdtemp()
+
+    click.secho('Downloading at {}'.format(path))
+
+    try:
+        client = new_client()
+
+        with spinner():
+            client.download_configurations(path, tree_names=list(tree_names),
+                                           delete_existing_trees=delete_existing)
+
+        click.secho('✅ Configuration Parameters downloaded successfully', fg='green')
+    except Exception as e:
+        click.secho(e, fg='red')
+        raise SystemExit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/project/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/create.py` & `rapyuta-io-cli-2.0.1/riocli/project/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/delete.py` & `rapyuta-io-cli-2.0.1/riocli/project/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/project/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/list.py` & `rapyuta-io-cli-2.0.1/riocli/project/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/model.py` & `rapyuta-io-cli-2.0.1/riocli/project/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 from rapyuta_io import Project as v1Project, Client
 
 from riocli.model import Model
-from riocli.project.validation import validate
+from riocli.utils.validate import validate_manifest, load_schema
 
 
 class Project(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
-        guid, obj = self.rc.find_depends({"kind": "project", "nameOrGUID": self.metadata.name})
+        guid, obj = self.rc.find_depends(
+            {"kind": "project", "nameOrGUID": self.metadata.name})
         if not guid:
             return False
 
         return obj
 
     def create_object(self, client: Client) -> v1Project:
         project = client.create_project(self.to_v1())
@@ -45,9 +46,13 @@
         return v1Project(self.metadata.name)
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
-    def validate(data) -> None:
-        validate(data)
+    def validate(data):
+        """
+        Validates if project data is matching with its corresponding schema
+        """
+        schema = load_schema('project')
+        validate_manifest(instance=data, schema=schema)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/select.py` & `rapyuta-io-cli-2.0.1/riocli/project/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/project/util.py` & `rapyuta-io-cli-2.0.1/riocli/project/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/rosbag/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/rosbag/blob.py` & `rapyuta-io-cli-2.0.1/riocli/rosbag/blob.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/rosbag/job.py` & `rapyuta-io-cli-2.0.1/riocli/rosbag/job.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/create.py` & `rapyuta-io-cli-2.0.1/riocli/secret/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/delete.py` & `rapyuta-io-cli-2.0.1/riocli/secret/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/docker_secret.py` & `rapyuta-io-cli-2.0.1/riocli/secret/docker_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/import_secret.py` & `rapyuta-io-cli-2.0.1/riocli/secret/import_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/secret/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/list.py` & `rapyuta-io-cli-2.0.1/riocli/secret/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/model.py` & `rapyuta-io-cli-2.0.1/riocli/secret/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
-from rapyuta_io import Secret as v1Secret, SecretConfigDocker, SecretConfigSourceBasicAuth, \
+from rapyuta_io import Secret as v1Secret, SecretConfigDocker, \
+    SecretConfigSourceBasicAuth, \
     SecretConfigSourceSSHAuth, Client
 
 from riocli.model import Model
-from riocli.secret.validation import validate
+from riocli.utils.validate import load_schema, validate_manifest
 
 
 class Secret(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
-        _, secret = self.rc.find_depends({'kind': 'secret', 'nameOrGUID': self.metadata.name})
+        _, secret = self.rc.find_depends(
+            {'kind': 'secret', 'nameOrGUID': self.metadata.name})
         if not secret:
             return False
 
         return secret
 
     def create_object(self, client: Client) -> v1Secret:
         secret = client.create_secret(self.to_v1())
@@ -68,9 +70,13 @@
         return v1Secret(self.metadata.name, config)
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
-    def validate(data) -> None:
-        validate(data)
+    def validate(data):
+        """
+        Validates if secret data is matching with its corresponding schema
+        """
+        schema = load_schema('secret')
+        validate_manifest(instance=data, schema=schema)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/source_secret.py` & `rapyuta-io-cli-2.0.1/riocli/secret/source_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/secret/util.py` & `rapyuta-io-cli-2.0.1/riocli/secret/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/shell/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/shell/prompt.py` & `rapyuta-io-cli-2.0.1/riocli/shell/prompt.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/static_route/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/create.py` & `rapyuta-io-cli-2.0.1/riocli/static_route/open.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
-from click_spinner import spinner
 
 from riocli.config import new_client
+from riocli.static_route.util import name_to_guid
 
 
-@click.command('create')
-@click.argument('prefix', type=str)
-def create_static_route(prefix: str) -> None:
+@click.command('open')
+@click.argument('static-route', type=str)
+@name_to_guid
+def open_static_route(static_route, static_route_guid) -> None:
     """
-    Creates a new instance of static route
+    Opens the static route in the default browser
     """
     try:
         client = new_client()
-        with spinner():
-            route = client.create_static_route(prefix)
-        click.secho("Static Route created successfully for URL {}".format(route.urlString), fg='green')
+        route = client.get_static_route(static_route_guid)
+        click.launch(url='https://{}'.format(route.urlString), wait=False)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/delete.py` & `rapyuta-io-cli-2.0.1/riocli/static_route/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/inspect.py` & `rapyuta-io-cli-2.0.1/riocli/static_route/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/list.py` & `rapyuta-io-cli-2.0.1/riocli/static_route/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/model.py` & `rapyuta-io-cli-2.0.1/riocli/static_route/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 # limitations under the License.
 import typing
 
 from rapyuta_io import Client
 from rapyuta_io.clients.static_route import StaticRoute as v1StaticRoute
 
 from riocli.model import Model
-from riocli.static_route.validation import validate
+from riocli.utils.validate import validate_manifest, load_schema
 
 
 class StaticRoute(Model):
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
-        _, static_route = self.rc.find_depends({"kind": "staticroute", "nameOrGUID": self.metadata.name})
+        _, static_route = self.rc.find_depends({'kind': 'staticroute',
+                                                'nameOrGUID': self.metadata.name})
         if not static_route:
             return False
 
         return static_route
 
     def create_object(self, client: Client) -> v1StaticRoute:
         static_route = client.create_static_route(self.metadata.name)
@@ -42,9 +43,13 @@
         client.delete_static_route(obj.guid)
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
-    def validate(data) -> None:
-        validate(data)
+    def validate(data):
+        """
+        Validates if static route data is matching with its corresponding schema
+        """
+        schema = load_schema('static_route')
+        validate_manifest(instance=data, schema=schema)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/open.py` & `rapyuta-io-cli-2.0.1/riocli/chart/info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2022 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 import click
+from click_help_colors import HelpColorsCommand
 
-from riocli.config import new_client
-from riocli.static_route.util import name_to_guid
+from riocli.chart.util import find_chart
+from riocli.utils import dump_all_yaml
 
 
-@click.command('open')
-@click.argument('static-route', type=str)
-@name_to_guid
-def open_static_route(static_route, static_route_guid) -> None:
-    """
-    Opens the static route in the default browser
-    """
-    try:
-        client = new_client()
-        route = client.get_static_route(static_route_guid)
-        click.launch(url='https://{}'.format(route.urlString), wait=False)
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+@click.command(
+    'info',
+    cls=HelpColorsCommand,
+    help_headers_color='yellow',
+    help_options_color='green',
+    help='Describe the available chart with versions',
+)
+@click.argument('chart', type=str)
+def info_chart(chart: str) -> None:
+    """Print a chart's details."""
+    versions = find_chart(chart)
+    dump_all_yaml(versions)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/static_route/util.py` & `rapyuta-io-cli-2.0.1/riocli/static_route/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/__init__.py` & `rapyuta-io-cli-2.0.1/riocli/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
         raise Exception('Invalid format')
 
 
 def dump_all_yaml(objs: typing.List):
     """
     Dump multiple documents as YAML separated by triple dash (---)
     """
-    click.echo(yaml.dump_all(objs, allow_unicode=True, explicit_start=True))
+    click.echo(yaml.safe_dump_all(objs, allow_unicode=True,
+                                  explicit_start=True))
 
 
 def run_bash(cmd, bg=False):
     cmd_parts = shlex.split(cmd)
 
     if bg is True:
         bg_output = subprocess.Popen(cmd_parts)
```

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/context.py` & `rapyuta-io-cli-2.0.1/riocli/utils/context.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/execute.py` & `rapyuta-io-cli-2.0.1/riocli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/mermaid.py` & `rapyuta-io-cli-2.0.1/riocli/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/selector.py` & `rapyuta-io-cli-2.0.1/riocli/utils/selector.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/riocli/utils/ssh_tunnel.py` & `rapyuta-io-cli-2.0.1/riocli/utils/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-1.0.0/setup.py` & `rapyuta-io-cli-2.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 
-
 """setup.py: setuptools control."""
 
-
 import re
-from setuptools import setup, find_packages
 
+from setuptools import setup, find_packages
 
 version = re.search(
     '^__version__\s*=\s*"(.*)"', open("riocli/bootstrap.py").read(), re.M
 ).group(1)
 
 
 with open("README.md", "rb") as f:
@@ -40,24 +38,26 @@
         "click-completion>=0.5.2",
         "click-help-colors>=0.9.1",
         "click-repl>=0.2.0",
         "click-spinner>=0.1.10",
         "click-plugins>=1.1.1",
         "click>=8.0.1",
         "dictdiffer>=0.9.0",
-        "fastjsonschema>=2.16.1",
         "graphlib-backport>=1.0.3",
         "jinja2>=3.0.1",
         "munch>=2.4.0",
         "python-dateutil>=2.8.2",
         "pytz",
         "pyyaml>=5.4.1",
-        "rapyuta-io>=1.8.0",
+        "rapyuta-io>=1.9.0",
         "requests>=2.20.0",
         "setuptools",
         "six>=1.13.0",
         "tabulate>=0.8.0",
         "urllib3>=1.23",
-        "pyrfc3339>=1.1"
+        "pyrfc3339>=1.1",
+        "directory-tree>=0.0.3.1",
+        "yaspin>=2.3.0",
+        "jsonschema>=4.0.0"
     ],
     setup_requires=["flake8"],
 )
```

