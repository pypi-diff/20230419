# Comparing `tmp/pulumi_linode-3.9.0a1655503909.tar.gz` & `tmp/pulumi_linode-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_linode-3.9.0a1655503909.tar", last modified: Fri Jun 17 22:15:45 2022, max compression
+gzip compressed data, was "dist/pulumi_linode-3.9.1.tar", last modified: Thu Aug  4 09:25:58 2022, max compression
```

## Comparing `pulumi_linode-3.9.0a1655503909.tar` & `pulumi_linode-3.9.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/
--rw-r--r--   0 runner    (1001) docker     (121)     3178 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/
--rw-r--r--   0 runner    (1001) docker     (121)     6689 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   119647 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2751 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    12735 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/database_access_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)    50518 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/database_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (121)    43867 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)    48158 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (121)    41463 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/domain.py
--rw-r--r--   0 runner    (1001) docker     (121)    34493 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (121)    29919 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/firewall.py
--rw-r--r--   0 runner    (1001) docker     (121)    13637 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/firewall_device.py
--rw-r--r--   0 runner    (1001) docker     (121)     7499 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     9184 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_backups.py
--rw-r--r--   0 runner    (1001) docker     (121)     7968 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_engines.py
--rw-r--r--   0 runner    (1001) docker     (121)    18337 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (121)    15984 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     8583 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_mysql_backups.py
--rw-r--r--   0 runner    (1001) docker     (121)    17371 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (121)     8717 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (121)    10751 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     9684 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     6931 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (121)     8679 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     9288 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     4423 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_instance_backups.py
--rw-r--r--   0 runner    (1001) docker     (121)     8142 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     8105 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4632 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (121)     5251 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (121)     5998 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7100 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     7993 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_networking_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     6691 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)    12829 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6814 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     6106 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_object_storage_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     8382 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_region.py
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    12168 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_stack_script.py
--rw-r--r--   0 runner    (1001) docker     (121)    11189 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_stack_scripts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5229 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     6420 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_vlans.py
--rw-r--r--   0 runner    (1001) docker     (121)     7744 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)    30532 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/image.py
--rw-r--r--   0 runner    (1001) docker     (121)   102212 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)    19056 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/instance_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     8062 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/instance_shared_ips.py
--rw-r--r--   0 runner    (1001) docker     (121)    15169 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (121)    24288 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    24297 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)    59410 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    25772 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (121)    26959 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)    14634 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/object_storage_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    49764 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/object_storage_object.py
--rw-r--r--   0 runner    (1001) docker     (121)   182476 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    16647 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    11412 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/rdns.py
--rw-r--r--   0 runner    (1001) docker     (121)     9809 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    34547 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/stack_script.py
--rw-r--r--   0 runner    (1001) docker     (121)    17818 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/token.py
--rw-r--r--   0 runner    (1001) docker     (121)    40395 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/user.py
--rw-r--r--   0 runner    (1001) docker     (121)    22043 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3178 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/pulumi_linode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-06-17 22:15:45.000000 pulumi_linode-3.9.0a1655503909/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/
+-rw-r--r--   0 runner    (1001) docker     (121)     6689 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   119659 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12684 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/database_access_controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50467 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/database_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43816 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48107 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41412 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/domain.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34442 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29868 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13586 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/firewall_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7458 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9143 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_database_backups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7927 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_database_engines.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18296 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_database_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15943 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8542 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_database_mysql_backups.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17330 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8676 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10710 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9643 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6890 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8638 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9247 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_instance_backups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8101 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8064 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4591 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5210 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5957 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7059 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7952 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_networking_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6650 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12788 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6773 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6065 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_object_storage_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8341 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12127 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11148 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_stack_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6379 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_vlans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7703 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30481 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)   102161 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19005 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/instance_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8011 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/instance_shared_ips.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15118 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24237 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24246 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59359 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25721 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28300 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14583 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/object_storage_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49713 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/object_storage_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)   182488 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18243 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    11361 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/rdns.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9758 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34496 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17767 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/token.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40344 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25350 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/pulumi_linode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-08-04 09:25:58.000000 pulumi_linode-3.9.1/setup.py
```

### Comparing `pulumi_linode-3.9.0a1655503909/PKG-INFO` & `pulumi_linode-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_linode
-Version: 3.9.0a1655503909
+Version: 3.9.1
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Description: [![Actions Status](https://github.com/pulumi/pulumi-linode/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-linode/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Flinode.svg)](https://www.npmjs.com/package/@pulumi/linode)
```

### Comparing `pulumi_linode-3.9.0a1655503909/README.md` & `pulumi_linode-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/__init__.py` & `pulumi_linode-3.9.1/pulumi_linode/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/_inputs.py` & `pulumi_linode-3.9.1/pulumi_linode/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/_utilities.py` & `pulumi_linode-3.9.1/pulumi_linode/_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,25 @@
 _version = _get_semver_version()
 _version_str = str(_version)
 
 
 def get_version():
     return _version_str
 
+def get_resource_opts_defaults() -> pulumi.ResourceOptions:
+    return pulumi.ResourceOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
+
+def get_invoke_opts_defaults() -> pulumi.InvokeOptions:
+    return pulumi.InvokeOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
 
 def get_resource_args_opts(resource_args_type, resource_options_type, *args, **kwargs):
     """
     Return the resource args and options given the *args and **kwargs of a resource's
     __init__ method.
     """
 
@@ -230,7 +241,10 @@
             'args': args_list,
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
+
+def get_plugin_download_url():
+	return None
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/config/vars.py` & `pulumi_linode-3.9.1/pulumi_linode/config/vars.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 import types
@@ -18,14 +19,22 @@
     def api_version(self) -> Optional[str]:
         """
         An HTTP User-Agent Prefix to prepend in API requests.
         """
         return __config__.get('apiVersion') or _utilities.get_env('LINODE_API_VERSION')
 
     @property
+    def config_path(self) -> Optional[str]:
+        return __config__.get('configPath')
+
+    @property
+    def config_profile(self) -> Optional[str]:
+        return __config__.get('configProfile')
+
+    @property
     def event_poll_ms(self) -> Optional[int]:
         """
         The rate in milliseconds to poll for events.
         """
         return __config__.get_int('eventPollMs')
 
     @property
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/database_access_controls.py` & `pulumi_linode-3.9.1/pulumi_linode/database_access_controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['DatabaseAccessControlsArgs', 'DatabaseAccessControls']
@@ -209,20 +210,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  database_id: Optional[pulumi.Input[int]] = None,
                  database_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatabaseAccessControlsArgs.__new__(DatabaseAccessControlsArgs)
 
             if allow_lists is None and not opts.urn:
                 raise TypeError("Missing required property 'allow_lists'")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/database_mongodb.py` & `pulumi_linode-3.9.1/pulumi_linode/database_mongodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -846,20 +847,17 @@
                  label: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
                  storage_engine: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMongodbUpdatesArgs']]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatabaseMongodbArgs.__new__(DatabaseMongodbArgs)
 
             __props__.__dict__["allow_lists"] = allow_lists
             __props__.__dict__["cluster_size"] = cluster_size
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/database_mysql.py` & `pulumi_linode-3.9.1/pulumi_linode/database_mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -747,20 +748,17 @@
                  label: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  replication_type: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatabaseMysqlArgs.__new__(DatabaseMysqlArgs)
 
             __props__.__dict__["allow_lists"] = allow_lists
             __props__.__dict__["cluster_size"] = cluster_size
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/database_postgresql.py` & `pulumi_linode-3.9.1/pulumi_linode/database_postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -800,20 +801,17 @@
                  region: Optional[pulumi.Input[str]] = None,
                  replication_commit_type: Optional[pulumi.Input[str]] = None,
                  replication_type: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  updates: Optional[pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatabasePostgresqlArgs.__new__(DatabasePostgresqlArgs)
 
             __props__.__dict__["allow_lists"] = allow_lists
             __props__.__dict__["cluster_size"] = cluster_size
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/domain.py` & `pulumi_linode-3.9.1/pulumi_linode/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['DomainArgs', 'Domain']
@@ -586,20 +587,17 @@
                  retry_sec: Optional[pulumi.Input[int]] = None,
                  soa_email: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ttl_sec: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DomainArgs.__new__(DomainArgs)
 
             __props__.__dict__["axfr_ips"] = axfr_ips
             __props__.__dict__["description"] = description
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/domain_record.py` & `pulumi_linode-3.9.1/pulumi_linode/domain_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['DomainRecordArgs', 'DomainRecord']
@@ -507,20 +508,17 @@
                  record_type: Optional[pulumi.Input[str]] = None,
                  service: Optional[pulumi.Input[str]] = None,
                  tag: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None,
                  ttl_sec: Optional[pulumi.Input[int]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DomainRecordArgs.__new__(DomainRecordArgs)
 
             if domain_id is None and not opts.urn:
                 raise TypeError("Missing required property 'domain_id'")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/firewall.py` & `pulumi_linode-3.9.1/pulumi_linode/firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -502,20 +503,17 @@
                  inbounds: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallInboundArgs']]]]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  linodes: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  outbound_policy: Optional[pulumi.Input[str]] = None,
                  outbounds: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallOutboundArgs']]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FirewallArgs.__new__(FirewallArgs)
 
             __props__.__dict__["disabled"] = disabled
             if inbound_policy is None and not opts.urn:
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/firewall_device.py` & `pulumi_linode-3.9.1/pulumi_linode/firewall_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['FirewallDeviceInitArgs', 'FirewallDevice']
@@ -252,20 +253,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  entity_id: Optional[pulumi.Input[int]] = None,
                  entity_type: Optional[pulumi.Input[str]] = None,
                  firewall_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FirewallDeviceInitArgs.__new__(FirewallDeviceInitArgs)
 
             if entity_id is None and not opts.urn:
                 raise TypeError("Missing required property 'entity_id'")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_account.py` & `pulumi_linode-3.9.1/pulumi_linode/get_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -191,18 +192,15 @@
     * `country` - The two-letter country code of this Account's billing address.
 
     * `zip` - The zip code of this Account's billing address.
 
     * `balance` - This Account's balance, in US dollars.
     """
     __args__ = dict()
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getAccount:getAccount', __args__, opts=opts, typ=GetAccountResult).value
 
     return AwaitableGetAccountResult(
         address1=__ret__.address1,
         address2=__ret__.address2,
         balance=__ret__.balance,
         city=__ret__.city,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_backups.py` & `pulumi_linode-3.9.1/pulumi_linode/get_database_backups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -165,18 +166,15 @@
     __args__ = dict()
     __args__['databaseId'] = database_id
     __args__['databaseType'] = database_type
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseBackups:getDatabaseBackups', __args__, opts=opts, typ=GetDatabaseBackupsResult).value
 
     return AwaitableGetDatabaseBackupsResult(
         backups=__ret__.backups,
         database_id=__ret__.database_id,
         database_type=__ret__.database_type,
         filters=__ret__.filters,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_engines.py` & `pulumi_linode-3.9.1/pulumi_linode/get_database_engines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -154,18 +155,15 @@
     :param str order_by: The attribute to order the results by. (`version`)
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseEngines:getDatabaseEngines', __args__, opts=opts, typ=GetDatabaseEnginesResult).value
 
     return AwaitableGetDatabaseEnginesResult(
         engines=__ret__.engines,
         filters=__ret__.filters,
         id=__ret__.id,
         latest=__ret__.latest,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_mongodb.py` & `pulumi_linode-3.9.1/pulumi_linode/get_database_mongodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -351,18 +352,15 @@
     * `week_of_month` - The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
 
     :param int database_id: The ID of the MongoDB database.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseMongodb:getDatabaseMongodb', __args__, opts=opts, typ=GetDatabaseMongodbResult).value
 
     return AwaitableGetDatabaseMongodbResult(
         allow_lists=__ret__.allow_lists,
         ca_cert=__ret__.ca_cert,
         cluster_size=__ret__.cluster_size,
         compression_type=__ret__.compression_type,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_mysql.py` & `pulumi_linode-3.9.1/pulumi_linode/get_database_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -307,18 +308,15 @@
     * `week_of_month` - The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
 
     :param int database_id: The ID of the MySQL database.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseMysql:getDatabaseMysql', __args__, opts=opts, typ=GetDatabaseMysqlResult).value
 
     return AwaitableGetDatabaseMysqlResult(
         allow_lists=__ret__.allow_lists,
         ca_cert=__ret__.ca_cert,
         cluster_size=__ret__.cluster_size,
         created=__ret__.created,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_mysql_backups.py` & `pulumi_linode-3.9.1/pulumi_linode/get_database_mysql_backups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -153,18 +154,15 @@
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseMysqlBackups:getDatabaseMysqlBackups', __args__, opts=opts, typ=GetDatabaseMysqlBackupsResult).value
 
     return AwaitableGetDatabaseMysqlBackupsResult(
         backups=__ret__.backups,
         database_id=__ret__.database_id,
         filters=__ret__.filters,
         id=__ret__.id,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_database_postgresql.py` & `pulumi_linode-3.9.1/pulumi_linode/get_database_postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -327,18 +328,15 @@
     * `week_of_month` - The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
 
     :param int database_id: The ID of the PostgreSQL database.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabasePostgresql:getDatabasePostgresql', __args__, opts=opts, typ=GetDatabasePostgresqlResult).value
 
     return AwaitableGetDatabasePostgresqlResult(
         allow_lists=__ret__.allow_lists,
         ca_cert=__ret__.ca_cert,
         cluster_size=__ret__.cluster_size,
         created=__ret__.created,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_databases.py` & `pulumi_linode-3.9.1/pulumi_linode/get_databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -162,18 +163,15 @@
     :param str order_by: The attribute to order the results by. (`version`)
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabases:getDatabases', __args__, opts=opts, typ=GetDatabasesResult).value
 
     return AwaitableGetDatabasesResult(
         databases=__ret__.databases,
         filters=__ret__.filters,
         id=__ret__.id,
         latest=__ret__.latest,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_domain.py` & `pulumi_linode-3.9.1/pulumi_linode/get_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -209,18 +210,15 @@
 
     :param str domain: The unique domain name of the Domain record to query.
     :param str id: The unique numeric ID of the Domain record to query.
     """
     __args__ = dict()
     __args__['domain'] = domain
     __args__['id'] = id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDomain:getDomain', __args__, opts=opts, typ=GetDomainResult).value
 
     return AwaitableGetDomainResult(
         axfr_ips=__ret__.axfr_ips,
         description=__ret__.description,
         domain=__ret__.domain,
         expire_sec=__ret__.expire_sec,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_domain_record.py` & `pulumi_linode-3.9.1/pulumi_linode/get_domain_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -192,18 +193,15 @@
     :param int id: The unique ID of the Domain Record.
     :param str name: The name of the Record.
     """
     __args__ = dict()
     __args__['domainId'] = domain_id
     __args__['id'] = id
     __args__['name'] = name
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDomainRecord:getDomainRecord', __args__, opts=opts, typ=GetDomainRecordResult).value
 
     return AwaitableGetDomainRecordResult(
         domain_id=__ret__.domain_id,
         id=__ret__.id,
         name=__ret__.name,
         port=__ret__.port,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_firewall.py` & `pulumi_linode-3.9.1/pulumi_linode/get_firewall.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -170,18 +171,15 @@
     ```
 
 
     :param int id: The Firewall's ID.
     """
     __args__ = dict()
     __args__['id'] = id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getFirewall:getFirewall', __args__, opts=opts, typ=GetFirewallResult).value
 
     return AwaitableGetFirewallResult(
         devices=__ret__.devices,
         disabled=__ret__.disabled,
         id=__ret__.id,
         inbound_policy=__ret__.inbound_policy,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_image.py` & `pulumi_linode-3.9.1/pulumi_linode/get_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -179,18 +180,15 @@
     * `vendor` - The upstream distribution vendor. `None` for private Images.
 
 
     :param str id: The unique ID of this Image.  The ID of private images begin with `private/` followed by the numeric identifier of the private image, for example `private/12345`.
     """
     __args__ = dict()
     __args__['id'] = id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getImage:getImage', __args__, opts=opts, typ=GetImageResult).value
 
     return AwaitableGetImageResult(
         created=__ret__.created,
         created_by=__ret__.created_by,
         deprecated=__ret__.deprecated,
         description=__ret__.description,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_images.py` & `pulumi_linode-3.9.1/pulumi_linode/get_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -178,18 +179,15 @@
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getImages:getImages', __args__, opts=opts, typ=GetImagesResult).value
 
     return AwaitableGetImagesResult(
         filters=__ret__.filters,
         id=__ret__.id,
         images=__ret__.images,
         latest=__ret__.latest,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_instance_backups.py` & `pulumi_linode-3.9.1/pulumi_linode/get_instance_backups.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -81,32 +82,20 @@
 
 
 def get_instance_backups(linode_id: Optional[int] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstanceBackupsResult:
     """
     Provides details about the backups of an Instance.
 
-    ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_linode as linode
-
-    my_backups = linode.get_instance_backups(id=123)
-    ```
-
 
     :param int linode_id: The Linode instance's ID.
     """
     __args__ = dict()
     __args__['linodeId'] = linode_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstanceBackups:getInstanceBackups', __args__, opts=opts, typ=GetInstanceBackupsResult).value
 
     return AwaitableGetInstanceBackupsResult(
         automatics=__ret__.automatics,
         currents=__ret__.currents,
         id=__ret__.id,
         in_progresses=__ret__.in_progresses,
@@ -115,20 +104,11 @@
 
 @_utilities.lift_output_func(get_instance_backups)
 def get_instance_backups_output(linode_id: Optional[pulumi.Input[int]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstanceBackupsResult]:
     """
     Provides details about the backups of an Instance.
 
-    ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_linode as linode
-
-    my_backups = linode.get_instance_backups(id=123)
-    ```
-
 
     :param int linode_id: The Linode instance's ID.
     """
     ...
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_instance_type.py` & `pulumi_linode-3.9.1/pulumi_linode/get_instance_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -168,18 +169,15 @@
 
 
     :param str id: Label used to identify instance type
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['label'] = label
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstanceType:getInstanceType', __args__, opts=opts, typ=GetInstanceTypeResult).value
 
     return AwaitableGetInstanceTypeResult(
         addons=__ret__.addons,
         class_=__ret__.class_,
         disk=__ret__.disk,
         id=__ret__.id,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_instance_types.py` & `pulumi_linode-3.9.1/pulumi_linode/get_instance_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -160,18 +161,15 @@
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['order'] = order
     __args__['orderBy'] = order_by
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstanceTypes:getInstanceTypes', __args__, opts=opts, typ=GetInstanceTypesResult).value
 
     return AwaitableGetInstanceTypesResult(
         filters=__ret__.filters,
         id=__ret__.id,
         order=__ret__.order,
         order_by=__ret__.order_by,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_instances.py` & `pulumi_linode-3.9.1/pulumi_linode/get_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -91,18 +92,15 @@
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['order'] = order
     __args__['orderBy'] = order_by
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstances:getInstances', __args__, opts=opts, typ=GetInstancesResult).value
 
     return AwaitableGetInstancesResult(
         filters=__ret__.filters,
         id=__ret__.id,
         instances=__ret__.instances,
         order=__ret__.order,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_ipv6_range.py` & `pulumi_linode-3.9.1/pulumi_linode/get_ipv6_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -116,18 +117,15 @@
     * `region` - The region for this range of IPv6 addresses.
 
 
     :param str range: The IPv6 range to retrieve information about.
     """
     __args__ = dict()
     __args__['range'] = range
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getIpv6Range:getIpv6Range', __args__, opts=opts, typ=GetIpv6RangeResult).value
 
     return AwaitableGetIpv6RangeResult(
         id=__ret__.id,
         is_bgp=__ret__.is_bgp,
         linodes=__ret__.linodes,
         prefix=__ret__.prefix,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_kernel.py` & `pulumi_linode-3.9.1/pulumi_linode/get_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -137,18 +138,15 @@
     * `xen` - If this Kernel is suitable for Xen Linodes.
 
 
     :param str id: The unique ID of this Kernel.
     """
     __args__ = dict()
     __args__['id'] = id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getKernel:getKernel', __args__, opts=opts, typ=GetKernelResult).value
 
     return AwaitableGetKernelResult(
         architecture=__ret__.architecture,
         deprecated=__ret__.deprecated,
         id=__ret__.id,
         kvm=__ret__.kvm,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_lke_cluster.py` & `pulumi_linode-3.9.1/pulumi_linode/get_lke_cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -173,18 +174,15 @@
     ```
 
 
     :param int id: The LKE Cluster's ID.
     """
     __args__ = dict()
     __args__['id'] = id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getLkeCluster:getLkeCluster', __args__, opts=opts, typ=GetLkeClusterResult).value
 
     return AwaitableGetLkeClusterResult(
         api_endpoints=__ret__.api_endpoints,
         control_planes=__ret__.control_planes,
         dashboard_url=__ret__.dashboard_url,
         id=__ret__.id,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_networking_ip.py` & `pulumi_linode-3.9.1/pulumi_linode/get_networking_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -162,18 +163,15 @@
     * `region` - The Region this IP address resides in. See all regions [here](https://api.linode.com/v4/regions).
 
 
     :param str address: The IP Address to access.  The address must be associated with the account and a resource that the user has access to view.
     """
     __args__ = dict()
     __args__['address'] = address
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getNetworkingIp:getNetworkingIp', __args__, opts=opts, typ=GetNetworkingIpResult).value
 
     return AwaitableGetNetworkingIpResult(
         address=__ret__.address,
         gateway=__ret__.gateway,
         id=__ret__.id,
         linode_id=__ret__.linode_id,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_node_balancer.py` & `pulumi_linode-3.9.1/pulumi_linode/get_node_balancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -164,18 +165,15 @@
     ```
 
 
     :param int id: The NodeBalancer's ID.
     """
     __args__ = dict()
     __args__['id'] = id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getNodeBalancer:getNodeBalancer', __args__, opts=opts, typ=GetNodeBalancerResult).value
 
     return AwaitableGetNodeBalancerResult(
         client_conn_throttle=__ret__.client_conn_throttle,
         created=__ret__.created,
         hostname=__ret__.hostname,
         id=__ret__.id,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_node_balancer_config.py` & `pulumi_linode-3.9.1/pulumi_linode/get_node_balancer_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -255,18 +256,15 @@
 
     :param int id: The config's ID.
     :param int nodebalancer_id: The ID of the NodeBalancer that contains the config.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['nodebalancerId'] = nodebalancer_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getNodeBalancerConfig:getNodeBalancerConfig', __args__, opts=opts, typ=GetNodeBalancerConfigResult).value
 
     return AwaitableGetNodeBalancerConfigResult(
         algorithm=__ret__.algorithm,
         check=__ret__.check,
         check_attempts=__ret__.check_attempts,
         check_body=__ret__.check_body,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_node_balancer_node.py` & `pulumi_linode-3.9.1/pulumi_linode/get_node_balancer_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -141,18 +142,15 @@
     :param int id: The node's ID.
     :param int nodebalancer_id: The ID of the NodeBalancer that contains the node.
     """
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['id'] = id
     __args__['nodebalancerId'] = nodebalancer_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getNodeBalancerNode:getNodeBalancerNode', __args__, opts=opts, typ=GetNodeBalancerNodeResult).value
 
     return AwaitableGetNodeBalancerNodeResult(
         address=__ret__.address,
         config_id=__ret__.config_id,
         id=__ret__.id,
         label=__ret__.label,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_object_storage_cluster.py` & `pulumi_linode-3.9.1/pulumi_linode/get_object_storage_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -112,18 +113,15 @@
     """
     __args__ = dict()
     __args__['domain'] = domain
     __args__['id'] = id
     __args__['region'] = region
     __args__['staticSiteDomain'] = static_site_domain
     __args__['status'] = status
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getObjectStorageCluster:getObjectStorageCluster', __args__, opts=opts, typ=GetObjectStorageClusterResult).value
 
     return AwaitableGetObjectStorageClusterResult(
         domain=__ret__.domain,
         id=__ret__.id,
         region=__ret__.region,
         static_site_domain=__ret__.static_site_domain,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_profile.py` & `pulumi_linode-3.9.1/pulumi_linode/get_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -180,18 +181,15 @@
     * `referrals.0.pending` - The number of pending signups for the referral code. To receive credit the signups must be completed.
 
     * `referrals.0.code` - The Profile referral code.  If new accounts use this when signing up for Linode, referring account will receive credit.
 
     * `referrals.0.url` - The referral URL.
     """
     __args__ = dict()
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getProfile:getProfile', __args__, opts=opts, typ=GetProfileResult).value
 
     return AwaitableGetProfileResult(
         authorized_keys=__ret__.authorized_keys,
         email=__ret__.email,
         email_notifications=__ret__.email_notifications,
         id=__ret__.id,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_region.py` & `pulumi_linode-3.9.1/pulumi_linode/get_region.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -72,18 +73,15 @@
 
     :param str country: The country the region resides in.
     :param str id: The code name of the region to select.
     """
     __args__ = dict()
     __args__['country'] = country
     __args__['id'] = id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getRegion:getRegion', __args__, opts=opts, typ=GetRegionResult).value
 
     return AwaitableGetRegionResult(
         country=__ret__.country,
         id=__ret__.id)
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_ssh_key.py` & `pulumi_linode-3.9.1/pulumi_linode/get_ssh_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -93,18 +94,15 @@
     ```
 
 
     :param str label: The label of the SSH Key to select.
     """
     __args__ = dict()
     __args__['label'] = label
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getSshKey:getSshKey', __args__, opts=opts, typ=GetSshKeyResult).value
 
     return AwaitableGetSshKeyResult(
         created=__ret__.created,
         id=__ret__.id,
         label=__ret__.label,
         ssh_key=__ret__.ssh_key)
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_stack_script.py` & `pulumi_linode-3.9.1/pulumi_linode/get_stack_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -219,18 +220,15 @@
 
 
     :param int id: The unique numeric ID of the StackScript to query.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['userDefinedFields'] = user_defined_fields
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getStackScript:getStackScript', __args__, opts=opts, typ=GetStackScriptResult).value
 
     return AwaitableGetStackScriptResult(
         created=__ret__.created,
         deployments_active=__ret__.deployments_active,
         deployments_total=__ret__.deployments_total,
         description=__ret__.description,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_stack_scripts.py` & `pulumi_linode-3.9.1/pulumi_linode/get_stack_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -189,18 +190,15 @@
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getStackScripts:getStackScripts', __args__, opts=opts, typ=GetStackScriptsResult).value
 
     return AwaitableGetStackScriptsResult(
         filters=__ret__.filters,
         id=__ret__.id,
         latest=__ret__.latest,
         order=__ret__.order,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_user.py` & `pulumi_linode-3.9.1/pulumi_linode/get_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -105,18 +106,15 @@
     * `restricted` - If true, this User must be granted access to perform actions or access entities on this Account.
 
 
     :param str username: The unique username of this User.
     """
     __args__ = dict()
     __args__['username'] = username
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
         email=__ret__.email,
         id=__ret__.id,
         restricted=__ret__.restricted,
         ssh_keys=__ret__.ssh_keys,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_vlans.py` & `pulumi_linode-3.9.1/pulumi_linode/get_vlans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -131,18 +132,15 @@
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['order'] = order
     __args__['orderBy'] = order_by
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getVlans:getVlans', __args__, opts=opts, typ=GetVlansResult).value
 
     return AwaitableGetVlansResult(
         filters=__ret__.filters,
         id=__ret__.id,
         order=__ret__.order,
         order_by=__ret__.order_by,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/get_volume.py` & `pulumi_linode-3.9.1/pulumi_linode/get_volume.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -161,18 +162,15 @@
     - `filesystem_path` - The full filesystem path for the Volume based on the Volume's label. Path is /dev/disk/by-id/scsi-0LinodeVolume + Volume label.
 
 
     :param int id: The unique numeric ID of the Volume record to query.
     """
     __args__ = dict()
     __args__['id'] = id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getVolume:getVolume', __args__, opts=opts, typ=GetVolumeResult).value
 
     return AwaitableGetVolumeResult(
         created=__ret__.created,
         filesystem_path=__ret__.filesystem_path,
         id=__ret__.id,
         label=__ret__.label,
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/image.py` & `pulumi_linode-3.9.1/pulumi_linode/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ImageArgs', 'Image']
@@ -513,20 +514,17 @@
                  disk_id: Optional[pulumi.Input[int]] = None,
                  file_hash: Optional[pulumi.Input[str]] = None,
                  file_path: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  linode_id: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ImageArgs.__new__(ImageArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["disk_id"] = disk_id
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/instance.py` & `pulumi_linode-3.9.1/pulumi_linode/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -1236,20 +1237,17 @@
                  stackscript_data: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  stackscript_id: Optional[pulumi.Input[int]] = None,
                  swap_size: Optional[pulumi.Input[int]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  watchdog_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
             __props__.__dict__["alerts"] = alerts
             __props__.__dict__["authorized_keys"] = authorized_keys
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/instance_ip.py` & `pulumi_linode-3.9.1/pulumi_linode/instance_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['InstanceIpArgs', 'InstanceIp']
@@ -334,20 +335,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  apply_immediately: Optional[pulumi.Input[bool]] = None,
                  linode_id: Optional[pulumi.Input[int]] = None,
                  public: Optional[pulumi.Input[bool]] = None,
                  rdns: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceIpArgs.__new__(InstanceIpArgs)
 
             __props__.__dict__["apply_immediately"] = apply_immediately
             if linode_id is None and not opts.urn:
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/instance_shared_ips.py` & `pulumi_linode-3.9.1/pulumi_linode/instance_shared_ips.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['InstanceSharedIpsArgs', 'InstanceSharedIps']
@@ -125,20 +126,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  linode_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceSharedIpsArgs.__new__(InstanceSharedIpsArgs)
 
             if addresses is None and not opts.urn:
                 raise TypeError("Missing required property 'addresses'")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/ipv6_range.py` & `pulumi_linode-3.9.1/pulumi_linode/ipv6_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['Ipv6RangeArgs', 'Ipv6Range']
@@ -259,20 +260,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  linode_id: Optional[pulumi.Input[int]] = None,
                  prefix_length: Optional[pulumi.Input[int]] = None,
                  route_target: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = Ipv6RangeArgs.__new__(Ipv6RangeArgs)
 
             __props__.__dict__["linode_id"] = linode_id
             if prefix_length is None and not opts.urn:
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/lke_cluster.py` & `pulumi_linode-3.9.1/pulumi_linode/lke_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -427,20 +428,17 @@
                  control_plane: Optional[pulumi.Input[pulumi.InputType['LkeClusterControlPlaneArgs']]] = None,
                  k8s_version: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  pools: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LkeClusterPoolArgs']]]]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = LkeClusterArgs.__new__(LkeClusterArgs)
 
             __props__.__dict__["control_plane"] = control_plane
             if k8s_version is None and not opts.urn:
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/node_balancer.py` & `pulumi_linode-3.9.1/pulumi_linode/node_balancer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -398,20 +399,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  client_conn_throttle: Optional[pulumi.Input[int]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NodeBalancerArgs.__new__(NodeBalancerArgs)
 
             __props__.__dict__["client_conn_throttle"] = client_conn_throttle
             __props__.__dict__["label"] = label
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/node_balancer_config.py` & `pulumi_linode-3.9.1/pulumi_linode/node_balancer_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -783,20 +784,17 @@
                  port: Optional[pulumi.Input[int]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  proxy_protocol: Optional[pulumi.Input[str]] = None,
                  ssl_cert: Optional[pulumi.Input[str]] = None,
                  ssl_key: Optional[pulumi.Input[str]] = None,
                  stickiness: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NodeBalancerConfigArgs.__new__(NodeBalancerConfigArgs)
 
             __props__.__dict__["algorithm"] = algorithm
             __props__.__dict__["check"] = check
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/node_balancer_node.py` & `pulumi_linode-3.9.1/pulumi_linode/node_balancer_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['NodeBalancerNodeArgs', 'NodeBalancerNode']
@@ -405,20 +406,17 @@
                  address: Optional[pulumi.Input[str]] = None,
                  config_id: Optional[pulumi.Input[int]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  mode: Optional[pulumi.Input[str]] = None,
                  nodebalancer_id: Optional[pulumi.Input[int]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NodeBalancerNodeArgs.__new__(NodeBalancerNodeArgs)
 
             if address is None and not opts.urn:
                 raise TypeError("Missing required property 'address'")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/object_storage_bucket.py` & `pulumi_linode-3.9.1/pulumi_linode/object_storage_bucket.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -166,25 +167,28 @@
 class _ObjectStorageBucketState:
     def __init__(__self__, *,
                  access_key: Optional[pulumi.Input[str]] = None,
                  acl: Optional[pulumi.Input[str]] = None,
                  cert: Optional[pulumi.Input['ObjectStorageBucketCertArgs']] = None,
                  cluster: Optional[pulumi.Input[str]] = None,
                  cors_enabled: Optional[pulumi.Input[bool]] = None,
+                 hostname: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  lifecycle_rules: Optional[pulumi.Input[Sequence[pulumi.Input['ObjectStorageBucketLifecycleRuleArgs']]]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  versioning: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering ObjectStorageBucket resources.
         :param pulumi.Input[str] access_key: The access key to authenticate with.
         :param pulumi.Input[str] acl: The Access Control Level of the bucket using a canned ACL string. See all ACL strings in the Linode API v4 documentation.
         :param pulumi.Input['ObjectStorageBucketCertArgs'] cert: The cert used by this Object Storage Bucket.
         :param pulumi.Input[str] cluster: The cluster of the Linode Object Storage Bucket.
         :param pulumi.Input[bool] cors_enabled: If true, the bucket will have CORS enabled for all origins.
+        :param pulumi.Input[str] hostname: The hostname where this bucket can be accessed. This hostname can be accessed through a browser if the bucket is made
+               public.
         :param pulumi.Input[str] label: The label of the Linode Object Storage Bucket.
         :param pulumi.Input[Sequence[pulumi.Input['ObjectStorageBucketLifecycleRuleArgs']]] lifecycle_rules: Lifecycle rules to be applied to the bucket.
         :param pulumi.Input[str] secret_key: The secret key to authenticate with.
         :param pulumi.Input[bool] versioning: Whether to enable versioning. Once you version-enable a bucket, it can never return to an unversioned state. You can, however, suspend versioning on that bucket. (Requires `access_key` and `secret_key`)
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
@@ -192,14 +196,16 @@
             pulumi.set(__self__, "acl", acl)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
         if cluster is not None:
             pulumi.set(__self__, "cluster", cluster)
         if cors_enabled is not None:
             pulumi.set(__self__, "cors_enabled", cors_enabled)
+        if hostname is not None:
+            pulumi.set(__self__, "hostname", hostname)
         if label is not None:
             pulumi.set(__self__, "label", label)
         if lifecycle_rules is not None:
             pulumi.set(__self__, "lifecycle_rules", lifecycle_rules)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if versioning is not None:
@@ -263,14 +269,27 @@
 
     @cors_enabled.setter
     def cors_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "cors_enabled", value)
 
     @property
     @pulumi.getter
+    def hostname(self) -> Optional[pulumi.Input[str]]:
+        """
+        The hostname where this bucket can be accessed. This hostname can be accessed through a browser if the bucket is made
+        public.
+        """
+        return pulumi.get(self, "hostname")
+
+    @hostname.setter
+    def hostname(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "hostname", value)
+
+    @property
+    @pulumi.getter
     def label(self) -> Optional[pulumi.Input[str]]:
         """
         The label of the Linode Object Storage Bucket.
         """
         return pulumi.get(self, "label")
 
     @label.setter
@@ -462,20 +481,17 @@
                  cluster: Optional[pulumi.Input[str]] = None,
                  cors_enabled: Optional[pulumi.Input[bool]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  lifecycle_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ObjectStorageBucketLifecycleRuleArgs']]]]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  versioning: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ObjectStorageBucketArgs.__new__(ObjectStorageBucketArgs)
 
             __props__.__dict__["access_key"] = access_key
             __props__.__dict__["acl"] = acl
@@ -486,14 +502,15 @@
             __props__.__dict__["cors_enabled"] = cors_enabled
             if label is None and not opts.urn:
                 raise TypeError("Missing required property 'label'")
             __props__.__dict__["label"] = label
             __props__.__dict__["lifecycle_rules"] = lifecycle_rules
             __props__.__dict__["secret_key"] = secret_key
             __props__.__dict__["versioning"] = versioning
+            __props__.__dict__["hostname"] = None
         super(ObjectStorageBucket, __self__).__init__(
             'linode:index/objectStorageBucket:ObjectStorageBucket',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -501,14 +518,15 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             access_key: Optional[pulumi.Input[str]] = None,
             acl: Optional[pulumi.Input[str]] = None,
             cert: Optional[pulumi.Input[pulumi.InputType['ObjectStorageBucketCertArgs']]] = None,
             cluster: Optional[pulumi.Input[str]] = None,
             cors_enabled: Optional[pulumi.Input[bool]] = None,
+            hostname: Optional[pulumi.Input[str]] = None,
             label: Optional[pulumi.Input[str]] = None,
             lifecycle_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ObjectStorageBucketLifecycleRuleArgs']]]]] = None,
             secret_key: Optional[pulumi.Input[str]] = None,
             versioning: Optional[pulumi.Input[bool]] = None) -> 'ObjectStorageBucket':
         """
         Get an existing ObjectStorageBucket resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
@@ -517,28 +535,31 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_key: The access key to authenticate with.
         :param pulumi.Input[str] acl: The Access Control Level of the bucket using a canned ACL string. See all ACL strings in the Linode API v4 documentation.
         :param pulumi.Input[pulumi.InputType['ObjectStorageBucketCertArgs']] cert: The cert used by this Object Storage Bucket.
         :param pulumi.Input[str] cluster: The cluster of the Linode Object Storage Bucket.
         :param pulumi.Input[bool] cors_enabled: If true, the bucket will have CORS enabled for all origins.
+        :param pulumi.Input[str] hostname: The hostname where this bucket can be accessed. This hostname can be accessed through a browser if the bucket is made
+               public.
         :param pulumi.Input[str] label: The label of the Linode Object Storage Bucket.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ObjectStorageBucketLifecycleRuleArgs']]]] lifecycle_rules: Lifecycle rules to be applied to the bucket.
         :param pulumi.Input[str] secret_key: The secret key to authenticate with.
         :param pulumi.Input[bool] versioning: Whether to enable versioning. Once you version-enable a bucket, it can never return to an unversioned state. You can, however, suspend versioning on that bucket. (Requires `access_key` and `secret_key`)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ObjectStorageBucketState.__new__(_ObjectStorageBucketState)
 
         __props__.__dict__["access_key"] = access_key
         __props__.__dict__["acl"] = acl
         __props__.__dict__["cert"] = cert
         __props__.__dict__["cluster"] = cluster
         __props__.__dict__["cors_enabled"] = cors_enabled
+        __props__.__dict__["hostname"] = hostname
         __props__.__dict__["label"] = label
         __props__.__dict__["lifecycle_rules"] = lifecycle_rules
         __props__.__dict__["secret_key"] = secret_key
         __props__.__dict__["versioning"] = versioning
         return ObjectStorageBucket(resource_name, opts=opts, __props__=__props__)
 
     @property
@@ -579,14 +600,23 @@
         """
         If true, the bucket will have CORS enabled for all origins.
         """
         return pulumi.get(self, "cors_enabled")
 
     @property
     @pulumi.getter
+    def hostname(self) -> pulumi.Output[str]:
+        """
+        The hostname where this bucket can be accessed. This hostname can be accessed through a browser if the bucket is made
+        public.
+        """
+        return pulumi.get(self, "hostname")
+
+    @property
+    @pulumi.getter
     def label(self) -> pulumi.Output[str]:
         """
         The label of the Linode Object Storage Bucket.
         """
         return pulumi.get(self, "label")
 
     @property
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/object_storage_key.py` & `pulumi_linode-3.9.1/pulumi_linode/object_storage_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -218,20 +219,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  bucket_accesses: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ObjectStorageKeyBucketAccessArgs']]]]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ObjectStorageKeyArgs.__new__(ObjectStorageKeyArgs)
 
             __props__.__dict__["bucket_accesses"] = bucket_accesses
             if label is None and not opts.urn:
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/object_storage_object.py` & `pulumi_linode-3.9.1/pulumi_linode/object_storage_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ObjectStorageObjectArgs', 'ObjectStorageObject']
@@ -736,20 +737,17 @@
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  metadata: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  source: Optional[pulumi.Input[str]] = None,
                  website_redirect: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ObjectStorageObjectArgs.__new__(ObjectStorageObjectArgs)
 
             if access_key is None and not opts.urn:
                 raise TypeError("Missing required property 'access_key'")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/outputs.py` & `pulumi_linode-3.9.1/pulumi_linode/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/provider.py` & `pulumi_linode-3.9.1/pulumi_linode/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,114 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
-                 token: pulumi.Input[str],
                  api_version: Optional[pulumi.Input[str]] = None,
+                 config_path: Optional[pulumi.Input[str]] = None,
+                 config_profile: Optional[pulumi.Input[str]] = None,
                  event_poll_ms: Optional[pulumi.Input[int]] = None,
                  lke_event_poll_ms: Optional[pulumi.Input[int]] = None,
                  lke_node_ready_poll_ms: Optional[pulumi.Input[int]] = None,
                  max_retry_delay_ms: Optional[pulumi.Input[int]] = None,
                  min_retry_delay_ms: Optional[pulumi.Input[int]] = None,
                  skip_instance_delete_poll: Optional[pulumi.Input[bool]] = None,
                  skip_instance_ready_poll: Optional[pulumi.Input[bool]] = None,
+                 token: Optional[pulumi.Input[str]] = None,
                  ua_prefix: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
-        :param pulumi.Input[str] token: The token that allows you access to your Linode account
         :param pulumi.Input[str] api_version: An HTTP User-Agent Prefix to prepend in API requests.
         :param pulumi.Input[int] event_poll_ms: The rate in milliseconds to poll for events.
         :param pulumi.Input[int] lke_event_poll_ms: The rate in milliseconds to poll for LKE events.
         :param pulumi.Input[int] lke_node_ready_poll_ms: The rate in milliseconds to poll for an LKE node to be ready.
         :param pulumi.Input[int] max_retry_delay_ms: Maximum delay in milliseconds before retrying a request.
         :param pulumi.Input[int] min_retry_delay_ms: Minimum delay in milliseconds before retrying a request.
         :param pulumi.Input[bool] skip_instance_delete_poll: Skip waiting for a linode_instance resource to finish deleting.
         :param pulumi.Input[bool] skip_instance_ready_poll: Skip waiting for a linode_instance resource to be running.
+        :param pulumi.Input[str] token: The token that allows you access to your Linode account
         :param pulumi.Input[str] ua_prefix: An HTTP User-Agent Prefix to prepend in API requests.
         :param pulumi.Input[str] url: The HTTP(S) API address of the Linode API to use.
         """
-        pulumi.set(__self__, "token", token)
         if api_version is None:
             api_version = _utilities.get_env('LINODE_API_VERSION')
         if api_version is not None:
             pulumi.set(__self__, "api_version", api_version)
+        if config_path is not None:
+            pulumi.set(__self__, "config_path", config_path)
+        if config_profile is not None:
+            pulumi.set(__self__, "config_profile", config_profile)
         if event_poll_ms is not None:
             pulumi.set(__self__, "event_poll_ms", event_poll_ms)
         if lke_event_poll_ms is not None:
             pulumi.set(__self__, "lke_event_poll_ms", lke_event_poll_ms)
         if lke_node_ready_poll_ms is not None:
             pulumi.set(__self__, "lke_node_ready_poll_ms", lke_node_ready_poll_ms)
         if max_retry_delay_ms is not None:
             pulumi.set(__self__, "max_retry_delay_ms", max_retry_delay_ms)
         if min_retry_delay_ms is not None:
             pulumi.set(__self__, "min_retry_delay_ms", min_retry_delay_ms)
         if skip_instance_delete_poll is not None:
             pulumi.set(__self__, "skip_instance_delete_poll", skip_instance_delete_poll)
         if skip_instance_ready_poll is not None:
             pulumi.set(__self__, "skip_instance_ready_poll", skip_instance_ready_poll)
+        if token is not None:
+            pulumi.set(__self__, "token", token)
         if ua_prefix is None:
             ua_prefix = _utilities.get_env('LINODE_UA_PREFIX')
         if ua_prefix is not None:
             pulumi.set(__self__, "ua_prefix", ua_prefix)
         if url is None:
             url = _utilities.get_env('LINODE_URL')
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
-    @pulumi.getter
-    def token(self) -> pulumi.Input[str]:
-        """
-        The token that allows you access to your Linode account
-        """
-        return pulumi.get(self, "token")
-
-    @token.setter
-    def token(self, value: pulumi.Input[str]):
-        pulumi.set(self, "token", value)
-
-    @property
     @pulumi.getter(name="apiVersion")
     def api_version(self) -> Optional[pulumi.Input[str]]:
         """
         An HTTP User-Agent Prefix to prepend in API requests.
         """
         return pulumi.get(self, "api_version")
 
     @api_version.setter
     def api_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_version", value)
 
     @property
+    @pulumi.getter(name="configPath")
+    def config_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "config_path")
+
+    @config_path.setter
+    def config_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "config_path", value)
+
+    @property
+    @pulumi.getter(name="configProfile")
+    def config_profile(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "config_profile")
+
+    @config_profile.setter
+    def config_profile(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "config_profile", value)
+
+    @property
     @pulumi.getter(name="eventPollMs")
     def event_poll_ms(self) -> Optional[pulumi.Input[int]]:
         """
         The rate in milliseconds to poll for events.
         """
         return pulumi.get(self, "event_poll_ms")
 
@@ -171,14 +185,26 @@
         return pulumi.get(self, "skip_instance_ready_poll")
 
     @skip_instance_ready_poll.setter
     def skip_instance_ready_poll(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "skip_instance_ready_poll", value)
 
     @property
+    @pulumi.getter
+    def token(self) -> Optional[pulumi.Input[str]]:
+        """
+        The token that allows you access to your Linode account
+        """
+        return pulumi.get(self, "token")
+
+    @token.setter
+    def token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "token", value)
+
+    @property
     @pulumi.getter(name="uaPrefix")
     def ua_prefix(self) -> Optional[pulumi.Input[str]]:
         """
         An HTTP User-Agent Prefix to prepend in API requests.
         """
         return pulumi.get(self, "ua_prefix")
 
@@ -201,14 +227,16 @@
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_version: Optional[pulumi.Input[str]] = None,
+                 config_path: Optional[pulumi.Input[str]] = None,
+                 config_profile: Optional[pulumi.Input[str]] = None,
                  event_poll_ms: Optional[pulumi.Input[int]] = None,
                  lke_event_poll_ms: Optional[pulumi.Input[int]] = None,
                  lke_node_ready_poll_ms: Optional[pulumi.Input[int]] = None,
                  max_retry_delay_ms: Optional[pulumi.Input[int]] = None,
                  min_retry_delay_ms: Optional[pulumi.Input[int]] = None,
                  skip_instance_delete_poll: Optional[pulumi.Input[bool]] = None,
                  skip_instance_ready_poll: Optional[pulumi.Input[bool]] = None,
@@ -236,15 +264,15 @@
         :param pulumi.Input[str] ua_prefix: An HTTP User-Agent Prefix to prepend in API requests.
         :param pulumi.Input[str] url: The HTTP(S) API address of the Linode API to use.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProviderArgs,
+                 args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The provider type for the linode package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
@@ -260,48 +288,47 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_version: Optional[pulumi.Input[str]] = None,
+                 config_path: Optional[pulumi.Input[str]] = None,
+                 config_profile: Optional[pulumi.Input[str]] = None,
                  event_poll_ms: Optional[pulumi.Input[int]] = None,
                  lke_event_poll_ms: Optional[pulumi.Input[int]] = None,
                  lke_node_ready_poll_ms: Optional[pulumi.Input[int]] = None,
                  max_retry_delay_ms: Optional[pulumi.Input[int]] = None,
                  min_retry_delay_ms: Optional[pulumi.Input[int]] = None,
                  skip_instance_delete_poll: Optional[pulumi.Input[bool]] = None,
                  skip_instance_ready_poll: Optional[pulumi.Input[bool]] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  ua_prefix: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             if api_version is None:
                 api_version = _utilities.get_env('LINODE_API_VERSION')
             __props__.__dict__["api_version"] = api_version
+            __props__.__dict__["config_path"] = config_path
+            __props__.__dict__["config_profile"] = config_profile
             __props__.__dict__["event_poll_ms"] = pulumi.Output.from_input(event_poll_ms).apply(pulumi.runtime.to_json) if event_poll_ms is not None else None
             __props__.__dict__["lke_event_poll_ms"] = pulumi.Output.from_input(lke_event_poll_ms).apply(pulumi.runtime.to_json) if lke_event_poll_ms is not None else None
             __props__.__dict__["lke_node_ready_poll_ms"] = pulumi.Output.from_input(lke_node_ready_poll_ms).apply(pulumi.runtime.to_json) if lke_node_ready_poll_ms is not None else None
             __props__.__dict__["max_retry_delay_ms"] = pulumi.Output.from_input(max_retry_delay_ms).apply(pulumi.runtime.to_json) if max_retry_delay_ms is not None else None
             __props__.__dict__["min_retry_delay_ms"] = pulumi.Output.from_input(min_retry_delay_ms).apply(pulumi.runtime.to_json) if min_retry_delay_ms is not None else None
             __props__.__dict__["skip_instance_delete_poll"] = pulumi.Output.from_input(skip_instance_delete_poll).apply(pulumi.runtime.to_json) if skip_instance_delete_poll is not None else None
             __props__.__dict__["skip_instance_ready_poll"] = pulumi.Output.from_input(skip_instance_ready_poll).apply(pulumi.runtime.to_json) if skip_instance_ready_poll is not None else None
-            if token is None and not opts.urn:
-                raise TypeError("Missing required property 'token'")
             __props__.__dict__["token"] = token
             if ua_prefix is None:
                 ua_prefix = _utilities.get_env('LINODE_UA_PREFIX')
             __props__.__dict__["ua_prefix"] = ua_prefix
             if url is None:
                 url = _utilities.get_env('LINODE_URL')
             __props__.__dict__["url"] = url
@@ -316,16 +343,26 @@
     def api_version(self) -> pulumi.Output[Optional[str]]:
         """
         An HTTP User-Agent Prefix to prepend in API requests.
         """
         return pulumi.get(self, "api_version")
 
     @property
+    @pulumi.getter(name="configPath")
+    def config_path(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "config_path")
+
+    @property
+    @pulumi.getter(name="configProfile")
+    def config_profile(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "config_profile")
+
+    @property
     @pulumi.getter
-    def token(self) -> pulumi.Output[str]:
+    def token(self) -> pulumi.Output[Optional[str]]:
         """
         The token that allows you access to your Linode account
         """
         return pulumi.get(self, "token")
 
     @property
     @pulumi.getter(name="uaPrefix")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/rdns.py` & `pulumi_linode-3.9.1/pulumi_linode/rdns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['RdnsArgs', 'Rdns']
@@ -186,20 +187,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  address: Optional[pulumi.Input[str]] = None,
                  rdns: Optional[pulumi.Input[str]] = None,
                  wait_for_available: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RdnsArgs.__new__(RdnsArgs)
 
             if address is None and not opts.urn:
                 raise TypeError("Missing required property 'address'")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/ssh_key.py` & `pulumi_linode-3.9.1/pulumi_linode/ssh_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['SshKeyArgs', 'SshKey']
@@ -173,20 +174,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  ssh_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SshKeyArgs.__new__(SshKeyArgs)
 
             if label is None and not opts.urn:
                 raise TypeError("Missing required property 'label'")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/stack_script.py` & `pulumi_linode-3.9.1/pulumi_linode/stack_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -547,20 +548,17 @@
                  images: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  is_public: Optional[pulumi.Input[bool]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  rev_note: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
                  user_defined_fields: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['StackScriptUserDefinedFieldArgs']]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = StackScriptArgs.__new__(StackScriptArgs)
 
             if description is None and not opts.urn:
                 raise TypeError("Missing required property 'description'")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/token.py` & `pulumi_linode-3.9.1/pulumi_linode/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['TokenArgs', 'Token']
@@ -267,20 +268,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  expiry: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  scopes: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TokenArgs.__new__(TokenArgs)
 
             __props__.__dict__["expiry"] = expiry
             __props__.__dict__["label"] = label
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/user.py` & `pulumi_linode-3.9.1/pulumi_linode/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -631,20 +632,17 @@
                  longview_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLongviewGrantArgs']]]]] = None,
                  nodebalancer_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserNodebalancerGrantArgs']]]]] = None,
                  restricted: Optional[pulumi.Input[bool]] = None,
                  stackscript_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserStackscriptGrantArgs']]]]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  volume_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserVolumeGrantArgs']]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UserArgs.__new__(UserArgs)
 
             __props__.__dict__["domain_grants"] = domain_grants
             if email is None and not opts.urn:
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode/volume.py` & `pulumi_linode-3.9.1/pulumi_linode/volume.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['VolumeArgs', 'Volume']
 
 @pulumi.input_type
 class VolumeArgs:
     def __init__(__self__, *,
                  label: pulumi.Input[str],
-                 region: pulumi.Input[str],
                  linode_id: Optional[pulumi.Input[int]] = None,
+                 region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
+                 source_volume_id: Optional[pulumi.Input[int]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Volume resource.
         :param pulumi.Input[str] label: The label of the Linode Volume
-        :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Volume.*.
         :param pulumi.Input[int] linode_id: The ID of a Linode Instance where the Volume should be attached.
+        :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
         :param pulumi.Input[int] size: Size of the Volume in GB.
+        :param pulumi.Input[int] source_volume_id: The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         pulumi.set(__self__, "label", label)
-        pulumi.set(__self__, "region", region)
         if linode_id is not None:
             pulumi.set(__self__, "linode_id", linode_id)
+        if region is not None:
+            pulumi.set(__self__, "region", region)
         if size is not None:
             pulumi.set(__self__, "size", size)
+        if source_volume_id is not None:
+            pulumi.set(__self__, "source_volume_id", source_volume_id)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def label(self) -> pulumi.Input[str]:
         """
@@ -44,50 +50,62 @@
         return pulumi.get(self, "label")
 
     @label.setter
     def label(self, value: pulumi.Input[str]):
         pulumi.set(self, "label", value)
 
     @property
-    @pulumi.getter
-    def region(self) -> pulumi.Input[str]:
-        """
-        The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Volume.*.
-        """
-        return pulumi.get(self, "region")
-
-    @region.setter
-    def region(self, value: pulumi.Input[str]):
-        pulumi.set(self, "region", value)
-
-    @property
     @pulumi.getter(name="linodeId")
     def linode_id(self) -> Optional[pulumi.Input[int]]:
         """
         The ID of a Linode Instance where the Volume should be attached.
         """
         return pulumi.get(self, "linode_id")
 
     @linode_id.setter
     def linode_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "linode_id", value)
 
     @property
     @pulumi.getter
+    def region(self) -> Optional[pulumi.Input[str]]:
+        """
+        The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
+        """
+        return pulumi.get(self, "region")
+
+    @region.setter
+    def region(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "region", value)
+
+    @property
+    @pulumi.getter
     def size(self) -> Optional[pulumi.Input[int]]:
         """
         Size of the Volume in GB.
         """
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "size", value)
 
     @property
+    @pulumi.getter(name="sourceVolumeId")
+    def source_volume_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
+        """
+        return pulumi.get(self, "source_volume_id")
+
+    @source_volume_id.setter
+    def source_volume_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "source_volume_id", value)
+
+    @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         A list of tags applied to this object. Tags are for organizational purposes only.
         """
         return pulumi.get(self, "tags")
 
@@ -100,37 +118,41 @@
 class _VolumeState:
     def __init__(__self__, *,
                  filesystem_path: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  linode_id: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
+                 source_volume_id: Optional[pulumi.Input[int]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Volume resources.
         :param pulumi.Input[str] filesystem_path: The full filesystem path for the Volume based on the Volume's label. Path is /dev/disk/by-id/scsi-0Linode_Volume_ +
                Volume label.
         :param pulumi.Input[str] label: The label of the Linode Volume
         :param pulumi.Input[int] linode_id: The ID of a Linode Instance where the Volume should be attached.
-        :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Volume.*.
+        :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
         :param pulumi.Input[int] size: Size of the Volume in GB.
+        :param pulumi.Input[int] source_volume_id: The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
         :param pulumi.Input[str] status: The status of the volume, indicating the current readiness state.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         if filesystem_path is not None:
             pulumi.set(__self__, "filesystem_path", filesystem_path)
         if label is not None:
             pulumi.set(__self__, "label", label)
         if linode_id is not None:
             pulumi.set(__self__, "linode_id", linode_id)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if size is not None:
             pulumi.set(__self__, "size", size)
+        if source_volume_id is not None:
+            pulumi.set(__self__, "source_volume_id", source_volume_id)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="filesystemPath")
@@ -169,15 +191,15 @@
     def linode_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "linode_id", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
-        The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Volume.*.
+        The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
@@ -190,14 +212,26 @@
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "size", value)
 
     @property
+    @pulumi.getter(name="sourceVolumeId")
+    def source_volume_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
+        """
+        return pulumi.get(self, "source_volume_id")
+
+    @source_volume_id.setter
+    def source_volume_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "source_volume_id", value)
+
+    @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
         The status of the volume, indicating the current readiness state.
         """
         return pulumi.get(self, "status")
 
@@ -223,14 +257,15 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  linode_id: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
+                 source_volume_id: Optional[pulumi.Input[int]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a Linode Volume resource.  This can be used to create, modify, and delete Linodes Block Storage Volumes.  Block Storage Volumes are removable storage disks that persist outside the life-cycle of Linode Instances. These volumes can be attached to and detached from Linode instances throughout a region.
 
         For more information, see [How to Use Block Storage with Your Linode](https://www.linode.com/docs/platform/block-storage/how-to-use-block-storage-with-your-linode/) and the [Linode APIv4 docs](https://developers.linode.com/api/v4#operation/createVolume).
 
@@ -268,14 +303,25 @@
                 ),
                 kernel="linode/latest-64bit",
                 label="boot-existing-volume",
             )],
             region="us-east",
             type="g6-nanode-1")
         ```
+
+        Volumes may also be cloned from existing volumes.
+
+        ```python
+        import pulumi
+        import pulumi_linode as linode
+
+        foobar = linode.Volume("foobar",
+            label="my-cloned-volume",
+            source_volume_id=12345)
+        ```
         ## Attributes
 
         This resource exports the following attributes:
 
         * `status` - The status of the Linode Volume. (`creating`, `active`, `resizing`, `contact_support`)
 
         * `filesystem_path` - The full filesystem path for the Volume based on the Volume's label. The path is "/dev/disk/by-id/scsi-0Linode_Volume_" + the Volume label
@@ -290,16 +336,17 @@
 
          The Linode Guide, [Import Existing Infrastructure to Terraform](https://www.linode.com/docs/applications/configuration-management/import-existing-infrastructure-to-terraform/), offers resource importing examples for Block Storage Volumes and other Linode resource types.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] label: The label of the Linode Volume
         :param pulumi.Input[int] linode_id: The ID of a Linode Instance where the Volume should be attached.
-        :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Volume.*.
+        :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
         :param pulumi.Input[int] size: Size of the Volume in GB.
+        :param pulumi.Input[int] source_volume_id: The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: VolumeArgs,
@@ -343,14 +390,25 @@
                 ),
                 kernel="linode/latest-64bit",
                 label="boot-existing-volume",
             )],
             region="us-east",
             type="g6-nanode-1")
         ```
+
+        Volumes may also be cloned from existing volumes.
+
+        ```python
+        import pulumi
+        import pulumi_linode as linode
+
+        foobar = linode.Volume("foobar",
+            label="my-cloned-volume",
+            source_volume_id=12345)
+        ```
         ## Attributes
 
         This resource exports the following attributes:
 
         * `status` - The status of the Linode Volume. (`creating`, `active`, `resizing`, `contact_support`)
 
         * `filesystem_path` - The full filesystem path for the Volume based on the Volume's label. The path is "/dev/disk/by-id/scsi-0Linode_Volume_" + the Volume label
@@ -380,35 +438,32 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  linode_id: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
+                 source_volume_id: Optional[pulumi.Input[int]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VolumeArgs.__new__(VolumeArgs)
 
             if label is None and not opts.urn:
                 raise TypeError("Missing required property 'label'")
             __props__.__dict__["label"] = label
             __props__.__dict__["linode_id"] = linode_id
-            if region is None and not opts.urn:
-                raise TypeError("Missing required property 'region'")
             __props__.__dict__["region"] = region
             __props__.__dict__["size"] = size
+            __props__.__dict__["source_volume_id"] = source_volume_id
             __props__.__dict__["tags"] = tags
             __props__.__dict__["filesystem_path"] = None
             __props__.__dict__["status"] = None
         super(Volume, __self__).__init__(
             'linode:index/volume:Volume',
             resource_name,
             __props__,
@@ -419,41 +474,44 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             filesystem_path: Optional[pulumi.Input[str]] = None,
             label: Optional[pulumi.Input[str]] = None,
             linode_id: Optional[pulumi.Input[int]] = None,
             region: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[int]] = None,
+            source_volume_id: Optional[pulumi.Input[int]] = None,
             status: Optional[pulumi.Input[str]] = None,
             tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'Volume':
         """
         Get an existing Volume resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] filesystem_path: The full filesystem path for the Volume based on the Volume's label. Path is /dev/disk/by-id/scsi-0Linode_Volume_ +
                Volume label.
         :param pulumi.Input[str] label: The label of the Linode Volume
         :param pulumi.Input[int] linode_id: The ID of a Linode Instance where the Volume should be attached.
-        :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Volume.*.
+        :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
         :param pulumi.Input[int] size: Size of the Volume in GB.
+        :param pulumi.Input[int] source_volume_id: The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
         :param pulumi.Input[str] status: The status of the volume, indicating the current readiness state.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VolumeState.__new__(_VolumeState)
 
         __props__.__dict__["filesystem_path"] = filesystem_path
         __props__.__dict__["label"] = label
         __props__.__dict__["linode_id"] = linode_id
         __props__.__dict__["region"] = region
         __props__.__dict__["size"] = size
+        __props__.__dict__["source_volume_id"] = source_volume_id
         __props__.__dict__["status"] = status
         __props__.__dict__["tags"] = tags
         return Volume(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="filesystemPath")
     def filesystem_path(self) -> pulumi.Output[str]:
@@ -479,27 +537,35 @@
         """
         return pulumi.get(self, "linode_id")
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
-        The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Volume.*.
+        The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def size(self) -> pulumi.Output[int]:
         """
         Size of the Volume in GB.
         """
         return pulumi.get(self, "size")
 
     @property
+    @pulumi.getter(name="sourceVolumeId")
+    def source_volume_id(self) -> pulumi.Output[Optional[int]]:
+        """
+        The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
+        """
+        return pulumi.get(self, "source_volume_id")
+
+    @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
         The status of the volume, indicating the current readiness state.
         """
         return pulumi.get(self, "status")
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode.egg-info/PKG-INFO` & `pulumi_linode-3.9.1/pulumi_linode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-linode
-Version: 3.9.0a1655503909
+Version: 3.9.1
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Description: [![Actions Status](https://github.com/pulumi/pulumi-linode/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-linode/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Flinode.svg)](https://www.npmjs.com/package/@pulumi/linode)
```

### Comparing `pulumi_linode-3.9.0a1655503909/pulumi_linode.egg-info/SOURCES.txt` & `pulumi_linode-3.9.1/pulumi_linode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_linode-3.9.0a1655503909/setup.py` & `pulumi_linode-3.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.0a1655503909"
-PLUGIN_VERSION = "3.9.0-alpha.1655503909+512b0c3b"
+VERSION = "3.9.1"
+PLUGIN_VERSION = "3.9.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'linode', PLUGIN_VERSION])
         except OSError as error:
```

