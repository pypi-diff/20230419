# Comparing `tmp/e2e_cli-0.9.9.7.tar.gz` & `tmp/e2e_cli-0.9.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2e_cli-0.9.9.7.tar", last modified: Fri Apr  7 13:47:15 2023, max compression
+gzip compressed data, was "e2e_cli-0.9.9.8.tar", last modified: Wed Apr 19 10:42:06 2023, max compression
```

## Comparing `e2e_cli-0.9.9.7.tar` & `e2e_cli-0.9.9.8.tar`

### file list

```diff
@@ -1,106 +1,105 @@
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.942518 e2e_cli-0.9.9.7/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/LICENSE
--rw-rw-r--   0 aman      (1000) aman      (1000)       31 2023-03-03 10:09:05.000000 e2e_cli-0.9.9.7/MANIFEST.in
--rw-rw-r--   0 aman      (1000) aman      (1000)      372 2023-04-07 13:47:15.942518 e2e_cli-0.9.9.7/PKG-INFO
--rw-rw-r--   0 aman      (1000) aman      (1000)     6237 2023-03-03 09:45:02.000000 e2e_cli-0.9.9.7/README.md
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.934518 e2e_cli-0.9.9.7/e2e_cli/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/__init__.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.934518 e2e_cli-0.9.9.7/e2e_cli/auto_scaling/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-22 08:23:32.000000 e2e_cli-0.9.9.7/e2e_cli/auto_scaling/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     4068 2023-04-07 12:51:56.000000 e2e_cli-0.9.9.7/e2e_cli/auto_scaling/auto_scaling.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     2139 2023-04-07 12:18:48.000000 e2e_cli-0.9.9.7/e2e_cli/auto_scaling/autoscaling_routing.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.934518 e2e_cli-0.9.9.7/e2e_cli/bucket_store/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/bucket_store/__init__.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.934518 e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_actions/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-20 13:31:40.000000 e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_actions/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     8272 2023-04-07 12:52:26.000000 e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_actions/bucket_actions.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.934518 e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_crud/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-22 08:23:41.000000 e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_crud/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     4074 2023-04-07 12:55:53.000000 e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_crud/bucket_storage.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     4826 2023-04-07 12:16:30.000000 e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_routing.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.934518 e2e_cli-0.9.9.7/e2e_cli/cdn/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/cdn/__init__.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.934518 e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_actions/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-22 08:23:23.000000 e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_actions/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3135 2023-04-06 11:06:02.000000 e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_actions/cdn_action.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.934518 e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_crud/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-22 08:23:19.000000 e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_crud/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3698 2023-04-07 12:53:46.000000 e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_crud/cdn.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3500 2023-04-07 12:57:28.000000 e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_routing.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     6181 2023-04-07 12:18:27.000000 e2e_cli-0.9.9.7/e2e_cli/commands_routing.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/config/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/config/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     6580 2023-04-07 06:58:38.000000 e2e_cli-0.9.9.7/e2e_cli/config/config.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3144 2023-04-07 12:20:30.000000 e2e_cli-0.9.9.7/e2e_cli/config/config_routing.py
--rw-rw-r--   0 aman      (1000) aman      (1000)      372 2023-03-24 06:11:14.000000 e2e_cli-0.9.9.7/e2e_cli/config/config_service.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/core/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/core/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     2249 2023-04-07 09:55:24.000000 e2e_cli-0.9.9.7/e2e_cli/core/alias_service.py
--rw-rw-r--   0 aman      (1000) aman      (1000)      579 2023-04-07 13:00:14.000000 e2e_cli-0.9.9.7/e2e_cli/core/constants.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3639 2023-03-10 13:20:42.000000 e2e_cli-0.9.9.7/e2e_cli/core/error_logs_service.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     1797 2023-04-04 13:21:23.000000 e2e_cli-0.9.9.7/e2e_cli/core/help_messages.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3263 2023-04-06 09:53:11.000000 e2e_cli-0.9.9.7/e2e_cli/core/helper_service.py
--rw-rw-r--   0 aman      (1000) aman      (1000)      657 2023-04-04 12:06:28.000000 e2e_cli-0.9.9.7/e2e_cli/core/py_manager.py
--rw-rw-r--   0 aman      (1000) aman      (1000)      455 2023-03-21 09:56:43.000000 e2e_cli-0.9.9.7/e2e_cli/core/request_service.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/dbaas/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/dbaas/__init__.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_actions/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-22 08:23:07.000000 e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_actions/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     8272 2023-04-06 12:16:27.000000 e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_actions/dbaas_action.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_crud/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-22 08:23:03.000000 e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_crud/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     5221 2023-03-24 06:12:26.000000 e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_crud/dbaas.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     8922 2023-03-24 06:22:28.000000 e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_crud/dbaas_services.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     5410 2023-04-07 12:22:15.000000 e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_routing.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/docs/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/docs/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     7055 2023-04-07 12:44:52.000000 e2e_cli-0.9.9.7/e2e_cli/docs/e2e_cli.1
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/image/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-17 14:00:12.000000 e2e_cli-0.9.9.7/e2e_cli/image/__init__.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/image/image_crud/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-17 10:56:29.000000 e2e_cli-0.9.9.7/e2e_cli/image/image_crud/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3345 2023-04-06 12:57:23.000000 e2e_cli-0.9.9.7/e2e_cli/image/image_crud/image.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/image/image_listing/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-17 10:56:22.000000 e2e_cli-0.9.9.7/e2e_cli/image/image_listing/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     1365 2023-03-24 06:10:02.000000 e2e_cli-0.9.9.7/e2e_cli/image/image_listing/image_list.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     2813 2023-04-07 13:07:44.000000 e2e_cli-0.9.9.7/e2e_cli/image/image_routing.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/loadbalancer/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/loadbalancer/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     4406 2023-03-02 07:23:13.000000 e2e_cli-0.9.9.7/e2e_cli/loadbalancer/lb.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     1530 2023-04-06 13:10:48.000000 e2e_cli-0.9.9.7/e2e_cli/loadbalancer/lb_routing.py
--rw-rw-r--   0 aman      (1000) aman      (1000)    42484 2023-03-24 06:23:22.000000 e2e_cli-0.9.9.7/e2e_cli/loadbalancer/lb_services.py
--rw-rw-r--   0 aman      (1000) aman      (1000)    14058 2023-04-07 12:30:51.000000 e2e_cli-0.9.9.7/e2e_cli/main.py
--rw-rw-r--   0 aman      (1000) aman      (1000)      459 2023-03-31 06:51:42.000000 e2e_cli-0.9.9.7/e2e_cli/man_display.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/node/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/node/__init__.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/node/node_actions/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-17 08:09:56.000000 e2e_cli-0.9.9.7/e2e_cli/node/node_actions/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     8128 2023-04-07 11:42:29.000000 e2e_cli-0.9.9.7/e2e_cli/node/node_actions/node_action.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/node/node_crud/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-17 14:01:01.000000 e2e_cli-0.9.9.7/e2e_cli/node/node_crud/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     6680 2023-04-07 13:02:21.000000 e2e_cli-0.9.9.7/e2e_cli/node/node_crud/node.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3666 2023-03-24 06:25:30.000000 e2e_cli-0.9.9.7/e2e_cli/node/node_crud/node_listing_service.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     5561 2023-04-07 12:24:49.000000 e2e_cli-0.9.9.7/e2e_cli/node/node_routing.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/volumes/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-02-17 14:04:58.000000 e2e_cli-0.9.9.7/e2e_cli/volumes/__init__.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_actions/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-22 09:26:32.000000 e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_actions/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     1839 2023-03-24 06:28:30.000000 e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_actions/volumes_action.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_crud/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-22 09:26:32.000000 e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_crud/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3930 2023-04-07 12:54:01.000000 e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_crud/volumes.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3158 2023-04-07 12:25:51.000000 e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_routing.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.938518 e2e_cli-0.9.9.7/e2e_cli/vpc/
--rw-rw-r--   0 aman      (1000) aman      (1000)        0 2023-03-22 08:29:40.000000 e2e_cli-0.9.9.7/e2e_cli/vpc/__init__.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     3510 2023-04-06 13:38:49.000000 e2e_cli-0.9.9.7/e2e_cli/vpc/vpc.py
--rw-rw-r--   0 aman      (1000) aman      (1000)     2474 2023-04-07 12:27:10.000000 e2e_cli-0.9.9.7/e2e_cli/vpc/vpc_routing.py
-drwxrwxr-x   0 aman      (1000) aman      (1000)        0 2023-04-07 13:47:15.934518 e2e_cli-0.9.9.7/e2e_cli.egg-info/
--rw-rw-r--   0 aman      (1000) aman      (1000)      372 2023-04-07 13:47:15.000000 e2e_cli-0.9.9.7/e2e_cli.egg-info/PKG-INFO
--rw-rw-r--   0 aman      (1000) aman      (1000)     2450 2023-04-07 13:47:15.000000 e2e_cli-0.9.9.7/e2e_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 aman      (1000) aman      (1000)        1 2023-04-07 13:47:15.000000 e2e_cli-0.9.9.7/e2e_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 aman      (1000) aman      (1000)       57 2023-04-07 13:47:15.000000 e2e_cli-0.9.9.7/e2e_cli.egg-info/entry_points.txt
--rw-rw-r--   0 aman      (1000) aman      (1000)       40 2023-04-07 13:47:15.000000 e2e_cli-0.9.9.7/e2e_cli.egg-info/requires.txt
--rw-rw-r--   0 aman      (1000) aman      (1000)        8 2023-04-07 13:47:15.000000 e2e_cli-0.9.9.7/e2e_cli.egg-info/top_level.txt
--rw-rw-r--   0 aman      (1000) aman      (1000)      432 2023-03-30 07:14:12.000000 e2e_cli-0.9.9.7/install_man.py
--rw-rw-r--   0 aman      (1000) aman      (1000)       38 2023-04-07 13:47:15.942518 e2e_cli-0.9.9.7/setup.cfg
--rw-rw-r--   0 aman      (1000) aman      (1000)      954 2023-04-07 13:47:09.000000 e2e_cli-0.9.9.7/setup.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.011713 e2e_cli-0.9.9.8/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/LICENSE
+-rw-r--r--   0 aman       (501) staff       (20)       31 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/MANIFEST.in
+-rw-r--r--   0 aman       (501) staff       (20)     2570 2023-04-19 10:42:06.011517 e2e_cli-0.9.9.8/PKG-INFO
+-rw-r--r--   0 aman       (501) staff       (20)     6237 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/README.md
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.996072 e2e_cli-0.9.9.8/e2e_cli/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.998082 e2e_cli-0.9.9.8/e2e_cli/auto_scaling/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/auto_scaling/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     4068 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/auto_scaling/auto_scaling.py
+-rw-r--r--   0 aman       (501) staff       (20)     2315 2023-04-19 08:31:18.000000 e2e_cli-0.9.9.8/e2e_cli/auto_scaling/autoscaling_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.998475 e2e_cli-0.9.9.8/e2e_cli/bucket_store/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.998904 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     8272 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_actions/bucket_actions.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.999486 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     4074 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_crud/bucket_storage.py
+-rw-r--r--   0 aman       (501) staff       (20)     5074 2023-04-19 08:32:45.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.999962 e2e_cli-0.9.9.8/e2e_cli/cdn/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.000383 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     3135 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_actions/cdn_action.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.000791 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     3698 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_crud/cdn.py
+-rw-r--r--   0 aman       (501) staff       (20)     3748 2023-04-19 08:32:53.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_routing.py
+-rw-r--r--   0 aman       (501) staff       (20)     6481 2023-04-19 08:39:16.000000 e2e_cli-0.9.9.8/e2e_cli/commands_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.001624 e2e_cli-0.9.9.8/e2e_cli/config/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/config/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     6580 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/config/config.py
+-rw-r--r--   0 aman       (501) staff       (20)     3208 2023-04-19 08:35:40.000000 e2e_cli-0.9.9.8/e2e_cli/config/config_routing.py
+-rw-r--r--   0 aman       (501) staff       (20)      372 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/config/config_service.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.003341 e2e_cli-0.9.9.8/e2e_cli/core/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     2249 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/alias_service.py
+-rw-r--r--   0 aman       (501) staff       (20)     1978 2023-04-19 07:52:48.000000 e2e_cli-0.9.9.8/e2e_cli/core/constants.py
+-rw-r--r--   0 aman       (501) staff       (20)     3639 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/error_logs_service.py
+-rw-r--r--   0 aman       (501) staff       (20)     1797 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/help_messages.py
+-rw-r--r--   0 aman       (501) staff       (20)     3263 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/helper_service.py
+-rw-r--r--   0 aman       (501) staff       (20)      657 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/py_manager.py
+-rw-r--r--   0 aman       (501) staff       (20)      455 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/request_service.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.003734 e2e_cli-0.9.9.8/e2e_cli/dbaas/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.004159 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     8272 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_actions/dbaas_action.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.004779 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     5221 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/dbaas.py
+-rw-r--r--   0 aman       (501) staff       (20)     8922 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/dbaas_services.py
+-rw-r--r--   0 aman       (501) staff       (20)     5658 2023-04-19 08:33:02.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.005194 e2e_cli-0.9.9.8/e2e_cli/docs/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/docs/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     7055 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/docs/e2e_cli.1
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.005577 e2e_cli-0.9.9.8/e2e_cli/image/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.005961 e2e_cli-0.9.9.8/e2e_cli/image/image_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     3345 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_crud/image.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.006389 e2e_cli-0.9.9.8/e2e_cli/image/image_listing/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_listing/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     1365 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_listing/image_list.py
+-rw-r--r--   0 aman       (501) staff       (20)     2989 2023-04-19 08:31:18.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.007405 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     4406 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb.py
+-rw-r--r--   0 aman       (501) staff       (20)     1745 2023-04-19 08:31:18.000000 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb_routing.py
+-rw-r--r--   0 aman       (501) staff       (20)    42484 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb_services.py
+-rw-r--r--   0 aman       (501) staff       (20)    15202 2023-04-19 08:59:40.000000 e2e_cli-0.9.9.8/e2e_cli/main.py
+-rw-r--r--   0 aman       (501) staff       (20)      459 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/man_display.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.007947 e2e_cli-0.9.9.8/e2e_cli/node/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.008369 e2e_cli-0.9.9.8/e2e_cli/node/node_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     8128 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_actions/node_action.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.009005 e2e_cli-0.9.9.8/e2e_cli/node/node_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     6680 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_crud/node.py
+-rw-r--r--   0 aman       (501) staff       (20)     3666 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_crud/node_listing_service.py
+-rw-r--r--   0 aman       (501) staff       (20)     5809 2023-04-19 08:32:06.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.009441 e2e_cli-0.9.9.8/e2e_cli/volumes/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.009865 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     1839 2023-04-18 10:34:31.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_actions/volumes_action.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.010458 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     3930 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_crud/volumes.py
+-rw-r--r--   0 aman       (501) staff       (20)     3406 2023-04-19 08:32:17.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.011155 e2e_cli-0.9.9.8/e2e_cli/vpc/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/vpc/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     3510 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/vpc/vpc.py
+-rw-r--r--   0 aman       (501) staff       (20)     2722 2023-04-19 08:32:26.000000 e2e_cli-0.9.9.8/e2e_cli/vpc/vpc_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.997356 e2e_cli-0.9.9.8/e2e_cli.egg-info/
+-rw-r--r--   0 aman       (501) staff       (20)     2570 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/PKG-INFO
+-rw-r--r--   0 aman       (501) staff       (20)     2435 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 aman       (501) staff       (20)        1 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 aman       (501) staff       (20)       57 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/entry_points.txt
+-rw-r--r--   0 aman       (501) staff       (20)       40 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/requires.txt
+-rw-r--r--   0 aman       (501) staff       (20)        8 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/top_level.txt
+-rw-r--r--   0 aman       (501) staff       (20)       38 2023-04-19 10:42:06.011794 e2e_cli-0.9.9.8/setup.cfg
+-rw-r--r--   0 aman       (501) staff       (20)      950 2023-04-19 10:41:10.000000 e2e_cli-0.9.9.8/setup.py
```

### Comparing `e2e_cli-0.9.9.7/README.md` & `e2e_cli-0.9.9.8/README.md`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/auto_scaling/auto_scaling.py` & `e2e_cli-0.9.9.8/e2e_cli/auto_scaling/auto_scaling.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/auto_scaling/autoscaling_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/auto_scaling/autoscaling_routing.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,17 @@
     def __init__(self, arguments):
         self.arguments = arguments
         
         
     def route(self, Parsing_Errors):
         if (self.arguments.args.autoscaling_commands is None):
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', 'autoscaling', '-h'])
 
         # elif (self.arguments.args.autoscaling_commands is not None) and (self.arguments.args.action is not None):
         #       Py_version_manager.py_print("Only one action at a time !!")
 
         elif(self.arguments.args.autoscaling_commands is not None):
             auto_scaling_operations = autoscaling_Crud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
@@ -39,8 +41,9 @@
                                 except KeyboardInterrupt:
                                     Py_version_manager.py_print(" ")
            
             
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_actions/bucket_actions.py` & `e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_actions/bucket_actions.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_crud/bucket_storage.py` & `e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_crud/bucket_storage.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/bucket_store/bucket_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_routing.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     def __init__(self, arguments):
         self.arguments = arguments
         
         
     def route(self, Parsing_Errors):
         if (self.arguments.args.bucket_commands is None) and (self.arguments.args.action is None):
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', 'bucket', '-h'])
 
 
         elif (self.arguments.args.bucket_commands is not None) and (self.arguments.args.action is not None):
               Py_version_manager.py_print("Only one action at a time !!")
 
 
@@ -94,13 +96,15 @@
                            Bucket_operations.add_permission()
                         except KeyboardInterrupt:
                             Py_version_manager.py_print(" ")
 
                 else:
                     Py_version_manager.py_print("command not found")
                     if(Parsing_Errors):
+                        Py_version_manager.py_print("Parsing Errors :")
                         Py_version_manager.py_print(*Parsing_Errors, sep="\n")
 
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_actions/cdn_action.py` & `e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_actions/cdn_action.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_crud/cdn.py` & `e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_crud/cdn.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/cdn/cdn_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_routing.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     def __init__(self, arguments):
         self.arguments = arguments
         
         
     def route(self, Parsing_Errors):
         if (self.arguments.args.action is None) and (self.arguments.args.cdn_commands is None):
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', 'cdn', '-h'])
 
 
         elif (self.arguments.args.cdn_commands is not None) and (self.arguments.args.action is not None):
               Py_version_manager.py_print("Only one action at a time !!")
 
 
@@ -70,14 +72,16 @@
                             cdn_operations.cdn_bandwidth_usage()
                         except KeyboardInterrupt:
                             Py_version_manager.py_print(" ")
                 
                 else:
                     Py_version_manager.py_print("command not found")
                     if(Parsing_Errors):
+                        Py_version_manager.py_print("Parsing Errors :")
                         Py_version_manager.py_print(*Parsing_Errors, sep="\n")
                 
 
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/commands_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/commands_routing.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 
         elif(self.arguments.args.info):
             help_messages.e2e_pakage_info()
 
 
         elif self.arguments.args.command is None:
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', "-h"])
 
 
         elif self.arguments.args.command == "help" :
                 man_page()
 
 
@@ -48,15 +50,17 @@
                     ConfigRouting(self.arguments).route(Parsing_Errors)
                 except Exception as e:
                     if("debug" in self.arguments.inputs):
                                 Checks.manage_exception(e)
                                 # action_on_exception(e, self.arguments.args.alias, traceback.print_exc())
             else:
                 if(Parsing_Errors):
+                    Py_version_manager.py_print("Parsing Errors :")
                     Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                    Py_version_manager.py_print("")
                 subprocess.call(['e2e_cli', "alias","-h"])
     
     
         else:
             if(self.arguments.args.alias=="default"):
                 Py_version_manager.py_print("Using default alias")
 
@@ -130,9 +134,10 @@
                             if("debug" in self.arguments.inputs):
                                 Checks.manage_exception(e)
                             # action_on_exception(e, self.arguments.args.alias, traceback.print_exc())  
 
             else:
                 Py_version_manager.py_print("Command not found!! for more help type e2e_cli help")
                 if(Parsing_Errors):
+                    Py_version_manager.py_print("Parsing Errors :")
                     Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/config/config.py` & `e2e_cli-0.9.9.8/e2e_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/config/config_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/config/config_routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,9 @@
                         Py_version_manager.py_print(" ")
                         pass
 
 
         else:
             Py_version_manager.py_print("Command not found!!")
             if(Parsing_errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/core/alias_service.py` & `e2e_cli-0.9.9.8/e2e_cli/core/alias_service.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/core/error_logs_service.py` & `e2e_cli-0.9.9.8/e2e_cli/core/error_logs_service.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/core/help_messages.py` & `e2e_cli-0.9.9.8/e2e_cli/core/help_messages.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/core/helper_service.py` & `e2e_cli-0.9.9.8/e2e_cli/core/helper_service.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/core/py_manager.py` & `e2e_cli-0.9.9.8/e2e_cli/core/py_manager.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_actions/dbaas_action.py` & `e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_actions/dbaas_action.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_crud/dbaas.py` & `e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/dbaas.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_crud/dbaas_services.py` & `e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/dbaas_services.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/dbaas/dbaas_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 class DBaaSRouting:
     def __init__(self, arguments):
         self.arguments = arguments
 
     def route(self, Parsing_Errors):
         if (self.arguments.args.dbaas_commands is None) and (self.arguments.args.action is None):
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli','dbaas', '-h'])
 
 
         elif (self.arguments.args.dbaas_commands is not None) and (self.arguments.args.action is not None):
               Py_version_manager.py_print("Only one action at a time !!")
 
 
@@ -112,14 +114,16 @@
                            DBaas_operations.remove_vpc()
                         except KeyboardInterrupt:
                             Py_version_manager.py_print(" ")
                 
                 else:
                     Py_version_manager.py_print("command not found")
                     if(Parsing_Errors):
+                        Py_version_manager.py_print("Parsing Errors :")
                         Py_version_manager.py_print(*Parsing_Errors, sep="\n")
                 
 
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/docs/e2e_cli.1` & `e2e_cli-0.9.9.8/e2e_cli/docs/e2e_cli.1`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/image/image_crud/image.py` & `e2e_cli-0.9.9.8/e2e_cli/image/image_crud/image.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/image/image_listing/image_list.py` & `e2e_cli-0.9.9.8/e2e_cli/image/image_listing/image_list.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/image/image_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/image/image_routing.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     def __init__(self, arguments):
         self.arguments = arguments
         
 
     def route(self, Parsing_Errors):
         if (self.arguments.args.image_commands is None) and (self.arguments.args.list_by is None):
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', 'image', '-h'])
 
 
         elif (self.arguments.args.image_commands is not None) and (self.arguments.args.list_by is not None):
             Py_version_manager.py_print("Only one action at a time !!")
 
 
@@ -55,8 +57,9 @@
         #                    image_operations.all()
         #                 except KeyboardInterrupt:
         #                     Py_version_manager.py_print(" ")
 
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/loadbalancer/lb.py` & `e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/loadbalancer/lb_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb_routing.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 class LBRouting:
     def __init__(self, arguments):
         self.arguments = arguments
 
     def route(self, Parsing_Errors):
         if self.arguments.args.lb_commands is None:
+            if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
+                Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', 'lb', '-h'])
 
 
         elif(self.arguments.args.lb_commands is not None):
             lb_class_object = LBClass(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
             
             if self.arguments.args.lb_commands == 'create':
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/loadbalancer/lb_services.py` & `e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb_services.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/main.py` & `e2e_cli-0.9.9.8/e2e_cli/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,143 +1,144 @@
 import argparse
 # import argcomplete working on auto-complete now 
 
 from e2e_cli.commands_routing import CommandsRouting
 from e2e_cli.core.error_logs_service import ErrorLogs
 from e2e_cli.core.py_manager import Py_version_manager
-from e2e_cli.core import help_messages
+from e2e_cli.core import help_messages, constants
 
 PARSING_ERROR_MSG=[]
 
 class Main:
+    # main class made for sub-commands/actions and formatting their usage
     def __init__(self):
         pass
 
     def FormatUsage(self, parser, action):
         if(action=="alias"):
-            format_string = "e2e_cli" + " alias" + " [-h]" + " {create,delete,list,edit/update} ... "
+            format_string = "e2e_cli" + " alias" + " [-h]" + " {add, add_file, delete, view, set}  "
         else:
-            format_string = "e2e_cli" + " --alias"+ " " + action + " [-h]" + " {create,delete,list,edit/update} ... "
+            format_string = "e2e_cli" + " --alias"+ " " + action + " [-h] " + action+"-command/--action  inputs... "
         parser.usage = format_string
 
-    def FormatUsageCommand(self, parser, action, command):
-        format_string = "e2e_cli" + " alias=" + "<alias_name>"+ " " + action + " [-h] " + command
-        parser.usage = format_string
+    # def FormatUsageCommand(self, parser, action, command):
+    #     format_string = "e2e_cli" + " alias=" + "<alias_name>"+ " " + action + " [-h] " + command
+    #     parser.usage = format_string
 
     def alias(self, parser):
         alias_sub_parser = parser.add_subparsers(title="Alias Commands", metavar="", dest="alias_commands")
         alias_add_sub_parser = alias_sub_parser.add_parser("add", help="To add api key and auth token")
         alias_file_sub_parser = alias_sub_parser.add_parser("add_file", help="To add api key and auth token via file")
         alias_delete_sub_parser = alias_sub_parser.add_parser("delete", help="To delete api key and auth token")
         alias_view_sub_parser = alias_sub_parser.add_parser("view", help="To view all alias and credentials")
         alias_set_default_sub_parser = alias_sub_parser.add_parser("set", help="To set default alias for system")
-        self.FormatUsageCommand(alias_add_sub_parser, "alias", "add")
-        self.FormatUsageCommand(alias_file_sub_parser, "alias", "add_file")
-        self.FormatUsageCommand(alias_delete_sub_parser, "alias", "delete")
-        self.FormatUsageCommand(alias_view_sub_parser, "alias", "view")
-        self.FormatUsageCommand(alias_set_default_sub_parser, "alias", "set")
+        # self.FormatUsageCommand(alias_add_sub_parser, "alias", "add")
+        # self.FormatUsageCommand(alias_file_sub_parser, "alias", "add_file")
+        # self.FormatUsageCommand(alias_delete_sub_parser, "alias", "delete")
+        # self.FormatUsageCommand(alias_view_sub_parser, "alias", "view")
+        # self.FormatUsageCommand(alias_set_default_sub_parser, "alias", "set")
 
     def node(self, parser):
         node_sub_parser = parser.add_subparsers(title="Node Commands", metavar="", dest="node_commands")
-        node_action=parser.add_argument('--action', help="Type of action to be performed your node")
+        node_action=parser.add_argument('-action', '--action', choices=constants.NODE_ACTIONS, metavar="", help="Actions on node are : "+constants.NODE_ACTIONS_STR)
         node_create_sub_parser = node_sub_parser.add_parser("create", help="To create a new node", formatter_class=help_messages.cli_formatter())
         node_delete_sub_parser = node_sub_parser.add_parser("delete", help="To delete a specific node", formatter_class=help_messages.cli_formatter())
         node_list_sub_parser = node_sub_parser.add_parser("list", help="To get a list of all nodes", formatter_class=help_messages.cli_formatter())
         node_get_sub_parser = node_sub_parser.add_parser("get", help="To get a list of all nodes", formatter_class=help_messages.cli_formatter())
-        self.FormatUsageCommand(node_action, "node", "actions")
-        self.FormatUsageCommand(node_create_sub_parser, "node", "create")
-        self.FormatUsageCommand(node_delete_sub_parser, "node", "delete")
-        self.FormatUsageCommand(node_list_sub_parser, "node", "list")
-        self.FormatUsageCommand(node_get_sub_parser, "node", "get")
+        # self.FormatUsageCommand(node_action, "node", "actions")
+        # self.FormatUsageCommand(node_create_sub_parser, "node", "create")
+        # self.FormatUsageCommand(node_delete_sub_parser, "node", "delete")
+        # self.FormatUsageCommand(node_list_sub_parser, "node", "list")
+        # self.FormatUsageCommand(node_get_sub_parser, "node", "get")
 
     def image(self, parser):
         image_sub_parser = parser.add_subparsers(title="Image Commands", metavar="", dest="image_commands")
-        image_list=parser.add_argument('--list_by', help="attribute/property by which you want to list images")
+        # image_list=parser.add_argument('--list_by', help="attribute/property by which you want to list images")
         image_create_sub_parser = image_sub_parser.add_parser("create", help="To create a new image")
         image_delete_sub_parser = image_sub_parser.add_parser("delete", help="To delete a specific image")
         image_list_sub_parser = image_sub_parser.add_parser("list", help="To get a list of all image")
         image_get_sub_parser = image_sub_parser.add_parser("rename", help="To rename a specific image")
-        self.FormatUsageCommand(image_list, "image", "list_by")
-        self.FormatUsageCommand(image_create_sub_parser, "image", "create")
-        self.FormatUsageCommand(image_delete_sub_parser, "image", "delete")
-        self.FormatUsageCommand(image_list_sub_parser, "image", "list")
-        self.FormatUsageCommand(image_get_sub_parser, "image", "rename")
+        # self.FormatUsageCommand(image_list, "image", "list_by")
+        # self.FormatUsageCommand(image_create_sub_parser, "image", "create")
+        # self.FormatUsageCommand(image_delete_sub_parser, "image", "delete")
+        # self.FormatUsageCommand(image_list_sub_parser, "image", "list")
+        # self.FormatUsageCommand(image_get_sub_parser, "image", "rename")
 
     def lb(self, parser):
         node_sub_parser = parser.add_subparsers(title="LB Commands", metavar="", dest="lb_commands")
         node_create_sub_parser = node_sub_parser.add_parser("create", help="To create a new node", formatter_class=help_messages.cli_formatter())
         node_delete_sub_parser = node_sub_parser.add_parser("delete", help="To delete a specific node", formatter_class=help_messages.cli_formatter())
         node_list_sub_parser = node_sub_parser.add_parser("list", help="To get a list of all nodes", formatter_class=help_messages.cli_formatter())
         node_edit_sub_parser = node_sub_parser.add_parser("edit", help="To get a list of all nodes", formatter_class=help_messages.cli_formatter())
-        self.FormatUsageCommand(node_create_sub_parser, "node", "create")
-        self.FormatUsageCommand(node_delete_sub_parser, "node", "delete")
-        self.FormatUsageCommand(node_list_sub_parser, "node", "list")
-        self.FormatUsageCommand(node_edit_sub_parser, "node", "edit")
+        # self.FormatUsageCommand(node_create_sub_parser, "node", "create")
+        # self.FormatUsageCommand(node_delete_sub_parser, "node", "delete")
+        # self.FormatUsageCommand(node_list_sub_parser, "node", "list")
+        # self.FormatUsageCommand(node_edit_sub_parser, "node", "edit")
 
     def bucket(self, parser):
         bucket_sub_parser = parser.add_subparsers(title="Bucket Commands", metavar="", dest="bucket_commands")
-        bucket_action=parser.add_argument('--action', help="Type of action to be performed your bucket")
+        bucket_action=parser.add_argument('-action', '--action', choices=constants.BUCKET_ACTIONS, metavar="", help="Actions on bucket are : "+constants.BUCKET_ACTIONS_STR)
         bucket_create_sub_parser = bucket_sub_parser.add_parser("create", help="To create a new bucket")
         bucket_delete_sub_parser = bucket_sub_parser.add_parser("delete", help="To delete a specific bucket")
         bucket_delete_sub_parser = bucket_sub_parser.add_parser("list", help="To get a list of all buckets")
-        self.FormatUsageCommand(bucket_action, "bucket", "actions")
-        self.FormatUsageCommand(bucket_create_sub_parser, "bucket", "create")
-        self.FormatUsageCommand(bucket_delete_sub_parser, "bucket", "delete")
-        self.FormatUsageCommand(bucket_delete_sub_parser, "bucket", "list")    
+        # self.FormatUsageCommand(bucket_action, "bucket", "actions")
+        # self.FormatUsageCommand(bucket_create_sub_parser, "bucket", "create")
+        # self.FormatUsageCommand(bucket_delete_sub_parser, "bucket", "delete")
+        # self.FormatUsageCommand(bucket_delete_sub_parser, "bucket", "list")    
 
     def autoscaling(self, parser):
         autoscaling_sub_parser = parser.add_subparsers(title="Autoscaling Commands", metavar="", dest="autoscaling_commands")
         autoscaling_create_sub_parser = autoscaling_sub_parser.add_parser("create", help="To create a new bucket")
         autoscaling_delete_sub_parser = autoscaling_sub_parser.add_parser("delete", help="To delete a specific bucket")
         autoscaling_delete_sub_parser = autoscaling_sub_parser.add_parser("list", help="To get a list of all buckets")
-        self.FormatUsageCommand(autoscaling_create_sub_parser, "autoscaling", "create")
-        self.FormatUsageCommand(autoscaling_delete_sub_parser, "autoscaling", "delete")
-        self.FormatUsageCommand(autoscaling_delete_sub_parser, "autoscaling", "list")
+        # self.FormatUsageCommand(autoscaling_create_sub_parser, "autoscaling", "create")
+        # self.FormatUsageCommand(autoscaling_delete_sub_parser, "autoscaling", "delete")
+        # self.FormatUsageCommand(autoscaling_delete_sub_parser, "autoscaling", "list")
 
     def vpc(self, parser):
         vpc_sub_parser = parser.add_subparsers(title="VPC Commands", metavar="", dest="vpc_commands")
         vpc_create_sub_parser = vpc_sub_parser.add_parser("create", help="To create a new bucket")
         vpc_delete_sub_parser = vpc_sub_parser.add_parser("delete", help="To delete a specific bucket")
         vpc_delete_sub_parser = vpc_sub_parser.add_parser("list", help="To get a list of all buckets")
-        self.FormatUsageCommand(vpc_create_sub_parser, "vpc", "create")
-        self.FormatUsageCommand(vpc_delete_sub_parser, "vpc", "delete")
-        self.FormatUsageCommand(vpc_delete_sub_parser, "vpc", "list")
+        # self.FormatUsageCommand(vpc_create_sub_parser, "vpc", "create")
+        # self.FormatUsageCommand(vpc_delete_sub_parser, "vpc", "delete")
+        # self.FormatUsageCommand(vpc_delete_sub_parser, "vpc", "list")
 
     def cdn(self, parser):
         cdn_sub_parser = parser.add_subparsers(title="CDN Commands", metavar="", dest="cdn_commands")
-        cdn_action=parser.add_argument('--action', help="Type of action to be performed your cdn")
+        cdn_action=parser.add_argument('-action', '--action', choices=constants.CDN_ACTIONS, metavar="", help="Actions on CDN are : "+constants.CDN_ACTIONS_STR)
         cdn_create_sub_parser = cdn_sub_parser.add_parser("create", help="To create a new cdn")
         cdn_delete_sub_parser = cdn_sub_parser.add_parser("delete", help="To delete a specific cdn")
         cdn_delete_sub_parser = cdn_sub_parser.add_parser("list", help="To get a list of all cdn")
-        self.FormatUsageCommand(cdn_action, "cdn", "actions")
-        self.FormatUsageCommand(cdn_create_sub_parser, "cdn", "create")
-        self.FormatUsageCommand(cdn_delete_sub_parser, "cdn", "delete")
-        self.FormatUsageCommand(cdn_delete_sub_parser, "cdn", "list")
+        # self.FormatUsageCommand(cdn_action, "cdn", "actions")
+        # self.FormatUsageCommand(cdn_create_sub_parser, "cdn", "create")
+        # self.FormatUsageCommand(cdn_delete_sub_parser, "cdn", "delete")
+        # self.FormatUsageCommand(cdn_delete_sub_parser, "cdn", "list")
 
     def volumes(self, parser):
-        volumes_sub_parser = parser.add_subparsers(title="Volumes Commands", metavar="", dest="volumes_commands")
-        volumes_action=parser.add_argument('--action', help="Type of action to be performed your volumes")
+        volumes_sub_parser = parser.add_subparsers(title="Volume Commands", metavar="", dest="volumes_commands")
+        volumes_action=parser.add_argument('-action', '--action', help="Type of action to be performed your volumes")
         volumes_create_sub_parser = volumes_sub_parser.add_parser("create", help="To create a new volumes")
         volumes_delete_sub_parser = volumes_sub_parser.add_parser("delete", help="To delete a specific volumes")
         volumes_delete_sub_parser = volumes_sub_parser.add_parser("list", help="To get a list of all volumes")
-        self.FormatUsageCommand(volumes_action, "volumes", "actions")
-        self.FormatUsageCommand(volumes_create_sub_parser, "volumes", "create")
-        self.FormatUsageCommand(volumes_delete_sub_parser, "volumes", "delete")
-        self.FormatUsageCommand(volumes_delete_sub_parser, "volumes", "list")
+        # self.FormatUsageCommand(volumes_action, "volumes", "actions")
+        # self.FormatUsageCommand(volumes_create_sub_parser, "volumes", "create")
+        # self.FormatUsageCommand(volumes_delete_sub_parser, "volumes", "delete")
+        # self.FormatUsageCommand(volumes_delete_sub_parser, "volumes", "list")
            
     def dbaas(self, parser):
         dbaas_sub_parser = parser.add_subparsers(title="DBaaS Commands", metavar="", dest="dbaas_commands")
-        dbaas_action=parser.add_argument('--action', help="Type of action to be performed your dbaas")
+        dbaas_action=parser.add_argument('-action', '--action', choices=constants.DBAAS_ACTIONS, metavar="", help="Actions on dbaas are : "+constants.DBAAS_ACTIONS_STR)
         dbaas_create_sub_parser = dbaas_sub_parser.add_parser("create", help="To launch a new dbaas")
         dbaas_delete_sub_parser = dbaas_sub_parser.add_parser("delete", help="To delete a created dbaas")
         dbaas_list_sub_parser = dbaas_sub_parser.add_parser("list", help="To list all of your dbaas")
-        self.FormatUsageCommand(dbaas_action, "dbaas", "actions")
-        self.FormatUsageCommand(dbaas_create_sub_parser, "dbaas", "create")
-        self.FormatUsageCommand(dbaas_list_sub_parser, "dbaas", "list")
-        self.FormatUsageCommand(dbaas_delete_sub_parser, "dbaas", "delete")
+        # self.FormatUsageCommand(dbaas_action, "dbaas", "actions")
+        # self.FormatUsageCommand(dbaas_create_sub_parser, "dbaas", "create")
+        # self.FormatUsageCommand(dbaas_list_sub_parser, "dbaas", "list")
+        # self.FormatUsageCommand(dbaas_delete_sub_parser, "dbaas", "delete")
 
 
 class Namespace(argparse._AttributeHolder):
     """Simple object for storing attributes.
     copied and over-written/modified here for getting unrecognised commands/inputs
     """
 
@@ -151,14 +152,16 @@
         return vars(self) == vars(other)
 
     def __contains__(self, key):
         return key in self.__dict__
 
 
 class ArgPaser(argparse.ArgumentParser):
+    """Custom argparse for our E2E CLI
+    Specifically modified to collect API inputs needed"""
 
     # used to collect input values 
     def inputs_list(self, argv):
         inputs=Namespace()
         for element in argv:
             if "=" in element:
                     x=element.split("=")
@@ -178,26 +181,29 @@
     def error(self, message):
         args = {'prog': self.prog, 'message': message}
         if("unrecognized arguments" not in args["message"]):
                         PARSING_ERROR_MSG.append( args["message"])
 
 
 def commanding(parser):
-    sub_parsers = parser.add_subparsers(title="Commands", dest="command")
-    alias_parser = sub_parsers.add_parser("help", help="To view man doc")
-    alias_parser = sub_parsers.add_parser("alias", help="To add delete tokens" )
-    node_parser = sub_parsers.add_parser("node", help="To apply crud operations over Nodes")
-    lb_parser = sub_parsers.add_parser("lb", help="To apply operations over Load-Balancer")
-    bucket_parser = sub_parsers.add_parser("bucket", help="To create/delete/list buckets of the user")
-    dbaas_parser = sub_parsers.add_parser("dbaas", help="To perform operations over DBaaS service provided")
-    image_parser = sub_parsers.add_parser("image", help="To perform operations over Image service provided")
-    autoscaling_parser= sub_parsers.add_parser("autoscaling", help="To create/delete/list autoscaling for the user")
-    vpc_parser= sub_parsers.add_parser("vpc", help="To create/delete/list vpc for the user")
-    cdn_parser= sub_parsers.add_parser("cdn", help="To create/delete/list cdn for the user")
-    volumes_parser= sub_parsers.add_parser("volumes", help="To create/delete/list volume for the user")
+    sub_parsers = parser.add_subparsers(title="Commands", metavar="", dest="command")
+    parser.usage="e2e_cli [-h] [-v] [--info] [--alias ALIAS]  Command  ..."
+    
+    sub_parsers.add_parser("help", help="To view man doc", formatter_class=argparse.RawTextHelpFormatter)
+    alias_parser = sub_parsers.add_parser("alias", help="To add delete tokens", formatter_class=argparse.RawTextHelpFormatter)
+    node_parser = sub_parsers.add_parser("node", help="To apply crud operations over Nodes", formatter_class=argparse.RawTextHelpFormatter)
+    lb_parser = sub_parsers.add_parser("lb", help="To apply operations over Load-Balancer", formatter_class=argparse.RawTextHelpFormatter)
+    bucket_parser = sub_parsers.add_parser("bucket", help="To create/delete/list buckets of the user", formatter_class=argparse.RawTextHelpFormatter)
+    dbaas_parser = sub_parsers.add_parser("dbaas", help="To perform operations over DBaaS service provided", formatter_class=argparse.RawTextHelpFormatter)
+    image_parser = sub_parsers.add_parser("image", help="To perform operations over Image service provided", formatter_class=argparse.RawTextHelpFormatter)
+    autoscaling_parser= sub_parsers.add_parser("autoscaling", help="To create/delete/list autoscaling for the user", formatter_class=argparse.RawTextHelpFormatter)
+    vpc_parser= sub_parsers.add_parser("vpc", help="To create/delete/list vpc for the user", formatter_class=argparse.RawTextHelpFormatter)
+    cdn_parser= sub_parsers.add_parser("cdn", help="To create/delete/list cdn for the user", formatter_class=argparse.RawTextHelpFormatter)
+    volumes_parser= sub_parsers.add_parser("volume", help="To create/delete/list volume for the user", formatter_class=argparse.RawTextHelpFormatter)
+    
     m = Main()
     m.alias(alias_parser)
     m.bucket(bucket_parser)
     m.node(node_parser)
     m.dbaas(dbaas_parser)
     m.lb(lb_parser)
     m.image(image_parser)
@@ -214,22 +220,23 @@
     m.FormatUsage(autoscaling_parser, "autoscaling")
     m.FormatUsage(vpc_parser, "vpc")
     m.FormatUsage(cdn_parser, "cdn")
     m.FormatUsage(volumes_parser, "volumes")
 
 
 def run_main_class():
-    parser = ArgPaser(description="E2E CLI", formatter_class=help_messages.cli_formatter())
+    parser = ArgPaser(description="E2E CLI", formatter_class=argparse.RawTextHelpFormatter)
 
     #version, info, and alias to be taken first else default
     parser.add_argument("-v", "--version", action='store_true', help="To view version Info")
     parser.add_argument( "--info", action='store_true', help="To view package Info")
-    parser.add_argument("--alias", default="default", type=str, help="The name of your access credentials valid option")
+    parser.add_argument("--alias", default="default", type=str, help="The name of your access credentials")
 
     # parsing our commands for routing
+    # breakpoint()
     commanding(parser)
 
     # breakpoint()
     args = parser.parse_args()
     commands_route = CommandsRouting(args)
     commands_route.route(PARSING_ERROR_MSG)
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/node/node_actions/node_action.py` & `e2e_cli-0.9.9.8/e2e_cli/node/node_actions/node_action.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/node/node_crud/node.py` & `e2e_cli-0.9.9.8/e2e_cli/node/node_crud/node.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/node/node_crud/node_listing_service.py` & `e2e_cli-0.9.9.8/e2e_cli/node/node_crud/node_listing_service.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/node/node_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/node/node_routing.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     def __init__(self, arguments):
         self.arguments = arguments
         
 
     def route(self, Parsing_Errors):
         if (self.arguments.args.node_commands is None) and (self.arguments.args.action is None):
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli','node', '-h'])
 
 
         elif (self.arguments.args.node_commands is not None) and (self.arguments.args.action is not None):
               Py_version_manager.py_print("Only one action at a time !!")
 
 
@@ -115,14 +117,16 @@
                            Node_operations.node_monitoring()
                         except KeyboardInterrupt:
                             Py_version_manager.py_print(" ")
                 
                 else:
                     Py_version_manager.py_print("command not found")
                     if(Parsing_Errors):
+                        Py_version_manager.py_print("Parsing Errors :")
                         Py_version_manager.py_print(*Parsing_Errors, sep="\n")
 
 
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_actions/volumes_action.py` & `e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_actions/volumes_action.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_crud/volumes.py` & `e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_crud/volumes.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/volumes/volumes_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_routing.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     def __init__(self, arguments):
         self.arguments = arguments
         
         
     def route(self,  Parsing_Errors):
         if (self.arguments.args.action is None) and (self.arguments.args.volumes_commands is None):
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', 'volumes', '-h'])
 
 
         elif (self.arguments.args.volumes_commands is not None) and (self.arguments.args.action is not None):
               Py_version_manager.py_print("Only one action at a time !!")
 
 
@@ -41,14 +43,15 @@
                             volumes_operations.list_volumes()
                         except KeyboardInterrupt:
                             Py_version_manager.py_print(" ")
 
                 else:
                     Py_version_manager.py_print("command not found")
                     if(Parsing_Errors):
+                        Py_version_manager.py_print("Parsing Errors :")
                         Py_version_manager.py_print(*Parsing_Errors, sep="\n")
         # elif self.arguments.args.action == "attach_volume":
         #     volumes_operations = volumesActions(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
         #     if(volumes_operations.possible):
         #                 try:
         #                     volumes_operations.attach_volume()
         #                 except KeyboardInterrupt:
@@ -62,8 +65,9 @@
         #                 except KeyboardInterrupt:
         #                     Py_version_manager.py_print(" ")
         
         
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli/vpc/vpc.py` & `e2e_cli-0.9.9.8/e2e_cli/vpc/vpc.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.7/e2e_cli/vpc/vpc_routing.py` & `e2e_cli-0.9.9.8/e2e_cli/vpc/vpc_routing.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,17 @@
     def __init__(self, arguments):
         self.arguments = arguments
         
         
     def route(self, Parsing_Errors):
         if (self.arguments.args.vpc_commands is None):
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', 'vpc', '-h'])
 
 
         elif (self.arguments.args.vpc_commands is not None) and (self.arguments.args.action is not None):
             Py_version_manager.py_print("Only one action at a time !!")
 
 
@@ -44,13 +46,15 @@
                                     vpc_operations.list_vpc()
                                 except KeyboardInterrupt:
                                     Py_version_manager.py_print(" ")
 
                 else:
                     Py_version_manager.py_print("command not found")
                     if(Parsing_Errors):
+                        Py_version_manager.py_print("Parsing Errors :")
                         Py_version_manager.py_print(*Parsing_Errors, sep="\n")
 
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
+                Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.7/e2e_cli.egg-info/SOURCES.txt` & `e2e_cli-0.9.9.8/e2e_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-install_man.py
 setup.py
 e2e_cli/__init__.py
 e2e_cli/commands_routing.py
 e2e_cli/main.py
 e2e_cli/man_display.py
 e2e_cli.egg-info/PKG-INFO
 e2e_cli.egg-info/SOURCES.txt
```

### Comparing `e2e_cli-0.9.9.7/setup.py` & `e2e_cli-0.9.9.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-import subprocess
+import subprocess, os
+
 try:
   from setuptools import setup, find_packages
 except ImportError:
-  subprocess.call["pip","install","setuptools"]
+  subprocess.call(["pip","install","setuptools"])
   from setuptools import setup, find_packages
 
+with open( (os.path.dirname(__file__)+"/e2e_cli/docs/PyPi_description.md") , 'r') as f:
+      pypi_text=f.read()
+
 setup(
     name='e2e_cli',
-    version='0.9.9.7',
+    version='0.9.9.8',
     description="This a E2E CLI tool for myAccount",
     author="Sajal&Aman@E2E_Networks_Ltd",
     packages=find_packages(),
     install_requires=['prettytable', 'requests', 'setuptools', 'chardet'],
     
     long_description_content_type="text/markdown",
-    long_description="The  E2E  Command  Line  Interface is a unified tool to manage your E2E services. A command line tool developed by E2E Networks Ltd.",
+    long_description=pypi_text,
     
     include_package_data = True,
     package_data = {
         '': ['*.1'],
         '': ['docs/*.1'],
         'docs': ['*.1'],
     },
```

