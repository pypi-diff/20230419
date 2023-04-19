# Comparing `tmp/weni_rp_apps-2.4.0a2.tar.gz` & `tmp/weni_rp_apps-2.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weni_rp_apps-2.4.0a2.tar", max compression
+gzip compressed data, was "weni_rp_apps-2.4.0a3.tar", max compression
```

## Comparing `weni_rp_apps-2.4.0a2.tar` & `weni_rp_apps-2.4.0a3.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0      646 2023-04-17 20:29:53.154021 weni_rp_apps-2.4.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/activities/__init__.py
--rw-r--r--   0        0        0      231 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/activities/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/activities/migrations/__init__.py
--rw-r--r--   0        0        0     1960 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/activities/signals.py
--rw-r--r--   0        0        0      366 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/activities/tasks.py
--rw-r--r--   0        0        0      325 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/analytics_api/README.md
--rw-r--r--   0        0        0       66 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/analytics_api/__init__.py
--rw-r--r--   0        0        0      264 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/analytics_api/apps.py
--rw-r--r--   0        0        0    13526 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/analytics_api/tests.py
--rw-r--r--   0        0        0      475 2023-04-17 20:29:37.277786 weni_rp_apps-2.4.0a2/weni/analytics_api/urls.py
--rw-r--r--   0        0        0     8909 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/analytics_api/views.py
--rw-r--r--   0        0        0       49 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/auth/__init__.py
--rw-r--r--   0        0        0      285 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/auth/apps.py
--rw-r--r--   0        0        0     1792 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/auth/backends.py
--rw-r--r--   0        0        0      430 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/auth/decorators.py
--rw-r--r--   0        0        0      733 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/auth/urls.py
--rw-r--r--   0        0        0     2645 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/auth/views.py
--rw-r--r--   0        0        0      309 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/channel_stats/README.md
--rw-r--r--   0        0        0       66 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/channel_stats/__init__.py
--rw-r--r--   0        0        0      264 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/channel_stats/apps.py
--rw-r--r--   0        0        0     6157 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/channel_stats/serializers.py
--rw-r--r--   0        0        0      317 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/channel_stats/urls.py
--rw-r--r--   0        0        0     3575 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/channel_stats/views.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/billing/__init__.py
--rw-r--r--   0        0        0      102 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/billing/apps.py
--rw-r--r--   0        0        0     3508 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/billing/queries.py
--rw-r--r--   0        0        0     3194 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/billing/serializers.py
--rw-r--r--   0        0        0     2072 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/billing/services.py
--rw-r--r--   0        0        0    11471 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/billing/tests.py
--rw-r--r--   0        0        0      231 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/billing/urls.py
--rw-r--r--   0        0        0       64 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/channel/__init__.py
--rw-r--r--   0        0        0      103 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/channel/apps.py
--rw-r--r--   0        0        0      352 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/channel/fields.py
--rw-r--r--   0        0        0     4110 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/channel/serializers.py
--rw-r--r--   0        0        0     4023 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/channel/services.py
--rw-r--r--   0        0        0     7747 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/channel/tests.py
--rw-r--r--   0        0        0      341 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/channel/urls.py
--rw-r--r--   0        0        0       70 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/classifier/__init__.py
--rw-r--r--   0        0        0      109 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/classifier/apps.py
--rw-r--r--   0        0        0     1262 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/classifier/serializers.py
--rw-r--r--   0        0        0     1175 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/classifier/services.py
--rw-r--r--   0        0        0     6460 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/classifier/tests.py
--rw-r--r--   0        0        0      249 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/classifier/urls.py
--rw-r--r--   0        0        0       61 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/core/__init__.py
--rw-r--r--   0        0        0      100 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/core/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/core/management/commands/__init__.py
--rw-r--r--   0        0        0     1573 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/core/management/commands/grpc.py
--rw-r--r--   0        0        0     1213 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/core/serializers.py
--rw-r--r--   0        0        0      965 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/core/services.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/core/tests.py
--rw-r--r--   0        0        0      700 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/core/urls.py
--rw-r--r--   0        0        0       58 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/flow/__init__.py
--rw-r--r--   0        0        0       97 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/flow/apps.py
--rw-r--r--   0        0        0      307 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/flow/serializers.py
--rw-r--r--   0        0        0      658 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/flow/services.py
--rw-r--r--   0        0        0     2766 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/flow/tests.py
--rw-r--r--   0        0        0      213 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/flow/urls.py
--rw-r--r--   0        0        0       56 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/org/__init__.py
--rw-r--r--   0        0        0       95 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/org/apps.py
--rw-r--r--   0        0        0     2770 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/org/serializers.py
--rw-r--r--   0        0        0     3957 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/org/services.py
--rw-r--r--   0        0        0     9824 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/org/tests.py
--rw-r--r--   0        0        0      207 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/org/urls.py
--rw-r--r--   0        0        0       68 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/statistic/__init__.py
--rw-r--r--   0        0        0      107 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/statistic/apps.py
--rw-r--r--   0        0        0      672 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/statistic/services.py
--rw-r--r--   0        0        0     3134 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/statistic/tests.py
--rw-r--r--   0        0        0      252 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/statistic/urls.py
--rw-r--r--   0        0        0       58 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/user/__init__.py
--rw-r--r--   0        0        0       97 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/user/apps.py
--rw-r--r--   0        0        0      843 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/user/serializers.py
--rw-r--r--   0        0        0     3906 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/user/services.py
--rw-r--r--   0        0        0    10078 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/user/tests.py
--rw-r--r--   0        0        0      347 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/grpc/user/urls.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/__init__.py
--rw-r--r--   0        0        0      328 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/apps.py
--rw-r--r--   0        0        0      300 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/authenticators.py
--rw-r--r--   0        0        0     1374 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/backends.py
--rw-r--r--   0        0        0     5562 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/channel/serializers.py
--rw-r--r--   0        0        0    16222 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/channel/tests.py
--rw-r--r--   0        0        0      427 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/channel/urls.py
--rw-r--r--   0        0        0     6910 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/channel/views.py
--rw-r--r--   0        0        0     1433 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/classifier/serializers.py
--rw-r--r--   0        0        0     8525 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/classifier/tests.py
--rw-r--r--   0        0        0      351 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/classifier/urls.py
--rw-r--r--   0        0        0     3169 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/classifier/views.py
--rw-r--r--   0        0        0      107 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/clients/__init__.py
--rw-r--r--   0        0        0      696 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/clients/authenticators.py
--rw-r--r--   0        0        0      486 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/clients/base.py
--rw-r--r--   0        0        0      580 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/clients/connect.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/externals/__init__.py
--rw-r--r--   0        0        0     1308 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/externals/serializers.py
--rw-r--r--   0        0        0      198 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/externals/urls.py
--rw-r--r--   0        0        0     1064 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/externals/views.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/flows/__init__.py
--rw-r--r--   0        0        0     1278 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/flows/serializers.py
--rw-r--r--   0        0        0     4283 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/flows/tests.py
--rw-r--r--   0        0        0      308 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/flows/urls.py
--rw-r--r--   0        0        0      974 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/flows/views.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/globals/__init__.py
--rw-r--r--   0        0        0     2286 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/globals/serializers.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/globals/tests/__init__.py
--rw-r--r--   0        0        0     2183 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/globals/tests/test_serializers.py
--rw-r--r--   0        0        0      220 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/globals/urls.py
--rw-r--r--   0        0        0     1485 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/globals/views.py
--rw-r--r--   0        0        0      868 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/migrations/0001_initial.py
--rw-r--r--   0        0        0     1032 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/migrations/0002_project.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/migrations/__init__.py
--rw-r--r--   0        0        0      813 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/models.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/orgs/__init__.py
--rw-r--r--   0        0        0     3369 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/orgs/serializers.py
--rw-r--r--   0        0        0    14533 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/orgs/tests.py
--rw-r--r--   0        0        0      300 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/orgs/urls.py
--rw-r--r--   0        0        0     4520 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/orgs/views.py
--rw-r--r--   0        0        0      246 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/permissions.py
--rw-r--r--   0        0        0     1993 2023-04-17 20:29:37.281786 weni_rp_apps-2.4.0a2/weni/internal/statistic/tests.py
--rw-r--r--   0        0        0      205 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/statistic/urls.py
--rw-r--r--   0        0        0      831 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/statistic/views.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/tests/__init__.py
--rw-r--r--   0        0        0     1249 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/tests/test_models.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/tickets/__init__.py
--rw-r--r--   0        0        0     1152 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/tickets/serializers.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/tickets/tests/__init__.py
--rw-r--r--   0        0        0     3398 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/tickets/tests/test_views.py
--rw-r--r--   0        0        0      443 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/tickets/urls.py
--rw-r--r--   0        0        0     1682 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/tickets/views.py
--rw-r--r--   0        0        0     1315 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/urls.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/users/__init__.py
--rw-r--r--   0        0        0      845 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/users/serializers.py
--rw-r--r--   0        0        0    11864 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/users/tests.py
--rw-r--r--   0        0        0      711 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/users/urls.py
--rw-r--r--   0        0        0     5655 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/users/views.py
--rw-r--r--   0        0        0      555 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/internal/views.py
--rw-r--r--   0        0        0       55 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/orgs_api/__init__.py
--rw-r--r--   0        0        0      253 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/orgs_api/apps.py
--rw-r--r--   0        0        0      906 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/orgs_api/serializers.py
--rw-r--r--   0        0        0     4030 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/orgs_api/tests.py
--rw-r--r--   0        0        0      178 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/orgs_api/urls.py
--rw-r--r--   0        0        0     1444 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/orgs_api/views.py
--rw-r--r--   0        0        0       45 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/s3/__init__.py
--rw-r--r--   0        0        0      243 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/s3/apps.py
--rw-r--r--   0        0        0      250 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/s3/urls.py
--rw-r--r--   0        0        0      550 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/s3/views.py
--rw-r--r--   0        0        0       79 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/serializers/__init__.py
--rw-r--r--   0        0        0      725 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/serializers/fields.py
--rw-r--r--   0        0        0      281 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/success_orgs/apps.py
--rw-r--r--   0        0        0     2403 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/success_orgs/business.py
--rw-r--r--   0        0        0      563 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/success_orgs/serializers.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/success_orgs/tests/__init__.py
--rw-r--r--   0        0        0     2980 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/success_orgs/tests/test_business.py
--rw-r--r--   0        0        0      494 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/success_orgs/urls.py
--rw-r--r--   0        0        0     2774 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/success_orgs/views.py
--rw-r--r--   0        0        0      318 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/template_message/README.md
--rw-r--r--   0        0        0       72 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/template_message/__init__.py
--rw-r--r--   0        0        0      294 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/template_message/apps.py
--rw-r--r--   0        0        0     2041 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/template_message/serializers.py
--rw-r--r--   0        0        0     5295 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/template_message/tests.py
--rw-r--r--   0        0        0      344 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/template_message/urls.py
--rw-r--r--   0        0        0     1651 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/template_message/views.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/templates/__init__.py
--rw-r--r--   0        0        0      559 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/templates/context_processors.py
--rw-r--r--   0        0        0      315 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/ticketer_queues/README.md
--rw-r--r--   0        0        0       70 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/ticketer_queues/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/ticketer_queues/apps.py
--rw-r--r--   0        0        0      242 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/ticketer_queues/serializers.py
--rw-r--r--   0        0        0     1584 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/ticketer_queues/tests.py
--rw-r--r--   0        0        0      378 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/ticketer_queues/urls.py
--rw-r--r--   0        0        0      849 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/ticketer_queues/views.py
--rw-r--r--   0        0        0        0 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/utils/__init__.py
--rw-r--r--   0        0        0     1091 2023-04-17 20:29:37.285786 weni_rp_apps-2.4.0a2/weni/utils/app_config.py
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.0a2/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-04-19 14:01:07.171892 weni_rp_apps-2.4.0a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/__init__.py
+-rw-r--r--   0        0        0      231 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/apps.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/migrations/__init__.py
+-rw-r--r--   0        0        0     1960 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/signals.py
+-rw-r--r--   0        0        0      366 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/tasks.py
+-rw-r--r--   0        0        0      325 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/README.md
+-rw-r--r--   0        0        0       66 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/__init__.py
+-rw-r--r--   0        0        0      264 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/apps.py
+-rw-r--r--   0        0        0    13526 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/tests.py
+-rw-r--r--   0        0        0      475 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/urls.py
+-rw-r--r--   0        0        0     8909 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/views.py
+-rw-r--r--   0        0        0       49 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/__init__.py
+-rw-r--r--   0        0        0      285 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/apps.py
+-rw-r--r--   0        0        0     1792 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/backends.py
+-rw-r--r--   0        0        0      430 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/decorators.py
+-rw-r--r--   0        0        0      733 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/urls.py
+-rw-r--r--   0        0        0     2645 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/views.py
+-rw-r--r--   0        0        0      309 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/README.md
+-rw-r--r--   0        0        0       66 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/__init__.py
+-rw-r--r--   0        0        0      264 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/apps.py
+-rw-r--r--   0        0        0     6157 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/serializers.py
+-rw-r--r--   0        0        0      317 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/urls.py
+-rw-r--r--   0        0        0     3575 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/__init__.py
+-rw-r--r--   0        0        0      102 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/apps.py
+-rw-r--r--   0        0        0     3508 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/queries.py
+-rw-r--r--   0        0        0     3194 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/serializers.py
+-rw-r--r--   0        0        0     2072 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/services.py
+-rw-r--r--   0        0        0    11471 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/tests.py
+-rw-r--r--   0        0        0      231 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/urls.py
+-rw-r--r--   0        0        0       64 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/apps.py
+-rw-r--r--   0        0        0      352 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/fields.py
+-rw-r--r--   0        0        0     4110 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/serializers.py
+-rw-r--r--   0        0        0     4023 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/services.py
+-rw-r--r--   0        0        0     7747 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/tests.py
+-rw-r--r--   0        0        0      341 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/urls.py
+-rw-r--r--   0        0        0       70 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/__init__.py
+-rw-r--r--   0        0        0      109 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/apps.py
+-rw-r--r--   0        0        0     1262 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/serializers.py
+-rw-r--r--   0        0        0     1175 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/services.py
+-rw-r--r--   0        0        0     6460 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/tests.py
+-rw-r--r--   0        0        0      249 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/urls.py
+-rw-r--r--   0        0        0       61 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/__init__.py
+-rw-r--r--   0        0        0      100 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/apps.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1573 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/management/commands/grpc.py
+-rw-r--r--   0        0        0     1213 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/serializers.py
+-rw-r--r--   0        0        0      965 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/services.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/tests.py
+-rw-r--r--   0        0        0      700 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/urls.py
+-rw-r--r--   0        0        0       58 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/__init__.py
+-rw-r--r--   0        0        0       97 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/apps.py
+-rw-r--r--   0        0        0      307 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/serializers.py
+-rw-r--r--   0        0        0      658 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/services.py
+-rw-r--r--   0        0        0     2766 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/tests.py
+-rw-r--r--   0        0        0      213 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/urls.py
+-rw-r--r--   0        0        0       56 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/__init__.py
+-rw-r--r--   0        0        0       95 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/apps.py
+-rw-r--r--   0        0        0     2770 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/serializers.py
+-rw-r--r--   0        0        0     3957 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/services.py
+-rw-r--r--   0        0        0     9824 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/tests.py
+-rw-r--r--   0        0        0      207 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/urls.py
+-rw-r--r--   0        0        0       68 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/apps.py
+-rw-r--r--   0        0        0      672 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/services.py
+-rw-r--r--   0        0        0     3134 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/tests.py
+-rw-r--r--   0        0        0      252 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/urls.py
+-rw-r--r--   0        0        0       58 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/__init__.py
+-rw-r--r--   0        0        0       97 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/apps.py
+-rw-r--r--   0        0        0      843 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/serializers.py
+-rw-r--r--   0        0        0     3906 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/services.py
+-rw-r--r--   0        0        0    10078 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/tests.py
+-rw-r--r--   0        0        0      347 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/urls.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/__init__.py
+-rw-r--r--   0        0        0      328 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/apps.py
+-rw-r--r--   0        0        0      300 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/authenticators.py
+-rw-r--r--   0        0        0     1374 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/backends.py
+-rw-r--r--   0        0        0     5562 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/channel/serializers.py
+-rw-r--r--   0        0        0    16222 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/channel/tests.py
+-rw-r--r--   0        0        0      427 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/channel/urls.py
+-rw-r--r--   0        0        0     7181 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/channel/views.py
+-rw-r--r--   0        0        0     1433 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/classifier/serializers.py
+-rw-r--r--   0        0        0     8525 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/classifier/tests.py
+-rw-r--r--   0        0        0      351 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/classifier/urls.py
+-rw-r--r--   0        0        0     3169 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/classifier/views.py
+-rw-r--r--   0        0        0      107 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/clients/__init__.py
+-rw-r--r--   0        0        0      696 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/clients/authenticators.py
+-rw-r--r--   0        0        0      486 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/clients/base.py
+-rw-r--r--   0        0        0      580 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/clients/connect.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/externals/__init__.py
+-rw-r--r--   0        0        0     1308 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/externals/serializers.py
+-rw-r--r--   0        0        0      198 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/externals/urls.py
+-rw-r--r--   0        0        0     1064 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/externals/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/__init__.py
+-rw-r--r--   0        0        0     1278 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/serializers.py
+-rw-r--r--   0        0        0     4283 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/tests.py
+-rw-r--r--   0        0        0      308 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/urls.py
+-rw-r--r--   0        0        0      974 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/__init__.py
+-rw-r--r--   0        0        0     2286 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/tests/__init__.py
+-rw-r--r--   0        0        0     2183 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/tests/test_serializers.py
+-rw-r--r--   0        0        0      220 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/urls.py
+-rw-r--r--   0        0        0     1485 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/views.py
+-rw-r--r--   0        0        0      868 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1032 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/migrations/0002_project.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/migrations/__init__.py
+-rw-r--r--   0        0        0      813 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/models.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/__init__.py
+-rw-r--r--   0        0        0     3459 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/serializers.py
+-rw-r--r--   0        0        0    14533 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/tests.py
+-rw-r--r--   0        0        0      300 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/urls.py
+-rw-r--r--   0        0        0     4571 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/views.py
+-rw-r--r--   0        0        0      246 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/permissions.py
+-rw-r--r--   0        0        0     1993 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/statistic/tests.py
+-rw-r--r--   0        0        0      205 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/statistic/urls.py
+-rw-r--r--   0        0        0      831 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/statistic/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tests/__init__.py
+-rw-r--r--   0        0        0     1249 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tests/test_models.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/__init__.py
+-rw-r--r--   0        0        0     1152 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/tests/__init__.py
+-rw-r--r--   0        0        0     3398 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/tests/test_views.py
+-rw-r--r--   0        0        0      443 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/urls.py
+-rw-r--r--   0        0        0     1858 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/views.py
+-rw-r--r--   0        0        0     1315 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/urls.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/__init__.py
+-rw-r--r--   0        0        0      845 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/serializers.py
+-rw-r--r--   0        0        0    11864 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/tests.py
+-rw-r--r--   0        0        0      711 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/urls.py
+-rw-r--r--   0        0        0     5746 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/views.py
+-rw-r--r--   0        0        0      555 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/views.py
+-rw-r--r--   0        0        0       55 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/apps.py
+-rw-r--r--   0        0        0      906 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/serializers.py
+-rw-r--r--   0        0        0     4030 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/tests.py
+-rw-r--r--   0        0        0      178 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/urls.py
+-rw-r--r--   0        0        0     1444 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/views.py
+-rw-r--r--   0        0        0       45 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/s3/__init__.py
+-rw-r--r--   0        0        0      243 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/s3/apps.py
+-rw-r--r--   0        0        0      250 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/s3/urls.py
+-rw-r--r--   0        0        0      550 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/s3/views.py
+-rw-r--r--   0        0        0       79 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/serializers/__init__.py
+-rw-r--r--   0        0        0      725 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/serializers/fields.py
+-rw-r--r--   0        0        0      281 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/apps.py
+-rw-r--r--   0        0        0     2403 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/business.py
+-rw-r--r--   0        0        0      563 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/tests/__init__.py
+-rw-r--r--   0        0        0     2980 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/tests/test_business.py
+-rw-r--r--   0        0        0      494 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/urls.py
+-rw-r--r--   0        0        0     2774 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/views.py
+-rw-r--r--   0        0        0      318 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/README.md
+-rw-r--r--   0        0        0       72 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/__init__.py
+-rw-r--r--   0        0        0      294 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/apps.py
+-rw-r--r--   0        0        0     2041 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/serializers.py
+-rw-r--r--   0        0        0     5295 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/tests.py
+-rw-r--r--   0        0        0      344 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/urls.py
+-rw-r--r--   0        0        0     1651 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/templates/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/templates/context_processors.py
+-rw-r--r--   0        0        0      315 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/README.md
+-rw-r--r--   0        0        0       70 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/apps.py
+-rw-r--r--   0        0        0      242 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/serializers.py
+-rw-r--r--   0        0        0     1584 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/tests.py
+-rw-r--r--   0        0        0      378 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/urls.py
+-rw-r--r--   0        0        0      849 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/utils/__init__.py
+-rw-r--r--   0        0        0     1091 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/utils/app_config.py
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.0a3/PKG-INFO
```

### Comparing `weni_rp_apps-2.4.0a2/pyproject.toml` & `weni_rp_apps-2.4.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weni-rp-apps"
-version = "2.4.0a2"
+version = "2.4.0a3"
 description = "Weni apps for Rapidpro Platform"
 authors = ["jcbalmeida"]
 license = "AGPL-3.0"
 packages = [
     { include = "weni" }
 ]
```

### Comparing `weni_rp_apps-2.4.0a2/weni/activities/signals.py` & `weni_rp_apps-2.4.0a3/weni/activities/signals.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/analytics_api/tests.py` & `weni_rp_apps-2.4.0a3/weni/analytics_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/analytics_api/views.py` & `weni_rp_apps-2.4.0a3/weni/analytics_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/auth/backends.py` & `weni_rp_apps-2.4.0a3/weni/auth/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/auth/urls.py` & `weni_rp_apps-2.4.0a3/weni/auth/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/auth/views.py` & `weni_rp_apps-2.4.0a3/weni/auth/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/channel_stats/serializers.py` & `weni_rp_apps-2.4.0a3/weni/channel_stats/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/channel_stats/views.py` & `weni_rp_apps-2.4.0a3/weni/channel_stats/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/billing/queries.py` & `weni_rp_apps-2.4.0a3/weni/grpc/billing/queries.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/billing/serializers.py` & `weni_rp_apps-2.4.0a3/weni/grpc/billing/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/billing/services.py` & `weni_rp_apps-2.4.0a3/weni/grpc/billing/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/billing/tests.py` & `weni_rp_apps-2.4.0a3/weni/grpc/billing/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/channel/serializers.py` & `weni_rp_apps-2.4.0a3/weni/grpc/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/channel/services.py` & `weni_rp_apps-2.4.0a3/weni/grpc/channel/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/channel/tests.py` & `weni_rp_apps-2.4.0a3/weni/grpc/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/classifier/serializers.py` & `weni_rp_apps-2.4.0a3/weni/grpc/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/classifier/services.py` & `weni_rp_apps-2.4.0a3/weni/grpc/classifier/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/classifier/tests.py` & `weni_rp_apps-2.4.0a3/weni/grpc/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/core/management/commands/grpc.py` & `weni_rp_apps-2.4.0a3/weni/grpc/core/management/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/core/serializers.py` & `weni_rp_apps-2.4.0a3/weni/grpc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/core/services.py` & `weni_rp_apps-2.4.0a3/weni/grpc/core/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/core/urls.py` & `weni_rp_apps-2.4.0a3/weni/grpc/core/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/flow/services.py` & `weni_rp_apps-2.4.0a3/weni/grpc/flow/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/flow/tests.py` & `weni_rp_apps-2.4.0a3/weni/grpc/flow/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/org/serializers.py` & `weni_rp_apps-2.4.0a3/weni/grpc/org/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/org/services.py` & `weni_rp_apps-2.4.0a3/weni/grpc/org/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/org/tests.py` & `weni_rp_apps-2.4.0a3/weni/grpc/org/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/statistic/services.py` & `weni_rp_apps-2.4.0a3/weni/grpc/statistic/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/statistic/tests.py` & `weni_rp_apps-2.4.0a3/weni/grpc/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/user/serializers.py` & `weni_rp_apps-2.4.0a3/weni/grpc/user/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/user/services.py` & `weni_rp_apps-2.4.0a3/weni/grpc/user/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/grpc/user/tests.py` & `weni_rp_apps-2.4.0a3/weni/grpc/user/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/backends.py` & `weni_rp_apps-2.4.0a3/weni/internal/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/channel/serializers.py` & `weni_rp_apps-2.4.0a3/weni/internal/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/channel/tests.py` & `weni_rp_apps-2.4.0a3/weni/internal/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/channel/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/channel/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,25 +94,31 @@
             "channel_types": channel_types,
         }
         return Response(payload)
 
     def retrieve(self, request, pk=None):
         channel_type = None
         fields_form = {}
-        code_type = pk
+        code_type =  pk
+        current_form = None
         if code_type:
             channel_type = TYPES.get(code_type.upper(), None)
 
         if channel_type is None:
             return Response(status=status.HTTP_404_NOT_FOUND)
 
         fields_in_form = []
         if channel_type.claim_view:
             if channel_type.claim_view.form_class:
-                form = channel_type.claim_view.form_class.base_fields
+                current_form = channel_type.claim_view.form_class
+            elif channel_type.claim_view.ClaimForm:
+                current_form = channel_type.claim_view.ClaimForm
+
+            if current_form:
+                form = current_form.base_fields
                 for field in form:
                     fields_in_form.append(extract_form_info(form[field], field))
 
                 if not (fields_in_form):
                     return Response(status=status.HTTP_404_NOT_FOUND)
 
                 fields_form["form"] = fields_in_form
@@ -177,28 +183,28 @@
 
 
 def extract_form_info(_form, name_form):
     detail = {}
     detail["name"] = name_form if name_form else None
 
     try:
-        detail["type"] = str(_form.widget.input_type)
-    except:
-        detail["type"] = None
+        detail['type'] = str(_form.widget.input_type)
+    except AttributeError:
+        detail['type'] = str(_form.widget.__class__.__name__).lower()
 
     if _form.help_text:
         detail["help_text"] = str(_form.help_text)
     else:
-        detail["help_text"] = None
+        detail['help_text'] = ''
 
     if detail.get("type") == "select":
         detail["choices"] = _form.choices
 
     if _form.label:
         detail["label"] = str(_form.label)
     else:
-        detail["label"] = None
+        detail['label'] = ''
 
     if not (detail.get("name")) or not (detail.get("type")):
         return None
 
     return detail
```

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/classifier/serializers.py` & `weni_rp_apps-2.4.0a3/weni/internal/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/classifier/tests.py` & `weni_rp_apps-2.4.0a3/weni/internal/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/classifier/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/classifier/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/clients/authenticators.py` & `weni_rp_apps-2.4.0a3/weni/internal/clients/authenticators.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/clients/connect.py` & `weni_rp_apps-2.4.0a3/weni/internal/clients/connect.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/externals/serializers.py` & `weni_rp_apps-2.4.0a3/weni/internal/externals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/externals/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/externals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/flows/serializers.py` & `weni_rp_apps-2.4.0a3/weni/internal/flows/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/flows/tests.py` & `weni_rp_apps-2.4.0a3/weni/internal/flows/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/flows/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/flows/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/globals/serializers.py` & `weni_rp_apps-2.4.0a3/weni/internal/globals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/globals/tests/test_serializers.py` & `weni_rp_apps-2.4.0a3/weni/internal/globals/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/globals/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/globals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/migrations/0001_initial.py` & `weni_rp_apps-2.4.0a3/weni/internal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/migrations/0002_project.py` & `weni_rp_apps-2.4.0a3/weni/internal/migrations/0002_project.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/models.py` & `weni_rp_apps-2.4.0a3/weni/internal/models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/orgs/serializers.py` & `weni_rp_apps-2.4.0a3/weni/internal/orgs/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         return project
 
 
 class OrgSerializer(serializers.ModelSerializer):
     users = serializers.SerializerMethodField()
     timezone = serializers.CharField()
     uuid = serializers.UUIDField(source="project_uuid")
+    flow_organization = serializers.UUIDField(source="uuid")
 
     def set_user_permission(self, user: dict, permission: str) -> dict:
         user["permission_type"] = permission
         return user
 
     def get_users(self, project: Project):
         values = ["id", "email", "username", "first_name", "last_name"]
@@ -63,23 +64,23 @@
 
         users = administrators + viewers + editors + surveyors
 
         return users
 
     class Meta:
         model = Project
-        fields = ["id", "name", "uuid", "timezone", "date_format", "users"]
+        fields = ["id", "name", "uuid", "timezone", "date_format", "users", "flow_organization"]
 
 
 class OrgCreateSerializer(serializers.ModelSerializer):
     user_email = serializers.EmailField()
 
     class Meta:
         model = Project
-        fields = ["name", "timezone", "user_email"]
+        fields = ["name", "timezone", "user_email", "uuid"]
 
 
 class OrgUpdateSerializer(serializers.ModelSerializer):
     project_uuid = serializers.CharField(read_only=True)
     modified_by = weni_serializers.UserEmailRelatedField(required=False, write_only=True)
     timezone = serializers.CharField(required=False)
     name = serializers.CharField(required=False)
```

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/orgs/tests.py` & `weni_rp_apps-2.4.0a3/weni/internal/orgs/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/orgs/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/orgs/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
         project = Project.objects.create(
             name=request.data.get("name"),
             timezone=request.data.get("timezone"),
             created_by=user,
             modified_by=user,
             plan="infinity",
+            project_uuid=request.data.get("uuid")
+
         )
 
         project.administrators.add(user)
         project.initialize()
 
         org_serializer = OrgSerializer(project)
```

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/statistic/tests.py` & `weni_rp_apps-2.4.0a3/weni/internal/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/statistic/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/statistic/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/tests/test_models.py` & `weni_rp_apps-2.4.0a3/weni/internal/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/tickets/serializers.py` & `weni_rp_apps-2.4.0a3/weni/internal/tickets/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/tickets/tests/test_views.py` & `weni_rp_apps-2.4.0a3/weni/internal/tickets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/tickets/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/tickets/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,7 +45,13 @@
 
     def update(self, request, *args, **kwargs):
         partial = kwargs.get("partial", False)
         if not partial:
             self.http_method_not_allowed(request, *args, **kwargs)
 
         return super().update(request, *args, **kwargs)
+
+    def perform_destroy(self, instance):
+        ticketer = instance.ticketer
+        # Release Ticketer
+        ticketer.release(self.request.user)
+        instance.delete()
```

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/urls.py` & `weni_rp_apps-2.4.0a3/weni/internal/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/users/serializers.py` & `weni_rp_apps-2.4.0a3/weni/internal/users/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/users/tests.py` & `weni_rp_apps-2.4.0a3/weni/internal/users/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/users/urls.py` & `weni_rp_apps-2.4.0a3/weni/internal/users/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/users/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/users/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,37 @@
 from rest_framework.decorators import action
 from rest_framework.response import Response
 from rest_framework import exceptions
 from rest_framework import mixins
 from rest_framework.exceptions import ValidationError
 
 from weni.internal.views import InternalGenericViewSet
-from weni.internal.users.serializers import UserAPITokenSerializer, UserSerializer, UserPermissionSerializer
+from weni.internal.users.serializers import (
+    UserAPITokenSerializer,
+    UserSerializer,
+    UserPermissionSerializer,
+)
 from temba.api.models import APIToken
 from temba.orgs.models import Org
 from weni.internal.models import Project
 
 
 if TYPE_CHECKING:
     from rest_framework.request import Request
 
 User = get_user_model()
 
 
 class UserViewSet(InternalGenericViewSet):
-    @action(detail=False, methods=["GET"], url_path="api-token", serializer_class=UserAPITokenSerializer)
+    @action(
+        detail=False,
+        methods=["GET"],
+        url_path="api-token",
+        serializer_class=UserAPITokenSerializer,
+    )
     def api_token(self, request: "Request", **kwargs):
         serializer = self.get_serializer(data=request.query_params)
         serializer.is_valid(raise_exception=True)
 
         try:
             api_token = APIToken.objects.get(**serializer.validated_data)
         except APIToken.DoesNotExist:
@@ -124,26 +133,29 @@
     serializer_class = UserSerializer
     queryset = User.objects.all()
     lookup_field = "uuid"
 
     def partial_update(self, request):
         instance = get_object_or_404(User, email=request.query_params.get("email"))
 
-        if request.data.get("language") not in [language[0] for language in settings.LANGUAGES]:
+        if request.data.get("language") not in [
+            language[0] for language in settings.LANGUAGES
+        ]:
             raise ValidationError("Invalid argument: language")
 
         user_settings = instance.get_settings()
         user_settings.language = request.data.get("language")
         user_settings.save()
 
         return Response(status=status.HTTP_200_OK)
 
     def retrieve(self, request):
         if not request.query_params.get("email"):
             raise ValidationError(detail="empty email")
 
         user = User.objects.get_or_create(
-            email=request.query_params.get("email"), defaults={"username": request.query_params.get("email")}
+            email=request.query_params.get("email"),
+            defaults={"username": request.query_params.get("email")},
         )
 
         serializer = self.get_serializer(user[0])
         return Response(serializer.data)
```

### Comparing `weni_rp_apps-2.4.0a2/weni/internal/views.py` & `weni_rp_apps-2.4.0a3/weni/internal/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/orgs_api/serializers.py` & `weni_rp_apps-2.4.0a3/weni/orgs_api/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/orgs_api/tests.py` & `weni_rp_apps-2.4.0a3/weni/orgs_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/orgs_api/views.py` & `weni_rp_apps-2.4.0a3/weni/orgs_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/s3/views.py` & `weni_rp_apps-2.4.0a3/weni/s3/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/serializers/fields.py` & `weni_rp_apps-2.4.0a3/weni/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/success_orgs/business.py` & `weni_rp_apps-2.4.0a3/weni/success_orgs/business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/success_orgs/serializers.py` & `weni_rp_apps-2.4.0a3/weni/success_orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/success_orgs/tests/test_business.py` & `weni_rp_apps-2.4.0a3/weni/success_orgs/tests/test_business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/success_orgs/views.py` & `weni_rp_apps-2.4.0a3/weni/success_orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/template_message/serializers.py` & `weni_rp_apps-2.4.0a3/weni/template_message/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/template_message/tests.py` & `weni_rp_apps-2.4.0a3/weni/template_message/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/template_message/views.py` & `weni_rp_apps-2.4.0a3/weni/template_message/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/templates/context_processors.py` & `weni_rp_apps-2.4.0a3/weni/templates/context_processors.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/ticketer_queues/tests.py` & `weni_rp_apps-2.4.0a3/weni/ticketer_queues/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/ticketer_queues/views.py` & `weni_rp_apps-2.4.0a3/weni/ticketer_queues/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/weni/utils/app_config.py` & `weni_rp_apps-2.4.0a3/weni/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a2/PKG-INFO` & `weni_rp_apps-2.4.0a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weni-rp-apps
-Version: 2.4.0a2
+Version: 2.4.0a3
 Summary: Weni apps for Rapidpro Platform
 License: AGPL-3.0
 Author: jcbalmeida
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

