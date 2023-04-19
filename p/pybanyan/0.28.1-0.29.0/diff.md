# Comparing `tmp/pybanyan-0.28.1.tar.gz` & `tmp/pybanyan-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybanyan-0.28.1.tar", last modified: Thu Apr  7 18:14:07 2022, max compression
+gzip compressed data, was "pybanyan-0.29.0.tar", last modified: Wed Apr 19 18:54:57 2023, max compression
```

## Comparing `pybanyan-0.28.1.tar` & `pybanyan-0.29.0.tar`

### file list

```diff
@@ -1,98 +1,110 @@
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.431360 pybanyan-0.28.1/
--rw-r--r--   0 tarun      (501) staff       (20)     3154 2022-04-07 18:13:06.000000 pybanyan-0.28.1/CHANGELOG.md
--rw-r--r--   0 tarun      (501) staff       (20)    10496 2021-06-10 22:03:22.000000 pybanyan-0.28.1/LICENSE.md
--rw-r--r--   0 tarun      (501) staff       (20)      141 2021-06-10 22:03:22.000000 pybanyan-0.28.1/MANIFEST.in
--rw-r--r--   0 tarun      (501) staff       (20)     9246 2022-04-07 18:14:07.431526 pybanyan-0.28.1/PKG-INFO
--rw-r--r--   0 tarun      (501) staff       (20)     7240 2022-04-07 18:04:43.000000 pybanyan-0.28.1/README.md
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.405197 pybanyan-0.28.1/banyan/
--rw-r--r--   0 tarun      (501) staff       (20)      136 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.407845 pybanyan-0.28.1/banyan/api/
--rw-r--r--   0 tarun      (501) staff       (20)    16881 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)      342 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/api/attachment.py
--rw-r--r--   0 tarun      (501) staff       (20)     1641 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/audit.py
--rw-r--r--   0 tarun      (501) staff       (20)     5057 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/base.py
--rw-r--r--   0 tarun      (501) staff       (20)     3749 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/cloud_resource.py
--rw-r--r--   0 tarun      (501) staff       (20)     6055 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/device.py
--rw-r--r--   0 tarun      (501) staff       (20)     6099 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/event_v2.py
--rw-r--r--   0 tarun      (501) staff       (20)      851 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/netagent.py
--rw-r--r--   0 tarun      (501) staff       (20)     2215 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/policy.py
--rw-r--r--   0 tarun      (501) staff       (20)     1469 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/role.py
--rw-r--r--   0 tarun      (501) staff       (20)     2113 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/service.py
--rw-r--r--   0 tarun      (501) staff       (20)     2594 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/service_infra.py
--rw-r--r--   0 tarun      (501) staff       (20)     2596 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/service_web.py
--rw-r--r--   0 tarun      (501) staff       (20)     1482 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/shield.py
--rw-r--r--   0 tarun      (501) staff       (20)     1520 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/api/user.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.411390 pybanyan-0.28.1/banyan/controllers/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     1054 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/admin.py
--rw-r--r--   0 tarun      (501) staff       (20)     1885 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/audit.py
--rw-r--r--   0 tarun      (501) staff       (20)     5704 2022-04-07 17:08:08.000000 pybanyan-0.28.1/banyan/controllers/base.py
--rw-r--r--   0 tarun      (501) staff       (20)    22251 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/controllers/cloud_resource.py
--rw-r--r--   0 tarun      (501) staff       (20)     4941 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/device.py
--rw-r--r--   0 tarun      (501) staff       (20)     3733 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/event.py
--rw-r--r--   0 tarun      (501) staff       (20)     3201 2021-08-16 21:32:36.000000 pybanyan-0.28.1/banyan/controllers/export.py
--rw-r--r--   0 tarun      (501) staff       (20)     2328 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/netagent.py
--rw-r--r--   0 tarun      (501) staff       (20)     6191 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/policy.py
--rw-r--r--   0 tarun      (501) staff       (20)     3850 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/role.py
--rw-r--r--   0 tarun      (501) staff       (20)    10470 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/controllers/service.py
--rw-r--r--   0 tarun      (501) staff       (20)     8849 2022-04-07 17:04:39.000000 pybanyan-0.28.1/banyan/controllers/service_infra.py
--rw-r--r--   0 tarun      (501) staff       (20)     9737 2022-04-07 17:04:59.000000 pybanyan-0.28.1/banyan/controllers/service_web.py
--rw-r--r--   0 tarun      (501) staff       (20)     3960 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/shield.py
--rw-r--r--   0 tarun      (501) staff       (20)     4289 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/controllers/user.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.411944 pybanyan-0.28.1/banyan/core/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/core/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)       66 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/core/exc.py
--rw-r--r--   0 tarun      (501) staff       (20)      177 2022-04-07 18:13:21.000000 pybanyan-0.28.1/banyan/core/version.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.412157 pybanyan-0.28.1/banyan/ext/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/ext/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.421519 pybanyan-0.28.1/banyan/ext/iaas/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/iaas/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)    10036 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/iaas/aws.py
--rw-r--r--   0 tarun      (501) staff       (20)     7166 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/iaas/azure_cloud.py
--rw-r--r--   0 tarun      (501) staff       (20)     2028 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/iaas/base.py
--rw-r--r--   0 tarun      (501) staff       (20)     4275 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/iaas/gcp.py
--rw-r--r--   0 tarun      (501) staff       (20)     4313 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/iaas/oracle_cloud.py
--rw-r--r--   0 tarun      (501) staff       (20)     4698 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/iaas/vmware.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.422111 pybanyan-0.28.1/banyan/ext/idp/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/idp/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     6070 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/idp/azure_ad.py
--rw-r--r--   0 tarun      (501) staff       (20)      910 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/idp/base.py
--rw-r--r--   0 tarun      (501) staff       (20)     3856 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/ext/idp/okta.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.425096 pybanyan-0.28.1/banyan/lib/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/lib/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     1627 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/lib/certs.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.426472 pybanyan-0.28.1/banyan/lib/cloud/
--rw-r--r--   0 tarun      (501) staff       (20)      587 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/lib/cloud/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     2312 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/lib/cloud/aws.py
--rw-r--r--   0 tarun      (501) staff       (20)    13055 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/lib/service.py
--rw-r--r--   0 tarun      (501) staff       (20)     3799 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/main.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.430186 pybanyan-0.28.1/banyan/model/
--rw-r--r--   0 tarun      (501) staff       (20)     5907 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/model/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     1441 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/model/attachment.py
--rw-r--r--   0 tarun      (501) staff       (20)     3622 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/model/audit.py
--rw-r--r--   0 tarun      (501) staff       (20)     2206 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/model/cloud_resource.py
--rw-r--r--   0 tarun      (501) staff       (20)     7350 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/model/event_v2.py
--rw-r--r--   0 tarun      (501) staff       (20)     3776 2021-08-16 21:32:36.000000 pybanyan-0.28.1/banyan/model/netagent.py
--rw-r--r--   0 tarun      (501) staff       (20)     4596 2022-03-30 03:52:15.000000 pybanyan-0.28.1/banyan/model/policy.py
--rw-r--r--   0 tarun      (501) staff       (20)     2406 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/model/role.py
--rw-r--r--   0 tarun      (501) staff       (20)    10544 2022-04-04 18:28:15.000000 pybanyan-0.28.1/banyan/model/service.py
--rw-r--r--   0 tarun      (501) staff       (20)    12428 2022-04-07 17:13:47.000000 pybanyan-0.28.1/banyan/model/service_infra.py
--rw-r--r--   0 tarun      (501) staff       (20)     6260 2022-04-04 23:57:25.000000 pybanyan-0.28.1/banyan/model/service_web.py
--rw-r--r--   0 tarun      (501) staff       (20)     2836 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/model/shield.py
--rw-r--r--   0 tarun      (501) staff       (20)     3262 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/model/trustscore.py
--rw-r--r--   0 tarun      (501) staff       (20)     6700 2021-08-16 21:32:36.000000 pybanyan-0.28.1/banyan/model/user_device.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.430436 pybanyan-0.28.1/banyan/plugins/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/plugins/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.430542 pybanyan-0.28.1/banyan/templates/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.28.1/banyan/templates/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2022-04-07 18:14:07.431244 pybanyan-0.28.1/pybanyan.egg-info/
--rw-r--r--   0 tarun      (501) staff       (20)     9246 2022-04-07 18:14:07.000000 pybanyan-0.28.1/pybanyan.egg-info/PKG-INFO
--rw-r--r--   0 tarun      (501) staff       (20)     2058 2022-04-07 18:14:07.000000 pybanyan-0.28.1/pybanyan.egg-info/SOURCES.txt
--rw-r--r--   0 tarun      (501) staff       (20)        1 2022-04-07 18:14:07.000000 pybanyan-0.28.1/pybanyan.egg-info/dependency_links.txt
--rw-r--r--   0 tarun      (501) staff       (20)       45 2022-04-07 18:14:07.000000 pybanyan-0.28.1/pybanyan.egg-info/entry_points.txt
--rw-r--r--   0 tarun      (501) staff       (20)      389 2022-04-07 18:14:07.000000 pybanyan-0.28.1/pybanyan.egg-info/requires.txt
--rw-r--r--   0 tarun      (501) staff       (20)        7 2022-04-07 18:14:07.000000 pybanyan-0.28.1/pybanyan.egg-info/top_level.txt
--rw-r--r--   0 tarun      (501) staff       (20)      130 2021-06-10 22:03:22.000000 pybanyan-0.28.1/requirements-dev.txt
--rw-r--r--   0 tarun      (501) staff       (20)      371 2022-03-30 03:52:15.000000 pybanyan-0.28.1/requirements.txt
--rw-r--r--   0 tarun      (501) staff       (20)       38 2022-04-07 18:14:07.431830 pybanyan-0.28.1/setup.cfg
--rw-r--r--   0 tarun      (501) staff       (20)     1517 2022-03-30 03:52:15.000000 pybanyan-0.28.1/setup.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.219082 pybanyan-0.29.0/
+-rw-r--r--   0 tarun      (501) staff       (20)     3256 2023-04-19 18:32:19.000000 pybanyan-0.29.0/CHANGELOG.md
+-rw-r--r--   0 tarun      (501) staff       (20)    10496 2021-06-10 22:03:22.000000 pybanyan-0.29.0/LICENSE.md
+-rw-r--r--   0 tarun      (501) staff       (20)      141 2021-06-10 22:03:22.000000 pybanyan-0.29.0/MANIFEST.in
+-rw-r--r--   0 tarun      (501) staff       (20)     8237 2023-04-19 18:54:57.219155 pybanyan-0.29.0/PKG-INFO
+-rw-r--r--   0 tarun      (501) staff       (20)     7756 2023-04-19 18:32:42.000000 pybanyan-0.29.0/README.md
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.201730 pybanyan-0.29.0/banyan/
+-rw-r--r--   0 tarun      (501) staff       (20)      136 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.206128 pybanyan-0.29.0/banyan/api/
+-rw-r--r--   0 tarun      (501) staff       (20)    17853 2023-04-17 18:19:15.000000 pybanyan-0.29.0/banyan/api/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)      397 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/access_tier.py
+-rw-r--r--   0 tarun      (501) staff       (20)      453 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/api_key.py
+-rw-r--r--   0 tarun      (501) staff       (20)      342 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/api/attachment.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1746 2022-04-07 19:03:43.000000 pybanyan-0.29.0/banyan/api/audit.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6173 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3749 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/cloud_resource.py
+-rw-r--r--   0 tarun      (501) staff       (20)      382 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/connector.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6392 2023-04-19 18:32:42.000000 pybanyan-0.29.0/banyan/api/device.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6069 2023-04-17 18:19:15.000000 pybanyan-0.29.0/banyan/api/event_v2.py
+-rw-r--r--   0 tarun      (501) staff       (20)      851 2022-11-29 19:34:37.000000 pybanyan-0.29.0/banyan/api/netagent.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2215 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/policy.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1469 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/role.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2113 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2594 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/service_infra.py
+-rw-r--r--   0 tarun      (501) staff       (20)      427 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/service_tunnel.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2596 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/service_web.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1482 2022-11-29 19:34:37.000000 pybanyan-0.29.0/banyan/api/shield.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1520 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/user.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.210186 pybanyan-0.29.0/banyan/controllers/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/controllers/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2442 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/access_tier.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1054 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/controllers/admin.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2504 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/api_key.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1885 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/controllers/audit.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6045 2023-04-17 18:19:15.000000 pybanyan-0.29.0/banyan/controllers/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)    21999 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/cloud_resource.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2574 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/connector.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6024 2023-04-19 18:32:42.000000 pybanyan-0.29.0/banyan/controllers/device.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3733 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/controllers/event.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3216 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/export.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2329 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/netagent.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6191 2022-11-29 19:34:37.000000 pybanyan-0.29.0/banyan/controllers/policy.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3850 2022-11-29 19:34:37.000000 pybanyan-0.29.0/banyan/controllers/role.py
+-rw-r--r--   0 tarun      (501) staff       (20)    10519 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)     8854 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/service_infra.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2136 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/service_tunnel.py
+-rw-r--r--   0 tarun      (501) staff       (20)     9748 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/service_web.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3966 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/shield.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4281 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/user.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.210595 pybanyan-0.29.0/banyan/core/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/core/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)       66 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/core/exc.py
+-rw-r--r--   0 tarun      (501) staff       (20)      177 2023-04-19 17:28:04.000000 pybanyan-0.29.0/banyan/core/version.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.210740 pybanyan-0.29.0/banyan/ext/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/ext/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.212497 pybanyan-0.29.0/banyan/ext/iaas/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)    10036 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/aws.py
+-rw-r--r--   0 tarun      (501) staff       (20)     7166 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/azure_cloud.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2028 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4275 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/gcp.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4313 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/oracle_cloud.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4698 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/vmware.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.213328 pybanyan-0.29.0/banyan/ext/idp/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/idp/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6070 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/idp/azure_ad.py
+-rw-r--r--   0 tarun      (501) staff       (20)      910 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/idp/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3856 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/idp/okta.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.213807 pybanyan-0.29.0/banyan/lib/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1627 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/certs.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.214192 pybanyan-0.29.0/banyan/lib/cloud/
+-rw-r--r--   0 tarun      (501) staff       (20)      587 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/cloud/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2312 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/cloud/aws.py
+-rw-r--r--   0 tarun      (501) staff       (20)    13055 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4281 2023-04-17 18:19:15.000000 pybanyan-0.29.0/banyan/main.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.217756 pybanyan-0.29.0/banyan/model/
+-rw-r--r--   0 tarun      (501) staff       (20)     5990 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2409 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/access_tier.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1137 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/api_key.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1441 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/model/attachment.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3887 2022-04-07 19:03:43.000000 pybanyan-0.29.0/banyan/model/audit.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2215 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/cloud_resource.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2095 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/connector.py
+-rw-r--r--   0 tarun      (501) staff       (20)     7350 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/model/event_v2.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3776 2021-08-16 21:32:36.000000 pybanyan-0.29.0/banyan/model/netagent.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4541 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/policy.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2351 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/role.py
+-rw-r--r--   0 tarun      (501) staff       (20)    10470 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)    12428 2022-04-07 17:13:47.000000 pybanyan-0.29.0/banyan/model/service_infra.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1953 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/service_tunnel.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6260 2022-04-04 23:57:25.000000 pybanyan-0.29.0/banyan/model/service_web.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2856 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/shield.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3262 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/model/trustscore.py
+-rw-r--r--   0 tarun      (501) staff       (20)     7580 2023-04-19 18:32:42.000000 pybanyan-0.29.0/banyan/model/user_device.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.218027 pybanyan-0.29.0/banyan/plugins/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/plugins/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.218134 pybanyan-0.29.0/banyan/templates/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/templates/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.218954 pybanyan-0.29.0/pybanyan.egg-info/
+-rw-r--r--   0 tarun      (501) staff       (20)     8237 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/PKG-INFO
+-rw-r--r--   0 tarun      (501) staff       (20)     2401 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/SOURCES.txt
+-rw-r--r--   0 tarun      (501) staff       (20)        1 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/dependency_links.txt
+-rw-r--r--   0 tarun      (501) staff       (20)       44 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/entry_points.txt
+-rw-r--r--   0 tarun      (501) staff       (20)      389 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/requires.txt
+-rw-r--r--   0 tarun      (501) staff       (20)        7 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/top_level.txt
+-rw-r--r--   0 tarun      (501) staff       (20)      130 2021-06-10 22:03:22.000000 pybanyan-0.29.0/requirements-dev.txt
+-rw-r--r--   0 tarun      (501) staff       (20)      371 2022-03-30 03:52:15.000000 pybanyan-0.29.0/requirements.txt
+-rw-r--r--   0 tarun      (501) staff       (20)       38 2023-04-19 18:54:57.219574 pybanyan-0.29.0/setup.cfg
+-rw-r--r--   0 tarun      (501) staff       (20)     1517 2022-03-30 03:52:15.000000 pybanyan-0.29.0/setup.py
```

### Comparing `pybanyan-0.28.1/CHANGELOG.md` & `pybanyan-0.29.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # PyBanyan Change History
 
+## 0.29.0
+
+ * make api_key the primary credential (refresh_token still works)
+ * use v2 Devices API 
+
 ## 0.28.1
 
  * bugfixes and dry changes for service abstractions 
 
 ## 0.28.0
 
  * improve service abstractions by adding `service-web` and `service-infra` commands
```

### Comparing `pybanyan-0.28.1/LICENSE.md` & `pybanyan-0.29.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/PKG-INFO` & `pybanyan-0.29.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,208 +1,213 @@
 Metadata-Version: 2.1
 Name: pybanyan
-Version: 0.28.1
+Version: 0.29.0
 Summary: API library and command-line interface for Banyan Security
 Home-page: https://github.com/banyansecurity/pybanyan/
 Author: Todd Radel
 Author-email: todd@banyansecurity.io
 License: apache
-Description: # API library and command-line interface for Banyan Security
-        [![Build Status](https://travis-ci.org/banyansecurity/pybanyan.svg?branch=master)](https://travis-ci.org/banyansecurity/pybanyan)
-        [![codecov](https://codecov.io/gh/banyansecurity/pybanyan/branch/master/graph/badge.svg)](https://codecov.io/gh/banyansecurity/pybanyan)
-        [![PyPI version](https://badge.fury.io/py/pybanyan.svg)](https://badge.fury.io/py/pybanyan)
-        
-        
-        ## Prerequisites
-        Python 3.7 or 3.8 must be installed.
-        
-        ## Installation 
-        ### Installing the easy way
-        
-        ```console
-        $ pip install pybanyan
-        ```
-        
-        ### Installing the hard way
-        
-        ```console
-        $ git clone https://github.com/banyansecurity/pybanyan.git
-        $ cd pybanyan
-        $ pip install -r requirements.txt
-        $ python setup.py install
-        ```
-        
-        ## Usage
-        
-        This package contains both an API client and a CLI tool.
-        To use either one, you need to [generate] an API token from the Banyan Command Center.
-        
-        ### API library
-        
-        Here's a sample script that uses the library to print the names of every service registered in Banyan:
-        
-        ```python
-        from banyan.api import BanyanApiClient
-        
-        c = BanyanApiClient()
-        for service in c.services.list():
-            print(service.name)
-        ```
-        
-        Output:
-        ```console
-        $ python examples/list_services.py
-        jira
-        jupyter
-        kube
-        mysql
-        rds-mysql
-        rds-pgsql
-        ```
-        
-        The `BanyanApiClient` class accepts optional arguments to specify the API server and refresh token. If not provided, 
-        it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_REFRESH_TOKEN`.
-        
-        Full API documentation will be available soon.
-        
-        ### Banyan CLI tool
-        
-        Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API token:
-        
-        ```ini
-        [banyan]
-        api_url = https://net.banyanops.com
-        refresh_token = MY_API_TOKEN
-        ```
-        
-        The CLI is invoked with the `banyan` tool. It contains a number of commands and sub-commands to help you work
-        with policies, roles, services, users, and other objects in Banyan. 
-        
-        Run the `banyan` tool by itself to see the available commands.
-        
-        ```console
-        $ banyan
-        usage: banyan [options] <command> <subcommand> [<subcommand> ...] [parameters]
-        
-        API library and command-line interface for Banyan Security
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -d, --debug           full application debug mode
-          -q, --quiet           suppress all console output
-          -v, --version         show program's version number and exit
-          --api-url API_URL     URL for the Banyan API server. Can also be configured
-                                via the BANYAN_API_URL environment variable.
-          --refresh-token REFRESH_TOKEN
-                                API token used for the initial authentication to the
-                                Banyan API server. Can also be configured via the
-                                BANYAN_REFRESH_TOKEN environment variable.
-          --output-format {table,json,yaml}, -o {table,json,yaml}
-                                desired output format (table, json, yaml)
-        
-        Commands:
-          {event,admin,device,user,netagent,shield,policy,role,service}
-            event               report on security and audit events
-            admin               manage administrator accounts
-            device              manage devices
-            user                manage user accounts
-            netagent            manage netagents (AccessTiers and HostAgents)
-            shield              manage Banyan Shield clusters
-            policy              manage authorization policies for users and workloads
-            role                manage user and workload roles
-            service             manage web and TCP services and workloads
-            cloud-resource      manage cloud resources discovered from IaaS
-        ```
-        
-        Each of the commands has multiple subcommands. For example, `banyan service` allows you to list services, create/delete, enable/disable, etc. Run the command without any subcommand to see the options:
-        
-        ```console
-        $ banyan service
-        usage: banyan service [-h]
-                              {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
-                              ...
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-        
-        sub-commands:
-          {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
-            attach-policy       attach a policy to a service
-            create              create a new service from a JSON specification
-            delete              delete a service
-            detach-policy       detach the active policy from a service
-            disable             disable a service
-            enable              enable a service
-            get                 show the definition of a registered service
-            list                list registered services
-            test                run sanity checks on a service
-            update              update an existing service from a JSON specification
-        ```
-        
-        To see the full help available for any command, just add the `-h` or `--help` option to the end of the command. 
-        For example:
-        
-        ```console
-        $ banyan service attach-policy --help
-        usage: banyan service attach-policy [-h] [--permissive] [--enforcing]
-                                            service_name_or_id policy_name_or_id
-        
-        positional arguments:
-          service_name_or_id  Name or ID of the service to attach a policy to.
-          policy_name_or_id   Name or ID of the policy to attach to the service.
-        
-        optional arguments:
-          -h, --help          show this help message and exit
-          --permissive        Set the policy to permissive mode (allow all traffic and
-                              log any unauthorized access).
-          --enforcing         Set the policy to enforcing mode (deny unauthorized
-                              access).
-        ```
-        
-        ## Integrations
-        
-        You can automate different types of workflows by integrating with external APIs. We provide pre-built integrations for 2 types of workflows:
-        
-        ### 1. Synchronize cloud resources from your IaaS provider
-        
-        You can discover and synchronize your IaaS (Infrastructure As A Service) resources into Banyan's inventory, so you can later publish some or all of them as Banyan services. Read our [overview on how Banyan synchronizes IaaS resources](docs/iaas/README.md), and then check out instructions to set up for your specific IaaS provider:
-        
-        - [AWS](docs/iaas/aws.md)
-        - [Azure Cloud](docs/iaas/azure_cloud.md)
-        - [GCP](docs/iaas/gcp.md)
-        - [Oracle Cloud](docs/iaas/oracle_cloud.md)
-        
-        ### 2. Bookmark Banyan services into your SSO catalog
-        
-        You can publish Banyan services as bookmark applications in your SSO (Single Sign On) portal, so your end-user can access them via their SSO catalog. Check out the provider-specific link for setup instructions.
-        
-        - [Okta](docs/idp/okta.md)
-        - [AzureAD](docs/idp/azure_ad.md)
-        
-        
-        ## Development
-        
-        To work on the pybanyan code, follow the instructions in the [documentation][devel]. 
-        
-        ## Support
-        
-        This API library and its accompanying CLI utility are provided free of charge and without support. To report 
-        issues with the library, please create a new [issue in Github][github-issue].
-        
-        ## Contributions
-        
-        We welcome your contributions in the form of pull requests! Please follow the standard [Github pull request 
-        workflow][github-pr].
-        
-        [generate]: https://docs.banyansecurity.io/docs/api-guide/introduction/
-        [github-pr]: https://gist.github.com/Chaser324/ce0505fbed06b947d962
-        [github-issue]: https://github.com/banyansecurity/pybanyan/issues/new
-        [devel]: https://pybanyan.readthedocs.io/development.html
-Platform: UNKNOWN
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: aws
 Provides-Extra: azure_cloud
 Provides-Extra: gcp
 Provides-Extra: oracle_cloud
 Provides-Extra: okta
 Provides-Extra: azure_ad
+License-File: LICENSE.md
+
+# API library and command-line interface for Banyan Security
+[![Build Status](https://travis-ci.org/banyansecurity/pybanyan.svg?branch=master)](https://travis-ci.org/banyansecurity/pybanyan)
+[![codecov](https://codecov.io/gh/banyansecurity/pybanyan/branch/master/graph/badge.svg)](https://codecov.io/gh/banyansecurity/pybanyan)
+[![PyPI version](https://badge.fury.io/py/pybanyan.svg)](https://badge.fury.io/py/pybanyan)
+
+
+## Prerequisites
+Python 3.7+ must be installed.
+
+## Installation 
+### Installing the easy way
+
+```console
+$ pip install pybanyan
+```
+
+### Installing the hard way
+
+```console
+$ git clone https://github.com/banyansecurity/pybanyan.git
+$ cd pybanyan
+$ pip install -r requirements.txt
+$ python setup.py install --user
+```
+
+## Usage
+
+This package contains both an API client and a CLI tool.
+To use either one, you need to [generate] an API token from the Banyan Command Center.
+
+### API library
+
+Here's a sample script that uses the library to print the names of every service registered in Banyan:
+
+```python
+from banyan.api import BanyanApiClient
+
+c = BanyanApiClient()
+for service in c.services.list():
+    print(service.name)
+```
+
+Output:
+```console
+$ python examples/list_services.py
+jira
+jupyter
+kube
+mysql
+rds-mysql
+rds-pgsql
+```
+
+The `BanyanApiClient` class accepts optional arguments to specify the API server and refresh token. If not provided, 
+it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_API_KEY`.
+
+Full API documentation will be available soon.
+
+### Banyan CLI tool
+
+Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API credential (you may use an `api_key` or `refresh_token`):
+
+```ini
+[banyan]
+api_url = https://net.banyanops.com
+api_key = MY_API_KEY
+```
+
+The CLI is invoked with the `banyan` tool. It contains a number of commands and sub-commands to help you work with policies, roles, services, users, and other objects in Banyan. 
+
+Run the `banyan` tool by itself to see the available commands.
+
+```console
+$ banyan
+usage: banyan [options] <command> <subcommand> [<subcommand> ...] [parameters]
+
+API library and command-line interface for Banyan Security
+
+options:
+  -h, --help            show this help message and exit
+  -d, --debug           full application debug mode
+  -q, --quiet           suppress all console output
+  --version, -v         show program's version number and exit
+  --api-url API_URL     URL for the Banyan API server. Can also be configured via the BANYAN_API_URL environment variable.
+  --api-key API_KEY     API credential used for the authentication to the Banyan API server. Can also be configured via the BANYAN_API_KEY or BANYAN_REFRESH_TOKEN environment
+                        variable.
+  --insecure-tls, -k    Allow connections to API servers with invalid TLS certificates.
+  --output-format {table,json,yaml}, -o {table,json,yaml}
+                        desired output format (table, json, yaml)
+
+Commands:
+  {netagent,service,shield,access-tier,api-key,audit,cloud-resource,connector,device,event,export,policy,role,service-infra,service-tunnel,service-web,user}
+    netagent            (deprecated: use access-tier) manage netagents
+    service             (deprecated: use service-web or service-infra) manage web and TCP services and workloads
+    shield              (deprecated) manage shield clusters
+    access-tier         manage access tiers
+    api-key             manage API keys
+    audit               retrieve audit logs
+    cloud-resource      manage cloud resources discovered from IaaS
+    connector           manage connectors
+    device              manage devices
+    event               report on security events
+    export              export all objects from an organization
+    policy              manage authorization policies for users and workloads
+    role                manage user and workload roles
+    service-infra       manage infrastructure services
+    service-tunnel      manage service tunnels
+    service-web         manage hosted website services
+    user                manage users
+```
+
+Each of the commands has multiple subcommands. For example, `banyan service` allows you to list services, create/delete, enable/disable, etc. Run the command without any subcommand to see the options:
+
+```console
+$ banyan service
+usage: banyan service [-h]
+                      {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
+                      ...
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+sub-commands:
+  {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
+    attach-policy       attach a policy to a service
+    create              create a new service from a JSON specification
+    delete              delete a service
+    detach-policy       detach the active policy from a service
+    disable             disable a service
+    enable              enable a service
+    get                 show the definition of a registered service
+    list                list registered services
+    test                run sanity checks on a service
+    update              update an existing service from a JSON specification
+```
+
+To see the full help available for any command, just add the `-h` or `--help` option to the end of the command. 
+For example:
+
+```console
+$ banyan service attach-policy --help
+usage: banyan service attach-policy [-h] [--permissive] [--enforcing]
+                                    service_name_or_id policy_name_or_id
+
+positional arguments:
+  service_name_or_id  Name or ID of the service to attach a policy to.
+  policy_name_or_id   Name or ID of the policy to attach to the service.
+
+optional arguments:
+  -h, --help          show this help message and exit
+  --permissive        Set the policy to permissive mode (allow all traffic and
+                      log any unauthorized access).
+  --enforcing         Set the policy to enforcing mode (deny unauthorized
+                      access).
+```
+
+## Integrations
+
+You can automate different types of workflows by integrating with external APIs. We provide pre-built integrations for 2 types of workflows:
+
+### 1. Synchronize cloud resources from your IaaS provider
+
+You can discover and synchronize your IaaS (Infrastructure As A Service) resources into Banyan's inventory, so you can later publish some or all of them as Banyan services. Read our [overview on how Banyan synchronizes IaaS resources](docs/iaas/README.md), and then check out instructions to set up for your specific IaaS provider:
+
+- [AWS](docs/iaas/aws.md)
+- [Azure Cloud](docs/iaas/azure_cloud.md)
+- [GCP](docs/iaas/gcp.md)
+- [Oracle Cloud](docs/iaas/oracle_cloud.md)
+
+### 2. Bookmark Banyan services into your SSO catalog
+
+You can publish Banyan services as bookmark applications in your SSO (Single Sign On) portal, so your end-user can access them via their SSO catalog. Check out the provider-specific link for setup instructions.
+
+- [Okta](docs/idp/okta.md)
+- [AzureAD](docs/idp/azure_ad.md)
+
+
+## Development
+
+To work on the pybanyan code, follow the instructions in the [documentation][devel]. 
+
+## Support
+
+This API library and its accompanying CLI utility are provided free of charge and without support. To report 
+issues with the library, please create a new [issue in Github][github-issue].
+
+## Contributions
+
+We welcome your contributions in the form of pull requests! Please follow the standard [Github pull request 
+workflow][github-pr].
+
+[generate]: https://docs.banyansecurity.io/docs/api-guide/introduction/
+[github-pr]: https://gist.github.com/Chaser324/ce0505fbed06b947d962
+[github-issue]: https://github.com/banyansecurity/pybanyan/issues/new
+[devel]: https://pybanyan.readthedocs.io/development.html
```

### Comparing `pybanyan-0.28.1/README.md` & `pybanyan-0.29.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # API library and command-line interface for Banyan Security
 [![Build Status](https://travis-ci.org/banyansecurity/pybanyan.svg?branch=master)](https://travis-ci.org/banyansecurity/pybanyan)
 [![codecov](https://codecov.io/gh/banyansecurity/pybanyan/branch/master/graph/badge.svg)](https://codecov.io/gh/banyansecurity/pybanyan)
 [![PyPI version](https://badge.fury.io/py/pybanyan.svg)](https://badge.fury.io/py/pybanyan)
 
 
 ## Prerequisites
-Python 3.7 or 3.8 must be installed.
+Python 3.7+ must be installed.
 
 ## Installation 
 ### Installing the easy way
 
 ```console
 $ pip install pybanyan
 ```
 
 ### Installing the hard way
 
 ```console
 $ git clone https://github.com/banyansecurity/pybanyan.git
 $ cd pybanyan
 $ pip install -r requirements.txt
-$ python setup.py install
+$ python setup.py install --user
 ```
 
 ## Usage
 
 This package contains both an API client and a CLI tool.
 To use either one, you need to [generate] an API token from the Banyan Command Center.
 
@@ -48,65 +48,69 @@
 kube
 mysql
 rds-mysql
 rds-pgsql
 ```
 
 The `BanyanApiClient` class accepts optional arguments to specify the API server and refresh token. If not provided, 
-it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_REFRESH_TOKEN`.
+it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_API_KEY`.
 
 Full API documentation will be available soon.
 
 ### Banyan CLI tool
 
-Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API token:
+Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API credential (you may use an `api_key` or `refresh_token`):
 
 ```ini
 [banyan]
 api_url = https://net.banyanops.com
-refresh_token = MY_API_TOKEN
+api_key = MY_API_KEY
 ```
 
-The CLI is invoked with the `banyan` tool. It contains a number of commands and sub-commands to help you work
-with policies, roles, services, users, and other objects in Banyan. 
+The CLI is invoked with the `banyan` tool. It contains a number of commands and sub-commands to help you work with policies, roles, services, users, and other objects in Banyan. 
 
 Run the `banyan` tool by itself to see the available commands.
 
 ```console
 $ banyan
 usage: banyan [options] <command> <subcommand> [<subcommand> ...] [parameters]
 
 API library and command-line interface for Banyan Security
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -d, --debug           full application debug mode
   -q, --quiet           suppress all console output
-  -v, --version         show program's version number and exit
-  --api-url API_URL     URL for the Banyan API server. Can also be configured
-                        via the BANYAN_API_URL environment variable.
-  --refresh-token REFRESH_TOKEN
-                        API token used for the initial authentication to the
-                        Banyan API server. Can also be configured via the
-                        BANYAN_REFRESH_TOKEN environment variable.
+  --version, -v         show program's version number and exit
+  --api-url API_URL     URL for the Banyan API server. Can also be configured via the BANYAN_API_URL environment variable.
+  --api-key API_KEY     API credential used for the authentication to the Banyan API server. Can also be configured via the BANYAN_API_KEY or BANYAN_REFRESH_TOKEN environment
+                        variable.
+  --insecure-tls, -k    Allow connections to API servers with invalid TLS certificates.
   --output-format {table,json,yaml}, -o {table,json,yaml}
                         desired output format (table, json, yaml)
 
 Commands:
-  {event,admin,device,user,netagent,shield,policy,role,service}
-    event               report on security and audit events
-    admin               manage administrator accounts
+  {netagent,service,shield,access-tier,api-key,audit,cloud-resource,connector,device,event,export,policy,role,service-infra,service-tunnel,service-web,user}
+    netagent            (deprecated: use access-tier) manage netagents
+    service             (deprecated: use service-web or service-infra) manage web and TCP services and workloads
+    shield              (deprecated) manage shield clusters
+    access-tier         manage access tiers
+    api-key             manage API keys
+    audit               retrieve audit logs
+    cloud-resource      manage cloud resources discovered from IaaS
+    connector           manage connectors
     device              manage devices
-    user                manage user accounts
-    netagent            manage netagents (AccessTiers and HostAgents)
-    shield              manage Banyan Shield clusters
+    event               report on security events
+    export              export all objects from an organization
     policy              manage authorization policies for users and workloads
     role                manage user and workload roles
-    service             manage web and TCP services and workloads
-    cloud-resource      manage cloud resources discovered from IaaS
+    service-infra       manage infrastructure services
+    service-tunnel      manage service tunnels
+    service-web         manage hosted website services
+    user                manage users
 ```
 
 Each of the commands has multiple subcommands. For example, `banyan service` allows you to list services, create/delete, enable/disable, etc. Run the command without any subcommand to see the options:
 
 ```console
 $ banyan service
 usage: banyan service [-h]
```

### Comparing `pybanyan-0.28.1/banyan/api/__init__.py` & `pybanyan-0.29.0/banyan/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,47 +10,51 @@
 from typing import Dict, Any, List, Union, Callable
 
 import urllib3
 import requests
 from cement import init_defaults
 from requests.auth import AuthBase
 
+from banyan.core.exc import BanyanError
 from banyan.api.attachment import AttachmentAPI
 from banyan.api.audit import AuditAPI
 from banyan.api.device import DeviceAPI
 from banyan.api.event_v2 import EventV2API
 from banyan.api.netagent import NetagentAPI
 from banyan.api.policy import PolicyAPI
 from banyan.api.role import RoleAPI
 from banyan.api.service import ServiceAPI
 from banyan.api.service_web import ServiceWebAPI
 from banyan.api.service_infra import ServiceInfraAPI
 from banyan.api.shield import ShieldAPI
 from banyan.api.user import UserAPI
 from banyan.api.cloud_resource import CloudResourceAPI
-from banyan.core.exc import BanyanError
+from banyan.api.api_key import ApiKeyAPI
+from banyan.api.connector import ConnectorAPI
+from banyan.api.access_tier import AccessTierAPI
+from banyan.api.service_tunnel import ServiceTunnelAPI
 
 JsonListOrObj = Union[List, Dict]
 ProgressCallback = Callable[[str, str, int, int, List[JsonListOrObj]], None]
 
 
 class BanyanApiClient:
     """
     Main class for interacting with the Banyan API.
 
-    :param api_server_url: URL for the Banyan Command Center. This should be the same as the
+    :param api_url: URL for the Banyan Command Center. This should be the same as the
         URL you enter in your browser to log into the Command Center. If not supplied, we will
-        look for an environment variable named :envvar:`BANYAN_API_URL`; if that is also not present,
-        the URL defaults to <https://net.banyanops.com>.
-    :type api_server_url: str
-    :param refresh_token: Initial API token used to authorize the connection. The refresh token
-        will then be exchanged for an access token. If not supplied, we look for an environment
-        varialbe named :envvar:`BANYAN_REFRESH_TOKEN`; if that is also not present, it causes a
-        :py:exc:`BanyanError`.
-    :type refresh_token: str
+        look for an environment variable named :envvar:`BANYAN_API_URL`; 
+        if that is also not present, the URL defaults to <https://net.banyanops.com>.
+    :type api_url: str
+    :param api_key: Initial API credential used to authorize the connection - can be an api key or
+        a refresh token (that will then be exchanged for an access token). If not supplied, we will
+        look for an environment variable named :envvar:`BANYAN_API_KEY` or :envvar:`BANYAN_REFRESH_TOKEN`; 
+        if that is also not present, it causes a :py:exc:`BanyanError`.
+    :type api_key: str
     :param debug: If True, extra debugging output from the Requests module will be logged.
     :type debug: bool
     :param log: Optional logger to use in debug mode. If not provided, the standard
         logger will be used.
     :type log: logging.Logger
     :raises: :py:exc:`BanyanError` if no refresh token is provided.
     """
@@ -76,28 +80,28 @@
             self._obj = parent
 
         def __call__(self, r: requests.Request) -> requests.Request:
             token = self._obj.access_token or self._obj.refresh_token
             r.headers['Authorization'] = f'Bearer {token}'
             return r
 
-    def __init__(self, api_server_url: str = None, refresh_token: str = None, debug: bool = False,
+    def __init__(self, api_url: str = None, api_key: str = None, debug: bool = False,
                  log: logging.Logger = None) -> None:
         self._debug = debug
         self._log = log
         self._progress_callback = None
         self._access_token = None
         self._insecure_tls = False
-        self._api_url = self._normalize_url(api_server_url or os.getenv('BANYAN_API_URL') or
-                                            BanyanApiClient.DEFAULT_API_URL)
-        self._refresh_token = refresh_token or os.getenv('BANYAN_REFRESH_TOKEN')
+        self._api_url = self._normalize_url(api_url or 
+                                            os.getenv('BANYAN_API_URL') or BanyanApiClient.DEFAULT_API_URL)
+        self._refresh_token = api_key or os.getenv('BANYAN_API_KEY') or os.getenv('BANYAN_REFRESH_TOKEN')
         if not self._refresh_token:
             self._read_config_file()
         if not self._refresh_token:
-            raise BanyanError("Refresh token must be set")
+            raise BanyanError("A api_key (API Key or Refresh Token) must be set")
         if self._debug:
             requests_log = logging.getLogger('requests.packages.urllib3')
             requests_log.setLevel(logging.DEBUG)
             requests_log.propagate = True
         self._http = self._create_session()        
         self._services = ServiceAPI(self)
         self._policies = PolicyAPI(self)
@@ -108,14 +112,18 @@
         self._users = UserAPI(self)
         self._devices = DeviceAPI(self)
         self._events = EventV2API(self)
         self._audit = AuditAPI(self)
         self._cloud_resources = CloudResourceAPI(self)
         self._services_web = ServiceWebAPI(self)
         self._services_infra = ServiceInfraAPI(self)
+        self._api_keys = ApiKeyAPI(self)
+        self._connectors = ConnectorAPI(self)
+        self._access_tiers = AccessTierAPI(self)
+        self._service_tunnels = ServiceTunnelAPI(self)
 
     def __del__(self):
         if self._http:
             try:
                 self._http.close()
             except Exception:
                 pass
@@ -125,15 +133,15 @@
     def _read_config_file(self):
         conf_path = Path.home() / '.banyan.conf'
         if conf_path.exists():
             try:
                 cp = configparser.ConfigParser(CONFIG)
                 cp.read(conf_path)
                 self._api_url = self._normalize_url(cp.get('banyan', 'api_url'))
-                self._refresh_token = cp.get('banyan', 'refresh_token')
+                self._refresh_token = cp.get('banyan', 'api_key') or cp.get('banyan', 'refresh_token')
             except configparser.Error:
                 pass
 
     # noinspection PyMethodMayBeStatic
     def _normalize_url(self, url: str) -> str:
         if '/api' not in url:
             url += '/api/v1'
@@ -258,24 +266,25 @@
 
     def paged_request(self, method: str, uri: str, params: Dict[str, Any] = None, data: Any = None,
                       json: str = None, headers: Dict[str, str] = None, accept: str = None,
                       progress_callback: ProgressCallback = None) -> JsonListOrObj:
         params = params or dict()
         skip = params.get('skip', 0)
         limit = params.get('limit', 1000)
+        search_uri = uri + "s"  # support plurals /v2/satellite -> satellites
         all_results = list()
         callback = progress_callback or self._progress_callback
 
         while True:
             params['skip'] = skip
             params['limit'] = limit
             results = self.api_request(method, uri, params, data, json, headers, accept)
             for key in results.keys():
-                logging.debug('Looking for %s in %s', key, uri)
-                if key in uri or key == 'data' or key == 'result':
+                logging.debug('Looking for %s in %s', key, search_uri)
+                if key in search_uri or key == 'data' or key == 'result':
                     if len(results[key]) == 0:
                         return all_results
                     all_results.extend(results[key])
                     logging.debug('Found %s, result count = %d, total count = %d',
                                   key, len(results[key]), len(all_results))
                     self._do_progress_callback(callback, method, uri, len(all_results),
                                                results.get('count', -1), results[key])
@@ -406,21 +415,37 @@
     def audit(self) -> AuditAPI:
         return self._audit
 
     @property
     def cloud_resources(self) -> CloudResourceAPI:
         return self._cloud_resources
 
+    @property
+    def api_keys(self) -> ApiKeyAPI:
+        return self._api_keys
+
+    @property
+    def connectors(self) -> ConnectorAPI:
+        return self._connectors
+
+    @property
+    def access_tiers(self) -> AccessTierAPI:
+        return self._access_tiers
+
+    @property
+    def service_tunnels(self) -> ServiceTunnelAPI:
+        return self._service_tunnels
 
 # configuration defaults
 CONFIG = init_defaults('banyan')
 CONFIG['banyan']['api_url'] = BanyanApiClient.DEFAULT_API_URL
 CONFIG['banyan']['refresh_token'] = None
+CONFIG['banyan']['api_key'] = None
 
 
 if __name__ == '__main__':
     logging.basicConfig(level=logging.DEBUG)
 
-    c = BanyanApiClient(api_server_url='https://gcstage.banyanops.com',
-                        refresh_token=os.getenv('BANYAN_REFRESH_TOKEN'), debug=True)
+    c = BanyanApiClient(api_url='https://preview.console.banyanops.com',
+                        refresh_token=os.getenv('BANYAN_API_KEY'), debug=True)
     print(c.get_access_token())
     print(c.services.list())
```

### Comparing `pybanyan-0.28.1/banyan/api/audit.py` & `pybanyan-0.29.0/banyan/api/audit.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,10 +31,12 @@
             (before_dt, 'end_time', int(before_dt.timestamp() * 1000000000) if before_dt else None),
             (after_dt, 'start_time', int(after_dt.timestamp() * 1000000000) if after_dt else None),
             (event_type, 'type', event_type),
             (action, 'action', action),
             (admin_email, 'admin_email', admin_email),
         ])
         response_json = self._client.api_request('GET', self.Meta.list_uri, params=params)
-        data: List[Resource] = self.Meta.info_class.Schema().load(response_json, many=True)
+        print(response_json['auditlogs'][19])
+        print(response_json['auditlogs'][20])
+        data: List[Resource] = self.Meta.info_class.Schema().load(response_json['auditlogs'], many=True)
         self._build_cache(data)
         return data
```

### Comparing `pybanyan-0.28.1/banyan/api/base.py` & `pybanyan-0.29.0/banyan/api/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -83,51 +83,83 @@
         else:
             return self.__getitem__(obj)
 
     def create(self, obj: Resource) -> Resource:
         if not self.Meta.insert_uri:
             raise BanyanError(f'{self.Meta.obj_name} API does not support creating objects')
         self._ensure_does_not_exist(obj.name)
-        response_json = self._client.api_request('POST',
-                                                 self.Meta.insert_uri,
-                                                 json=obj.Schema().dump(obj))
-        new_obj = self.Meta.info_class.Schema().load(response_json)
 
-        if self._cache:
-            self._cache.append(new_obj)
-            self._by_name[new_obj.name.lower()] = new_obj
-            self._by_id[str(new_obj.id).lower()] = new_obj
 
-        return new_obj
+        if hasattr(self.Meta, 'uri_param'):
+            # v1 pattern
+            response_json = self._client.api_request('POST',
+                                                    self.Meta.insert_uri,
+                                                    json=obj.Schema().dump(obj))
+            new_obj = self.Meta.info_class.Schema().load(response_json)
+            if self._cache:
+                self._cache.append(new_obj)
+                self._by_name[new_obj.name.lower()] = new_obj
+                self._by_id[str(new_obj.id).lower()] = new_obj
+            return new_obj
+        else:
+            # v2 pattern
+            response_json = self._client.api_request('POST',
+                                                    self.Meta.insert_uri,
+                                                    json=obj.Schema().dump(obj))          
+            if self._cache:
+                self.list()
+            return response_json
+
 
     def update(self, obj: Resource) -> Resource:
         if not self.Meta.insert_uri:
             raise BanyanError(f'{self.Meta.obj_name} API does not support updating objects')
         self._ensure_exists(obj.name)
-        response_json = self._client.api_request('POST',
-                                                 self.Meta.insert_uri,
-                                                 json=obj.Schema().dump(obj))
-        updated_obj = self.Meta.info_class.Schema().load(response_json)
 
-        if self._cache:
-            old_obj = self._by_id[str(obj.id).lower()]
-            self._cache.remove(old_obj)
-            self._cache.append(updated_obj)
-            self._by_name[updated_obj.name.lower()] = updated_obj
-            self._by_id[str(updated_obj.id).lower()] = updated_obj
+        if hasattr(self.Meta, 'uri_param'):
+            # v1 pattern
+            response_json = self._client.api_request('POST',
+                                                    self.Meta.insert_uri,
+                                                    json=obj.Schema().dump(obj))
+            updated_obj = self.Meta.info_class.Schema().load(response_json)
+
+            if self._cache:
+                old_obj = self._by_id[str(obj.id).lower()]
+                self._cache.remove(old_obj)
+                self._cache.append(updated_obj)
+                self._by_name[updated_obj.name.lower()] = updated_obj
+                self._by_id[str(updated_obj.id).lower()] = updated_obj
+
+            return updated_obj
+        else:
+            # v2 pattern
+            upd_uri = f'{self.Meta.insert_uri}/{str(obj.id)}'
+            response_json = self._client.api_request('PUT',
+                                                    upd_uri,
+                                                    json=obj.Schema().dump(obj))
+            if self._cache:
+                self.list()
+            return response_json
 
-        return updated_obj
 
     def delete(self, obj: ResourceOrName) -> str:
         if not self.Meta.delete_uri:
             raise BanyanError(f'{self.Meta.obj_name} API does not support deleting objects')
         obj = self.find(obj)
         assert isinstance(obj, Resource)
-        json_response = self._client.api_request('DELETE',
-                                                 self.Meta.delete_uri,
-                                                 params={self.Meta.uri_param: str(obj.id)})
+
+        if hasattr(self.Meta, 'uri_param'):
+            # v1 pattern
+            del_uri = self.Meta.delete_uri
+            params = {self.Meta.uri_param: str(obj.id)}
+        else:
+            # v2 pattern
+            del_uri = self.Meta.delete_uri.replace('ID', str(obj.id))
+            params = {}
+
+        json_response = self._client.api_request('DELETE', del_uri, params=params)
         if self._cache:
             self._cache.remove(obj)
             del self._by_name[obj.name.lower()]
             del self._by_id[str(obj.id).lower()]
 
-        return json_response['Message']
+        return json_response
```

### Comparing `pybanyan-0.28.1/banyan/api/cloud_resource.py` & `pybanyan-0.29.0/banyan/api/cloud_resource.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/api/device.py` & `pybanyan-0.29.0/banyan/api/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 from banyan.api.base import ApiBase
 from banyan.core.exc import BanyanError
-from banyan.model.user_device import Device, TrustScore
+from banyan.model.user_device import Device, DeviceV2, TrustScore
 
 
 class DeviceAPI(ApiBase):
     """
     API service for dealing with end-user devices (laptops, tablets, phones, etc).
 
     """
@@ -15,17 +15,17 @@
     _UPDATE_FIELDS = ['architecture', 'model', 'platform', 'ownership', 'is_banned']
 
     class Meta:
         """
         :meta private:
         """
         data_class = Device
-        info_class = Device
+        info_class = DeviceV2
         arg_type = str
-        list_uri = '/devices'
+        list_uri = '/v2/devices'
         delete_uri = '/delete_device'
         insert_uri = '/mdm/update_device'
         uri_param = 'SerialNumber'
         obj_name = 'device'
         supports_paging = True
 
     def create(self, obj: Device):
@@ -35,63 +35,73 @@
 
         :param obj: A device which will definitely not be created.
         :type obj: Device
         :raises: :py:exc:`BanyanError`
         """
         raise BanyanError('devices cannot be created via the API')
 
-    def update(self, obj: Device) -> str:
+    def update(self, obj: DeviceV2) -> str:
         """
         Updates a limited set of properties belonging to a device. The properties that can be updated are:
 
         * Device hardware data: :py:data:`architecture`, :py:data:`model`, and :py:data:`platform`.
         * Corporate ownership status: :py:data:`ownership`.
         * Banned status: :py:data:`is_banned`.
-        * User-friendly device name: :py:data:`device_friendly_name`.
+        * Device Management status: :py:data:`mdm_present`, :py:data:`mdm_vendor_name`.
 
         Changes to any other fields in the :py:class:`Device` object will be ignored.
 
         :param obj: The device to be updated.
         :type obj: Device
         :return: Message from the server indicating success or failure.
         :rtype: str
         """
         self._ensure_exists(obj.serial_number)
+        change_attr = {
+            "Model": obj.model,
+            "Ownership": obj.ownership,
+            "Platform": obj.platform,
+            "OS": obj.os,
+            "Architecture": obj.architecture,
+            "Banned": obj.banned,
+            "IsMDMPresent": obj.mdm_present,
+            "MDMVendorName": obj.mdm_vendor_name
+        }
         response_json = self._client.api_request('POST',
                                                  self.Meta.insert_uri,
                                                  params={self.Meta.uri_param: obj.serial_number},
-                                                 json=obj.Schema(only=DeviceAPI._UPDATE_FIELDS).dump(obj))
+                                                 json=change_attr)
         return response_json['Message']
 
-    def ban(self, obj: Device) -> str:
+    def ban(self, obj: DeviceV2) -> str:
         """
         Bans a device, preventing it from accessing sites controlled by Banyan.
 
         :param obj: The device to be banned.
         :type obj: Device
         :return: Message from the server indicating success or failure.
         :rtype: str
         """
-        obj.is_banned = True
+        obj.banned = True
         return self.update(obj)
 
-    def unban(self, obj: Device) -> str:
+    def unban(self, obj: DeviceV2) -> str:
         """
         Un-bans a device, allowing it to resume accessing sites controlled by Banyan.
 
         .. note:: After a device is unbanned, it must send updated Trust Factors to the server
            before it will be allowed to access anything. This happens automatically about once an hour,
            or can be forced manually by clicking the "Send Device Features" link in the app settings.
 
         :param obj: The device to be unbanned.
         :type obj: Device
         :return: Message from the server indicating success or failure.
         :rtype: str
         """
-        obj.is_banned = False
+        obj.banned = False
         return self.update(obj)
 
     def set_max_trustlevel(self, obj: Device, max_level: str, reason: str, ext_source: str) -> str:
         """
         Overrides the maximum trust score a device will be allowed to have.
 
         :param obj: The device to be updated.
```

### Comparing `pybanyan-0.28.1/banyan/api/event_v2.py` & `pybanyan-0.29.0/banyan/api/event_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from datetime import datetime, timedelta
 from typing import List, Dict, Any, Set
 from uuid import UUID
 
-from semver import deprecated
-
 from banyan.api.base import ApiBase, Resource
 from banyan.model import BanyanApiObject
 from banyan.model.event_v2 import EventV2, EventOrID
 
 
 class EventV2API(ApiBase):
     class Meta:
@@ -36,15 +34,15 @@
                                    device_id, device_serial, container_id, service_name, event_id)
         return self._count(params)
 
     def _count(self, params: Dict[str, Any]) -> int:
         response_json = self._client.api_request('GET', '/events/count', params=params)
         return response_json['data']
 
-    @deprecated(replace='banyan.api.event_v2.list')
+    #@deprecated(replace='banyan.api.event_v2.list')
     def list2(self, before_dt: datetime = None, after_dt: datetime = None, order: str = None,
               event_type: str = None, subtype: str = None, action: str = None,
               email_address: str = None, device_id: str = None, device_serial: str = None,
               container_id: str = None, service_name: str = None, event_id: str = None) -> List[Resource]:
         params = self._make_params(before_dt, after_dt, order, event_type, subtype, action, email_address,
                                    device_id, device_serial, container_id, service_name, event_id)
         return self._list_paged(params)
```

### Comparing `pybanyan-0.28.1/banyan/api/netagent.py` & `pybanyan-0.29.0/banyan/api/netagent.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/api/policy.py` & `pybanyan-0.29.0/banyan/api/policy.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/api/role.py` & `pybanyan-0.29.0/banyan/api/role.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/api/service.py` & `pybanyan-0.29.0/banyan/api/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/api/service_infra.py` & `pybanyan-0.29.0/banyan/api/service_infra.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/api/service_web.py` & `pybanyan-0.29.0/banyan/api/service_web.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/api/shield.py` & `pybanyan-0.29.0/banyan/api/shield.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/api/user.py` & `pybanyan-0.29.0/banyan/api/user.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/controllers/admin.py` & `pybanyan-0.29.0/banyan/controllers/admin.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/controllers/audit.py` & `pybanyan-0.29.0/banyan/controllers/audit.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/controllers/base.py` & `pybanyan-0.29.0/banyan/controllers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,32 +32,32 @@
             # add a version banner
             (['--version', '-v'],
              {'action': 'version',
               'version': VERSION_BANNER}),
             (['--api-url'],
              {'help': 'URL for the Banyan API server. Can also be configured via the BANYAN_API_URL '
                       'environment variable.'}),
-            (['--refresh-token'],
-             {'help': 'API token used for the initial authentication to the Banyan API server. Can also be '
-                      'configured via the BANYAN_REFRESH_TOKEN environment variable.'}),
+            (['--api-key'],
+             {'help': 'API credential used for the authentication to the Banyan API server. Can also be '
+                      'configured via the BANYAN_API_KEY or BANYAN_REFRESH_TOKEN environment variable.'}),
             (['--insecure-tls', '-k'],
              {'action': 'store_true',
              'help': 'Allow connections to API servers with invalid TLS certificates.'}),
             (['--output-format', '-o'],
              {'choices': ['table', 'json', 'yaml'],
               'help': 'desired output format (table, json, yaml)'}),
         ]
 
     def _post_argument_parsing(self):
         super()._post_argument_parsing()
         self.app.client.insecure_tls = self.app.pargs.insecure_tls
         if self.app.pargs.api_url:
             self.app.client.api_url = self.app.pargs.api_url
-        if self.app.pargs.refresh_token:
-            self.app.client.refresh_token = self.app.pargs.refresh_token
+        if self.app.pargs.api_key:
+            self.app.client.refresh_token = self.app.pargs.api_key
 
     def _default(self):
         """Default action if no sub-command is passed."""
         self.app.args.print_help()
 
     @staticmethod
     def get_json_input(arg: str):
@@ -66,14 +66,26 @@
         elif arg == '-':
             arg = sys.stdin.read()
         else:
             arg = arg.encode('utf-8')
         return json.loads(arg)       
 
     @staticmethod
+    def trunc(value, num_chars, align_left = False) -> str:
+        if not value:
+            return ''
+        value = str(value)
+        if len(value) < num_chars + 3:
+            return value
+        elif align_left:
+            return value[:num_chars] + '...'
+        else:
+            return '...' + value[-num_chars:]
+
+    @staticmethod
     def wait_for_input(wait: bool, text: str):
         print('\n--> %s:' % text)
         if not wait:
             return
         user_input = input('press enter to continue, type "stop" to stop ...\n')
         if 'stop' in user_input:
             raise RuntimeError('User terminated workflow')
```

### Comparing `pybanyan-0.28.1/banyan/controllers/cloud_resource.py` & `pybanyan-0.29.0/banyan/controllers/cloud_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,58 +21,50 @@
         stacked_on = 'base'
         help = 'manage cloud resources discovered from IaaS'
 
     @property
     def _client(self) -> BanyanApiClient:
         return self.app.client
 
-    def trunc(self, value, num_chars) -> str:
-        if not value:
-            return ''
-        value = str(value)
-        if len(value) < num_chars + 3:
-            return value
-        else:
-            return '...' + value[-num_chars:]
 
     @ex(help='list cloud_resources',
         arguments=[
-            (['--cloud'], 
+            (['--cloud'],
             {
                 'help': 'filter by provider - AWS | AZURE | GCP | OCI | ...'
             }),
-            (['--account'], 
+            (['--account'],
             {
                 'help': 'filter by account'
             }),
-            (['--region'], 
+            (['--region'],
             {
                 'help': 'filter by region/location/zone'
             }),
-            (['--resource_type'], 
+            (['--resource_type'],
             {
                 'help': 'filter by type - ec2 | vm | rds | ...'
             })
         ])
     def list(self):
         params={'cloud_provider': self.app.pargs.cloud, 'account': self.app.pargs.account, 'region': self.app.pargs.region, 'resource_type': self.app.pargs.resource_type}
         synced_resources: List[CloudResourceInfo] = self._client.cloud_resources.list(params=params)
-        results = list()
+        results = []
         headers = ['Name', 'ID', 'Cloud', 'Account', 'Region', 'Type', 'Private Address', 'Public Address', '# Tags', 'Status']
         for res in synced_resources:
-            new_res = [res.name[:20], res.resource_udid, res.cloud_provider, self.trunc(res.account,6), 
+            new_res = [res.name[:20], res.resource_udid, res.cloud_provider, Base.trunc(res.account,6), 
                        res.region, res.resource_type, 
-                       self.trunc(res.private_ip or res.private_dns_name, 24), 
-                       self.trunc(res.public_ip or res.public_dns_name, 24), 
+                       Base.trunc(res.private_ip or res.private_dns_name, 24), 
+                       Base.trunc(res.public_ip or res.public_dns_name, 24), 
                        len(res.tags or []), res.status]
             results.append(new_res)
         self.app.render(results, handler='tabulate', headers=headers, tablefmt='simple')
 
 
-    @ex(help='show details & tags of a cloud_resource', 
+    @ex(help='show details & tags of a cloud_resource',
         arguments=[
             (['resource_uuid'],
             {
                 'help': 'get discovered resource by Banyan UUID.'
             }),            
         ])
     def get(self):
@@ -80,28 +72,28 @@
         d_resource: CloudResourceInfo = self._client.cloud_resources.get(id)
         dr_json = CloudResourceInfo.Schema().dump(d_resource)
         self.app.render(dr_json, handler='json', indent=2, sort_keys=True)
 
 
     @ex(help='create a new cloud_resource',
         arguments=[
-            (['resources_json'], 
+            (['resources_json'],
             {
                 'help': 'JSON blob describing the new discovered resource(s) to be created, or a filename '
                          'containing JSON prefixed by "@" (example: @res.json).'
             }),
         ])
     def create(self):
         d_resource = Base.get_json_input(self.app.pargs.resources_json)
         d_resource: CloudResourceInfo = self._client.cloud_resources.create(d_resource)
         dr_json = CloudResource.Schema().dump(d_resource)
         self.app.render(dr_json, handler='json', indent=2, sort_keys=True)
 
 
-    @ex(hide=True, help='update status for a given cloud_resource record', 
+    @ex(hide=True, help='update status for a given cloud_resource record',
         arguments=[
             (['resource_uuid'],
             {
                 'help': 'Banyan UUID of discovered resource to update.'
             }),
             (['status'],
             {
@@ -145,15 +137,15 @@
             }),            
         ])
     def list_associations(self):
         assocs = self._client.cloud_resources.associations(self.app.pargs.resource_uuid)
         results = list()
         headers = ['ID', 'Resource ID', 'Resource Name', 'Resource Type', 'Service ID', 'Service Name', 'Resource Status']
         for res in assocs:
-            new_res = [res.id, self.trunc(res.resource_udid,9), res.resource_name, res.resource_type, 
+            new_res = [res.id, Base.trunc(res.resource_udid,9), res.resource_name, res.resource_type, 
                        res.service_id, res.service_name, res.resource_status]
             results.append(new_res)
         self.app.render(results, handler='tabulate', headers=headers, tablefmt='simple')
 
 
     @ex(hide=True, help='associate cloud_resource with service', 
         arguments=[
```

### Comparing `pybanyan-0.28.1/banyan/controllers/device.py` & `pybanyan-0.29.0/banyan/controllers/device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from cement import Controller, ex
 
 from banyan.api import DeviceAPI
 from banyan.controllers.base import Base
-from banyan.model.user_device import Device, TrustScore, TrustLevel
+from banyan.model.user_device import Device, DeviceV2, TrustScore, TrustLevel
 
 
 class DeviceController(Controller):
     class Meta:
         label = 'device'
         stacked_type = 'nested'
         stacked_on = 'base'
@@ -16,18 +16,19 @@
     def _client(self) -> DeviceAPI:
         return self.app.client.devices
 
     @ex(help='list devices')
     def list(self):
         devices = self._client.list()
         results = list()
-        headers = ['Device Name', 'Serial Number', 'Platform', 'Ownership', 'Trust Score', 'Banned', 'Last Login']
+        headers = ['Device Name', 'Serial Number', 'Platform', 'Ownership', 'MDM', 'MDM Vendor', 'Trust Level', 'Trust Status', 'Last Login']
         for device in devices:
-            new_row = [device.device_friendly_name, device.serial_number, device.platform,
-                       device.ownership, device.trust_data.level, device.is_banned,
+            new_row = [Base.trunc(device.device_friendly_name, 8, True), device.serial_number, device.platform,
+                       device.ownership, device.mdm_present, device.mdm_vendor_name,
+                       device.trust_level, device.trust_status,
                        device.last_login.strftime(Base.TABLE_DATE_FORMAT) if device.last_login else 'None']
             results.append(new_row)
         results.sort(key=lambda x: x[0])
         self.app.render(results, handler='tabulate', headers=headers, tablefmt='simple')
 
     @ex(help='show detailed information about a device',
         arguments=[
@@ -35,22 +36,45 @@
              {
                  'help': 'Serial number of the device.'
              }),
         ])
     def get(self):
         serial_number = self.app.pargs.serial_number
         device = self._client.find(serial_number)
-        device_json = Device.Schema().dump(device)
+        device_json = DeviceV2.Schema().dump(device)
         # colorized_json = highlight(policy_json, lexers.JsonLexer(), formatters.Terminal256Formatter(style="default"))
         self.app.render(device_json, handler='json', indent=2, sort_keys=True)
 
-    # TODO: implement /mdm/update_device?SerialNumber=X
-    @ex(help='update device status')
+    @ex(help='update device attributes to set MDM vendor presence',
+        arguments=[
+            (['serial_number'],
+             {
+                 'help': 'Serial number of the device.'
+             }),
+             (['--mdm_present'], 
+             {
+                 'required': True,
+                 'choices': ["true", "True", "false", "False"],
+                 'help': 'Set MDM present to true/false.'
+             }),
+             (['--mdm_vendor_name'],
+             {
+                 'required': True,        
+                 'help': 'Set MDM vendor name.'        
+             })
+        ])        
     def update(self):
-        pass
+        # get the device first
+        serial_number = self.app.pargs.serial_number
+        device = self._client.find(serial_number)
+        device.mdm_present = self.app.pargs.mdm_present.lower() == "true"
+        device.mdm_vendor_name = self.app.pargs.mdm_vendor_name
+        print(self._client.update(device))
+        device_json = DeviceV2.Schema().dump(device)
+        self.app.render(device_json, handler='json', indent=2, sort_keys=True)
 
     # TODO: implement /delete_device?Email=X&SerialNumber=Y
     @ex(help='delete a device')
     def delete(self):
         pass
 
     # TODO: implement /device/unregister
```

### Comparing `pybanyan-0.28.1/banyan/controllers/event.py` & `pybanyan-0.29.0/banyan/controllers/event.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/controllers/export.py` & `pybanyan-0.29.0/banyan/controllers/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         )
     def roles(self):
         role_path = self._mkdir('roles')
         self.app.print(f' * Exporting roles to {role_path}')
         all_roles = self._client.roles.list()
         for role in all_roles:
             with open(self._mkfile(role_path, f'{role.name}.role.json'), 'w') as f:
-                f.write(role.role.Schema().dumps(role.role))
+                f.write(role.role_spec.Schema().dumps(role.role))
 
     @ex(help='export policies from an organization',
         arguments=[
             (['--path'],
              {
                  'help': 'Directory to place the object JSON files.',
                  'default': os.getcwd()
@@ -58,15 +58,15 @@
         )
     def policies(self):
         policy_path = self._mkdir('policies')
         self.app.print(f' * Exporting policies to {policy_path}')
         all_policies = self._client.policies.list()
         for policy in all_policies:
             with open(self._mkfile(policy_path, f'{policy.name}.policy.json'), 'w') as f:
-                f.write(policy.policy.Schema().dumps(policy.policy))
+                f.write(policy.policy_spec.Schema().dumps(policy.policy))
 
     @ex(help='export services from an organization',
         arguments=[
             (['--path'],
              {
                  'help': 'Directory to place the object JSON files.',
                  'default': os.getcwd()
@@ -75,15 +75,15 @@
         )
     def services(self):
         service_path = self._mkdir('services')
         self.app.print(f' * Exporting services to {service_path}')
         all_services = self._client.services.list()
         for service in all_services:
             with open(self._mkfile(service_path, f'{service.name}.service.json'), 'w') as f:
-                f.write(service.service.Schema().dumps(service.service))
+                f.write(service.service_spec.Schema().dumps(service.service))
             attached = self._client.services.attached_policy(service)
             if attached:
                 with open(self._mkfile(service_path, f'{service.name}.attach.json'), 'w') as f:
                     f.write(attached.Schema().dumps(attached))
 
     def _mkdir(self, subdir: str) -> str:
         path = os.path.join(self.app.pargs.path, subdir)
```

### Comparing `pybanyan-0.28.1/banyan/controllers/netagent.py` & `pybanyan-0.29.0/banyan/controllers/netagent.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class NetagentController(Controller):
     class Meta:
         label = 'netagent'
         stacked_type = 'nested'
         stacked_on = 'base'
-        help = 'manage netagents (AccessTiers and HostAgents)'
+        help = '(deprecated: use access-tier) manage netagents'
 
     @property
     def _client(self) -> NetagentAPI:
         return self.app.client.netagents
 
     @ex(help='list netagents',
         arguments=[
```

### Comparing `pybanyan-0.28.1/banyan/controllers/policy.py` & `pybanyan-0.29.0/banyan/controllers/policy.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/controllers/role.py` & `pybanyan-0.29.0/banyan/controllers/role.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/controllers/service.py` & `pybanyan-0.29.0/banyan/controllers/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 
 class ServiceController(Controller):
     class Meta:
         label = 'service'
         stacked_type = 'nested'
         stacked_on = 'base'
-        help = '(deprecated) manage web and TCP services and workloads'
+        help = '(deprecated: use service-web or service-infra) manage web and TCP services and workloads'
 
     @property
     def _client(self) -> ServiceAPI:
         return self.app.client.services
 
     @ex(help='list registered services')
     def list(self):
         services: List[ServiceInfo] = self._client.list()
         results = list()
         headers = ['Name', 'ID', 'Type', 'Enabled', 'Created', 'Last Updated']
         for service in services:
-            app_type = service.service.metadata.tags.service_app_type
+            app_type = service.service_spec.metadata.tags.service_app_type
             new_row = [service.service_name, service.service_id, app_type, service.enabled,
                        service.created_at.strftime(Base.TABLE_DATE_FORMAT),
                        service.last_updated_at.strftime(Base.TABLE_DATE_FORMAT)]
             results.append(new_row)
         results.sort(key=lambda x: x[0])
         self.app.render(results, handler='tabulate', headers=headers, tablefmt='simple')
 
@@ -206,15 +206,15 @@
         try:
             from banyan.ext.idp.okta import OktaApplicationController
         except Exception as ex:
             raise NotImplementedError("Okta SDK not configured correctly > %s" % ex.args[0])
 
         self._client.list()
         service_info: ServiceInfo = self._client[self.app.pargs.service_name]
-        if not service_info.service.spec.http_settings.oidc_settings.enabled:
+        if not service_info.service_spec.spec.http_settings.oidc_settings.enabled:
             raise RuntimeError('Service needs to be of type WEB')
 
         Base.wait_for_input(True, 'Get service to add to Okta:')
         svc = service_info.service
         service_json = Service.Schema().dump(svc)
         self.app.render(service_json, handler='json', indent=2, sort_keys=True)
 
@@ -243,15 +243,15 @@
         try:
             from banyan.ext.idp.azure_ad import AzureADApplicationController
         except Exception as ex:
             raise NotImplementedError("Azure AD Microsoft Graph SDK not configured correctly > %s" % ex.args[0]) 
 
         self._client.list()
         service_info: ServiceInfo = self._client[self.app.pargs.service_name]
-        if not service_info.service.spec.http_settings.oidc_settings.enabled:
+        if not service_info.service_spec.spec.http_settings.oidc_settings.enabled:
             raise RuntimeError('Service needs to be of type WEB')
 
         Base.wait_for_input(True, 'Get service to add to AzureAD:')
         svc = service_info.service
         service_json = Service.Schema().dump(svc)
         self.app.render(service_json, handler='json', indent=2, sort_keys=True)
```

### Comparing `pybanyan-0.28.1/banyan/controllers/service_infra.py` & `pybanyan-0.29.0/banyan/controllers/service_infra.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     @ex(help='list infrastructure services')
     def list(self):
         services: List[ServiceInfo] = self._client.list()
         results = list()
         headers = ['Name', 'ID', 'Type', 'Enabled', 'Created', 'Last Updated']
         for service in services:
-            app_type = service.service.metadata.tags.service_app_type
+            app_type = service.service_spec.metadata.tags.service_app_type
             new_row = [service.service_name, service.service_id, app_type, service.enabled,
                        service.created_at.strftime(Base.TABLE_DATE_FORMAT),
                        service.last_updated_at.strftime(Base.TABLE_DATE_FORMAT)]
             results.append(new_row)
         results.sort(key=lambda x: x[0])
         self.app.render(results, handler='tabulate', headers=headers, tablefmt='simple')
```

### Comparing `pybanyan-0.28.1/banyan/controllers/service_web.py` & `pybanyan-0.29.0/banyan/controllers/service_web.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     def _client(self) -> ServiceWebAPI:
         return self.app.client.services_web
 
 
     @ex(help='list hosted website services')
     def list(self):
         services: List[ServiceInfo] = self._client.list()
-        results = list()
+        results = []
         headers = ['Name', 'ID', 'Type', 'Enabled', 'Created', 'Last Updated']
         for service in services:
-            app_type = service.service.metadata.tags.service_app_type
+            app_type = service.service_spec.metadata.tags.service_app_type
             new_row = [service.service_name, service.service_id, app_type, service.enabled,
                        service.created_at.strftime(Base.TABLE_DATE_FORMAT),
                        service.last_updated_at.strftime(Base.TABLE_DATE_FORMAT)]
             results.append(new_row)
         results.sort(key=lambda x: x[0])
         self.app.render(results, handler='tabulate', headers=headers, tablefmt='simple')
 
@@ -186,15 +186,15 @@
         try:
             from banyan.ext.idp.okta import OktaApplicationController
         except Exception as exc:
             raise NotImplementedError("Okta SDK not configured correctly > %s" % exc.args[0])
 
         self._client.list()
         service_info: ServiceInfo = self._client[self.app.pargs.service_name]
-        if not service_info.service.spec.http_settings.oidc_settings.enabled:
+        if not service_info.service_spec.spec.http_settings.oidc_settings.enabled:
             raise RuntimeError('Service needs to be of type WEB')
 
         Base.wait_for_input(True, 'Get service to add to Okta:')
         svc = service_info.service
         service_json = Service.Schema().dump(svc)
         self.app.render(service_json, handler='json', indent=2, sort_keys=True)
 
@@ -223,15 +223,15 @@
         try:
             from banyan.ext.idp.azure_ad import AzureADApplicationController
         except Exception as exc:
             raise NotImplementedError("Azure AD Microsoft Graph SDK not configured correctly > %s" % exc.args[0]) 
 
         self._client.list()
         service_info: ServiceInfo = self._client[self.app.pargs.service_name]
-        if not service_info.service.spec.http_settings.oidc_settings.enabled:
+        if not service_info.service_spec.spec.http_settings.oidc_settings.enabled:
             raise RuntimeError('Service needs to be of type WEB')
 
         Base.wait_for_input(True, 'Get service to add to AzureAD:')
         svc = service_info.service
         service_json = Service.Schema().dump(svc)
         self.app.render(service_json, handler='json', indent=2, sort_keys=True)
```

### Comparing `pybanyan-0.28.1/banyan/controllers/shield.py` & `pybanyan-0.29.0/banyan/controllers/shield.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class ShieldController(Controller):
     class Meta:
         label = 'shield'
         stacked_type = 'nested'
         stacked_on = 'base'
-        help = 'manage Banyan Shield clusters'
+        help = '(deprecated) manage shield clusters'
 
     @property
     def _client(self) -> ShieldAPI:
         return self.app.client.shields
 
     @ex(help='list shields')
     def list(self):
```

### Comparing `pybanyan-0.28.1/banyan/controllers/user.py` & `pybanyan-0.29.0/banyan/controllers/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class UserController(Controller):
     class Meta:
         label = 'user'
         stacked_type = 'nested'
         stacked_on = 'base'
-        help = 'manage user accounts'
+        help = 'manage users'
 
     @property
     def _client(self) -> UserAPI:
         return self.app.client.users
 
     @ex(help='list users')
     def list(self):
```

### Comparing `pybanyan-0.28.1/banyan/ext/iaas/aws.py` & `pybanyan-0.29.0/banyan/ext/iaas/aws.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/ext/iaas/azure_cloud.py` & `pybanyan-0.29.0/banyan/ext/iaas/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/ext/iaas/base.py` & `pybanyan-0.29.0/banyan/ext/iaas/base.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/ext/iaas/gcp.py` & `pybanyan-0.29.0/banyan/ext/iaas/gcp.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/ext/iaas/oracle_cloud.py` & `pybanyan-0.29.0/banyan/ext/iaas/oracle_cloud.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/ext/iaas/vmware.py` & `pybanyan-0.29.0/banyan/ext/iaas/vmware.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/ext/idp/azure_ad.py` & `pybanyan-0.29.0/banyan/ext/idp/azure_ad.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/ext/idp/base.py` & `pybanyan-0.29.0/banyan/ext/idp/base.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/ext/idp/okta.py` & `pybanyan-0.29.0/banyan/ext/idp/okta.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/lib/certs.py` & `pybanyan-0.29.0/banyan/lib/certs.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/lib/cloud/__init__.py` & `pybanyan-0.29.0/banyan/lib/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/lib/cloud/aws.py` & `pybanyan-0.29.0/banyan/lib/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/lib/service.py` & `pybanyan-0.29.0/banyan/lib/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/main.py` & `pybanyan-0.29.0/banyan/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,26 +15,34 @@
 from banyan.controllers.role import RoleController
 from banyan.controllers.service import ServiceController
 from banyan.controllers.service_web import ServiceWebController
 from banyan.controllers.service_infra import ServiceInfraController
 from banyan.controllers.shield import ShieldController
 from banyan.controllers.user import UserController
 from banyan.controllers.cloud_resource import CloudResourceController
+from banyan.controllers.api_key import ApiKeyController
+from banyan.controllers.connector import ConnectorController
+from banyan.controllers.access_tier import AccessTierController
+from banyan.controllers.service_tunnel import ServiceTunnelController
+
 from .core.exc import BanyanError
 
 # configuration defaults
 CONFIG = init_defaults('banyan')
 CONFIG['banyan']['api_url'] = BanyanApiClient.DEFAULT_API_URL
 CONFIG['banyan']['refresh_token'] = None
+CONFIG['banyan']['api_key'] = None
 
 
 def extend_client(app: App) -> None:
     api_url = app.config.get('banyan', 'api_url')
     refresh_token = app.config.get('banyan', 'refresh_token')
-    client = BanyanApiClient(api_url, refresh_token, debug=app.debug)
+    api_key = app.config.get('banyan', 'api_key')
+    credential = api_key or refresh_token
+    client = BanyanApiClient(api_url, credential, debug=app.debug)
     app.extend('client', client)
 
 
 def set_logging(app: App) -> None:
     if app.debug:
         logging.basicConfig(level=logging.DEBUG)
 
@@ -78,28 +86,31 @@
 
         # set the output handler
         output_handler = 'tabulate'
 
         # register handlers
         handlers = [
             Base,
-            CloudResourceController,
-            ServiceInfraController,
+            UserController,
             ServiceWebController,
-            ServiceController,
+            ServiceTunnelController,
+            ServiceInfraController,
             RoleController,
             PolicyController,
-            ShieldController,
-            NetagentController,
-            UserController,
-            DeviceController,
-            AdminController,
+            ExportController,
             EventV2Controller,
+            DeviceController,
+            ConnectorController,
+            CloudResourceController,
             AuditController,
-            ExportController
+            ApiKeyController,
+            AccessTierController,
+            ShieldController,
+            ServiceController,
+            NetagentController,
         ]
 
 
 class MyAppTest(TestApp, MyApp):
     """A sub-class of MyApp that is better suited for testing."""
 
     class Meta:
```

### Comparing `pybanyan-0.28.1/banyan/model/__init__.py` & `pybanyan-0.29.0/banyan/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from abc import ABC
 from dataclasses import field
 from datetime import datetime
 from ipaddress import IPv4Interface
-from typing import ClassVar, Type, Union
+from typing import ClassVar, Type, Union, Optional
 
 from aenum import StrEnum
 from marshmallow import fields, Schema, post_dump
 from marshmallow_dataclass import dataclass
 from semver import VersionInfo
 
 from banyan.core.exc import BanyanError
 
-API_VERSION = "rbac.banyanops.com/v1"
-
 
 class BanyanEnum(StrEnum):
 
     # noinspection PyTypeChecker
     @classmethod
     def choices(cls):
         return [m.value for m in cls]
@@ -130,23 +128,27 @@
             return str(value)
         else:
             return super()._serialize(value, attr, data, **kwargs)
 
 
 @dataclass
 class BanyanApiObject:
+    API_VERSION = "rbac.banyanops.com/v1"
     TYPE = "origin"
-    apiVersion: str
+    KIND = ""
+
+    apiVersion: Optional[str]
+    type: Optional[str]
     kind: str
-    type: str
     Schema: ClassVar[Type[Schema]] = Schema
 
     def __post_init__(self):
-        self.apiVersion = API_VERSION
+        self.apiVersion = self.API_VERSION
         self.type = self.TYPE
+        self.kind = self.KIND
 
     @property
     def name(self) -> str:
         raise NotImplementedError('not implemented in the base class')
 
 
 @dataclass
```

### Comparing `pybanyan-0.28.1/banyan/model/attachment.py` & `pybanyan-0.29.0/banyan/model/attachment.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/model/audit.py` & `pybanyan-0.29.0/banyan/model/audit.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,34 +14,42 @@
 from banyan.model.service import ServiceInfo
 
 
 class AuditEventType(BanyanEnum):
     ADMIN_SIGN_ON = "admin_sign_on"
     IDP_SETTINGS = "idp_settings"
     MDM_SETTINGS = "mdm_settings"
-    TRUSTSCORE_FACTORS = "trustscore_factors"
-    UNKNOWN_DEVICE_SETTINGS = "unknown_device"
-    SECURITY_ATTACH_POLICY = "security_attach_policy"
     POLICY = "policy"
     REGISTERED_SERVICE = "registered_service"
     ROLE = "role"
+    SECURITY_ATTACH_POLICY = "security_attach_policy"
+    TRUSTSCORE_FACTORS = "trustscore_factors"
+    UNKNOWN_DEVICE_SETTINGS = "unknown_device"
     DEVICE_REGISTRATION_IDP_SETTINGS = "device_registration_idp_settings"
     ADMIN_USER = "admin_user"
     MDM_DEPLOY_OTP_SKIP_ROLE = "mdm_deploy_otp_skip_role"
     MDM_DEPLOY_KEY = "mdm_deploy_key"
     INVITATION_CODE = "invitation_code"
     TRUSTSCORE_TTL = "trustscore_ttl"
     ENDUSER_DEVICE = "enduser_device"
     PREFERRED_APPLICATIONS = "preferred_applications"
     LATEST_OS_CONFIG = "latest_os_config"
     TRUST_CONFIG = "trust_config"
     ROOT_CERTS = "root_certs"
     SAAS_APPLICATIONS = "saas_applications"
     IDP_ROUTED_APPLICATIONS = "idp_routed_applications"
-
+    ACCESS_TIER = "access_tier"
+    CONNECTOR = "satellite"
+    ACCESS_TIER_TUNNEL = "access_tier_tunnel"
+    API_KEY = "api_key"
+    ENDUSER = "enduser"
+    DEVICE = "device"
+    SERVICE_TUNNEL = "service_tunnel"
+    REFRESH_TOKEN = "refresh_token"
+    ORG = "org"
 
 class AuditAction(BanyanEnum):
     UPDATE = "update"
     CREATE = "create"
     DELETE = "delete"
     ENABLE = "enable"
     DISABLE = "disable"
```

### Comparing `pybanyan-0.28.1/banyan/model/cloud_resource.py` & `pybanyan-0.29.0/banyan/model/cloud_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,8 +93,9 @@
     resource_status: str = field(metadata={"data_key": "status"})
     service_id: str
     service_name: str
     Schema: ClassVar[Type[Schema]] = Schema
 
     @property
     def cloud_resource_id(self) -> str:
-        return str(self.resource_udid)
+        return str(self.resource_udid)
+
```

### Comparing `pybanyan-0.28.1/banyan/model/event_v2.py` & `pybanyan-0.29.0/banyan/model/event_v2.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/model/netagent.py` & `pybanyan-0.29.0/banyan/model/netagent.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/model/policy.py` & `pybanyan-0.29.0/banyan/model/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,17 +128,14 @@
         unknown = EXCLUDE
         ordered = True
 
     KIND = "BanyanPolicy"
     metadata: Metadata
     spec: Spec
 
-    def __post_init__(self):
-        self.kind = self.KIND
-
     @property
     def name(self):
         return self.metadata.name
 
 
 @dataclass
 class PolicyInfo(InfoBase):
@@ -149,15 +146,15 @@
     policy_name: str = field(metadata={'data_key': 'PolicyName'})
     spec: str = field(metadata={'data_key': 'PolicySpec'})
     description: str = field(metadata={'data_key': 'Description'})
     version: int = field(metadata={'data_key': 'PolicyVersion'})
     Schema: ClassVar[Schema] = Schema
 
     @property
-    def policy(self) -> Policy:
+    def policy_spec(self) -> Policy:
         return Policy.Schema().loads(self.spec)
 
     @property
     def name(self) -> str:
         return self.policy_name
 
     @property
```

### Comparing `pybanyan-0.28.1/banyan/model/role.py` & `pybanyan-0.29.0/banyan/model/role.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,14 @@
         unknown = EXCLUDE
         ordered = True
 
     KIND = "BanyanRole"
     metadata: Metadata
     spec: Spec
 
-    def __post_init__(self):
-        self.kind = self.KIND
-
     @property
     def name(self):
         return self.metadata.name
 
 
 @dataclass
 class RoleInfo(InfoBase):
@@ -84,15 +81,15 @@
     description: str = field(metadata={'data_key': 'Description'})
 
     type: str = field(metadata={'data_key': 'RoleType'})
     version: int = field(metadata={'data_key': 'RoleVersion'})
     enabled: bool = field(metadata={'data_key': 'Enabled'})
 
     @property
-    def role(self) -> Role:
+    def role_spec(self) -> Role:
         return Role.Schema().loads(self.spec)
 
     @property
     def name(self) -> str:
         return self.role_name
 
     @property
```

### Comparing `pybanyan-0.28.1/banyan/model/service.py` & `pybanyan-0.29.0/banyan/model/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,14 @@
     class Meta:
         unknown = EXCLUDE
 
     attributes: Attributes
     backend: Backend
     cert_settings: CertSettings
     http_settings: HttpSettings
-    client_cidrs: List[ClientCIDRs] = field(default_factory=list) # deprecated
 
 
 @dataclass
 class Service(BanyanApiObject):
     class Meta:
         unknown = EXCLUDE
         ordered = True
@@ -357,15 +356,15 @@
     protocol: str = field(metadata={'data_key': 'Protocol'})
     domain: str = field(metadata={'data_key': 'Domain'})
     port: int = field(metadata={'data_key': 'Port'})
     enabled: bool = field(metadata={'data_key': 'Enabled'})
     Schema: ClassVar[Schema] = Schema
 
     @property
-    def service(self) -> Service:
+    def service_spec(self) -> Service:
         return Service.Schema().loads(self.spec)
 
     @property
     def oidc_client(self) -> OIDCClient:
         return OIDCClient.Schema().loads(self.oidc_client_spec)
 
     @property
```

### Comparing `pybanyan-0.28.1/banyan/model/service_infra.py` & `pybanyan-0.29.0/banyan/model/service_infra.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/model/service_web.py` & `pybanyan-0.29.0/banyan/model/service_web.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/model/shield.py` & `pybanyan-0.29.0/banyan/model/shield.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import field
 from datetime import datetime
 from ipaddress import IPv4Address
-from typing import List, Dict, ClassVar, Type
+from typing import List, Dict, ClassVar, Type, Optional
 from uuid import UUID
 
 import OpenSSL.crypto
 from marshmallow import fields, Schema, EXCLUDE
 from marshmallow_dataclass import dataclass
 from semver import VersionInfo
 
@@ -24,15 +24,15 @@
     group_type: str = field(metadata={"data_key": "GroupType"})
     cluster_mgr_type: str = field(metadata={"data_key": "ClusterMgrType"})
     cluster_mgr_ip: IPv4Address = field(metadata={"marshmallow_field": fields.String(data_key="ClusterMgrIP")})
     version: VersionInfo = field(metadata={"marshmallow_field": VersionField(data_key="ShieldVersion")})
     auto_upgrade: bool = field(metadata={"data_key": "AutoUpgrade"})
     one_time_key: UUID = field(metadata={"data_key": "OneTimeKey"})
     otk_expire_dt: datetime = field(metadata={"data_key": "OTKExpiryTime"})
-    scep_enabled: bool = field(metadata={"data_key": "SCEPEnabled"})
+    scep_enabled: Optional[bool] = field(metadata={"data_key": "SCEPEnabled"})
     public_addr: str = field(metadata={"data_key": "PublicAddr"})
     ca_cert_str: str = field(metadata={"data_key": "CACert"})
     otk_enabled: bool = field(metadata={"data_key": "OTKEnabled"})
     ssh_ca_public_key: str = field(metadata={"data_key": "SSHCAPublicKey"})
     Schema: ClassVar[Type[Schema]] = Schema
 
     def load_cacert(self) -> OpenSSL.crypto.X509:
```

### Comparing `pybanyan-0.28.1/banyan/model/trustscore.py` & `pybanyan-0.29.0/banyan/model/trustscore.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.28.1/banyan/model/user_device.py` & `pybanyan-0.29.0/banyan/model/user_device.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import field
 from datetime import datetime
 from typing import Dict, List, ClassVar, Type, Optional
+from uuid import UUID
 
 from marshmallow import Schema, validate, EXCLUDE
 from marshmallow_dataclass import dataclass
 from semver import VersionInfo
 
 from banyan.model import NanoTimestampField, Resource, BanyanEnum, VersionField
 from banyan.model.trustscore import TrustFactorsV2, TrustLevel
@@ -87,14 +88,47 @@
 class DeviceOwnership(BanyanEnum):
     CORPORATE_DEDICATED = 'Corporate Dedicated'
     CORPORATE_SHARED = 'Corporate Shared'
     EMPLOYEE_OWNED = 'Employee Owned'
     OTHER = 'Other'
 
 
+@dataclass 
+class DeviceV2(Resource):
+    class Meta:
+        unknown = EXCLUDE
+
+    device_id: UUID = field(metadata={"data_key": "id"})
+    device_friendly_name: str = field(metadata={"data_key": "name"})
+    serial_number: str
+    ownership: str
+    platform: str
+    model: str
+    os: str
+    architecture: str
+    app_version: str
+    banned: bool
+    mdm_present: bool
+    mdm_vendor_name: str
+    trust_level: str
+    trust_status: str
+    trust_profile_display_name: str
+    threat_profile_display_name: str 
+    created_at: datetime = field(metadata={"marshmallow_field": NanoTimestampField()})
+    last_login: datetime = field(metadata={"marshmallow_field": NanoTimestampField()})
+
+    @property
+    def name(self) -> str:
+        return self.device_friendly_name
+
+    @property
+    def id(self) -> str:
+        return self.serial_number       
+
+
 @dataclass
 class Device(Resource):
     class Meta:
         unknown = EXCLUDE
 
     serial_number: str = field(metadata={'data_key': 'SerialNumber'})
     device_id: str = field(metadata={'data_key': 'DeviceID', 'allow_none': True})
```

### Comparing `pybanyan-0.28.1/pybanyan.egg-info/PKG-INFO` & `pybanyan-0.29.0/pybanyan.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,208 +1,213 @@
 Metadata-Version: 2.1
 Name: pybanyan
-Version: 0.28.1
+Version: 0.29.0
 Summary: API library and command-line interface for Banyan Security
 Home-page: https://github.com/banyansecurity/pybanyan/
 Author: Todd Radel
 Author-email: todd@banyansecurity.io
 License: apache
-Description: # API library and command-line interface for Banyan Security
-        [![Build Status](https://travis-ci.org/banyansecurity/pybanyan.svg?branch=master)](https://travis-ci.org/banyansecurity/pybanyan)
-        [![codecov](https://codecov.io/gh/banyansecurity/pybanyan/branch/master/graph/badge.svg)](https://codecov.io/gh/banyansecurity/pybanyan)
-        [![PyPI version](https://badge.fury.io/py/pybanyan.svg)](https://badge.fury.io/py/pybanyan)
-        
-        
-        ## Prerequisites
-        Python 3.7 or 3.8 must be installed.
-        
-        ## Installation 
-        ### Installing the easy way
-        
-        ```console
-        $ pip install pybanyan
-        ```
-        
-        ### Installing the hard way
-        
-        ```console
-        $ git clone https://github.com/banyansecurity/pybanyan.git
-        $ cd pybanyan
-        $ pip install -r requirements.txt
-        $ python setup.py install
-        ```
-        
-        ## Usage
-        
-        This package contains both an API client and a CLI tool.
-        To use either one, you need to [generate] an API token from the Banyan Command Center.
-        
-        ### API library
-        
-        Here's a sample script that uses the library to print the names of every service registered in Banyan:
-        
-        ```python
-        from banyan.api import BanyanApiClient
-        
-        c = BanyanApiClient()
-        for service in c.services.list():
-            print(service.name)
-        ```
-        
-        Output:
-        ```console
-        $ python examples/list_services.py
-        jira
-        jupyter
-        kube
-        mysql
-        rds-mysql
-        rds-pgsql
-        ```
-        
-        The `BanyanApiClient` class accepts optional arguments to specify the API server and refresh token. If not provided, 
-        it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_REFRESH_TOKEN`.
-        
-        Full API documentation will be available soon.
-        
-        ### Banyan CLI tool
-        
-        Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API token:
-        
-        ```ini
-        [banyan]
-        api_url = https://net.banyanops.com
-        refresh_token = MY_API_TOKEN
-        ```
-        
-        The CLI is invoked with the `banyan` tool. It contains a number of commands and sub-commands to help you work
-        with policies, roles, services, users, and other objects in Banyan. 
-        
-        Run the `banyan` tool by itself to see the available commands.
-        
-        ```console
-        $ banyan
-        usage: banyan [options] <command> <subcommand> [<subcommand> ...] [parameters]
-        
-        API library and command-line interface for Banyan Security
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -d, --debug           full application debug mode
-          -q, --quiet           suppress all console output
-          -v, --version         show program's version number and exit
-          --api-url API_URL     URL for the Banyan API server. Can also be configured
-                                via the BANYAN_API_URL environment variable.
-          --refresh-token REFRESH_TOKEN
-                                API token used for the initial authentication to the
-                                Banyan API server. Can also be configured via the
-                                BANYAN_REFRESH_TOKEN environment variable.
-          --output-format {table,json,yaml}, -o {table,json,yaml}
-                                desired output format (table, json, yaml)
-        
-        Commands:
-          {event,admin,device,user,netagent,shield,policy,role,service}
-            event               report on security and audit events
-            admin               manage administrator accounts
-            device              manage devices
-            user                manage user accounts
-            netagent            manage netagents (AccessTiers and HostAgents)
-            shield              manage Banyan Shield clusters
-            policy              manage authorization policies for users and workloads
-            role                manage user and workload roles
-            service             manage web and TCP services and workloads
-            cloud-resource      manage cloud resources discovered from IaaS
-        ```
-        
-        Each of the commands has multiple subcommands. For example, `banyan service` allows you to list services, create/delete, enable/disable, etc. Run the command without any subcommand to see the options:
-        
-        ```console
-        $ banyan service
-        usage: banyan service [-h]
-                              {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
-                              ...
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-        
-        sub-commands:
-          {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
-            attach-policy       attach a policy to a service
-            create              create a new service from a JSON specification
-            delete              delete a service
-            detach-policy       detach the active policy from a service
-            disable             disable a service
-            enable              enable a service
-            get                 show the definition of a registered service
-            list                list registered services
-            test                run sanity checks on a service
-            update              update an existing service from a JSON specification
-        ```
-        
-        To see the full help available for any command, just add the `-h` or `--help` option to the end of the command. 
-        For example:
-        
-        ```console
-        $ banyan service attach-policy --help
-        usage: banyan service attach-policy [-h] [--permissive] [--enforcing]
-                                            service_name_or_id policy_name_or_id
-        
-        positional arguments:
-          service_name_or_id  Name or ID of the service to attach a policy to.
-          policy_name_or_id   Name or ID of the policy to attach to the service.
-        
-        optional arguments:
-          -h, --help          show this help message and exit
-          --permissive        Set the policy to permissive mode (allow all traffic and
-                              log any unauthorized access).
-          --enforcing         Set the policy to enforcing mode (deny unauthorized
-                              access).
-        ```
-        
-        ## Integrations
-        
-        You can automate different types of workflows by integrating with external APIs. We provide pre-built integrations for 2 types of workflows:
-        
-        ### 1. Synchronize cloud resources from your IaaS provider
-        
-        You can discover and synchronize your IaaS (Infrastructure As A Service) resources into Banyan's inventory, so you can later publish some or all of them as Banyan services. Read our [overview on how Banyan synchronizes IaaS resources](docs/iaas/README.md), and then check out instructions to set up for your specific IaaS provider:
-        
-        - [AWS](docs/iaas/aws.md)
-        - [Azure Cloud](docs/iaas/azure_cloud.md)
-        - [GCP](docs/iaas/gcp.md)
-        - [Oracle Cloud](docs/iaas/oracle_cloud.md)
-        
-        ### 2. Bookmark Banyan services into your SSO catalog
-        
-        You can publish Banyan services as bookmark applications in your SSO (Single Sign On) portal, so your end-user can access them via their SSO catalog. Check out the provider-specific link for setup instructions.
-        
-        - [Okta](docs/idp/okta.md)
-        - [AzureAD](docs/idp/azure_ad.md)
-        
-        
-        ## Development
-        
-        To work on the pybanyan code, follow the instructions in the [documentation][devel]. 
-        
-        ## Support
-        
-        This API library and its accompanying CLI utility are provided free of charge and without support. To report 
-        issues with the library, please create a new [issue in Github][github-issue].
-        
-        ## Contributions
-        
-        We welcome your contributions in the form of pull requests! Please follow the standard [Github pull request 
-        workflow][github-pr].
-        
-        [generate]: https://docs.banyansecurity.io/docs/api-guide/introduction/
-        [github-pr]: https://gist.github.com/Chaser324/ce0505fbed06b947d962
-        [github-issue]: https://github.com/banyansecurity/pybanyan/issues/new
-        [devel]: https://pybanyan.readthedocs.io/development.html
-Platform: UNKNOWN
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: aws
 Provides-Extra: azure_cloud
 Provides-Extra: gcp
 Provides-Extra: oracle_cloud
 Provides-Extra: okta
 Provides-Extra: azure_ad
+License-File: LICENSE.md
+
+# API library and command-line interface for Banyan Security
+[![Build Status](https://travis-ci.org/banyansecurity/pybanyan.svg?branch=master)](https://travis-ci.org/banyansecurity/pybanyan)
+[![codecov](https://codecov.io/gh/banyansecurity/pybanyan/branch/master/graph/badge.svg)](https://codecov.io/gh/banyansecurity/pybanyan)
+[![PyPI version](https://badge.fury.io/py/pybanyan.svg)](https://badge.fury.io/py/pybanyan)
+
+
+## Prerequisites
+Python 3.7+ must be installed.
+
+## Installation 
+### Installing the easy way
+
+```console
+$ pip install pybanyan
+```
+
+### Installing the hard way
+
+```console
+$ git clone https://github.com/banyansecurity/pybanyan.git
+$ cd pybanyan
+$ pip install -r requirements.txt
+$ python setup.py install --user
+```
+
+## Usage
+
+This package contains both an API client and a CLI tool.
+To use either one, you need to [generate] an API token from the Banyan Command Center.
+
+### API library
+
+Here's a sample script that uses the library to print the names of every service registered in Banyan:
+
+```python
+from banyan.api import BanyanApiClient
+
+c = BanyanApiClient()
+for service in c.services.list():
+    print(service.name)
+```
+
+Output:
+```console
+$ python examples/list_services.py
+jira
+jupyter
+kube
+mysql
+rds-mysql
+rds-pgsql
+```
+
+The `BanyanApiClient` class accepts optional arguments to specify the API server and refresh token. If not provided, 
+it gets them from environment variables named `BANYAN_API_URL` and `BANYAN_API_KEY`.
+
+Full API documentation will be available soon.
+
+### Banyan CLI tool
+
+Before you use the CLI, create a file called `~/.banyan.conf` in your home directory and paste in your API credential (you may use an `api_key` or `refresh_token`):
+
+```ini
+[banyan]
+api_url = https://net.banyanops.com
+api_key = MY_API_KEY
+```
+
+The CLI is invoked with the `banyan` tool. It contains a number of commands and sub-commands to help you work with policies, roles, services, users, and other objects in Banyan. 
+
+Run the `banyan` tool by itself to see the available commands.
+
+```console
+$ banyan
+usage: banyan [options] <command> <subcommand> [<subcommand> ...] [parameters]
+
+API library and command-line interface for Banyan Security
+
+options:
+  -h, --help            show this help message and exit
+  -d, --debug           full application debug mode
+  -q, --quiet           suppress all console output
+  --version, -v         show program's version number and exit
+  --api-url API_URL     URL for the Banyan API server. Can also be configured via the BANYAN_API_URL environment variable.
+  --api-key API_KEY     API credential used for the authentication to the Banyan API server. Can also be configured via the BANYAN_API_KEY or BANYAN_REFRESH_TOKEN environment
+                        variable.
+  --insecure-tls, -k    Allow connections to API servers with invalid TLS certificates.
+  --output-format {table,json,yaml}, -o {table,json,yaml}
+                        desired output format (table, json, yaml)
+
+Commands:
+  {netagent,service,shield,access-tier,api-key,audit,cloud-resource,connector,device,event,export,policy,role,service-infra,service-tunnel,service-web,user}
+    netagent            (deprecated: use access-tier) manage netagents
+    service             (deprecated: use service-web or service-infra) manage web and TCP services and workloads
+    shield              (deprecated) manage shield clusters
+    access-tier         manage access tiers
+    api-key             manage API keys
+    audit               retrieve audit logs
+    cloud-resource      manage cloud resources discovered from IaaS
+    connector           manage connectors
+    device              manage devices
+    event               report on security events
+    export              export all objects from an organization
+    policy              manage authorization policies for users and workloads
+    role                manage user and workload roles
+    service-infra       manage infrastructure services
+    service-tunnel      manage service tunnels
+    service-web         manage hosted website services
+    user                manage users
+```
+
+Each of the commands has multiple subcommands. For example, `banyan service` allows you to list services, create/delete, enable/disable, etc. Run the command without any subcommand to see the options:
+
+```console
+$ banyan service
+usage: banyan service [-h]
+                      {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
+                      ...
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+sub-commands:
+  {attach-policy,create,delete,detach-policy,disable,enable,get,list,test,update}
+    attach-policy       attach a policy to a service
+    create              create a new service from a JSON specification
+    delete              delete a service
+    detach-policy       detach the active policy from a service
+    disable             disable a service
+    enable              enable a service
+    get                 show the definition of a registered service
+    list                list registered services
+    test                run sanity checks on a service
+    update              update an existing service from a JSON specification
+```
+
+To see the full help available for any command, just add the `-h` or `--help` option to the end of the command. 
+For example:
+
+```console
+$ banyan service attach-policy --help
+usage: banyan service attach-policy [-h] [--permissive] [--enforcing]
+                                    service_name_or_id policy_name_or_id
+
+positional arguments:
+  service_name_or_id  Name or ID of the service to attach a policy to.
+  policy_name_or_id   Name or ID of the policy to attach to the service.
+
+optional arguments:
+  -h, --help          show this help message and exit
+  --permissive        Set the policy to permissive mode (allow all traffic and
+                      log any unauthorized access).
+  --enforcing         Set the policy to enforcing mode (deny unauthorized
+                      access).
+```
+
+## Integrations
+
+You can automate different types of workflows by integrating with external APIs. We provide pre-built integrations for 2 types of workflows:
+
+### 1. Synchronize cloud resources from your IaaS provider
+
+You can discover and synchronize your IaaS (Infrastructure As A Service) resources into Banyan's inventory, so you can later publish some or all of them as Banyan services. Read our [overview on how Banyan synchronizes IaaS resources](docs/iaas/README.md), and then check out instructions to set up for your specific IaaS provider:
+
+- [AWS](docs/iaas/aws.md)
+- [Azure Cloud](docs/iaas/azure_cloud.md)
+- [GCP](docs/iaas/gcp.md)
+- [Oracle Cloud](docs/iaas/oracle_cloud.md)
+
+### 2. Bookmark Banyan services into your SSO catalog
+
+You can publish Banyan services as bookmark applications in your SSO (Single Sign On) portal, so your end-user can access them via their SSO catalog. Check out the provider-specific link for setup instructions.
+
+- [Okta](docs/idp/okta.md)
+- [AzureAD](docs/idp/azure_ad.md)
+
+
+## Development
+
+To work on the pybanyan code, follow the instructions in the [documentation][devel]. 
+
+## Support
+
+This API library and its accompanying CLI utility are provided free of charge and without support. To report 
+issues with the library, please create a new [issue in Github][github-issue].
+
+## Contributions
+
+We welcome your contributions in the form of pull requests! Please follow the standard [Github pull request 
+workflow][github-pr].
+
+[generate]: https://docs.banyansecurity.io/docs/api-guide/introduction/
+[github-pr]: https://gist.github.com/Chaser324/ce0505fbed06b947d962
+[github-issue]: https://github.com/banyansecurity/pybanyan/issues/new
+[devel]: https://pybanyan.readthedocs.io/development.html
```

### Comparing `pybanyan-0.28.1/pybanyan.egg-info/SOURCES.txt` & `pybanyan-0.29.0/pybanyan.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,41 +5,49 @@
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 banyan/__init__.py
 banyan/main.py
 banyan/api/__init__.py
+banyan/api/access_tier.py
+banyan/api/api_key.py
 banyan/api/attachment.py
 banyan/api/audit.py
 banyan/api/base.py
 banyan/api/cloud_resource.py
+banyan/api/connector.py
 banyan/api/device.py
 banyan/api/event_v2.py
 banyan/api/netagent.py
 banyan/api/policy.py
 banyan/api/role.py
 banyan/api/service.py
 banyan/api/service_infra.py
+banyan/api/service_tunnel.py
 banyan/api/service_web.py
 banyan/api/shield.py
 banyan/api/user.py
 banyan/controllers/__init__.py
+banyan/controllers/access_tier.py
 banyan/controllers/admin.py
+banyan/controllers/api_key.py
 banyan/controllers/audit.py
 banyan/controllers/base.py
 banyan/controllers/cloud_resource.py
+banyan/controllers/connector.py
 banyan/controllers/device.py
 banyan/controllers/event.py
 banyan/controllers/export.py
 banyan/controllers/netagent.py
 banyan/controllers/policy.py
 banyan/controllers/role.py
 banyan/controllers/service.py
 banyan/controllers/service_infra.py
+banyan/controllers/service_tunnel.py
 banyan/controllers/service_web.py
 banyan/controllers/shield.py
 banyan/controllers/user.py
 banyan/core/__init__.py
 banyan/core/exc.py
 banyan/core/version.py
 banyan/ext/__init__.py
@@ -56,23 +64,27 @@
 banyan/ext/idp/okta.py
 banyan/lib/__init__.py
 banyan/lib/certs.py
 banyan/lib/service.py
 banyan/lib/cloud/__init__.py
 banyan/lib/cloud/aws.py
 banyan/model/__init__.py
+banyan/model/access_tier.py
+banyan/model/api_key.py
 banyan/model/attachment.py
 banyan/model/audit.py
 banyan/model/cloud_resource.py
+banyan/model/connector.py
 banyan/model/event_v2.py
 banyan/model/netagent.py
 banyan/model/policy.py
 banyan/model/role.py
 banyan/model/service.py
 banyan/model/service_infra.py
+banyan/model/service_tunnel.py
 banyan/model/service_web.py
 banyan/model/shield.py
 banyan/model/trustscore.py
 banyan/model/user_device.py
 banyan/plugins/__init__.py
 banyan/templates/__init__.py
 pybanyan.egg-info/PKG-INFO
```

### Comparing `pybanyan-0.28.1/setup.py` & `pybanyan-0.29.0/setup.py`

 * *Files identical despite different names*

