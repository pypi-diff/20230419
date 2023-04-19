# Comparing `tmp/pybanyan-0.29.0.tar.gz` & `tmp/pybanyan-0.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybanyan-0.29.0.tar", last modified: Wed Apr 19 18:54:57 2023, max compression
+gzip compressed data, was "pybanyan-0.29.1.tar", last modified: Wed Apr 19 20:45:41 2023, max compression
```

## Comparing `pybanyan-0.29.0.tar` & `pybanyan-0.29.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.219082 pybanyan-0.29.0/
--rw-r--r--   0 tarun      (501) staff       (20)     3256 2023-04-19 18:32:19.000000 pybanyan-0.29.0/CHANGELOG.md
--rw-r--r--   0 tarun      (501) staff       (20)    10496 2021-06-10 22:03:22.000000 pybanyan-0.29.0/LICENSE.md
--rw-r--r--   0 tarun      (501) staff       (20)      141 2021-06-10 22:03:22.000000 pybanyan-0.29.0/MANIFEST.in
--rw-r--r--   0 tarun      (501) staff       (20)     8237 2023-04-19 18:54:57.219155 pybanyan-0.29.0/PKG-INFO
--rw-r--r--   0 tarun      (501) staff       (20)     7756 2023-04-19 18:32:42.000000 pybanyan-0.29.0/README.md
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.201730 pybanyan-0.29.0/banyan/
--rw-r--r--   0 tarun      (501) staff       (20)      136 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.206128 pybanyan-0.29.0/banyan/api/
--rw-r--r--   0 tarun      (501) staff       (20)    17853 2023-04-17 18:19:15.000000 pybanyan-0.29.0/banyan/api/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)      397 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/access_tier.py
--rw-r--r--   0 tarun      (501) staff       (20)      453 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/api_key.py
--rw-r--r--   0 tarun      (501) staff       (20)      342 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/api/attachment.py
--rw-r--r--   0 tarun      (501) staff       (20)     1746 2022-04-07 19:03:43.000000 pybanyan-0.29.0/banyan/api/audit.py
--rw-r--r--   0 tarun      (501) staff       (20)     6173 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/base.py
--rw-r--r--   0 tarun      (501) staff       (20)     3749 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/cloud_resource.py
--rw-r--r--   0 tarun      (501) staff       (20)      382 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/connector.py
--rw-r--r--   0 tarun      (501) staff       (20)     6392 2023-04-19 18:32:42.000000 pybanyan-0.29.0/banyan/api/device.py
--rw-r--r--   0 tarun      (501) staff       (20)     6069 2023-04-17 18:19:15.000000 pybanyan-0.29.0/banyan/api/event_v2.py
--rw-r--r--   0 tarun      (501) staff       (20)      851 2022-11-29 19:34:37.000000 pybanyan-0.29.0/banyan/api/netagent.py
--rw-r--r--   0 tarun      (501) staff       (20)     2215 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/policy.py
--rw-r--r--   0 tarun      (501) staff       (20)     1469 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/role.py
--rw-r--r--   0 tarun      (501) staff       (20)     2113 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/service.py
--rw-r--r--   0 tarun      (501) staff       (20)     2594 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/service_infra.py
--rw-r--r--   0 tarun      (501) staff       (20)      427 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/api/service_tunnel.py
--rw-r--r--   0 tarun      (501) staff       (20)     2596 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/service_web.py
--rw-r--r--   0 tarun      (501) staff       (20)     1482 2022-11-29 19:34:37.000000 pybanyan-0.29.0/banyan/api/shield.py
--rw-r--r--   0 tarun      (501) staff       (20)     1520 2022-04-04 18:28:15.000000 pybanyan-0.29.0/banyan/api/user.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.210186 pybanyan-0.29.0/banyan/controllers/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/controllers/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     2442 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/access_tier.py
--rw-r--r--   0 tarun      (501) staff       (20)     1054 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/controllers/admin.py
--rw-r--r--   0 tarun      (501) staff       (20)     2504 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/api_key.py
--rw-r--r--   0 tarun      (501) staff       (20)     1885 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/controllers/audit.py
--rw-r--r--   0 tarun      (501) staff       (20)     6045 2023-04-17 18:19:15.000000 pybanyan-0.29.0/banyan/controllers/base.py
--rw-r--r--   0 tarun      (501) staff       (20)    21999 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/cloud_resource.py
--rw-r--r--   0 tarun      (501) staff       (20)     2574 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/connector.py
--rw-r--r--   0 tarun      (501) staff       (20)     6024 2023-04-19 18:32:42.000000 pybanyan-0.29.0/banyan/controllers/device.py
--rw-r--r--   0 tarun      (501) staff       (20)     3733 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/controllers/event.py
--rw-r--r--   0 tarun      (501) staff       (20)     3216 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/export.py
--rw-r--r--   0 tarun      (501) staff       (20)     2329 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/netagent.py
--rw-r--r--   0 tarun      (501) staff       (20)     6191 2022-11-29 19:34:37.000000 pybanyan-0.29.0/banyan/controllers/policy.py
--rw-r--r--   0 tarun      (501) staff       (20)     3850 2022-11-29 19:34:37.000000 pybanyan-0.29.0/banyan/controllers/role.py
--rw-r--r--   0 tarun      (501) staff       (20)    10519 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/service.py
--rw-r--r--   0 tarun      (501) staff       (20)     8854 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/service_infra.py
--rw-r--r--   0 tarun      (501) staff       (20)     2136 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/service_tunnel.py
--rw-r--r--   0 tarun      (501) staff       (20)     9748 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/service_web.py
--rw-r--r--   0 tarun      (501) staff       (20)     3966 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/shield.py
--rw-r--r--   0 tarun      (501) staff       (20)     4281 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/controllers/user.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.210595 pybanyan-0.29.0/banyan/core/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/core/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)       66 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/core/exc.py
--rw-r--r--   0 tarun      (501) staff       (20)      177 2023-04-19 17:28:04.000000 pybanyan-0.29.0/banyan/core/version.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.210740 pybanyan-0.29.0/banyan/ext/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/ext/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.212497 pybanyan-0.29.0/banyan/ext/iaas/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)    10036 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/aws.py
--rw-r--r--   0 tarun      (501) staff       (20)     7166 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/azure_cloud.py
--rw-r--r--   0 tarun      (501) staff       (20)     2028 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/base.py
--rw-r--r--   0 tarun      (501) staff       (20)     4275 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/gcp.py
--rw-r--r--   0 tarun      (501) staff       (20)     4313 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/oracle_cloud.py
--rw-r--r--   0 tarun      (501) staff       (20)     4698 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/iaas/vmware.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.213328 pybanyan-0.29.0/banyan/ext/idp/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/idp/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     6070 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/idp/azure_ad.py
--rw-r--r--   0 tarun      (501) staff       (20)      910 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/idp/base.py
--rw-r--r--   0 tarun      (501) staff       (20)     3856 2022-03-30 03:52:15.000000 pybanyan-0.29.0/banyan/ext/idp/okta.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.213807 pybanyan-0.29.0/banyan/lib/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     1627 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/certs.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.214192 pybanyan-0.29.0/banyan/lib/cloud/
--rw-r--r--   0 tarun      (501) staff       (20)      587 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/cloud/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     2312 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/cloud/aws.py
--rw-r--r--   0 tarun      (501) staff       (20)    13055 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/lib/service.py
--rw-r--r--   0 tarun      (501) staff       (20)     4281 2023-04-17 18:19:15.000000 pybanyan-0.29.0/banyan/main.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.217756 pybanyan-0.29.0/banyan/model/
--rw-r--r--   0 tarun      (501) staff       (20)     5990 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/__init__.py
--rw-r--r--   0 tarun      (501) staff       (20)     2409 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/access_tier.py
--rw-r--r--   0 tarun      (501) staff       (20)     1137 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/api_key.py
--rw-r--r--   0 tarun      (501) staff       (20)     1441 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/model/attachment.py
--rw-r--r--   0 tarun      (501) staff       (20)     3887 2022-04-07 19:03:43.000000 pybanyan-0.29.0/banyan/model/audit.py
--rw-r--r--   0 tarun      (501) staff       (20)     2215 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/cloud_resource.py
--rw-r--r--   0 tarun      (501) staff       (20)     2095 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/connector.py
--rw-r--r--   0 tarun      (501) staff       (20)     7350 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/model/event_v2.py
--rw-r--r--   0 tarun      (501) staff       (20)     3776 2021-08-16 21:32:36.000000 pybanyan-0.29.0/banyan/model/netagent.py
--rw-r--r--   0 tarun      (501) staff       (20)     4541 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/policy.py
--rw-r--r--   0 tarun      (501) staff       (20)     2351 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/role.py
--rw-r--r--   0 tarun      (501) staff       (20)    10470 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/service.py
--rw-r--r--   0 tarun      (501) staff       (20)    12428 2022-04-07 17:13:47.000000 pybanyan-0.29.0/banyan/model/service_infra.py
--rw-r--r--   0 tarun      (501) staff       (20)     1953 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/service_tunnel.py
--rw-r--r--   0 tarun      (501) staff       (20)     6260 2022-04-04 23:57:25.000000 pybanyan-0.29.0/banyan/model/service_web.py
--rw-r--r--   0 tarun      (501) staff       (20)     2856 2022-12-01 04:15:52.000000 pybanyan-0.29.0/banyan/model/shield.py
--rw-r--r--   0 tarun      (501) staff       (20)     3262 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/model/trustscore.py
--rw-r--r--   0 tarun      (501) staff       (20)     7580 2023-04-19 18:32:42.000000 pybanyan-0.29.0/banyan/model/user_device.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.218027 pybanyan-0.29.0/banyan/plugins/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/plugins/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.218134 pybanyan-0.29.0/banyan/templates/
--rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.0/banyan/templates/__init__.py
-drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 18:54:57.218954 pybanyan-0.29.0/pybanyan.egg-info/
--rw-r--r--   0 tarun      (501) staff       (20)     8237 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/PKG-INFO
--rw-r--r--   0 tarun      (501) staff       (20)     2401 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/SOURCES.txt
--rw-r--r--   0 tarun      (501) staff       (20)        1 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/dependency_links.txt
--rw-r--r--   0 tarun      (501) staff       (20)       44 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/entry_points.txt
--rw-r--r--   0 tarun      (501) staff       (20)      389 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/requires.txt
--rw-r--r--   0 tarun      (501) staff       (20)        7 2023-04-19 18:54:57.000000 pybanyan-0.29.0/pybanyan.egg-info/top_level.txt
--rw-r--r--   0 tarun      (501) staff       (20)      130 2021-06-10 22:03:22.000000 pybanyan-0.29.0/requirements-dev.txt
--rw-r--r--   0 tarun      (501) staff       (20)      371 2022-03-30 03:52:15.000000 pybanyan-0.29.0/requirements.txt
--rw-r--r--   0 tarun      (501) staff       (20)       38 2023-04-19 18:54:57.219574 pybanyan-0.29.0/setup.cfg
--rw-r--r--   0 tarun      (501) staff       (20)     1517 2022-03-30 03:52:15.000000 pybanyan-0.29.0/setup.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.559155 pybanyan-0.29.1/
+-rw-r--r--   0 tarun      (501) staff       (20)     3304 2023-04-19 20:44:30.000000 pybanyan-0.29.1/CHANGELOG.md
+-rw-r--r--   0 tarun      (501) staff       (20)    10496 2021-06-10 22:03:22.000000 pybanyan-0.29.1/LICENSE.md
+-rw-r--r--   0 tarun      (501) staff       (20)      141 2021-06-10 22:03:22.000000 pybanyan-0.29.1/MANIFEST.in
+-rw-r--r--   0 tarun      (501) staff       (20)     8237 2023-04-19 20:45:41.559230 pybanyan-0.29.1/PKG-INFO
+-rw-r--r--   0 tarun      (501) staff       (20)     7756 2023-04-19 18:32:42.000000 pybanyan-0.29.1/README.md
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.543570 pybanyan-0.29.1/banyan/
+-rw-r--r--   0 tarun      (501) staff       (20)      136 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.547887 pybanyan-0.29.1/banyan/api/
+-rw-r--r--   0 tarun      (501) staff       (20)    17853 2023-04-17 18:19:15.000000 pybanyan-0.29.1/banyan/api/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)      397 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/access_tier.py
+-rw-r--r--   0 tarun      (501) staff       (20)      453 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/api_key.py
+-rw-r--r--   0 tarun      (501) staff       (20)      342 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/api/attachment.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1746 2022-04-07 19:03:43.000000 pybanyan-0.29.1/banyan/api/audit.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6173 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3749 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/cloud_resource.py
+-rw-r--r--   0 tarun      (501) staff       (20)      382 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/connector.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6392 2023-04-19 18:32:42.000000 pybanyan-0.29.1/banyan/api/device.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6069 2023-04-17 18:19:15.000000 pybanyan-0.29.1/banyan/api/event_v2.py
+-rw-r--r--   0 tarun      (501) staff       (20)      851 2022-11-29 19:34:37.000000 pybanyan-0.29.1/banyan/api/netagent.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2215 2023-04-19 20:35:30.000000 pybanyan-0.29.1/banyan/api/policy.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1469 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/role.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2113 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2594 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/service_infra.py
+-rw-r--r--   0 tarun      (501) staff       (20)      427 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/api/service_tunnel.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2596 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/service_web.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1467 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/api/shield.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1520 2022-04-04 18:28:15.000000 pybanyan-0.29.1/banyan/api/user.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.551462 pybanyan-0.29.1/banyan/controllers/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/controllers/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2442 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/access_tier.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1054 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/controllers/admin.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2504 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/api_key.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1885 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/controllers/audit.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6045 2023-04-17 18:19:15.000000 pybanyan-0.29.1/banyan/controllers/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)    21999 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/cloud_resource.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2574 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/connector.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6024 2023-04-19 18:32:42.000000 pybanyan-0.29.1/banyan/controllers/device.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3733 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/controllers/event.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3216 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/export.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2329 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/netagent.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6198 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/controllers/policy.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3850 2022-11-29 19:34:37.000000 pybanyan-0.29.1/banyan/controllers/role.py
+-rw-r--r--   0 tarun      (501) staff       (20)    10519 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)     8869 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/controllers/service_infra.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2136 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/service_tunnel.py
+-rw-r--r--   0 tarun      (501) staff       (20)     9763 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/controllers/service_web.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3966 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/shield.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4281 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/controllers/user.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.551845 pybanyan-0.29.1/banyan/core/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/core/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)       66 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/core/exc.py
+-rw-r--r--   0 tarun      (501) staff       (20)      177 2023-04-19 20:43:56.000000 pybanyan-0.29.1/banyan/core/version.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.551974 pybanyan-0.29.1/banyan/ext/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/ext/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.553135 pybanyan-0.29.1/banyan/ext/iaas/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)    10036 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/aws.py
+-rw-r--r--   0 tarun      (501) staff       (20)     7166 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/azure_cloud.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2028 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4275 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/gcp.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4313 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/oracle_cloud.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4698 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/iaas/vmware.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.553719 pybanyan-0.29.1/banyan/ext/idp/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/idp/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6070 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/idp/azure_ad.py
+-rw-r--r--   0 tarun      (501) staff       (20)      910 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/idp/base.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3856 2022-03-30 03:52:15.000000 pybanyan-0.29.1/banyan/ext/idp/okta.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.554147 pybanyan-0.29.1/banyan/lib/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1627 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/certs.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.554483 pybanyan-0.29.1/banyan/lib/cloud/
+-rw-r--r--   0 tarun      (501) staff       (20)      587 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/cloud/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2312 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/cloud/aws.py
+-rw-r--r--   0 tarun      (501) staff       (20)    13055 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/lib/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4281 2023-04-17 18:19:15.000000 pybanyan-0.29.1/banyan/main.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.557860 pybanyan-0.29.1/banyan/model/
+-rw-r--r--   0 tarun      (501) staff       (20)     5990 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/__init__.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2409 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/access_tier.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1137 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/api_key.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1471 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/model/attachment.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3887 2022-04-07 19:03:43.000000 pybanyan-0.29.1/banyan/model/audit.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2215 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/cloud_resource.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2095 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/connector.py
+-rw-r--r--   0 tarun      (501) staff       (20)     7350 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/model/event_v2.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3776 2021-08-16 21:32:36.000000 pybanyan-0.29.1/banyan/model/netagent.py
+-rw-r--r--   0 tarun      (501) staff       (20)     4591 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/model/policy.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2351 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/role.py
+-rw-r--r--   0 tarun      (501) staff       (20)    10470 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/service.py
+-rw-r--r--   0 tarun      (501) staff       (20)    12428 2022-04-07 17:13:47.000000 pybanyan-0.29.1/banyan/model/service_infra.py
+-rw-r--r--   0 tarun      (501) staff       (20)     1953 2022-12-01 04:15:52.000000 pybanyan-0.29.1/banyan/model/service_tunnel.py
+-rw-r--r--   0 tarun      (501) staff       (20)     6260 2022-04-04 23:57:25.000000 pybanyan-0.29.1/banyan/model/service_web.py
+-rw-r--r--   0 tarun      (501) staff       (20)     2914 2023-04-19 20:43:31.000000 pybanyan-0.29.1/banyan/model/shield.py
+-rw-r--r--   0 tarun      (501) staff       (20)     3262 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/model/trustscore.py
+-rw-r--r--   0 tarun      (501) staff       (20)     7580 2023-04-19 18:32:42.000000 pybanyan-0.29.1/banyan/model/user_device.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.558081 pybanyan-0.29.1/banyan/plugins/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/plugins/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.558187 pybanyan-0.29.1/banyan/templates/
+-rw-r--r--   0 tarun      (501) staff       (20)        0 2021-06-10 22:03:22.000000 pybanyan-0.29.1/banyan/templates/__init__.py
+drwxr-xr-x   0 tarun      (501) staff       (20)        0 2023-04-19 20:45:41.559031 pybanyan-0.29.1/pybanyan.egg-info/
+-rw-r--r--   0 tarun      (501) staff       (20)     8237 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/PKG-INFO
+-rw-r--r--   0 tarun      (501) staff       (20)     2401 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/SOURCES.txt
+-rw-r--r--   0 tarun      (501) staff       (20)        1 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/dependency_links.txt
+-rw-r--r--   0 tarun      (501) staff       (20)       44 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/entry_points.txt
+-rw-r--r--   0 tarun      (501) staff       (20)      389 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/requires.txt
+-rw-r--r--   0 tarun      (501) staff       (20)        7 2023-04-19 20:45:41.000000 pybanyan-0.29.1/pybanyan.egg-info/top_level.txt
+-rw-r--r--   0 tarun      (501) staff       (20)      130 2021-06-10 22:03:22.000000 pybanyan-0.29.1/requirements-dev.txt
+-rw-r--r--   0 tarun      (501) staff       (20)      371 2022-03-30 03:52:15.000000 pybanyan-0.29.1/requirements.txt
+-rw-r--r--   0 tarun      (501) staff       (20)       38 2023-04-19 20:45:41.559451 pybanyan-0.29.1/setup.cfg
+-rw-r--r--   0 tarun      (501) staff       (20)     1517 2022-03-30 03:52:15.000000 pybanyan-0.29.1/setup.py
```

### Comparing `pybanyan-0.29.0/CHANGELOG.md` & `pybanyan-0.29.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # PyBanyan Change History
 
+## 0.29.1
+
+ * bugfixes to close Github tickets
+
 ## 0.29.0
 
  * make api_key the primary credential (refresh_token still works)
  * use v2 Devices API 
 
 ## 0.28.1
```

### Comparing `pybanyan-0.29.0/LICENSE.md` & `pybanyan-0.29.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/PKG-INFO` & `pybanyan-0.29.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybanyan
-Version: 0.29.0
+Version: 0.29.1
 Summary: API library and command-line interface for Banyan Security
 Home-page: https://github.com/banyansecurity/pybanyan/
 Author: Todd Radel
 Author-email: todd@banyansecurity.io
 License: apache
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pybanyan-0.29.0/README.md` & `pybanyan-0.29.1/README.md`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/__init__.py` & `pybanyan-0.29.1/banyan/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/audit.py` & `pybanyan-0.29.1/banyan/api/audit.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/base.py` & `pybanyan-0.29.1/banyan/api/base.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/cloud_resource.py` & `pybanyan-0.29.1/banyan/api/cloud_resource.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/device.py` & `pybanyan-0.29.1/banyan/api/device.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/event_v2.py` & `pybanyan-0.29.1/banyan/api/event_v2.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/netagent.py` & `pybanyan-0.29.1/banyan/api/netagent.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/policy.py` & `pybanyan-0.29.1/banyan/api/policy.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/role.py` & `pybanyan-0.29.1/banyan/api/role.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/service.py` & `pybanyan-0.29.1/banyan/api/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/service_infra.py` & `pybanyan-0.29.1/banyan/api/service_infra.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/service_web.py` & `pybanyan-0.29.1/banyan/api/service_web.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/api/shield.py` & `pybanyan-0.29.1/banyan/api/shield.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         shields = self.list()
         # what defines a shield as "enabled"?
         return [x for x in shields if self.status(str(x.shield_id)) == 'REPORTING']
 
     def status(self, shield_name_or_id: str) -> str:
         shield: Shield = self.find(shield_name_or_id)
         activity = self.config.last_activity_map[shield.id]
-        now = datetime.now(tz=timezone.utc)
+        now = datetime.now()
         age = now - activity.last_activity_time
         return 'INACTIVE' if age.total_seconds() >= 900 else 'REPORTING'
 
     @property
     def config(self) -> ShieldConfig:
         self._ensure_cache()
         return self._config
```

### Comparing `pybanyan-0.29.0/banyan/api/user.py` & `pybanyan-0.29.1/banyan/api/user.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/access_tier.py` & `pybanyan-0.29.1/banyan/controllers/access_tier.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/admin.py` & `pybanyan-0.29.1/banyan/controllers/admin.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/api_key.py` & `pybanyan-0.29.1/banyan/controllers/api_key.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/audit.py` & `pybanyan-0.29.1/banyan/controllers/audit.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/base.py` & `pybanyan-0.29.1/banyan/controllers/base.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/cloud_resource.py` & `pybanyan-0.29.1/banyan/controllers/cloud_resource.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/connector.py` & `pybanyan-0.29.1/banyan/controllers/connector.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/device.py` & `pybanyan-0.29.1/banyan/controllers/device.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/event.py` & `pybanyan-0.29.1/banyan/controllers/event.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/export.py` & `pybanyan-0.29.1/banyan/controllers/export.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/netagent.py` & `pybanyan-0.29.1/banyan/controllers/netagent.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/policy.py` & `pybanyan-0.29.1/banyan/controllers/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     def list_attachments(self):
         policy: PolicyInfo = self._client[self.app.pargs.policy_name]
         attach_api: AttachmentAPI = self.app.client.attachments
         attachments = attach_api.list()
         results = list()
         headers = ['Object Name', 'Object ID', 'Type', 'Attached At', 'Attached By']
         for a in attachments:
-            if a.policy_id == policy.id:
+            if a.policy_id == policy.policy_id:
                 new_row = [a.attached_to_name, a.attached_to_id, a.attached_to_type,
                            a.attached_at.strftime(Base.TABLE_DATE_FORMAT), a.attached_by]
                 results.append(new_row)
         results.sort(key=lambda x: x[0])
         self.app.render(results, handler='tabulate', headers=headers, tablefmt='simple')
 
     @ex(help='attach a policy to a service',
```

### Comparing `pybanyan-0.29.0/banyan/controllers/role.py` & `pybanyan-0.29.1/banyan/controllers/role.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/service.py` & `pybanyan-0.29.1/banyan/controllers/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/service_infra.py` & `pybanyan-0.29.1/banyan/controllers/service_infra.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
              {
                  'metavar': 'service_name_or_id',
                  'help': 'Name or ID of the service to display.'
              }),
         ])
     def get(self):
         info: ServiceInfo = self._client[self.app.pargs.service_name]
-        service_json = Service.Schema().dump(info.service)
+        service_json = Service.Schema().dump(info.service_spec)
         # colorized_json = highlight(service_json, lexers.JsonLexer(), formatters.Terminal256Formatter(style="default"))
         self.app.render(service_json, handler='json', indent=2, sort_keys=True)
 
 
     @ex(help='create a new infrastructure service from a JSON specification',
         arguments=[
             (['service_spec'],
@@ -137,15 +137,15 @@
                 'default': True,
                 'help': 'Set the policy to enforcing mode (deny unauthorized access).',
             }),
         ])
     def attach_policy(self):
         result = self._client.attach(self.app.pargs.service_name, self.app.pargs.policy_name, self.app.pargs.enforcing)
         mode = 'ENFORCING' if result.enabled else 'PERMISSIVE'
-        self.app.print(f'Policy {result.policy_id} attached to service {result.service_id} in {mode} mode.')
+        self.app.print(f'Policy {result.policy_id} attached to service {self.app.pargs.service_name} in {mode} mode.')
 
     @ex(help='detach the active policy from an infrastructure service',
         arguments=[
             (['service_name'],
              {
                  'metavar': 'service_name_or_id',
                  'help': 'Name or ID of the service to attach a policy to.',
```

### Comparing `pybanyan-0.29.0/banyan/controllers/service_tunnel.py` & `pybanyan-0.29.1/banyan/controllers/service_tunnel.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/service_web.py` & `pybanyan-0.29.1/banyan/controllers/service_web.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
              {
                  'metavar': 'service_name_or_id',
                  'help': 'Name or ID of the service to display.'
              }),
         ])
     def get(self):
         info: ServiceInfo = self._client[self.app.pargs.service_name]
-        service_json = Service.Schema().dump(info.service)
+        service_json = Service.Schema().dump(info.service_spec)
         # colorized_json = highlight(service_json, lexers.JsonLexer(), formatters.Terminal256Formatter(style="default"))
         self.app.render(service_json, handler='json', indent=2, sort_keys=True)
 
     @ex(help='create a new hosted website service from a JSON specification',
         arguments=[
             (['service_spec'],
              {
@@ -137,15 +137,15 @@
                 'default': True,
                 'help': 'Set the policy to enforcing mode (deny unauthorized access).',
             }),
         ])
     def attach_policy(self):
         result = self._client.attach(self.app.pargs.service_name, self.app.pargs.policy_name, self.app.pargs.enforcing)
         mode = 'ENFORCING' if result.enabled else 'PERMISSIVE'
-        self.app.print(f'Policy {result.policy_id} attached to service {result.service_id} in {mode} mode.')
+        self.app.print(f'Policy {result.policy_id} attached to service {self.app.pargs.service_name} in {mode} mode.')
 
     @ex(help='detach the active policy from a hosted website service',
         arguments=[
             (['service_name'],
              {
                  'metavar': 'service_name_or_id',
                  'help': 'Name or ID of the service to attach a policy to.',
```

### Comparing `pybanyan-0.29.0/banyan/controllers/shield.py` & `pybanyan-0.29.1/banyan/controllers/shield.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/controllers/user.py` & `pybanyan-0.29.1/banyan/controllers/user.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/ext/iaas/aws.py` & `pybanyan-0.29.1/banyan/ext/iaas/aws.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/ext/iaas/azure_cloud.py` & `pybanyan-0.29.1/banyan/ext/iaas/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/ext/iaas/base.py` & `pybanyan-0.29.1/banyan/ext/iaas/base.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/ext/iaas/gcp.py` & `pybanyan-0.29.1/banyan/ext/iaas/gcp.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/ext/iaas/oracle_cloud.py` & `pybanyan-0.29.1/banyan/ext/iaas/oracle_cloud.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/ext/iaas/vmware.py` & `pybanyan-0.29.1/banyan/ext/iaas/vmware.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/ext/idp/azure_ad.py` & `pybanyan-0.29.1/banyan/ext/idp/azure_ad.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/ext/idp/base.py` & `pybanyan-0.29.1/banyan/ext/idp/base.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/ext/idp/okta.py` & `pybanyan-0.29.1/banyan/ext/idp/okta.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/lib/certs.py` & `pybanyan-0.29.1/banyan/lib/certs.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/lib/cloud/__init__.py` & `pybanyan-0.29.1/banyan/lib/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/lib/cloud/aws.py` & `pybanyan-0.29.1/banyan/lib/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/lib/service.py` & `pybanyan-0.29.1/banyan/lib/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/main.py` & `pybanyan-0.29.1/banyan/main.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/__init__.py` & `pybanyan-0.29.1/banyan/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/access_tier.py` & `pybanyan-0.29.1/banyan/model/access_tier.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/api_key.py` & `pybanyan-0.29.1/banyan/model/api_key.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/attachment.py` & `pybanyan-0.29.1/banyan/model/attachment.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from banyan.model import NanoTimestampField, Resource, BanyanEnum
 
 
 class AttachmentType(BanyanEnum):
     SERVICE = "service"
     SAAS_APP = "saasapp"
+    TUNNEL = "service_tunnel"
 
 
 @dataclass
 class Attachment(Resource):
     class Meta:
         unknown = EXCLUDE
```

### Comparing `pybanyan-0.29.0/banyan/model/audit.py` & `pybanyan-0.29.1/banyan/model/audit.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/cloud_resource.py` & `pybanyan-0.29.1/banyan/model/cloud_resource.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/connector.py` & `pybanyan-0.29.1/banyan/model/connector.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/event_v2.py` & `pybanyan-0.29.1/banyan/model/event_v2.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/netagent.py` & `pybanyan-0.29.1/banyan/model/netagent.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/policy.py` & `pybanyan-0.29.1/banyan/model/policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,21 +164,21 @@
 
 @dataclass
 class PolicyAttachInfo:
     class Meta:
         unknown = EXCLUDE
 
     policy_id: UUID = field(metadata={'data_key': 'PolicyID'})
-    policy_name: str = field(metadata={'data_key': 'PolicyName'})
-    attached_id: str = field(metadata={'data_key': 'AttachedToID'})
-    attached_name: str = field(metadata={'data_key': 'AttachedToName'})
-    attached_type: str = field(metadata={'data_key': 'AttachedToType'})
     enabled: bool = field(metadata={'data_key': 'Enabled'})
     attached_at: datetime = field(metadata={'marshmallow_field': NanoTimestampField(data_key='AttachedAt')})
-    attached_by: str = field(metadata={'data_key': 'AttachedBy'})
+    policy_name: Optional[str] = field(metadata={'data_key': 'PolicyName'})
+    attached_by: Optional[str] = field(metadata={'data_key': 'AttachedBy'})
+    attached_id: Optional[str] = field(metadata={'data_key': 'AttachedToID'})
+    attached_name: Optional[str] = field(metadata={'data_key': 'AttachedToName'})
+    attached_type: Optional[str] = field(metadata={'data_key': 'AttachedToType'})
     detached_at: Optional[datetime] = field(default=None,
                                             metadata={'marshmallow_field': NanoTimestampField(data_key='DetachedAt')})
     detached_by: Optional[str] = field(default=None, metadata={'data_key': 'DetachedBy'})
     Schema: ClassVar[Schema] = Schema
 
 
 PolicyInfoOrName = Union[PolicyInfo, str]
```

### Comparing `pybanyan-0.29.0/banyan/model/role.py` & `pybanyan-0.29.1/banyan/model/role.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/service.py` & `pybanyan-0.29.1/banyan/model/service.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/service_infra.py` & `pybanyan-0.29.1/banyan/model/service_infra.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/service_tunnel.py` & `pybanyan-0.29.1/banyan/model/service_tunnel.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/service_web.py` & `pybanyan-0.29.1/banyan/model/service_web.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/shield.py` & `pybanyan-0.29.1/banyan/model/shield.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from uuid import UUID
 
 import OpenSSL.crypto
 from marshmallow import fields, Schema, EXCLUDE
 from marshmallow_dataclass import dataclass
 from semver import VersionInfo
 
-from banyan.model import Resource, VersionField
+from banyan.model import NanoTimestampField, Resource, VersionField
 from banyan.model.netagent import Netagent
 
 
 @dataclass
 class Shield(Resource):
     class Meta:
         unknown = EXCLUDE
@@ -49,15 +49,15 @@
 
 
 @dataclass
 class ShieldLastActivity:
     class Meta:
         unknown = EXCLUDE
 
-    last_activity_time: datetime = field(metadata={"data_key": "InsertTime"})
+    last_activity_time: datetime = field(metadata={"marshmallow_field": NanoTimestampField(data_key='InsertTime')})
     status: str = field(metadata={"data_key": "Status"})
     uuid: UUID = field(metadata={"data_key": "UUID"})
     Schema: ClassVar[Type[Schema]] = Schema
 
 
 @dataclass
 class ShieldConfig:
```

### Comparing `pybanyan-0.29.0/banyan/model/trustscore.py` & `pybanyan-0.29.1/banyan/model/trustscore.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/banyan/model/user_device.py` & `pybanyan-0.29.1/banyan/model/user_device.py`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/pybanyan.egg-info/PKG-INFO` & `pybanyan-0.29.1/pybanyan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybanyan
-Version: 0.29.0
+Version: 0.29.1
 Summary: API library and command-line interface for Banyan Security
 Home-page: https://github.com/banyansecurity/pybanyan/
 Author: Todd Radel
 Author-email: todd@banyansecurity.io
 License: apache
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pybanyan-0.29.0/pybanyan.egg-info/SOURCES.txt` & `pybanyan-0.29.1/pybanyan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybanyan-0.29.0/setup.py` & `pybanyan-0.29.1/setup.py`

 * *Files identical despite different names*

