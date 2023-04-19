# Comparing `tmp/weni_rp_apps-2.4.0a3.tar.gz` & `tmp/weni_rp_apps-2.4.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weni_rp_apps-2.4.0a3.tar", max compression
+gzip compressed data, was "weni_rp_apps-2.4.0a4.tar", max compression
```

## Comparing `weni_rp_apps-2.4.0a3.tar` & `weni_rp_apps-2.4.0a4.tar`

### file list

```diff
@@ -1,173 +1,172 @@
--rw-r--r--   0        0        0      646 2023-04-19 14:01:07.171892 weni_rp_apps-2.4.0a3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/__init__.py
--rw-r--r--   0        0        0      231 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/apps.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/migrations/__init__.py
--rw-r--r--   0        0        0     1960 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/signals.py
--rw-r--r--   0        0        0      366 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/activities/tasks.py
--rw-r--r--   0        0        0      325 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/README.md
--rw-r--r--   0        0        0       66 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/__init__.py
--rw-r--r--   0        0        0      264 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/apps.py
--rw-r--r--   0        0        0    13526 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/tests.py
--rw-r--r--   0        0        0      475 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/urls.py
--rw-r--r--   0        0        0     8909 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/analytics_api/views.py
--rw-r--r--   0        0        0       49 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/__init__.py
--rw-r--r--   0        0        0      285 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/apps.py
--rw-r--r--   0        0        0     1792 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/backends.py
--rw-r--r--   0        0        0      430 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/decorators.py
--rw-r--r--   0        0        0      733 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/urls.py
--rw-r--r--   0        0        0     2645 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/auth/views.py
--rw-r--r--   0        0        0      309 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/README.md
--rw-r--r--   0        0        0       66 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/__init__.py
--rw-r--r--   0        0        0      264 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/apps.py
--rw-r--r--   0        0        0     6157 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/serializers.py
--rw-r--r--   0        0        0      317 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/urls.py
--rw-r--r--   0        0        0     3575 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/channel_stats/views.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/__init__.py
--rw-r--r--   0        0        0      102 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/apps.py
--rw-r--r--   0        0        0     3508 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/queries.py
--rw-r--r--   0        0        0     3194 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/serializers.py
--rw-r--r--   0        0        0     2072 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/services.py
--rw-r--r--   0        0        0    11471 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/tests.py
--rw-r--r--   0        0        0      231 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/billing/urls.py
--rw-r--r--   0        0        0       64 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/__init__.py
--rw-r--r--   0        0        0      103 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/apps.py
--rw-r--r--   0        0        0      352 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/fields.py
--rw-r--r--   0        0        0     4110 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/serializers.py
--rw-r--r--   0        0        0     4023 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/services.py
--rw-r--r--   0        0        0     7747 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/tests.py
--rw-r--r--   0        0        0      341 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/channel/urls.py
--rw-r--r--   0        0        0       70 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/__init__.py
--rw-r--r--   0        0        0      109 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/apps.py
--rw-r--r--   0        0        0     1262 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/serializers.py
--rw-r--r--   0        0        0     1175 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/services.py
--rw-r--r--   0        0        0     6460 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/tests.py
--rw-r--r--   0        0        0      249 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/classifier/urls.py
--rw-r--r--   0        0        0       61 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/__init__.py
--rw-r--r--   0        0        0      100 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/apps.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/management/commands/__init__.py
--rw-r--r--   0        0        0     1573 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/management/commands/grpc.py
--rw-r--r--   0        0        0     1213 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/serializers.py
--rw-r--r--   0        0        0      965 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/services.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/tests.py
--rw-r--r--   0        0        0      700 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/core/urls.py
--rw-r--r--   0        0        0       58 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/__init__.py
--rw-r--r--   0        0        0       97 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/apps.py
--rw-r--r--   0        0        0      307 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/serializers.py
--rw-r--r--   0        0        0      658 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/services.py
--rw-r--r--   0        0        0     2766 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/tests.py
--rw-r--r--   0        0        0      213 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/flow/urls.py
--rw-r--r--   0        0        0       56 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/__init__.py
--rw-r--r--   0        0        0       95 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/apps.py
--rw-r--r--   0        0        0     2770 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/serializers.py
--rw-r--r--   0        0        0     3957 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/services.py
--rw-r--r--   0        0        0     9824 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/tests.py
--rw-r--r--   0        0        0      207 2023-04-19 14:00:49.951641 weni_rp_apps-2.4.0a3/weni/grpc/org/urls.py
--rw-r--r--   0        0        0       68 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/__init__.py
--rw-r--r--   0        0        0      107 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/apps.py
--rw-r--r--   0        0        0      672 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/services.py
--rw-r--r--   0        0        0     3134 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/tests.py
--rw-r--r--   0        0        0      252 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/statistic/urls.py
--rw-r--r--   0        0        0       58 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/__init__.py
--rw-r--r--   0        0        0       97 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/apps.py
--rw-r--r--   0        0        0      843 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/serializers.py
--rw-r--r--   0        0        0     3906 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/services.py
--rw-r--r--   0        0        0    10078 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/tests.py
--rw-r--r--   0        0        0      347 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/grpc/user/urls.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/__init__.py
--rw-r--r--   0        0        0      328 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/apps.py
--rw-r--r--   0        0        0      300 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/authenticators.py
--rw-r--r--   0        0        0     1374 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/backends.py
--rw-r--r--   0        0        0     5562 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/channel/serializers.py
--rw-r--r--   0        0        0    16222 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/channel/tests.py
--rw-r--r--   0        0        0      427 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/channel/urls.py
--rw-r--r--   0        0        0     7181 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/channel/views.py
--rw-r--r--   0        0        0     1433 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/classifier/serializers.py
--rw-r--r--   0        0        0     8525 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/classifier/tests.py
--rw-r--r--   0        0        0      351 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/classifier/urls.py
--rw-r--r--   0        0        0     3169 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/classifier/views.py
--rw-r--r--   0        0        0      107 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/clients/__init__.py
--rw-r--r--   0        0        0      696 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/clients/authenticators.py
--rw-r--r--   0        0        0      486 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/clients/base.py
--rw-r--r--   0        0        0      580 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/clients/connect.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/externals/__init__.py
--rw-r--r--   0        0        0     1308 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/externals/serializers.py
--rw-r--r--   0        0        0      198 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/externals/urls.py
--rw-r--r--   0        0        0     1064 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/externals/views.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/__init__.py
--rw-r--r--   0        0        0     1278 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/serializers.py
--rw-r--r--   0        0        0     4283 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/tests.py
--rw-r--r--   0        0        0      308 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/urls.py
--rw-r--r--   0        0        0      974 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/flows/views.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/__init__.py
--rw-r--r--   0        0        0     2286 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/serializers.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/tests/__init__.py
--rw-r--r--   0        0        0     2183 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/tests/test_serializers.py
--rw-r--r--   0        0        0      220 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/urls.py
--rw-r--r--   0        0        0     1485 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/globals/views.py
--rw-r--r--   0        0        0      868 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/migrations/0001_initial.py
--rw-r--r--   0        0        0     1032 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/migrations/0002_project.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/migrations/__init__.py
--rw-r--r--   0        0        0      813 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/models.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/__init__.py
--rw-r--r--   0        0        0     3459 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/serializers.py
--rw-r--r--   0        0        0    14533 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/tests.py
--rw-r--r--   0        0        0      300 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/urls.py
--rw-r--r--   0        0        0     4571 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/orgs/views.py
--rw-r--r--   0        0        0      246 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/permissions.py
--rw-r--r--   0        0        0     1993 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/statistic/tests.py
--rw-r--r--   0        0        0      205 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/statistic/urls.py
--rw-r--r--   0        0        0      831 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/statistic/views.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tests/__init__.py
--rw-r--r--   0        0        0     1249 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tests/test_models.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/__init__.py
--rw-r--r--   0        0        0     1152 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/serializers.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/tests/__init__.py
--rw-r--r--   0        0        0     3398 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/tests/test_views.py
--rw-r--r--   0        0        0      443 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/urls.py
--rw-r--r--   0        0        0     1858 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/tickets/views.py
--rw-r--r--   0        0        0     1315 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/urls.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/__init__.py
--rw-r--r--   0        0        0      845 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/serializers.py
--rw-r--r--   0        0        0    11864 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/tests.py
--rw-r--r--   0        0        0      711 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/urls.py
--rw-r--r--   0        0        0     5746 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/users/views.py
--rw-r--r--   0        0        0      555 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/internal/views.py
--rw-r--r--   0        0        0       55 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/__init__.py
--rw-r--r--   0        0        0      253 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/apps.py
--rw-r--r--   0        0        0      906 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/serializers.py
--rw-r--r--   0        0        0     4030 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/tests.py
--rw-r--r--   0        0        0      178 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/urls.py
--rw-r--r--   0        0        0     1444 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/orgs_api/views.py
--rw-r--r--   0        0        0       45 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/s3/__init__.py
--rw-r--r--   0        0        0      243 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/s3/apps.py
--rw-r--r--   0        0        0      250 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/s3/urls.py
--rw-r--r--   0        0        0      550 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/s3/views.py
--rw-r--r--   0        0        0       79 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/serializers/__init__.py
--rw-r--r--   0        0        0      725 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/serializers/fields.py
--rw-r--r--   0        0        0      281 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/apps.py
--rw-r--r--   0        0        0     2403 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/business.py
--rw-r--r--   0        0        0      563 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/serializers.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/tests/__init__.py
--rw-r--r--   0        0        0     2980 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/tests/test_business.py
--rw-r--r--   0        0        0      494 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/urls.py
--rw-r--r--   0        0        0     2774 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/success_orgs/views.py
--rw-r--r--   0        0        0      318 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/README.md
--rw-r--r--   0        0        0       72 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/__init__.py
--rw-r--r--   0        0        0      294 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/apps.py
--rw-r--r--   0        0        0     2041 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/serializers.py
--rw-r--r--   0        0        0     5295 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/tests.py
--rw-r--r--   0        0        0      344 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/urls.py
--rw-r--r--   0        0        0     1651 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/template_message/views.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/templates/__init__.py
--rw-r--r--   0        0        0      559 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/templates/context_processors.py
--rw-r--r--   0        0        0      315 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/README.md
--rw-r--r--   0        0        0       70 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/__init__.py
--rw-r--r--   0        0        0      291 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/apps.py
--rw-r--r--   0        0        0      242 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/serializers.py
--rw-r--r--   0        0        0     1584 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/tests.py
--rw-r--r--   0        0        0      378 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/urls.py
--rw-r--r--   0        0        0      849 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/ticketer_queues/views.py
--rw-r--r--   0        0        0        0 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/utils/__init__.py
--rw-r--r--   0        0        0     1091 2023-04-19 14:00:49.955641 weni_rp_apps-2.4.0a3/weni/utils/app_config.py
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.0a3/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-04-19 15:02:28.925304 weni_rp_apps-2.4.0a4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/activities/__init__.py
+-rw-r--r--   0        0        0      231 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/activities/apps.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/activities/migrations/__init__.py
+-rw-r--r--   0        0        0     1960 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/activities/signals.py
+-rw-r--r--   0        0        0      366 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/activities/tasks.py
+-rw-r--r--   0        0        0      325 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/analytics_api/README.md
+-rw-r--r--   0        0        0       66 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/analytics_api/__init__.py
+-rw-r--r--   0        0        0      264 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/analytics_api/apps.py
+-rw-r--r--   0        0        0    13526 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/analytics_api/tests.py
+-rw-r--r--   0        0        0      475 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/analytics_api/urls.py
+-rw-r--r--   0        0        0     8909 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/analytics_api/views.py
+-rw-r--r--   0        0        0       49 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/auth/__init__.py
+-rw-r--r--   0        0        0      285 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/auth/apps.py
+-rw-r--r--   0        0        0     1792 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/auth/backends.py
+-rw-r--r--   0        0        0      430 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/auth/decorators.py
+-rw-r--r--   0        0        0      733 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/auth/urls.py
+-rw-r--r--   0        0        0     2645 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/auth/views.py
+-rw-r--r--   0        0        0      309 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/channel_stats/README.md
+-rw-r--r--   0        0        0       66 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/channel_stats/__init__.py
+-rw-r--r--   0        0        0      264 2023-04-19 15:02:04.257413 weni_rp_apps-2.4.0a4/weni/channel_stats/apps.py
+-rw-r--r--   0        0        0     6157 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/channel_stats/serializers.py
+-rw-r--r--   0        0        0      317 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/channel_stats/urls.py
+-rw-r--r--   0        0        0     3575 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/channel_stats/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/billing/__init__.py
+-rw-r--r--   0        0        0      102 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/billing/apps.py
+-rw-r--r--   0        0        0     3508 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/billing/queries.py
+-rw-r--r--   0        0        0     3194 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/billing/serializers.py
+-rw-r--r--   0        0        0     2072 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/billing/services.py
+-rw-r--r--   0        0        0    11471 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/billing/tests.py
+-rw-r--r--   0        0        0      231 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/billing/urls.py
+-rw-r--r--   0        0        0       64 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/channel/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/channel/apps.py
+-rw-r--r--   0        0        0      352 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/channel/fields.py
+-rw-r--r--   0        0        0     4110 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/channel/serializers.py
+-rw-r--r--   0        0        0     4023 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/channel/services.py
+-rw-r--r--   0        0        0     7747 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/channel/tests.py
+-rw-r--r--   0        0        0      341 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/channel/urls.py
+-rw-r--r--   0        0        0       70 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/classifier/__init__.py
+-rw-r--r--   0        0        0      109 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/classifier/apps.py
+-rw-r--r--   0        0        0     1262 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/classifier/serializers.py
+-rw-r--r--   0        0        0     1175 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/classifier/services.py
+-rw-r--r--   0        0        0     6460 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/classifier/tests.py
+-rw-r--r--   0        0        0      249 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/classifier/urls.py
+-rw-r--r--   0        0        0       61 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/core/__init__.py
+-rw-r--r--   0        0        0      100 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/core/apps.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1573 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/core/management/commands/grpc.py
+-rw-r--r--   0        0        0     1213 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/core/serializers.py
+-rw-r--r--   0        0        0      965 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/core/services.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/core/tests.py
+-rw-r--r--   0        0        0      700 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/core/urls.py
+-rw-r--r--   0        0        0       58 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/flow/__init__.py
+-rw-r--r--   0        0        0       97 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/flow/apps.py
+-rw-r--r--   0        0        0      307 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/flow/serializers.py
+-rw-r--r--   0        0        0      658 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/flow/services.py
+-rw-r--r--   0        0        0     2766 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/flow/tests.py
+-rw-r--r--   0        0        0      213 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/flow/urls.py
+-rw-r--r--   0        0        0       56 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/org/__init__.py
+-rw-r--r--   0        0        0       95 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/org/apps.py
+-rw-r--r--   0        0        0     2770 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/org/serializers.py
+-rw-r--r--   0        0        0     3957 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/org/services.py
+-rw-r--r--   0        0        0     9824 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/org/tests.py
+-rw-r--r--   0        0        0      207 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/org/urls.py
+-rw-r--r--   0        0        0       68 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/statistic/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/statistic/apps.py
+-rw-r--r--   0        0        0      672 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/statistic/services.py
+-rw-r--r--   0        0        0     3134 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/statistic/tests.py
+-rw-r--r--   0        0        0      252 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/statistic/urls.py
+-rw-r--r--   0        0        0       58 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/user/__init__.py
+-rw-r--r--   0        0        0       97 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/user/apps.py
+-rw-r--r--   0        0        0      843 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/user/serializers.py
+-rw-r--r--   0        0        0     3906 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/user/services.py
+-rw-r--r--   0        0        0    10078 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/user/tests.py
+-rw-r--r--   0        0        0      347 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/grpc/user/urls.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/internal/__init__.py
+-rw-r--r--   0        0        0      328 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/internal/apps.py
+-rw-r--r--   0        0        0      300 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/internal/authenticators.py
+-rw-r--r--   0        0        0     1374 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/internal/backends.py
+-rw-r--r--   0        0        0     5433 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/internal/channel/serializers.py
+-rw-r--r--   0        0        0    15855 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/internal/channel/tests.py
+-rw-r--r--   0        0        0      427 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/internal/channel/urls.py
+-rw-r--r--   0        0        0     7049 2023-04-19 15:02:04.261413 weni_rp_apps-2.4.0a4/weni/internal/channel/views.py
+-rw-r--r--   0        0        0     1433 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/classifier/serializers.py
+-rw-r--r--   0        0        0     8525 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/classifier/tests.py
+-rw-r--r--   0        0        0      351 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/classifier/urls.py
+-rw-r--r--   0        0        0     3169 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/classifier/views.py
+-rw-r--r--   0        0        0      107 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/clients/__init__.py
+-rw-r--r--   0        0        0      696 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/clients/authenticators.py
+-rw-r--r--   0        0        0      486 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/clients/base.py
+-rw-r--r--   0        0        0      580 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/clients/connect.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/externals/__init__.py
+-rw-r--r--   0        0        0     1308 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/externals/serializers.py
+-rw-r--r--   0        0        0      294 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/externals/urls.py
+-rw-r--r--   0        0        0     1501 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/externals/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/flows/__init__.py
+-rw-r--r--   0        0        0     1278 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/flows/serializers.py
+-rw-r--r--   0        0        0     4283 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/flows/tests.py
+-rw-r--r--   0        0        0      308 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/flows/urls.py
+-rw-r--r--   0        0        0      974 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/flows/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/globals/__init__.py
+-rw-r--r--   0        0        0     2286 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/globals/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/globals/tests/__init__.py
+-rw-r--r--   0        0        0     2183 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/globals/tests/test_serializers.py
+-rw-r--r--   0        0        0      220 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/globals/urls.py
+-rw-r--r--   0        0        0     1055 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/globals/views.py
+-rw-r--r--   0        0        0      868 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/migrations/__init__.py
+-rw-r--r--   0        0        0      460 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/models.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/orgs/__init__.py
+-rw-r--r--   0        0        0     3264 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/orgs/serializers.py
+-rw-r--r--   0        0        0    14123 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/orgs/tests.py
+-rw-r--r--   0        0        0      300 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/orgs/urls.py
+-rw-r--r--   0        0        0     4230 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/orgs/views.py
+-rw-r--r--   0        0        0      246 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/permissions.py
+-rw-r--r--   0        0        0     1993 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/statistic/tests.py
+-rw-r--r--   0        0        0      205 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/statistic/urls.py
+-rw-r--r--   0        0        0      831 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/statistic/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/tests/__init__.py
+-rw-r--r--   0        0        0     1249 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/tests/test_models.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/tickets/__init__.py
+-rw-r--r--   0        0        0     1152 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/tickets/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/tickets/tests/__init__.py
+-rw-r--r--   0        0        0     3398 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/tickets/tests/test_views.py
+-rw-r--r--   0        0        0      443 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/tickets/urls.py
+-rw-r--r--   0        0        0     1682 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/tickets/views.py
+-rw-r--r--   0        0        0     1315 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/urls.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/users/__init__.py
+-rw-r--r--   0        0        0      840 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/users/serializers.py
+-rw-r--r--   0        0        0    10909 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/users/tests.py
+-rw-r--r--   0        0        0      711 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/users/urls.py
+-rw-r--r--   0        0        0     5341 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/users/views.py
+-rw-r--r--   0        0        0      555 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/internal/views.py
+-rw-r--r--   0        0        0       55 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/orgs_api/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/orgs_api/apps.py
+-rw-r--r--   0        0        0      906 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/orgs_api/serializers.py
+-rw-r--r--   0        0        0     4030 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/orgs_api/tests.py
+-rw-r--r--   0        0        0      178 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/orgs_api/urls.py
+-rw-r--r--   0        0        0     1444 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/orgs_api/views.py
+-rw-r--r--   0        0        0       45 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/s3/__init__.py
+-rw-r--r--   0        0        0      243 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/s3/apps.py
+-rw-r--r--   0        0        0      250 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/s3/urls.py
+-rw-r--r--   0        0        0      550 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/s3/views.py
+-rw-r--r--   0        0        0       79 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/serializers/__init__.py
+-rw-r--r--   0        0        0      495 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/serializers/fields.py
+-rw-r--r--   0        0        0      281 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/success_orgs/apps.py
+-rw-r--r--   0        0        0     2403 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/success_orgs/business.py
+-rw-r--r--   0        0        0      563 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/success_orgs/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/success_orgs/tests/__init__.py
+-rw-r--r--   0        0        0     2980 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/success_orgs/tests/test_business.py
+-rw-r--r--   0        0        0      494 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/success_orgs/urls.py
+-rw-r--r--   0        0        0     2774 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/success_orgs/views.py
+-rw-r--r--   0        0        0      318 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/template_message/README.md
+-rw-r--r--   0        0        0       72 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/template_message/__init__.py
+-rw-r--r--   0        0        0      294 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/template_message/apps.py
+-rw-r--r--   0        0        0     2041 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/template_message/serializers.py
+-rw-r--r--   0        0        0     5295 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/template_message/tests.py
+-rw-r--r--   0        0        0      344 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/template_message/urls.py
+-rw-r--r--   0        0        0     1651 2023-04-19 15:02:04.265413 weni_rp_apps-2.4.0a4/weni/template_message/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/templates/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/templates/context_processors.py
+-rw-r--r--   0        0        0      315 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/ticketer_queues/README.md
+-rw-r--r--   0        0        0       70 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/ticketer_queues/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/ticketer_queues/apps.py
+-rw-r--r--   0        0        0      242 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/ticketer_queues/serializers.py
+-rw-r--r--   0        0        0     1584 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/ticketer_queues/tests.py
+-rw-r--r--   0        0        0      378 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/ticketer_queues/urls.py
+-rw-r--r--   0        0        0      849 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/ticketer_queues/views.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/utils/__init__.py
+-rw-r--r--   0        0        0     1091 2023-04-19 15:02:04.269413 weni_rp_apps-2.4.0a4/weni/utils/app_config.py
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.0a4/PKG-INFO
```

### Comparing `weni_rp_apps-2.4.0a3/pyproject.toml` & `weni_rp_apps-2.4.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weni-rp-apps"
-version = "2.4.0a3"
+version = "2.4.0a4"
 description = "Weni apps for Rapidpro Platform"
 authors = ["jcbalmeida"]
 license = "AGPL-3.0"
 packages = [
     { include = "weni" }
 ]
```

### Comparing `weni_rp_apps-2.4.0a3/weni/activities/signals.py` & `weni_rp_apps-2.4.0a4/weni/activities/signals.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/analytics_api/tests.py` & `weni_rp_apps-2.4.0a4/weni/analytics_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/analytics_api/views.py` & `weni_rp_apps-2.4.0a4/weni/analytics_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/auth/backends.py` & `weni_rp_apps-2.4.0a4/weni/auth/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/auth/urls.py` & `weni_rp_apps-2.4.0a4/weni/auth/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/auth/views.py` & `weni_rp_apps-2.4.0a4/weni/auth/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/channel_stats/serializers.py` & `weni_rp_apps-2.4.0a4/weni/channel_stats/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/channel_stats/views.py` & `weni_rp_apps-2.4.0a4/weni/channel_stats/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/billing/queries.py` & `weni_rp_apps-2.4.0a4/weni/grpc/billing/queries.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/billing/serializers.py` & `weni_rp_apps-2.4.0a4/weni/grpc/billing/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/billing/services.py` & `weni_rp_apps-2.4.0a4/weni/grpc/billing/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/billing/tests.py` & `weni_rp_apps-2.4.0a4/weni/grpc/billing/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/channel/serializers.py` & `weni_rp_apps-2.4.0a4/weni/grpc/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/channel/services.py` & `weni_rp_apps-2.4.0a4/weni/grpc/channel/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/channel/tests.py` & `weni_rp_apps-2.4.0a4/weni/grpc/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/classifier/serializers.py` & `weni_rp_apps-2.4.0a4/weni/grpc/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/classifier/services.py` & `weni_rp_apps-2.4.0a4/weni/grpc/classifier/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/classifier/tests.py` & `weni_rp_apps-2.4.0a4/weni/grpc/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/core/management/commands/grpc.py` & `weni_rp_apps-2.4.0a4/weni/grpc/core/management/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/core/serializers.py` & `weni_rp_apps-2.4.0a4/weni/grpc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/core/services.py` & `weni_rp_apps-2.4.0a4/weni/grpc/core/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/core/urls.py` & `weni_rp_apps-2.4.0a4/weni/grpc/core/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/flow/services.py` & `weni_rp_apps-2.4.0a4/weni/grpc/flow/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/flow/tests.py` & `weni_rp_apps-2.4.0a4/weni/grpc/flow/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/org/serializers.py` & `weni_rp_apps-2.4.0a4/weni/grpc/org/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/org/services.py` & `weni_rp_apps-2.4.0a4/weni/grpc/org/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/org/tests.py` & `weni_rp_apps-2.4.0a4/weni/grpc/org/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/statistic/services.py` & `weni_rp_apps-2.4.0a4/weni/grpc/statistic/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/statistic/tests.py` & `weni_rp_apps-2.4.0a4/weni/grpc/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/user/serializers.py` & `weni_rp_apps-2.4.0a4/weni/grpc/user/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/user/services.py` & `weni_rp_apps-2.4.0a4/weni/grpc/user/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/grpc/user/tests.py` & `weni_rp_apps-2.4.0a4/weni/grpc/user/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/backends.py` & `weni_rp_apps-2.4.0a4/weni/internal/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/channel/serializers.py` & `weni_rp_apps-2.4.0a4/weni/internal/channel/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 from django.contrib.messages.middleware import MessageMiddleware
 from django.shortcuts import get_object_or_404
 from django.test import RequestFactory
 
 from rest_framework import serializers
 from rest_framework import exceptions
 
-from weni.serializers import fields as weni_serializers
+from weni.grpc.core import serializers as weni_serializers
 
 from temba.channels.models import Channel
 from temba.orgs.models import Org
 from temba.utils import analytics
-from weni.internal.models import Project
 
 
 class ChannelWACSerializer(serializers.Serializer):
     user = weni_serializers.UserEmailRelatedField(required=True, write_only=True)
-    org = weni_serializers.ProjectUUIDRelatedField(required=True, write_only=True)
+    org = weni_serializers.OrgUUIDRelatedField(required=True, write_only=True)
     phone_number_id = serializers.CharField(required=True, write_only=True)
     uuid = serializers.CharField(read_only=True)
     name = serializers.CharField(read_only=True)
     address = serializers.CharField(read_only=True)
     config = serializers.JSONField(required=True)
 
     class Meta:
@@ -47,15 +46,15 @@
             raise serializers.ValidationError({"error": "You need to define a wa_verified_name in config"})
         return value
 
     def create(self, validated_data):
         channel_type = Channel.get_type_from_code("WAC")
         schemes = channel_type.schemes
 
-        org = validated_data["org"].org
+        org = validated_data.get("org")
         name = validated_data.get("name")
         phone_number_id = validated_data.get("phone_number_id")
         config = validated_data.get("config", {})
         user = validated_data.get("user")
 
         channel = Channel.objects.create(
             org=org,
@@ -86,37 +85,37 @@
     data = serializers.JSONField(write_only=True)
     channeltype_code = serializers.CharField(required=True, write_only=True)
 
     def create(self, validated_data):
         data = validated_data.get("data")
 
         user = get_object_or_404(User, email=validated_data.get("user"))
-        org = get_object_or_404(Project, project_uuid=validated_data.get("org"))
+        org = get_object_or_404(Org, uuid=validated_data.get("org"))
 
         channel_type = Channel.get_type_from_code(validated_data.get("channeltype_code"))
 
         if channel_type is None:
             channel_type_code = validated_data.get("channeltype_code")
             raise exceptions.ValidationError(f"No channels found with '{channel_type_code}' code")
 
-        url = self.create_channel(user, org.org, data, channel_type)
+        url = self.create_channel(user, org, data, channel_type)
 
         if url is None:
             raise exceptions.ValidationError(f"Url not created")
 
         if "/users/login/?next=" in url:
-            raise exceptions.ValidationError(f"User: {user.email} do not have permission in Org: {org.org.uuid}")
+            raise exceptions.ValidationError(f"User: {user.email} do not have permission in Org: {org.uuid}")
 
         regex = "[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}"
         channe_uuid = re.findall(regex, url)[0]
         channel = Channel.objects.get(uuid=channe_uuid)
 
         return channel
 
-    def create_channel(self, user: User, org: Project, data: dict, channel_type) -> str:
+    def create_channel(self, user: User, org: Org, data: dict, channel_type) -> str:
         factory = RequestFactory()
         url = f"channels/types/{channel_type.slug}/claim"
 
         request = factory.post(url, data)
         middleware = SessionMiddleware()
         middleware.process_request(request)
         request.session.save()
@@ -145,10 +144,9 @@
             "address",
             "org",
             "is_active",
         ) 
 
     def to_representation(self, instance):
         ret = super().to_representation(instance)
-        ret["org"] = instance.org.project.project_uuid if hasattr(instance.org, "project") else None
-
+        ret['org'] = instance.org.uuid
         return ret
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/channel/tests.py` & `weni_rp_apps-2.4.0a4/weni/internal/channel/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,22 +17,18 @@
 from temba.api.models import APIToken
 from temba.flows.models import Flow
 from temba.orgs.models import Org, OrgRole
 from temba.contacts.models import Contact
 from temba.channels.models import Channel
 from temba.channels.types import TYPES
 from temba.tests import TembaTest, mock_mailroom
-from weni.internal.models import Project
-
-from .views import AvailableChannels, ChannelEndpoint, extract_form_info, extract_type_info
-
-view_class = ChannelEndpoint
-view_class.permission_classes = []
 
+from .views import AvailableChannels, extract_form_info, extract_type_info
 
+ 
 class TembaRequestMixin(ABC):
     def reverse(self, viewname, kwargs=None, query_params=None):
         url = reverse(viewname, kwargs=kwargs)
 
         if query_params:
             return "%s?%s" % (url, urlencode(query_params))
         else:
@@ -48,38 +44,38 @@
         url = self.reverse(self.get_url_namespace(), kwargs={"uuid": uuid})
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.get(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     def request_post(self, data):
         url = reverse(self.get_url_namespace())
-        token = APIToken.get_or_create(self.project, self.admin, Group.objects.get(name="Administrators"))
+        token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.post(
             url, HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
         )
 
-    def request_delete(self, uuid, **query_params):
-        url = self.reverse(self.get_url_namespace(), kwargs={"uuid": uuid}, query_params=query_params)
+    def request_delete(self, uuid):
+        url = self.reverse(self.get_url_namespace(), kwargs={"uuid": uuid})
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.delete(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     @abstractmethod
     def get_url_namespace(self):
         ...
 
 
 class CreateWACServiceTest(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
-        self.project = Project.objects.create(
+        self.org = Org.objects.create(
             name="Weni", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
         )
-        self.project.add_user(self.user, OrgRole.ADMINISTRATOR)
+        self.org.add_user(self.user, OrgRole.ADMINISTRATOR)
 
         self.config = {
             "wa_number": "5561995743921",
             "wa_verified_name": "Weni Test",
             "wa_waba_id": "2433443436435435",
             "wa_currency": "USD",
             "wa_business_id": "3443243234254322",
@@ -91,15 +87,15 @@
     @patch("temba.channels.types.whatsapp_cloud.type.WhatsAppCloudType.activate")
     def test_create_whatsapp_cloud_channel(self, mock):
         mock.return_value = None
 
         phone_number_id = "5426423432"
 
         payload = {
-            "org": str(self.project.project_uuid),
+            "org": str(self.org.uuid),
             "user": self.user.email,
             "phone_number_id": phone_number_id,
             "config": self.config,
         }
 
         channel = self.request_post(data=payload).json()
 
@@ -111,15 +107,15 @@
     @patch("temba.channels.types.whatsapp_cloud.type.WhatsAppCloudType.activate")
     def test_create_whatsapp_cloud_channel_invalid_address(self, mock):
         mock.return_value = None
 
         phone_number_id = "5426423432"
 
         payload = {
-            "org": str(self.project.project_uuid),
+            "org": str(self.org.uuid),
             "user": self.user.email,
             "phone_number_id": phone_number_id,
             "config": self.config,
         }
 
         self.request_post(data=payload)
 
@@ -133,74 +129,76 @@
     def get_url_namespace(self):
         return "channel-create-wac"
 
 
 class ReleaseChannelTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.org_user = User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
-        self.my_org = Project.objects.create(
+        self.my_org = Org.objects.create(
             name="Weni", timezone="Africa/Kigali", created_by=self.org_user, modified_by=self.org_user
         )
 
         super().setUp()
-        self.channel_obj = Channel.create(self.my_org.org, self.org_user, None, "WWC", "Test WWC")
+
+        self.channel_obj = Channel.create(self.my_org, self.org_user, None, "WWC", "Test WWC")
 
     def test_released_channel_is_active_equal_to_false(self):
-        response = self.request_delete(uuid=str(self.channel_obj.uuid), user=self.org_user.email)
-        self.assertEqual(response.status_code, 200)
+        self.request_delete(uuid=str(self.channel_obj.uuid))
         self.assertFalse(Channel.objects.get(id=self.channel_obj.id).is_active)
 
     def get_url_namespace(self):
         return "channel-detail"
 
 
 class CreateChannelTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.org_user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
-        self.project = Project.objects.create(
+        self.my_org = Org.objects.create(
             name="Weni", timezone="America/Sao_Paulo", created_by=self.org_user, modified_by=self.org_user
         )
-        self.project.add_user(self.org_user, OrgRole.ADMINISTRATOR)
+        self.my_org.add_user(self.org_user, OrgRole.ADMINISTRATOR)
 
         super().setUp()
 
     def test_create_weni_web_chat_channel(self):
         payload = {
             "user": self.org_user.email,
-            "org": str(self.project.project_uuid),
+            "org": str(self.my_org.uuid),
             "data": {"name": "test", "base_url": "https://weni.ai"},
             "channeltype_code": "WWC",
         }
 
         response = self.request_post(data=payload).json()
 
+        print(response)
+
         channel = Channel.objects.get(uuid=response.get("uuid"))
         self.assertEqual(channel.address, response.get("address"))
         self.assertEqual(channel.name, response.get("name"))
         self.assertEqual(channel.config.get("base_url"), "https://weni.ai")
-        self.assertEqual(channel.org, self.project.org)
+        self.assertEqual(channel.org, self.my_org)
         self.assertEqual(channel.created_by, self.org_user)
         self.assertEqual(channel.modified_by, self.org_user)
         self.assertEqual(channel.channel_type, "WWC")
 
     def get_url_namespace(self):
         return "channel-list"
 
 
 class RetrieveChannelTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
-        self.project = Project.objects.create(
+        self.org = Org.objects.create(
             name="Weni", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
         )
 
         super().setUp()
 
         self.channel_obj = Channel.create(
-            self.project.org, self.user, None, "WWC", "Test WWC", "test", {"fake_key": "fake_value"}
+            self.org, self.user, None, "WWC", "Test WWC", "test", {"fake_key": "fake_value"}
         )
 
     def test_channel_retrieve_returned_fields(self):
         response = self.request_detail(uuid=str(self.channel_obj.uuid)).json()
 
         self.assertEqual(response.get("name"), self.channel_obj.name)
         self.assertEqual(response.get("address"), self.channel_obj.address)
@@ -212,24 +210,24 @@
 
 class ListChannelTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.admin = User.objects.create_user(
             username="testuseradmin", password="123", email="test@weni.ai", is_superuser=True
         )
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
-        self.projects = [
-            Project.objects.create(
-                name=f"Org {project}", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
+        self.orgs = [
+            Org.objects.create(
+                name=f"Org {org}", timezone="America/Sao_Paulo", created_by=self.user, modified_by=self.user
             )
-            for project in range(2)
+            for org in range(2)
         ]
 
         for channel in range(6):
             Channel.create(
-                self.projects[0] if channel % 2 == 0 else self.projects[1],
+                self.orgs[0] if channel % 2 == 0 else self.orgs[1],
                 self.user,
                 None,
                 "WWC" if channel % 2 == 0 else "VK",
                 f"Test {channel}",
                 "test",
                 {},
             )
@@ -241,149 +239,147 @@
         self.assertEqual(len(response), 7)
 
     def test_list_channels_filtered_by_type(self):
         response = self.request_get(channel_type="WWC").json()
         self.assertEqual(len(response), 3)
 
     def test_list_channels_filtered_by_org_uuid(self):
-        org_uuid = str(self.projects[0].project_uuid)
-
+        org_uuid = str(self.orgs[0].uuid)
         response = self.request_get(org=org_uuid).json()
-
         self.assertEqual(len(response), 3)
 
         channel = Channel.objects.get(uuid=response[0].get("uuid"))
-
-        self.assertEqual(channel.org, self.projects[0].org)
+        self.assertEqual(channel.org, self.orgs[0])
 
     def get_url_namespace(self):
         return "channel-list"
 
 
 class ListChannelAvailableTestCase(TembaTest, TembaRequestMixin):
-    url = "/api/v2/flows-backend/channels/"
-
+    url ='/api/v2/flows-backend/channels/'
+    
     def setUp(self):
         super().setUp()
         content_type = ContentType.objects.get_for_model(User)
         self.user = User.objects.create_user(username="fake@weni.ai", password="123", email="fake@weni.ai")
-        self.admin.user_permissions.create(codename="can_communicate_internally", content_type=content_type)
+        self.admin.user_permissions.create(codename='can_communicate_internally', content_type=content_type)
 
     def test_list_all_channels(self):
         factory = APIRequestFactory()
-        view = AvailableChannels.as_view({"get": "list"})
+        view = AvailableChannels.as_view({'get': 'list'})
         view.permission_classes = []
 
         request = factory.get(self.url)
         force_authenticate(request, user=self.admin)
         response = view(request)
         total_attrs = 0
 
-        channel_types = response.data.get("channel_types")
+        channel_types = response.data.get('channel_types')
         for key in channel_types.keys():
-            attributes = response.data.get("channel_types").get(key)
+            attributes = response.data.get('channel_types').get(key)
             if attributes:
-                if len(attributes) > 0:
+                if len(attributes)>0:
                     total_attrs += 1
 
         # checks if status code is 200 - ok
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         # checks if the amount of #types returned is equivalent to the available response types
-        self.assertEqual(len(TYPES), len(response.data.get("channel_types")))
+        self.assertEqual(len(TYPES), len(response.data.get('channel_types')))
         # checks if response data have existing attributes
         self.assertEqual(total_attrs, len(TYPES))
 
     def test_list_channels_without_authentication(self):
-        """testing without authenticated user"""
+        """ testing without authenticated user """
         factory = APIRequestFactory()
-        view = AvailableChannels.as_view({"get": "list"})
+        view = AvailableChannels.as_view({'get': 'list'})
 
         request = factory.get(self.url)
         response = view(request)
         self.assertEqual(response.status_code, status.HTTP_401_UNAUTHORIZED)
 
     def test_list_channels_without_permission(self):
-        """testing user without permission"""
+        """ testing user without permission """
         factory = APIRequestFactory()
-        view = AvailableChannels.as_view({"get": "list"})
+        view = AvailableChannels.as_view({'get': 'list'})
 
         request = factory.get(self.url)
         force_authenticate(request, user=self.user)
         response = view(request)
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
     def test_retrieve_channel_with_permission(self):
-        """Testing retrieve response is ok"""
+        """ Testing retrieve response is ok """
         have_attribute = False
         have_form = False
         form_ok = True
-
+        
         factory = APIRequestFactory()
         request = factory.get(self.url)
-        view = AvailableChannels.as_view({"get": "retrieve"})
+        view = AvailableChannels.as_view({'get': 'retrieve'})
         view.permission_classes = []
         force_authenticate(request, user=self.admin)
-        response = view(request, "ac")
+        response = view(request, 'ac')
 
-        if response.data.get("attributes"):
+        if response.data.get('attributes'):
             have_attribute = True
 
-        if response.data.get("form"):
+        if response.data.get('form'):
             have_form = True
-            if len(response.data.get("form")) > 0:
-                form = response.data.get("form")
+            if len(response.data.get('form'))>0:
+                form = response.data.get('form')
                 for field in form:
-                    if not field.get("name") or not field.get("type") or not field.get("help_text"):
+                    if not field.get('name') \
+                        or not field.get('type') \
+                            or not field.get('help_text'):
                         form_ok = False
-
+                            
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         self.assertEqual(True, have_attribute)
         if have_form:
             self.assertEqual(True, form_ok)
 
     def test_retrieve_channel_without_permission(self):
-        """testing retrieve without permission"""
+        """ testing retrieve without permission """
         factory = APIRequestFactory()
-        view = AvailableChannels.as_view({"get": "retrieve"})
+        view = AvailableChannels.as_view({'get': 'retrieve'})
 
         request = factory.get(self.url)
         force_authenticate(request, user=self.user)
-        response = view(request, "ac")
+        response = view(request, 'ac')
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
-
+    
     def test_retrieve_channel_without_authentication(self):
-        """testing retrieve without being authenticated"""
+        """ testing retrieve without being authenticated """
         factory = APIRequestFactory()
-        view = AvailableChannels.as_view({"get": "retrieve"})
+        view = AvailableChannels.as_view({'get': 'retrieve'})
 
         request = factory.get(self.url)
-        response = view(request, "ac")
+        response = view(request, 'ac')
         self.assertEqual(response.status_code, status.HTTP_401_UNAUTHORIZED)
 
-    def get_url_namespace(self):
-        return "api.v2.flows_backend.channels-list"
-
-    '''def test_invalid_response_info_form(self):
-        """test missing values"""
-        self.assertEqual(extract_form_info("", "name_field"), None)
+    def test_invalid_response_info_form(self):
+        """ test missing values """
+        self.assertEqual(extract_form_info('', 'name_field'), None)
 
     def test_invalid_response_info_type(self):
-        """test missing values"""
-        self.assertEqual(extract_type_info(""), None)'''
+        """ test missing values """
+        self.assertEqual(extract_type_info(''), None)
+
+    def get_url_namespace(self):
+        return "api.v2.flows_backend.channels-list"
 
 
-'''class FormatFunctionTestCase(TestCase):
+class FormatFunctionTestCase(TestCase):
     types = TYPES
 
     def test_form_with_values(self):
         """ checks if the treatment was done correctly """
         test_form = {
             'widget': to_object(**{'input_type': 'text'}),
-            'help_text': 'test field',
-            'label': 'test_label'
+            'help_text': 'test field'
         }
 
         expect_form = {
             'name': 'test_form01',
             'type': 'text',
             'help_text': 'test field'
         }
@@ -391,25 +387,23 @@
         result = extract_form_info(to_object(**test_form),'test_form01')
         self.assertEqual(result, expect_form)
 
     def test_form_without_name_value(self):
         """ check response without #name attribute """
         test_form = {
             'widget': to_object(**{'input_type': 'text'}),
-            'help_text': 'test field',
-            'label': 'test_label'
+            'help_text': 'test field'
         }
         result = extract_form_info(to_object(**test_form),'')
         self.assertEqual(result, None)
         
     def test_form_without_type_value(self):
         """ check response without #widget attribute """
         test_form = {
-            'help_text': 'test field',
-            'label': 'test_label'
+            'help_text': 'test field'
         }
         result = extract_form_info(to_object(**test_form),'test_form03')
         self.assertEqual(result, None)
 
     def test_type_contains_code_and_name(self):
         """ make sure that all results have code and name """
         have_code_name = True
@@ -428,8 +422,7 @@
             result = extract_type_info(type_in)
             self.assertEqual(type(result), dict)
 
 
 class to_object:
     def __init__(self, **entries):
         return self.__dict__.update(entries)
-'''
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/channel/views.py` & `weni_rp_apps-2.4.0a4/weni/internal/channel/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 from temba.channels.models import Channel
 from temba.channels.types import TYPES
 
 from .serializers import ChannelSerializer, CreateChannelSerializer, ChannelWACSerializer
 
 User = get_user_model()
 
-
 class ChannelEndpoint(viewsets.ModelViewSet, InternalGenericViewSet):
     serializer_class = ChannelSerializer
     lookup_field = "uuid"
 
     def get_queryset(self):
         channel_type = self.request.query_params.get("channel_type")
         org = self.request.query_params.get("org")
+
         queryset = Channel.objects.all()
 
         if channel_type is not None:
             return queryset.filter(channel_type=channel_type)
 
         if org is not None:
-            return queryset.filter(org__project__project_uuid=org)
+            return queryset.filter(org__uuid=org)
 
         return queryset
 
     def retrieve(self, request, uuid=None):
         try:
             channel = Channel.objects.get(uuid=uuid)
         except Channel.DoesNotExist:
@@ -54,15 +54,15 @@
 
         serializer.save()
 
         return JsonResponse(data=serializer.data, status=status.HTTP_200_OK)
 
     def destroy(self, request, uuid=None):
         channel = get_object_or_404(Channel, uuid=uuid)
-        user = get_object_or_404(User, email=request.query_params.get("user"))
+        user = get_object_or_404(User, email=request.data.get("user"))
 
         channel.release(user)
 
         return Response(status=status.HTTP_200_OK)
 
     @action(methods=["POST"], detail=False)
     def create_wac(self, request):
@@ -73,138 +73,140 @@
 
         serializer.save()
 
         return JsonResponse(data=serializer.data, status=status.HTTP_200_OK)
 
 
 class AvailableChannels(viewsets.ViewSet, InternalGenericViewSet):
+
     def list(self, request):
         types_available = TYPES
         channel_types = {}
         for value in types_available:
             if value not in settings.DISABLED_CHANNELS_INTEGRATIONS:
                 fields_types = {}
-                attibutes_type = extract_type_info(types_available[value])
+                attibutes_type =  extract_type_info(types_available[value])
                 if not (attibutes_type):
                     return Response(status=status.HTTP_404_NOT_FOUND)
 
-                fields_types["attributes"] = attibutes_type
+                fields_types['attributes'] = attibutes_type
                 channel_types[value] = fields_types
 
         payload = {
             "channel_types": channel_types,
         }
         return Response(payload)
 
     def retrieve(self, request, pk=None):
         channel_type = None
         fields_form = {}
         code_type =  pk
-        current_form = None
         if code_type:
             channel_type = TYPES.get(code_type.upper(), None)
 
         if channel_type is None:
             return Response(status=status.HTTP_404_NOT_FOUND)
 
         fields_in_form = []
         if channel_type.claim_view:
             if channel_type.claim_view.form_class:
-                current_form = channel_type.claim_view.form_class
-            elif channel_type.claim_view.ClaimForm:
-                current_form = channel_type.claim_view.ClaimForm
-
-            if current_form:
-                form = current_form.base_fields
+                form = channel_type.claim_view.form_class.base_fields
                 for field in form:
                     fields_in_form.append(extract_form_info(form[field], field))
 
                 if not (fields_in_form):
                     return Response(status=status.HTTP_404_NOT_FOUND)
 
-                fields_form["form"] = fields_in_form
+                fields_form['form'] = fields_in_form
 
             fields_types = {}
-            attibutes_type = extract_type_info(channel_type)
+            attibutes_type =  extract_type_info(channel_type)
             if not (attibutes_type):
                 return Response(status=status.HTTP_404_NOT_FOUND)
 
-            fields_types["attributes"] = attibutes_type
+            fields_types['attributes'] = attibutes_type
 
-        payload = {"attributes": fields_types.get("attributes"), "form": fields_form.get("form")}
+        payload = {
+            "attributes": fields_types.get('attributes'),
+            "form": fields_form.get('form')
+        }
 
         return Response(payload)
 
 
 def extract_type_info(_class):
     channel = {}
     type_exclude = ["<class 'function'>"]
-    items_exclude = ["redact_response_keys", "claim_view_kwargs", "extra_links", "redact_request_keys"]
+    items_exclude = ["redact_response_keys", "claim_view_kwargs", 
+                     "extra_links", "redact_request_keys"]
 
     for i in _class.__class__.__dict__.items():
-        if not i[0].startswith("_"):
-            if not inspect.isclass(i[1]) and str(type(i[1])) not in (type_exclude) and i[0] not in items_exclude:
+        if not i[0].startswith('_'):
+            if not inspect.isclass(i[1]) and str(type(i[1])) not in(type_exclude) \
+                and i[0] not in items_exclude:
                 if str(type(i[1])) == "<enum 'Category'>":
-                    channel[i[0]] = {"name": i[1].name if i[1].name else "", "value": i[1].value if i[1].value else ""}
+                    channel[i[0]] = {"name": i[1].name if i[1].name else "",
+                                    "value": i[1].value if i[1].value else ""}
 
                 elif i[0] == "configuration_urls":
                     if i[1]:
                         if i[1][0]:
                             urls_list = []
                             url_dict = {}
                             for url in i[1]:
-                                if url.get("label"):
-                                    url_dict["label"] = str(url.get("label"))
+                                if url.get('label'):
+                                    url_dict['label'] = str(url.get('label'))
 
-                                if i[1][0].get("url"):
-                                    url_dict["url"] = str(url.get("url"))
+                                if i[1][0].get('url'):
+                                    url_dict['url'] = str(url.get('url'))
 
-                                if i[1][0].get("description"):
-                                    url_dict["description"] = str(url.get("description"))
+                                if i[1][0].get('description'):
+                                    url_dict['description'] = str(url.get('description'))
 
                             urls_list.append(url_dict)
                             channel[i[0]] = urls_list
 
                 elif i[0] == "configuration_blurb":
                     channel[i[0]] = str(i[1])
 
                 elif i[0] == "claim_blurb":
                     channel[i[0]] = str(i[1])
 
                 elif (i[0]) == "ivr_protocol":
-                    channel[i[0]] = {"name": i[1].name if i[1].name else "", "value": i[1].value if i[1].value else ""}
+                    channel[i[0]] = {"name": i[1].name if i[1].name else "", 
+                                    "value": i[1].value if i[1].value else ""}
                 else:
-                    channel[i[0]] = i[1]
+                    channel[i[0]] = (i[1])
 
-    if (not (channel.get("code"))) or (not (len(channel)) > 0) or (not (channel.get("name"))):
+    if (not (channel.get('code'))) or (not (len(channel))>0) \
+        or (not (channel.get('name'))):
         return None
 
-    channel["num_fields"] = len(channel)
-    return channel
-
+    channel['num_fields'] = len(channel)
+    return ((channel))
 
 def extract_form_info(_form, name_form):
     detail = {}
-    detail["name"] = name_form if name_form else None
+    detail['name'] = name_form if name_form else None
 
     try:
         detail['type'] = str(_form.widget.input_type)
-    except AttributeError:
-        detail['type'] = str(_form.widget.__class__.__name__).lower()
+    except:
+        detail['type'] = None
 
     if _form.help_text:
-        detail["help_text"] = str(_form.help_text)
+        detail['help_text'] = str(_form.help_text)
     else:
-        detail['help_text'] = ''
+        detail['help_text'] = None
 
-    if detail.get("type") == "select":
-        detail["choices"] = _form.choices
+    if detail.get('type') == 'select':
+        detail['choices'] = _form.choices
 
     if _form.label:
-        detail["label"] = str(_form.label)
+        detail['label'] = str(_form.label)
     else:
-        detail['label'] = ''
+        detail['label'] = None
 
-    if not (detail.get("name")) or not (detail.get("type")):
+    if not (detail.get('name')) or not (detail.get('type')):
         return None
 
-    return detail
+    return detail
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/classifier/serializers.py` & `weni_rp_apps-2.4.0a4/weni/internal/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/classifier/tests.py` & `weni_rp_apps-2.4.0a4/weni/internal/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/classifier/views.py` & `weni_rp_apps-2.4.0a4/weni/internal/classifier/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/clients/authenticators.py` & `weni_rp_apps-2.4.0a4/weni/internal/clients/authenticators.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/clients/connect.py` & `weni_rp_apps-2.4.0a4/weni/internal/clients/connect.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/externals/serializers.py` & `weni_rp_apps-2.4.0a4/weni/internal/externals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/flows/serializers.py` & `weni_rp_apps-2.4.0a4/weni/internal/flows/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/flows/tests.py` & `weni_rp_apps-2.4.0a4/weni/internal/flows/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/flows/views.py` & `weni_rp_apps-2.4.0a4/weni/internal/flows/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/globals/serializers.py` & `weni_rp_apps-2.4.0a4/weni/internal/globals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/globals/tests/test_serializers.py` & `weni_rp_apps-2.4.0a4/weni/internal/globals/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/globals/views.py` & `weni_rp_apps-2.4.0a4/weni/internal/externals/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-from rest_framework import mixins
-from rest_framework import status
+from typing import TYPE_CHECKING
+
+from django.contrib.auth.models import User
+from django.shortcuts import get_object_or_404
+from rest_framework.views import APIView
 from rest_framework.response import Response
-from rest_framework.exceptions import ValidationError
+from rest_framework.renderers import JSONRenderer
+from rest_framework.permissions import IsAuthenticated
+from rest_framework import status
+
+from weni.internal.authenticators import InternalOIDCAuthentication
+from weni.internal.permissions import CanCommunicateInternally
+from weni.internal.externals.serializers import ExternalServicesSerializer
+from temba.externals.models import ExternalService
+
 
-from temba.globals.models import Global
-from temba.orgs.models import Org
-from weni.internal.views import InternalGenericViewSet
-from weni.internal.globals.serializers import GlobalSerializer
-
-
-class GlobalViewSet(
-    mixins.CreateModelMixin,
-    mixins.RetrieveModelMixin,
-    mixins.DestroyModelMixin,
-    mixins.ListModelMixin,
-    InternalGenericViewSet,
-):
-    serializer_class = GlobalSerializer
-    lookup_field = "uuid"
-
-    def get_queryset(self):
-        queryset = Global.objects.filter(is_active=True)
-        org = self.request.query_params.get("org")
-
-        try:
-            org_object = Org.objects.get(uuid=org)
-            queryset = queryset.filter(org=org_object)
-            return queryset
+if TYPE_CHECKING:
+    from rest_framework.request import Request
 
-        except Org.DoesNotExist as error:
-            raise ValidationError(detail={"message": str(error)})
 
+class ExternalServicesAPIView(APIView):
+    authentication_classes = [InternalOIDCAuthentication]
+    permission_classes = [IsAuthenticated, CanCommunicateInternally]
+    pagination_class = None
+    renderer_classes = [JSONRenderer]
+    throttle_classes = []
 
-    def create(self, request, *args, **kwargs):
-        serializer = self.get_serializer(data=request.data, many=True)
+    def post(self, request: "Request") -> Response:
+        serializer = ExternalServicesSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
+        serializer.save()
 
-        self.perform_create(serializer.validated_data)
+        return Response(serializer.data, status=status.HTTP_201_CREATED)
 
-        headers = self.get_success_headers(serializer.data)
+    def delete(self, request, uuid=None):
+        external_service = get_object_or_404(ExternalService, uuid=uuid)
+        user = get_object_or_404(User, email=request.query_params.get("user"))
 
-        return Response(serializer.data, status=status.HTTP_201_CREATED, headers=headers)
+        external_service.release(user)
 
-    def perform_create(self, validated_data_list):
-        self.get_serializer().create_many(validated_data_list)
+        return Response(status=status.HTTP_204_NO_CONTENT)
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/migrations/0001_initial.py` & `weni_rp_apps-2.4.0a4/weni/internal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/orgs/serializers.py` & `weni_rp_apps-2.4.0a4/weni/internal/orgs/serializers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from rest_framework import serializers
 from django.contrib.auth import get_user_model
 
-from weni.internal.models import Project
+from temba.orgs.models import Org
 from weni.grpc.core import serializers as weni_serializers
 
 
 User = get_user_model()
 
 
 class TemplateOrgSerializer(serializers.ModelSerializer):
+
     user_email = serializers.EmailField(write_only=True)
     timezone = serializers.CharField()
 
     class Meta:
-        model = Project
+        model = Org
         fields = ("user_email", "name", "timezone", "uuid")
         read_only_fields = ("uuid",)
 
     def validate(self, attrs):
         attrs = dict(attrs)
         user_email = attrs.get("user_email")
 
@@ -28,72 +29,74 @@
         attrs.pop("user_email")
 
         return super().validate(attrs)
 
     def create(self, validated_data):
         validated_data["plan"] = "infinity"
 
-        project = super().create(validated_data)
-        project.administrators.add(validated_data.get("created_by"))
-        project.initialize(sample_flows=False)
+        org = super().create(validated_data)
+
+        org.administrators.add(validated_data.get("created_by"))
+        org.initialize(sample_flows=False, internal_ticketer=False)
 
-        return project
+        return org
 
 
 class OrgSerializer(serializers.ModelSerializer):
+
     users = serializers.SerializerMethodField()
     timezone = serializers.CharField()
-    uuid = serializers.UUIDField(source="project_uuid")
-    flow_organization = serializers.UUIDField(source="uuid")
 
     def set_user_permission(self, user: dict, permission: str) -> dict:
         user["permission_type"] = permission
         return user
 
-    def get_users(self, project: Project):
+    def get_users(self, org: Org):
         values = ["id", "email", "username", "first_name", "last_name"]
 
-        administrators = list(project.administrators.all().values(*values))
-        viewers = list(project.viewers.all().values(*values))
-        editors = list(project.editors.all().values(*values))
-        surveyors = list(project.surveyors.all().values(*values))
+        administrators = list(org.administrators.all().values(*values))
+        viewers = list(org.viewers.all().values(*values))
+        editors = list(org.editors.all().values(*values))
+        surveyors = list(org.surveyors.all().values(*values))
 
         administrators = list(map(lambda user: self.set_user_permission(user, "administrator"), administrators))
         viewers = list(map(lambda user: self.set_user_permission(user, "viewer"), viewers))
         editors = list(map(lambda user: self.set_user_permission(user, "editor"), editors))
         surveyors = list(map(lambda user: self.set_user_permission(user, "surveyor"), surveyors))
 
         users = administrators + viewers + editors + surveyors
 
         return users
 
     class Meta:
-        model = Project
-        fields = ["id", "name", "uuid", "timezone", "date_format", "users", "flow_organization"]
+        model = Org
+        fields = ["id", "name", "uuid", "timezone", "date_format", "users"]
 
 
 class OrgCreateSerializer(serializers.ModelSerializer):
+
     user_email = serializers.EmailField()
 
     class Meta:
-        model = Project
-        fields = ["name", "timezone", "user_email", "uuid"]
+        model = Org
+        fields = ["name", "timezone", "user_email"]
 
 
 class OrgUpdateSerializer(serializers.ModelSerializer):
-    project_uuid = serializers.CharField(read_only=True)
+
+    uuid = serializers.CharField(read_only=True)
     modified_by = weni_serializers.UserEmailRelatedField(required=False, write_only=True)
     timezone = serializers.CharField(required=False)
     name = serializers.CharField(required=False)
     plan_end = serializers.DateTimeField(required=False)
 
     class Meta:
-        model = Project
+        model = Org
         fields = [
-            "project_uuid",
+            "uuid",
             "modified_by",
             "name",
             "timezone",
             "date_format",
             "plan",
             "plan_end",
             "brand",
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/orgs/tests.py` & `weni_rp_apps-2.4.0a4/weni/internal/orgs/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 import random
 from unittest.mock import patch
 
 from django.contrib.auth.models import Group
 from django.contrib.auth.models import User
+from django.conf import settings
 from django.utils.http import urlencode
 from django.urls import reverse
 
-from weni.internal.models import Project
+from temba.orgs.models import Org
+
 from temba.api.models import APIToken
 from temba.tests import TembaTest
-from weni.internal.orgs.views import OrgViewSet
-
-
-view_class = OrgViewSet
-view_class.permission_classes = []
 
 
 class TembaRequestMixin(ABC):
     def reverse(self, viewname, kwargs=None, query_params=None):
         url = reverse(viewname, kwargs=kwargs)
 
         if query_params:
@@ -32,71 +29,72 @@
         url = self.reverse(self.get_url_namespace(), query_params=query_params)
         url = url.replace("channel", "channel.json")
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.get(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     def request_detail(self, uuid):
-        url = self.reverse(self.get_url_namespace(), kwargs={"project_uuid": uuid})
+        url = self.reverse(self.get_url_namespace(), kwargs={"uuid": uuid})
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.get(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     def request_post(self, data):
         url = reverse(self.get_url_namespace())
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.post(
             url, HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
         )
 
     def request_delete(self, uuid, **query_params):
-        url = self.reverse(self.get_url_namespace(), kwargs={"project_uuid": uuid}, query_params=query_params)
+        url = self.reverse(self.get_url_namespace(), kwargs={"uuid": uuid}, query_params=query_params)
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.delete(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     def request_patch(self, uuid, data):
-        url = self.reverse(self.get_url_namespace(), kwargs={"project_uuid": uuid})
+        url = self.reverse(self.get_url_namespace(), kwargs={"uuid": uuid})
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.patch(
             url, HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
         )
 
     @abstractmethod
     def get_url_namespace(self):
         ...
 
 
 class OrgListTest(TembaTest, TembaRequestMixin):
+
     WRONG_ID = -1
     WRONG_UUID = "31313-dasda-dasdasd-23123"
     WRONG_EMAIL = "wrong@email.com"
 
     def setUp(self):
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         User.objects.create_user(username="weniuser", password="123", email="wene@user.com")
 
         user = User.objects.get(username="testuser")
 
-        Project.objects.create(name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user)
-        Project.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
-        Project.objects.create(name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user)
 
         super().setUp()
 
     def test_list_orgs(self):
         response = self.request_get()
         self.assertEqual(response.status_code, 400)
 
         response = self.request_get(user_email="wrong@email.com")
         self.assertEqual(response.status_code, 404)
 
-        orgs = Project.objects.all()
+        orgs = Org.objects.all()
         user = User.objects.get(username="testuser")
 
         weni_org = orgs.get(name="Weni")
         temba_org = orgs.get(name="Tembinha")
         test_org = orgs.get(name="Test")
 
         weni_org.administrators.add(user)
@@ -117,74 +115,71 @@
         self.assertEquals(len(response), 2)
 
         test_org.editors.add(user)
         response = self.request_get(user_email=user.email).json()
         self.assertEquals(len(response), 3)
 
     def test_list_users_on_org(self):
-        org = Project.objects.get(name="Tembinha")
+        org = Org.objects.get(name="Tembinha")
 
         testuser = User.objects.get(username="testuser")
         weniuser = User.objects.get(username="weniuser")
 
         org.administrators.add(testuser)
         response = self.request_get(user_email=testuser.email).json()
-
         self.assertEquals(len(response[0].get("users")), 1)
 
         org.administrators.add(weniuser)
         response = self.request_get(user_email=testuser.email).json()
         self.assertEquals(len(response[0].get("users")), 2)
 
     def get_url_namespace(self):
         return "orgs-list"
 
 
 class OrgCreateTest(TembaTest, TembaRequestMixin):
+
     WRONG_ID = -1
     WRONG_UUID = "31313-dasda-dasdasd-23123"
     WRONG_EMAIL = "wrong@email.com"
 
     def setUp(self):
+
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         User.objects.create_user(username="weniuser", password="123", email="wene@user.com")
 
         user = User.objects.get(username="testuser")
 
-        Project.objects.create(
-            name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user, plan="infinity"
-        )
-        Project.objects.create(
-            name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user, plan="infinity"
-        )
-        Project.objects.create(
-            name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user, plan="infinity"
-        )
+        Org.objects.create(name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user)
 
         super().setUp()
 
     @patch("temba.orgs.models.Org.create_sample_flows")
     def test_create_org(self, mock):
+
         org_name = "TestCreateOrg"
-        user = User.objects.get(username="weniuser")
+        user = User.objects.first()
+
         response = self.request_post(data=dict(name=org_name, timezone="Wrong/Zone", user_email=user.email)).json()
 
         self.assertEqual(response.get("timezone")[0], '"Wrong/Zone" is not a valid choice.')
 
         response = self.request_post(
             data=dict(name=org_name, timezone="Africa/Kigali", user_email="newemail@email.com")
         ).json()
 
         newuser_qs = User.objects.filter(email="newemail@email.com")
 
         self.assertTrue(newuser_qs.exists())
 
         newuser = newuser_qs.first()
 
-        orgs = Project.objects.filter(name=org_name)
+        orgs = Org.objects.filter(name=org_name)
         org = orgs.first()
 
         self.assertEquals(orgs.count(), 1)
 
         created_by = org.created_by
         modified_by = org.modified_by
         administrators = org.administrators.all()
@@ -204,32 +199,34 @@
         self.assertEqual(User.objects.filter(email="newemail@email.com").count(), 1)
 
     def get_url_namespace(self):
         return "orgs-list"
 
 
 class OrgRetrieveTest(TembaTest, TembaRequestMixin):
+
     WRONG_ID = -1
     WRONG_UUID = "31313-dasda-dasdasd-23123"
     WRONG_EMAIL = "wrong@email.com"
 
     def setUp(self):
+
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         User.objects.create_user(username="weniuser", password="123", email="wene@user.com")
 
         user = User.objects.get(username="testuser")
 
-        Project.objects.create(name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user)
-        Project.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
-        Project.objects.create(name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user)
 
         super().setUp()
 
     def test_retrieve_org(self):
-        org = Project.objects.first()
+        org = Org.objects.last()
         user = User.objects.last()
 
         permission_types = ("administrator", "viewer", "editor", "surveyor")
 
         random_permission = random.choice(permission_types)
 
         if random_permission == "administrator":
@@ -237,18 +234,19 @@
         if random_permission == "viewer":
             org.viewers.add(user)
         if random_permission == "editor":
             org.editors.add(user)
         if random_permission == "surveyor":
             org.surveyors.add(user)
 
-        org_uuid = str(org.project_uuid)
+        org_uuid = str(org.uuid)
         org_timezone = str(org.timezone)
 
         response = self.request_detail(uuid=org_uuid).json()
+
         response_user = response.get("users")[-1]
 
         self.assertEqual(response.get("id"), org.id)
         self.assertEqual(response.get("name"), org.name)
         self.assertEqual(response.get("uuid"), org_uuid)
         self.assertEqual(org_timezone, response.get("timezone"))
         self.assertEqual(org.date_format, response.get("date_format"))
@@ -260,123 +258,127 @@
         self.assertEqual(response_user.get("permission_type"), random_permission)
 
     def get_url_namespace(self):
         return "orgs-detail"
 
 
 class OrgDestroyTest(TembaTest, TembaRequestMixin):
+
     WRONG_ID = -1
     WRONG_UUID = "31313-dasda-dasdasd-23123"
     WRONG_EMAIL = "wrong@email.com"
 
     def setUp(self):
+
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         User.objects.create_user(username="weniuser", password="123", email="wene@user.com")
 
         user = User.objects.get(username="testuser")
 
-        Project.objects.create(name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user)
-        Project.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
-        Project.objects.create(name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user)
 
         super().setUp()
 
     def test_destroy_org(self):
-        project = Project.objects.last()
-        is_active = project.is_active
-        modified_by = project.modified_by
+        org = Org.objects.last()
+        is_active = org.is_active
+        modified_by = org.modified_by
 
         weniuser = User.objects.get(username="weniuser")
 
-        self.request_delete(uuid=str(project.uuid), user_email=weniuser.email)
+        self.request_delete(uuid=str(org.uuid), user_email=weniuser.email)
 
-        destroyed_org = Project.objects.get(id=project.id)
+        destroyed_org = Org.objects.get(id=org.id)
 
         self.assertFalse(destroyed_org.is_active)
         self.assertNotEquals(is_active, destroyed_org.is_active)
         self.assertEquals(weniuser, destroyed_org.modified_by)
         self.assertNotEquals(modified_by, destroyed_org.modified_by)
 
     def get_url_namespace(self):
         return "orgs-detail"
 
 
 class OrgUpdateTest(TembaTest, TembaRequestMixin):
+
     WRONG_ID = -1
     WRONG_UUID = "31313-dasda-dasdasd-23123"
     WRONG_EMAIL = "wrong@email.com"
 
     def setUp(self):
+
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
         User.objects.create_user(username="weniuser", password="123", email="wene@user.com")
 
         user = User.objects.get(username="testuser")
 
-        Project.objects.create(name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user)
-        Project.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
-        Project.objects.create(name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Tembinha", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Weni", timezone="Africa/Kigali", created_by=user, modified_by=user)
+        Org.objects.create(name="Test", timezone="Africa/Kigali", created_by=user, modified_by=user)
 
         super().setUp()
 
     def test_update_org(self):
-        project = Project.objects.first()
+        org = Org.objects.first()
 
-        permission_error_message = f"User: {self.user.id} has no permission to update Org: {project.project_uuid}"
+        permission_error_message = f"User: {self.user.id} has no permission to update Org: {org.uuid}"
 
-        response = self.request_patch(uuid=str(project.project_uuid), data=dict(modified_by=self.user.email)).json()
+        response = self.request_patch(uuid=str(org.uuid), data=dict(modified_by=self.user.email)).json()
 
         self.assertEqual(response[0], permission_error_message)
 
         self.user.is_superuser = True
         self.user.save()
 
-        project.administrators.add(self.user)
+        org.administrators.add(self.user)
 
         update_fields = {
             "name": "NewOrgName",
             "timezone": "America/Maceio",
             "date_format": "M",
-            "plan": "infinity",
+            "plan": settings.INFINITY_PLAN,
             "plan_end": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
             "brand": "push.ia",
             "is_anon": True,
             "is_multi_user": True,
             "is_multi_org": True,
             "is_suspended": True,
             "modified_by": self.user.email,
         }
 
-        response = self.request_patch(uuid=str(project.project_uuid), data=update_fields).json()
+        response = self.request_patch(uuid=str(org.uuid), data=update_fields).json()
 
-        updated_org = Project.objects.get(pk=project.pk)
+        updated_org = Org.objects.get(pk=org.pk)
 
         self.assertEquals(update_fields.get("name"), updated_org.name)
-        self.assertNotEquals(project.name, updated_org.name)
+        self.assertNotEquals(org.name, updated_org.name)
 
         self.assertEquals(update_fields.get("timezone"), str(updated_org.timezone))
-        self.assertNotEquals(project.timezone, updated_org.timezone)
+        self.assertNotEquals(org.timezone, updated_org.timezone)
 
         self.assertEquals(update_fields.get("date_format"), updated_org.date_format)
-        self.assertNotEquals(project.date_format, updated_org.date_format)
+        self.assertNotEquals(org.date_format, updated_org.date_format)
 
-        self.assertEquals(updated_org.plan, "infinity")
-        self.assertNotEquals(project.plan, updated_org.plan)
+        self.assertEquals(updated_org.plan, settings.INFINITY_PLAN)
+        self.assertNotEquals(org.plan, updated_org.plan)
         self.assertFalse(updated_org.uses_topups)
         self.assertEquals(updated_org.plan_end, None)
 
         self.assertEquals(update_fields.get("brand"), updated_org.brand)
-        self.assertNotEquals(project.brand, updated_org.brand)
+        self.assertNotEquals(org.brand, updated_org.brand)
 
         self.assertEquals(update_fields.get("is_anon"), updated_org.is_anon)
-        self.assertNotEquals(project.is_anon, updated_org.is_anon)
+        self.assertNotEquals(org.is_anon, updated_org.is_anon)
 
         self.assertEquals(update_fields.get("is_multi_user"), updated_org.is_multi_user)
-        self.assertNotEquals(project.is_multi_user, updated_org.is_multi_user)
+        self.assertNotEquals(org.is_multi_user, updated_org.is_multi_user)
 
         self.assertEquals(update_fields.get("is_multi_org"), updated_org.is_multi_org)
-        self.assertNotEquals(project.is_multi_org, updated_org.is_multi_org)
+        self.assertNotEquals(org.is_multi_org, updated_org.is_multi_org)
 
         self.assertEquals(update_fields.get("is_suspended"), updated_org.is_suspended)
-        self.assertNotEquals(project.is_suspended, updated_org.is_suspended)
+        self.assertNotEquals(org.is_suspended, updated_org.is_suspended)
 
     def get_url_namespace(self):
         return "orgs-detail"
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/orgs/views.py` & `weni_rp_apps-2.4.0a4/weni/internal/orgs/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,118 +12,116 @@
 from weni.internal.orgs.serializers import (
     TemplateOrgSerializer,
     OrgCreateSerializer,
     OrgSerializer,
     OrgUpdateSerializer,
 )
 
-from weni.internal.models import Project
+from temba.orgs.models import Org
 
 
 class TemplateOrgViewSet(CreateModelMixin, InternalGenericViewSet):
     serializer_class = TemplateOrgSerializer
 
 
 class OrgViewSet(viewsets.ModelViewSet, InternalGenericViewSet):
-    queryset = Project.objects
-    lookup_field = "project_uuid"
+    queryset = Org.objects
+    lookup_field = "uuid"
 
     def list(self, request):
         user = self.get_user(request)
-        orgs_ids = self.get_orgs(user).values_list("id", flat=True)
-        projects = Project.objects.filter(id__in=orgs_ids)
-        serializer = OrgSerializer(projects, many=True)
+        orgs = self.get_orgs(user)
+
+        serializer = OrgSerializer(orgs, many=True)
 
         return Response(serializer.data)
 
     def create(self, request):
         serializer = OrgCreateSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         user, created = User.objects.get_or_create(
             email=request.data.get("user_email"), defaults={"username": request.data.get("user_email")}
         )
 
-        project = Project.objects.create(
+        org = Org.objects.create(
             name=request.data.get("name"),
             timezone=request.data.get("timezone"),
             created_by=user,
             modified_by=user,
             plan="infinity",
-            project_uuid=request.data.get("uuid")
-
         )
 
-        project.administrators.add(user)
-        project.initialize()
+        org.administrators.add(user)
+        org.initialize()
 
-        org_serializer = OrgSerializer(project)
+        org_serializer = OrgSerializer(org)
 
         return Response(org_serializer.data)
 
-    def retrieve(self, request, project_uuid=None):
-        project = get_object_or_404(Project, project_uuid=project_uuid)
-        serializer = OrgSerializer(project)
+    def retrieve(self, request, uuid=None):
+        org = get_object_or_404(Org, uuid=uuid)
+        serializer = OrgSerializer(org)
 
         return Response(serializer.data)
 
-    def destroy(self, request, project_uuid=None):
-        project = get_object_or_404(Project, uuid=project_uuid)
+    def destroy(self, request, uuid=None):
+        org = get_object_or_404(Org, uuid=uuid)
         user = get_object_or_404(User, email=request.query_params.get("user_email"))
 
-        self.pre_destroy(project, user)
-        project.release(user)
+        self.pre_destroy(org, user)
+        org.release(user)
 
         return Response(status=status.HTTP_204_NO_CONTENT)
 
-    def partial_update(self, request, project_uuid=None):
-        project = get_object_or_404(Project, project_uuid=project_uuid)
+    def partial_update(self, request, uuid=None):
+        org = get_object_or_404(Org, uuid=uuid)
 
-        serializer = OrgUpdateSerializer(project, data=request.data)
+        serializer = OrgUpdateSerializer(org, data=request.data)
         serializer.is_valid(raise_exception=True)
 
         modified_by = serializer.validated_data.get("modified_by", None)
         plan = serializer.validated_data.get("plan", None)
 
-        if modified_by and not self._user_has_permisson(modified_by, project) and not modified_by.is_superuser:
+        if modified_by and not self._user_has_permisson(modified_by, org) and not modified_by.is_superuser:
             raise exceptions.ValidationError(
-                f"User: {modified_by.pk} has no permission to update Org: {project.project_uuid}",
+                f"User: {modified_by.pk} has no permission to update Org: {org.uuid}",
             )
 
         if plan is not None and plan == settings.INFINITY_PLAN:
-            project.uses_topups = False
-            project.plan_end = None
+            org.uses_topups = False
+            org.plan_end = None
 
             serializer.save(plan_end=None)
             return Response(serializer.data)
 
         serializer.save()
         return Response(serializer.data)
 
-    def pre_destroy(self, org: Project, user: User):
+    def pre_destroy(self, org: Org, user: User):
         if user.id and user.id > 0 and hasattr(org, "modified_by_id"):
             org.modified_by = user
 
             # Interim fix, remove after implementation in the model.
             org.save(update_fields=["modified_by"])
 
     def get_user(self, request):
         user_email = request.query_params.get("user_email")
 
         if not user_email:
             raise exceptions.ValidationError("Email cannot be null")
 
         return get_object_or_404(User, email=request.query_params.get("user_email"))
 
-    def _user_has_permisson(self, user: User, project: Project) -> bool:
+    def _user_has_permisson(self, user: User, org: Org) -> bool:
         return (
-            user.org_admins.filter(pk=project.pk)
-            or user.org_viewers.filter(pk=project.pk)
-            or user.org_editors.filter(pk=project.pk)
-            or user.org_surveyors.filter(pk=project.pk)
+            user.org_admins.filter(pk=org.pk)
+            or user.org_viewers.filter(pk=org.pk)
+            or user.org_editors.filter(pk=org.pk)
+            or user.org_surveyors.filter(pk=org.pk)
         )
 
     def get_orgs(self, user: User):
         admins = user.org_admins.filter(is_active=True)
         viewers = user.org_viewers.filter(is_active=True)
         editors = user.org_editors.filter(is_active=True)
         surveyors = user.org_surveyors.filter(is_active=True)
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/statistic/tests.py` & `weni_rp_apps-2.4.0a4/weni/internal/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/statistic/views.py` & `weni_rp_apps-2.4.0a4/weni/internal/statistic/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/tests/test_models.py` & `weni_rp_apps-2.4.0a4/weni/internal/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/tickets/serializers.py` & `weni_rp_apps-2.4.0a4/weni/internal/tickets/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/tickets/tests/test_views.py` & `weni_rp_apps-2.4.0a4/weni/internal/tickets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/tickets/views.py` & `weni_rp_apps-2.4.0a4/weni/internal/tickets/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,13 +45,7 @@
 
     def update(self, request, *args, **kwargs):
         partial = kwargs.get("partial", False)
         if not partial:
             self.http_method_not_allowed(request, *args, **kwargs)
 
         return super().update(request, *args, **kwargs)
-
-    def perform_destroy(self, instance):
-        ticketer = instance.ticketer
-        # Release Ticketer
-        ticketer.release(self.request.user)
-        instance.delete()
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/urls.py` & `weni_rp_apps-2.4.0a4/weni/internal/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/users/serializers.py` & `weni_rp_apps-2.4.0a4/weni/internal/users/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from django.contrib.auth import get_user_model
 
 from rest_framework import serializers
 
-from weni.serializers import fields as weni_serializers
+from weni.grpc.core import serializers as weni_serializers
 
 User = get_user_model()
 
 
 class UserAPITokenSerializer(serializers.Serializer):
     user = weni_serializers.UserEmailRelatedField(required=True)
-    project = weni_serializers.ProjectUUIDRelatedField(required=True)
+    org = weni_serializers.OrgUUIDRelatedField(required=True)
 
 
 class UserPermissionSerializer(serializers.Serializer):
     administrator = serializers.BooleanField(default=False)
     viewer = serializers.BooleanField(default=False)
     editor = serializers.BooleanField(default=False)
     surveyor = serializers.BooleanField(default=False)
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/users/tests.py` & `weni_rp_apps-2.4.0a4/weni/internal/users/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,14 @@
 from django.urls import reverse
 from django.utils.http import urlencode
 
 from temba.api.models import APIToken
 
 from temba.tests import TembaTest
 from temba.orgs.models import Org
-from weni.internal.models import Project
-from weni.internal.users.views import UserEndpoint, UserPermissionEndpoint, UserViewSet
-
-view_set = UserViewSet
-view_set.permission_classes = []
-
-view_permissions = UserPermissionEndpoint
-view_permissions.permission_classes = []
-
-view_endpoint = UserEndpoint
-view_endpoint.permission_classes = []
 
 
 class TembaRequestMixin(ABC):
     def reverse(self, viewname, kwargs=None, query_params=None):
         url = reverse(viewname, kwargs=kwargs)
 
         if query_params:
@@ -59,15 +48,15 @@
 
         return self.client.post(
             url, HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
         )
 
     def request_delete(self, data, **kwargs):
         url = self.reverse(self.get_url_namespace(), query_params=kwargs)
-        token = APIToken.get_or_create(self.project, self.admin, Group.objects.get(name="Administrators"))
+        token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.delete(
             f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}", data=json.dumps(data), content_type="application/json"
         )
 
     @abstractmethod
     def get_url_namespace(self):
@@ -75,95 +64,91 @@
 
 
 class UserPermissionUpdateDestroyTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.admin = User.objects.create_user(
             username="testuser", password="123", email="test@weni.ai", is_superuser=True
         )
-
-        self.project = Project.objects.create(
-            name="Test", timezone="Africa/Kigali", created_by=self.admin, modified_by=self.admin
-        )
         super().setUp()
 
     def test_user_permission_destroy(self):
-        project = Project.objects.first()
+        org = Org.objects.first()
         user = User.objects.first()
 
         destroy_wrong_permission = self.request_delete(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="adm")
+            data=dict(org_uuid=str(org.uuid), user_email=user.email, permission="adm")
         )
         self.assertEqual(destroy_wrong_permission.status_code, 400)
         self.assertEqual(destroy_wrong_permission.json()[0], "adm is not a valid permission!")
 
-        self.request_patch(data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="viewer"))
-        user_permissions = self._get_user_permissions(project=project, user=user)
+        self.request_patch(data=dict(org_uuid=str(org.uuid), user_email=user.email, permission="viewer"))
+        user_permissions = self._get_user_permissions(org=org, user=user)
 
-        self.request_delete(data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="viewer"))
-        user_permissions_removed = self._get_user_permissions(project=project, user=user)
+        self.request_delete(data=dict(org_uuid=str(org.uuid), user_email=user.email, permission="viewer"))
+        user_permissions_removed = self._get_user_permissions(org=org, user=user)
 
         self.assertFalse(user_permissions_removed.get("viewer", False))
         self.assertNotEquals(user_permissions, user_permissions_removed)
 
     def test_user_permission_update(self):
-        project = Project.objects.first()
+        org = Org.objects.first()
         user = User.objects.first()
 
         update_wrong_permission_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="adm")
+            data=dict(org_uuid=str(org.uuid), user_email=user.email, permission="adm")
         )
         self.assertEqual(update_wrong_permission_response.status_code, 400)
         self.assertEqual(update_wrong_permission_response.json()[0], "adm is not a valid permission!")
 
         update_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="administrator")
+            data=dict(org_uuid=str(org.uuid), user_email=user.email, permission="administrator")
         ).json()
-        user_permissions = self._get_user_permissions(project, user)
+        user_permissions = self._get_user_permissions(org, user)
 
         self.assertTrue(user_permissions.get("administrator"))
         self.assertTrue(self._permission_is_unique_true(update_response, "administrator"))
 
         update_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="viewer")
+            data=dict(org_uuid=str(org.uuid), user_email=user.email, permission="viewer")
         ).json()
-        user_permissions = self._get_user_permissions(project, user)
+        user_permissions = self._get_user_permissions(org, user)
 
         self.assertTrue(user_permissions.get("viewer"))
         self.assertTrue(self._permission_is_unique_true(update_response, "viewer"))
 
         update_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="editor")
+            data=dict(org_uuid=str(org.uuid), user_email=user.email, permission="editor")
         ).json()
-        user_permissions = self._get_user_permissions(project, user)
+        user_permissions = self._get_user_permissions(org, user)
 
         self.assertTrue(user_permissions.get("editor"))
         self.assertTrue(self._permission_is_unique_true(update_response, "editor"))
 
         update_response = self.request_patch(
-            data=dict(org_uuid=str(project.project_uuid), user_email=user.email, permission="surveyor")
+            data=dict(org_uuid=str(org.uuid), user_email=user.email, permission="surveyor")
         ).json()
-        user_permissions = self._get_user_permissions(project, user)
+        user_permissions = self._get_user_permissions(org, user)
 
         self.assertTrue(user_permissions.get("surveyor"))
         self.assertTrue(self._permission_is_unique_true(update_response, "surveyor"))
 
-    def _get_permissions(self, project: Project) -> dict:
+    def _get_permissions(self, org: Org) -> dict:
         return {
-            "administrator": project.administrators,
-            "viewer": project.viewers,
-            "editor": project.editors,
-            "surveyor": project.surveyors,
+            "administrator": org.administrators,
+            "viewer": org.viewers,
+            "editor": org.editors,
+            "surveyor": org.surveyors,
         }
 
-    def _get_user_permissions(self, project: Project, user: User) -> dict:
+    def _get_user_permissions(self, org: Org, user: User) -> dict:
         permissions = {}
-        project_permissions = self._get_permissions(project)
+        org_permissions = self._get_permissions(org)
 
-        for perm_name, project_field in project_permissions.items():
-            if project_field.filter(pk=user.id).exists():
+        for perm_name, org_field in org_permissions.items():
+            if org_field.filter(pk=user.id).exists():
                 permissions[perm_name] = True
 
         return permissions
 
     def _permission_is_unique_true(self, response, permission: str) -> bool:
         permissions = {
             "administrator": response.get("administrator"),
@@ -180,62 +165,59 @@
 
 
 class UserPermissionRetrieveTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         self.admin = User.objects.create_user(
             username="testuser", password="123", email="test@weni.ai", is_superuser=True
         )
-        self.project = Project.objects.create(
-            name="Test", timezone="Africa/Kigali", created_by=self.admin, modified_by=self.admin
-        )
         super().setUp()
 
     def test_user_permission_retrieve(self):
-        project = Project.objects.first()
+        org = Org.objects.first()
         user = User.objects.first()
 
-        response_wrong_project = self.request_detail(
+        response_wrong_org = self.request_detail(
             org_uuid="f7e70145-6d17-4384-a1f2-d6981397866a", user_email="wrong@weni.ai"
         )
 
-        self.assertEqual(response_wrong_project.status_code, 404)
-        self.assertEqual(response_wrong_project.json().get("detail"), "Not found.")
+        self.assertEqual(response_wrong_org.status_code, 404)
+        self.assertEqual(response_wrong_org.json().get("detail"), "Not found.")
 
-        project.administrators.add(user)
+        org.administrators.add(user)
 
-        response_wrong_user = self.request_detail(org_uuid=project.project_uuid, user_email=0)
+        response_wrong_user = self.request_detail(org_uuid=org.uuid, user_email=0)
 
         self.assertEqual(response_wrong_user.status_code, 404)
         self.assertEqual(response_wrong_user.json().get("detail"), "Not found.")
 
-        response = self.request_detail(org_uuid=project.project_uuid, user_email=user.email).json()
+        response = self.request_detail(org_uuid=org.uuid, user_email=user.email).json()
 
         self.assertTrue(response.get("administrator"))
         self.assertTrue(self.permission_is_unique_true(response, "administrator"))
 
-        project.administrators.remove(user)
-        project.viewers.add(user)
+        org.administrators.remove(user)
+        org.viewers.add(user)
 
-        response = self.request_detail(org_uuid=project.project_uuid, user_email=user.email).json()
+        response = self.request_detail(org_uuid=org.uuid, user_email=user.email).json()
 
         self.assertTrue(response.get("viewer"))
         self.assertTrue(self.permission_is_unique_true(response, "viewer"))
 
-        project.viewers.remove(user)
-        project.editors.add(user)
+        org.viewers.remove(user)
+        org.editors.add(user)
 
-        response = self.request_detail(org_uuid=project.project_uuid, user_email=user.email).json()
+        response = self.request_detail(org_uuid=org.uuid, user_email=user.email).json()
 
         self.assertTrue(response.get("editor"))
         self.assertTrue(self.permission_is_unique_true(response, "editor"))
 
-        project.editors.remove(user)
-        project.surveyors.add(user)
+        org.editors.remove(user)
+        org.surveyors.add(user)
 
-        response = self.request_detail(org_uuid=project.project_uuid, user_email=user.email).json()
+        response = self.request_detail(org_uuid=org.uuid, user_email=user.email).json()
 
         self.assertTrue(response.get("surveyor"))
         self.assertTrue(self.permission_is_unique_true(response, "surveyor"))
 
     def permission_is_unique_true(self, response, permission: str) -> bool:
         permissions = {
             "administrator": response.get("administrator"),
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/users/urls.py` & `weni_rp_apps-2.4.0a4/weni/internal/users/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/users/views.py` & `weni_rp_apps-2.4.0a4/weni/internal/users/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,154 +8,136 @@
 from rest_framework.decorators import action
 from rest_framework.response import Response
 from rest_framework import exceptions
 from rest_framework import mixins
 from rest_framework.exceptions import ValidationError
 
 from weni.internal.views import InternalGenericViewSet
-from weni.internal.users.serializers import (
-    UserAPITokenSerializer,
-    UserSerializer,
-    UserPermissionSerializer,
-)
+from weni.internal.users.serializers import UserAPITokenSerializer, UserSerializer, UserPermissionSerializer
 from temba.api.models import APIToken
 from temba.orgs.models import Org
-from weni.internal.models import Project
 
 
 if TYPE_CHECKING:
     from rest_framework.request import Request
 
 User = get_user_model()
 
 
 class UserViewSet(InternalGenericViewSet):
-    @action(
-        detail=False,
-        methods=["GET"],
-        url_path="api-token",
-        serializer_class=UserAPITokenSerializer,
-    )
+    @action(detail=False, methods=["GET"], url_path="api-token", serializer_class=UserAPITokenSerializer)
     def api_token(self, request: "Request", **kwargs):
+
         serializer = self.get_serializer(data=request.query_params)
         serializer.is_valid(raise_exception=True)
 
         try:
             api_token = APIToken.objects.get(**serializer.validated_data)
         except APIToken.DoesNotExist:
             raise exceptions.PermissionDenied()
 
-        return Response(
-            dict(user=api_token.user.email, project=api_token.project.project_uuid, api_token=api_token.key)
-        )
+        return Response(dict(user=api_token.user.email, org=api_token.org.uuid, api_token=api_token.key))
 
 
 class UserPermissionEndpoint(InternalGenericViewSet):
     serializer_class = UserPermissionSerializer
 
     def retrieve(self, request):
-        project = get_object_or_404(Project, project_uuid=request.query_params.get("org_uuid"))
-        user = get_object_or_404(
-            User, email=request.query_params.get("user_email"), is_active=request.query_params.get("is_active", True)
-        )
+        org = get_object_or_404(Org, uuid=request.query_params.get("org_uuid"))
+        user = get_object_or_404(User, email=request.query_params.get("user_email"), is_active=request.query_params.get("is_active", True))
 
-        permissions = self._get_user_permissions(project, user)
+        permissions = self._get_user_permissions(org, user)
         serializer = self.get_serializer(permissions)
 
         return Response(serializer.data)
 
     def partial_update(self, request):
-        project = get_object_or_404(Project, project_uuid=request.data.get("org_uuid"))
-        user = get_object_or_404(
-            User, email=request.data.get("user_email"), is_active=request.query_params.get("is_active", True)
-        )
+        org = get_object_or_404(Org, uuid=request.data.get("org_uuid"))
+        user = get_object_or_404(User, email=request.data.get("user_email"), is_active=request.query_params.get("is_active", True))
 
-        self._validate_permission(project, request.data.get("permission", ""))
-        self._set_user_permission(project, user, request.data.get("permission", ""))
+        self._validate_permission(org, request.data.get("permission", ""))
+        self._set_user_permission(org, user, request.data.get("permission", ""))
 
-        permissions = self._get_user_permissions(project, user)
+        permissions = self._get_user_permissions(org, user)
         serializer = self.get_serializer(permissions)
 
         return Response(serializer.data)
 
     def destroy(self, request):
-        project = get_object_or_404(Project, project_uuid=request.data.get("org_uuid"))
-        user = get_object_or_404(
-            User, email=request.data.get("user_email"), is_active=request.query_params.get("is_active", True)
-        )
+        org = get_object_or_404(Org, uuid=request.data.get("org_uuid"))
+        user = get_object_or_404(User, email=request.data.get("user_email"), is_active=request.query_params.get("is_active", True))
 
-        self._validate_permission(project, request.data.get("permission", ""))
-        self._remove_user_permission(project, user, request.data.get("permission", ""))
+        self._validate_permission(org, request.data.get("permission", ""))
+        self._remove_user_permission(org, user, request.data.get("permission", ""))
 
-        permissions = self._get_user_permissions(project, user)
+        permissions = self._get_user_permissions(org, user)
         serializer = self.get_serializer(permissions)
 
         return Response(serializer.data)
 
-    def _remove_user_permission(self, project: Project, user: User, permission: str):
-        permissions = self._get_permissions(project)
+    def _remove_user_permission(self, org: Org, user: User, permission: str):
+        permissions = self._get_permissions(org)
         permissions.get(permission).remove(user)
 
-    def _set_user_permission(self, project: Project, user: User, permission: str):
-        permissions = self._get_permissions(project)
+    def _set_user_permission(self, org: Org, user: User, permission: str):
+        permissions = self._get_permissions(org)
 
-        for perm_name, project_field in permissions.items():
+        for perm_name, org_field in permissions.items():
             if not perm_name == permission:
-                project_field.remove(user)
+                org_field.remove(user)
 
         permissions.get(permission).add(user)
 
-    def _validate_permission(self, project: Project, permission: str):
-        permissions_keys = self._get_permissions(project).keys()
+    def _validate_permission(self, org: Org, permission: str):
+        permissions_keys = self._get_permissions(org).keys()
 
         if permission not in permissions_keys:
             raise ValidationError(detail=f"{permission} is not a valid permission!")
 
-    def _get_permissions(self, project: Project) -> dict:
+    def _get_permissions(self, org: Org) -> dict:
         return {
-            "administrator": project.administrators,
-            "viewer": project.viewers,
-            "editor": project.editors,
-            "surveyor": project.surveyors,
+            "administrator": org.administrators,
+            "viewer": org.viewers,
+            "editor": org.editors,
+            "surveyor": org.surveyors,
         }
 
-    def _get_user_permissions(self, project: Project, user: User) -> dict:
+    def _get_user_permissions(self, org: Org, user: User) -> dict:
         permissions = {}
-        project_permissions = self._get_permissions(project)
+        org_permissions = self._get_permissions(org)
 
-        for perm_name, project_field in project_permissions.items():
-            if project_field.filter(pk=user.id).exists():
+        for perm_name, org_field in org_permissions.items():
+            if org_field.filter(pk=user.id).exists():
                 permissions[perm_name] = True
 
         return permissions
 
 
 class UserEndpoint(InternalGenericViewSet, mixins.RetrieveModelMixin):
+
     serializer_class = UserSerializer
     queryset = User.objects.all()
     lookup_field = "uuid"
 
+
     def partial_update(self, request):
         instance = get_object_or_404(User, email=request.query_params.get("email"))
 
-        if request.data.get("language") not in [
-            language[0] for language in settings.LANGUAGES
-        ]:
+        if request.data.get("language") not in [language[0] for language in settings.LANGUAGES]:
             raise ValidationError("Invalid argument: language")
 
         user_settings = instance.get_settings()
         user_settings.language = request.data.get("language")
         user_settings.save()
 
         return Response(status=status.HTTP_200_OK)
 
     def retrieve(self, request):
         if not request.query_params.get("email"):
             raise ValidationError(detail="empty email")
 
         user = User.objects.get_or_create(
-            email=request.query_params.get("email"),
-            defaults={"username": request.query_params.get("email")},
+            email=request.query_params.get("email"), defaults={"username": request.query_params.get("email")}
         )
 
         serializer = self.get_serializer(user[0])
         return Response(serializer.data)
```

### Comparing `weni_rp_apps-2.4.0a3/weni/internal/views.py` & `weni_rp_apps-2.4.0a4/weni/internal/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/orgs_api/serializers.py` & `weni_rp_apps-2.4.0a4/weni/orgs_api/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/orgs_api/tests.py` & `weni_rp_apps-2.4.0a4/weni/orgs_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/orgs_api/views.py` & `weni_rp_apps-2.4.0a4/weni/orgs_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/s3/views.py` & `weni_rp_apps-2.4.0a4/weni/s3/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/success_orgs/business.py` & `weni_rp_apps-2.4.0a4/weni/success_orgs/business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/success_orgs/serializers.py` & `weni_rp_apps-2.4.0a4/weni/success_orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/success_orgs/tests/test_business.py` & `weni_rp_apps-2.4.0a4/weni/success_orgs/tests/test_business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/success_orgs/views.py` & `weni_rp_apps-2.4.0a4/weni/success_orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/template_message/serializers.py` & `weni_rp_apps-2.4.0a4/weni/template_message/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/template_message/tests.py` & `weni_rp_apps-2.4.0a4/weni/template_message/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/template_message/views.py` & `weni_rp_apps-2.4.0a4/weni/template_message/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/templates/context_processors.py` & `weni_rp_apps-2.4.0a4/weni/templates/context_processors.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/ticketer_queues/tests.py` & `weni_rp_apps-2.4.0a4/weni/ticketer_queues/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/ticketer_queues/views.py` & `weni_rp_apps-2.4.0a4/weni/ticketer_queues/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/weni/utils/app_config.py` & `weni_rp_apps-2.4.0a4/weni/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.0a3/PKG-INFO` & `weni_rp_apps-2.4.0a4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weni-rp-apps
-Version: 2.4.0a3
+Version: 2.4.0a4
 Summary: Weni apps for Rapidpro Platform
 License: AGPL-3.0
 Author: jcbalmeida
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

