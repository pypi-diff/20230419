# Comparing `tmp/sqlmesh-0.4.2.dev9.tar.gz` & `tmp/sqlmesh-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.4.2.dev9.tar", last modified: Tue Apr 18 04:12:59 2023, max compression
+gzip compressed data, was "sqlmesh-0.5.0.tar", last modified: Wed Apr 19 01:51:19 2023, max compression
```

## Comparing `sqlmesh-0.4.2.dev9.tar` & `sqlmesh-0.5.0.tar`

### file list

```diff
@@ -1,692 +1,742 @@
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.396966 sqlmesh-0.4.2.dev9/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.321769 sqlmesh-0.4.2.dev9/.circleci/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1872 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/.circleci/config.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)     4414 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/.circleci/continue_config.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)       66 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/.dockerignore
--rw-r--r--   0 izeigerman   (501) staff       (20)     2152 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/.gitignore
--rw-r--r--   0 izeigerman   (501) staff       (20)     1900 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/.pre-commit-config.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)      234 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/.readthedocs.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)      135 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/Dockerfile.api
--rw-r--r--   0 izeigerman   (501) staff       (20)      383 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/Dockerfile.app
--rw-r--r--   0 izeigerman   (501) staff       (20)    11346 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/LICENSE
--rw-r--r--   0 izeigerman   (501) staff       (20)     1855 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/Makefile
--rw-r--r--   0 izeigerman   (501) staff       (20)     2011 2023-04-18 04:12:59.397046 sqlmesh-0.4.2.dev9/PKG-INFO
--rw-r--r--   0 izeigerman   (501) staff       (20)     1250 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/README.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1008 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docker-compose.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.323791 sqlmesh-0.4.2.dev9/docs/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.309533 sqlmesh-0.4.2.dev9/docs/_readthedocs/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.323910 sqlmesh-0.4.2.dev9/docs/_readthedocs/html/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/docs/_readthedocs/html/.keep
--rw-r--r--   0 izeigerman   (501) staff       (20)     9981 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/comparisons.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.325008 sqlmesh-0.4.2.dev9/docs/concepts/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.325258 sqlmesh-0.4.2.dev9/docs/concepts/architecture/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1334 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/architecture/serialization.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1113 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     6693 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/docs/concepts/audits.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     3866 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/environments.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5914 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/glossary.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       13 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/hooks.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     3027 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/macros.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.325839 sqlmesh-0.4.2.dev9/docs/concepts/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     9934 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/model_kinds.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     7454 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/overview.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/python_models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     4938 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/seed_models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5356 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/models/sql_models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     6631 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/overview.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.325957 sqlmesh-0.4.2.dev9/docs/concepts/plans/
--rw-r--r--   0 izeigerman   (501) staff       (20)    43124 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 izeigerman   (501) staff       (20)     8981 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/plans.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       37 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/concepts/team_development.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5699 2023-02-27 20:36:43.000000 sqlmesh-0.4.2.dev9/docs/concepts/tests.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      607 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/docs/development.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.326561 sqlmesh-0.4.2.dev9/docs/guides/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1953 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/guides/connections.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    10756 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/guides/models.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     2136 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/guides/projects.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.327152 sqlmesh-0.4.2.dev9/docs/guides/scheduling/
--rw-r--r--   0 izeigerman   (501) staff       (20)   740917 2023-02-24 17:54:11.000000 sqlmesh-0.4.2.dev9/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   379880 2023-02-24 17:54:11.000000 sqlmesh-0.4.2.dev9/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 izeigerman   (501) staff       (20)     5648 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/guides/scheduling.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1854 2023-02-27 20:36:43.000000 sqlmesh-0.4.2.dev9/docs/guides/testing.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     5510 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/docs/index.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      290 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/docs/installation.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.327958 sqlmesh-0.4.2.dev9/docs/integrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2905 2023-04-03 17:47:07.000000 sqlmesh-0.4.2.dev9/docs/integrations/airflow.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     7309 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/integrations/dbt.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    20383 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/integrations/engines.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      926 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/integrations/github.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      217 2023-03-25 06:07:32.000000 sqlmesh-0.4.2.dev9/docs/integrations/overview.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      665 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/docs/prerequisites.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    10774 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/docs/quick_start.md
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.328548 sqlmesh-0.4.2.dev9/docs/reference/
--rw-r--r--   0 izeigerman   (501) staff       (20)     5816 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/cli.md
--rw-r--r--   0 izeigerman   (501) staff       (20)    13240 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/configuration.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     4091 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/notebook.md
--rw-r--r--   0 izeigerman   (501) staff       (20)     1127 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/overview.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       14 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/reference/python.md
--rw-r--r--   0 izeigerman   (501) staff       (20)       16 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/docs/release_notes.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      122 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/docs/requirements.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)     3249 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/docs/sqlmesh.png
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.328672 sqlmesh-0.4.2.dev9/examples/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.329367 sqlmesh-0.4.2.dev9/examples/airflow/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1713 2023-04-09 02:39:12.000000 sqlmesh-0.4.2.dev9/examples/airflow/Dockerfile.template
--rw-r--r--   0 izeigerman   (501) staff       (20)     2164 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/examples/airflow/Makefile
--rw-r--r--   0 izeigerman   (501) staff       (20)      942 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/airflow/README.md
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.4.2.dev9/examples/airflow/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.329499 sqlmesh-0.4.2.dev9/examples/airflow/dags/
--rw-r--r--   0 izeigerman   (501) staff       (20)      263 2023-03-09 17:15:39.000000 sqlmesh-0.4.2.dev9/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3515 2023-04-09 02:39:12.000000 sqlmesh-0.4.2.dev9/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/airflow/requirements.txt
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.329801 sqlmesh-0.4.2.dev9/examples/airflow/spark_conf/
--rw-r--r--   0 izeigerman   (501) staff       (20)      872 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 izeigerman   (501) staff       (20)      151 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.330329 sqlmesh-0.4.2.dev9/examples/sushi/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.330590 sqlmesh-0.4.2.dev9/examples/sushi/audits/
--rw-r--r--   0 izeigerman   (501) staff       (20)      105 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/audits/items.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      119 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/audits/order_items.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      829 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi/config.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.330726 sqlmesh-0.4.2.dev9/examples/sushi/data/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi/data/.keep
--rw-r--r--   0 izeigerman   (501) staff       (20)      551 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/helper.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.330960 sqlmesh-0.4.2.dev9/examples/sushi/hooks/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/hooks/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.331220 sqlmesh-0.4.2.dev9/examples/sushi/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/macros/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      702 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/macros/macros.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.332573 sqlmesh-0.4.2.dev9/examples/sushi/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)      913 2023-03-13 20:04:07.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      204 2023-03-03 17:17:44.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/customers.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)     1914 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/items.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1892 2023-03-13 20:04:07.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/order_items.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1646 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/orders.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      346 2023-03-25 04:59:10.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      465 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      123 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      688 2023-04-18 04:08:52.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      197 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.332693 sqlmesh-0.4.2.dev9/examples/sushi/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-03-24 20:49:46.000000 sqlmesh-0.4.2.dev9/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.332824 sqlmesh-0.4.2.dev9/examples/sushi/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1459 2023-02-27 20:51:17.000000 sqlmesh-0.4.2.dev9/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.333510 sqlmesh-0.4.2.dev9/examples/sushi_dbt/
--rw-r--r--   0 izeigerman   (501) staff       (20)       15 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/.gitignore
--rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/.user.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.333661 sqlmesh-0.4.2.dev9/examples/sushi_dbt/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-14 18:30:53.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      507 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.333933 sqlmesh-0.4.2.dev9/examples/sushi_dbt/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-03-03 23:53:25.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-02-28 16:05:24.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.334936 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1125 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      182 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)      309 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-01-31 01:13:15.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      752 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      186 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.311399 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335093 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335247 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335528 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335676 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335776 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335878 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.335976 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      783 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.336619 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)       97 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-01-31 01:13:15.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.336748 sqlmesh-0.4.2.dev9/examples/sushi_dbt/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.336878 sqlmesh-0.4.2.dev9/examples/sushi_dbt/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.4.2.dev9/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.337132 sqlmesh-0.4.2.dev9/examples/wursthall/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.312325 sqlmesh-0.4.2.dev9/examples/wursthall/audits/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.337304 sqlmesh-0.4.2.dev9/examples/wursthall/audits/db/
--rw-r--r--   0 izeigerman   (501) staff       (20)      141 2023-01-31 01:13:15.000000 sqlmesh-0.4.2.dev9/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       66 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/config.yaml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.337654 sqlmesh-0.4.2.dev9/examples/wursthall/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/macros/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      618 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.337833 sqlmesh-0.4.2.dev9/examples/wursthall/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.338355 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/
--rw-r--r--   0 izeigerman   (501) staff       (20)      428 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      256 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)     3145 2023-02-16 23:39:50.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      537 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339022 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1667 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      120 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)     3419 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      892 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.312821 sqlmesh-0.4.2.dev9/examples/wursthall/seeds/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339172 sqlmesh-0.4.2.dev9/examples/wursthall/seeds/src/
--rw-r--r--   0 izeigerman   (501) staff       (20)     7416 2023-01-25 18:34:48.000000 sqlmesh-0.4.2.dev9/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339435 sqlmesh-0.4.2.dev9/examples/wursthall/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-02-20 22:54:27.000000 sqlmesh-0.4.2.dev9/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)      955 2023-02-20 22:54:27.000000 sqlmesh-0.4.2.dev9/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 izeigerman   (501) staff       (20)     2094 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/mkdocs.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339581 sqlmesh-0.4.2.dev9/pdoc/
--rwxr-xr-x   0 izeigerman   (501) staff       (20)     1153 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/pdoc/cli.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339727 sqlmesh-0.4.2.dev9/pdoc/templates/
--rw-r--r--   0 izeigerman   (501) staff       (20)      131 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.339882 sqlmesh-0.4.2.dev9/posts/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.341317 sqlmesh-0.4.2.dev9/posts/virtual_environments/
--rw-r--r--   0 izeigerman   (501) staff       (20)   318753 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/change_categorization.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   274526 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/isolated_rigid_envs.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   163619 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/partial_breaking.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   298971 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/stateful_envs.png
--rw-r--r--   0 izeigerman   (501) staff       (20)   366545 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/virtual_envs.png
--rw-r--r--   0 izeigerman   (501) staff       (20)  1344487 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments/virtual_envs_end_to_end.png
--rw-r--r--   0 izeigerman   (501) staff       (20)    18666 2023-04-17 20:22:17.000000 sqlmesh-0.4.2.dev9/posts/virtual_environments.md
--rw-r--r--   0 izeigerman   (501) staff       (20)      734 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/pytest.ini
--rw-r--r--   0 izeigerman   (501) staff       (20)     1344 2023-04-18 04:12:59.397589 sqlmesh-0.4.2.dev9/setup.cfg
--rw-r--r--   0 izeigerman   (501) staff       (20)     3056 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/setup.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.342715 sqlmesh-0.4.2.dev9/sqlmesh/
--rw-r--r--   0 izeigerman   (501) staff       (20)        3 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/.airflowignore
--rw-r--r--   0 izeigerman   (501) staff       (20)     3676 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      173 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh/_version.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.344096 sqlmesh-0.4.2.dev9/sqlmesh/cli/
--rw-r--r--   0 izeigerman   (501) staff       (20)      821 2023-04-18 04:08:49.000000 sqlmesh-0.4.2.dev9/sqlmesh/cli/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4314 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/cli/example_project.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8938 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/cli/main.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1391 2023-01-20 19:19:17.000000 sqlmesh-0.4.2.dev9/sqlmesh/cli/options.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.346536 sqlmesh-0.4.2.dev9/sqlmesh/core/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      586 2023-01-20 19:19:17.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/_typing.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.346969 sqlmesh-0.4.2.dev9/sqlmesh/core/audit/
--rw-r--r--   0 izeigerman   (501) staff       (20)      449 2023-01-27 03:51:22.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1071 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8136 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.348250 sqlmesh-0.4.2.dev9/sqlmesh/core/config/
--rw-r--r--   0 izeigerman   (501) staff       (20)      638 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4412 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1001 2023-02-22 17:05:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      940 2023-02-08 20:28:46.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18770 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/connection.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3355 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/loader.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1655 2023-02-08 20:28:46.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/model.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5389 2023-02-22 17:05:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/root.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8432 2023-02-22 17:05:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    29182 2023-04-18 02:47:18.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/console.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      731 2023-03-16 20:42:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/constants.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    34133 2023-04-18 02:26:32.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8612 2023-03-10 17:30:08.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/context_diff.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    17626 2023-03-24 20:30:06.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/dialect.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.349928 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2390 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      762 2023-01-18 00:01:51.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    28278 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4238 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    10243 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      393 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1930 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1971 2023-03-01 20:53:43.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1398 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7713 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1181 2023-03-01 20:53:43.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2658 2023-03-01 00:12:50.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3678 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1815 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/environment.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      742 2023-02-09 01:00:20.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/hooks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9362 2023-03-08 20:46:19.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/loader.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18920 2023-03-24 20:30:06.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/macros.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.350896 sqlmesh-0.4.2.dev9/sqlmesh/core/model/
--rw-r--r--   0 izeigerman   (501) staff       (20)      546 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1498 2023-04-17 22:52:49.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/cache.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1300 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2417 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/decorator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    47553 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/definition.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7382 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/kind.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12622 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/meta.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2017 2023-03-15 19:25:00.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/model/seed.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2314 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.351261 sqlmesh-0.4.2.dev9/sqlmesh/core/plan/
--rw-r--r--   0 izeigerman   (501) staff       (20)      191 2022-12-27 15:59:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    24483 2023-04-18 04:09:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/plan/definition.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8075 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12174 2023-03-24 20:30:06.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/renderer.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15386 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/scheduler.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    19427 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.351751 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/
--rw-r--r--   0 izeigerman   (501) staff       (20)      527 2023-02-13 20:33:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    31251 2023-04-18 04:05:15.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18706 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.352240 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/
--rw-r--r--   0 izeigerman   (501) staff       (20)      692 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13080 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12222 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    19996 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12062 2023-04-18 02:26:32.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/test.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1412 2022-12-24 00:00:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/core/user.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354033 sqlmesh-0.4.2.dev9/sqlmesh/dbt/
--rw-r--r--   0 izeigerman   (501) staff       (20)       79 2023-03-13 19:40:14.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9390 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/adapter.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15639 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    11330 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/builtin.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1969 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/column.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9663 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3229 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/loader.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9390 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/model.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12410 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/package.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3530 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/profile.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4412 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/project.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1049 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/seed.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3145 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/source.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    11118 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/target.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-02 18:36:40.000000 sqlmesh-0.4.2.dev9/sqlmesh/dbt/util.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354255 sqlmesh-0.4.2.dev9/sqlmesh/engines/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4437 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/commands.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354501 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3414 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354848 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      148 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2571 2023-02-14 21:38:26.000000 sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.354969 sqlmesh-0.4.2.dev9/sqlmesh/integrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.355424 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2210 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/notification_operator_provider.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1726 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/notification_target.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1829 2023-01-18 20:54:37.000000 sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/shared.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    13153 2023-03-15 19:24:58.000000 sqlmesh-0.4.2.dev9/sqlmesh/magics.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.355782 sqlmesh-0.4.2.dev9/sqlmesh/migrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/migrations/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1749 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/py.typed
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.355930 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.357195 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-04 00:12:26.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4020 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3830 2023-03-09 17:15:48.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    18799 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.357548 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-16 21:08:59.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2132 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      868 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8508 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.358623 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1341 2023-01-18 20:54:37.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6307 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2549 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      877 2023-01-31 17:31:24.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1211 2023-01-20 19:19:17.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1340 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5222 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    10922 2023-03-09 17:15:48.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4400 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1292 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4139 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5006 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.360288 sqlmesh-0.4.2.dev9/sqlmesh/utils/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4326 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/concurrency.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7530 2023-02-14 22:10:01.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      410 2022-12-30 16:25:50.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/conversions.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4329 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/dag.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7549 2023-04-18 02:34:51.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/date.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1244 2023-02-04 22:32:08.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/errors.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15925 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/jinja.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15093 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-03-07 23:18:33.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/pandas.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1609 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/pydantic.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1534 2023-01-25 18:09:57.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/rich.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6166 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/transactional_file.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1301 2023-03-13 19:40:14.000000 sqlmesh-0.4.2.dev9/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.343576 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2011 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 izeigerman   (501) staff       (20)    20173 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)        1 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)      142 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)      787 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-04-18 04:12:59.000000 sqlmesh-0.4.2.dev9/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 izeigerman   (501) staff       (20)    21020 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/sqlmesh.svg
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.360610 sqlmesh-0.4.2.dev9/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      285 2023-02-07 17:58:48.000000 sqlmesh-0.4.2.dev9/tests/common_fixtures.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3773 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/conftest.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.363636 sqlmesh-0.4.2.dev9/tests/core/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/core/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.364777 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    27289 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1298 2023-02-07 16:29:13.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-07 23:18:33.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1281 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2613 2023-02-14 20:17:36.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7155 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3245 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     7073 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/tests/core/test_audit.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6611 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      850 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_connection_config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    10703 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/test_context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2749 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/tests/core/test_dialect.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      464 2022-12-28 17:42:44.000000 sqlmesh-0.4.2.dev9/tests/core/test_environment.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    25987 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_integration.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5760 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_macros.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    24586 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_model.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15859 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/test_plan.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3886 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/core/test_plan_evaluator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4557 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/test_scheduler.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    29395 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/test_schema_diff.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      857 2023-01-06 17:16:27.000000 sqlmesh-0.4.2.dev9/tests/core/test_seed.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    25050 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/test_snapshot.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9922 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    21886 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/core/test_state_sync.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.365473 sqlmesh-0.4.2.dev9/tests/dbt/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-16 16:43:18.000000 sqlmesh-0.4.2.dev9/tests/dbt/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      630 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/dbt/conftest.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2564 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/dbt/test_adapter.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    12387 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/dbt/test_config.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    16511 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/tests/dbt/test_transformation.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.365718 sqlmesh-0.4.2.dev9/tests/engines/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/engines/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.366142 sqlmesh-0.4.2.dev9/tests/engines/spark/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/engines/spark/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      357 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/engines/spark/conftest.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1503 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.316475 sqlmesh-0.4.2.dev9/tests/fixtures/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.315288 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.366966 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.367114 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.315423 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1055 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.367276 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 izeigerman   (501) staff       (20)    10264 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.367604 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.368374 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)      334 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      863 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      196 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.315742 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.368533 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.368677 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.368944 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.369396 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1155 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      108 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 izeigerman   (501) staff       (20)      193 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.369542 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.369680 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.369800 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)      540 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)     1249 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.370097 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 izeigerman   (501) staff       (20)       42 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.370233 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.370688 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.370840 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371107 sqlmesh-0.4.2.dev9/tests/fixtures/migrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)     9823 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/fixtures/migrations/environments.json
--rw-r--r--   0 izeigerman   (501) staff       (20)    25229 2023-04-10 17:15:07.000000 sqlmesh-0.4.2.dev9/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371463 sqlmesh-0.4.2.dev9/tests/integrations/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/integrations/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371734 sqlmesh-0.4.2.dev9/tests/integrations/github/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/integrations/github/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371873 sqlmesh-0.4.2.dev9/tests/integrations/github/fixtures/
--rw-r--r--   0 izeigerman   (501) staff       (20)      816 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/integrations/github/fixtures/pull_request_review.json
--rw-r--r--   0 izeigerman   (501) staff       (20)      477 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/integrations/github/test_notification_target.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.371992 sqlmesh-0.4.2.dev9/tests/schedulers/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/schedulers/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.372877 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1414 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.373292 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3866 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4280 2023-03-09 17:15:48.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     9673 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1226 2023-03-13 21:05:48.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6043 2023-03-02 21:54:32.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5785 2023-03-02 21:54:32.000000 sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.374814 sqlmesh-0.4.2.dev9/tests/utils/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/utils/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3580 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/utils/test_concurrency.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     6430 2023-02-14 21:38:26.000000 sqlmesh-0.4.2.dev9/tests/utils/test_connection_pool.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1381 2023-02-14 17:01:23.000000 sqlmesh-0.4.2.dev9/tests/utils/test_dag.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1818 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/utils/test_date.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      551 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/utils/test_filesystem.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5516 2023-03-07 20:10:54.000000 sqlmesh-0.4.2.dev9/tests/utils/test_jinja.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5790 2023-03-03 23:53:25.000000 sqlmesh-0.4.2.dev9/tests/utils/test_metaprogramming.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2501 2023-03-07 23:18:33.000000 sqlmesh-0.4.2.dev9/tests/utils/test_pandas.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      518 2022-12-13 22:24:29.000000 sqlmesh-0.4.2.dev9/tests/utils/test_pydantic.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2911 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/tests/utils/test_transactional_file.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1194 2023-03-13 19:40:14.000000 sqlmesh-0.4.2.dev9/tests/utils/test_yaml.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.375038 sqlmesh-0.4.2.dev9/tests/web/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/tests/web/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)    15137 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/tests/web/test_main.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.375155 sqlmesh-0.4.2.dev9/web/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/web/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.377130 sqlmesh-0.4.2.dev9/web/client/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1104 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/.eslintrc.js
--rw-r--r--   0 izeigerman   (501) staff       (20)       94 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/.gitignore
--rw-r--r--   0 izeigerman   (501) staff       (20)      129 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/.prettierignore
--rw-r--r--   0 izeigerman   (501) staff       (20)      403 2023-02-14 21:38:26.000000 sqlmesh-0.4.2.dev9/web/client/.prettierrc.js
--rw-r--r--   0 izeigerman   (501) staff       (20)     1076 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/web/client/index.html
--rw-r--r--   0 izeigerman   (501) staff       (20)    36926 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/openapi.json
--rw-r--r--   0 izeigerman   (501) staff       (20)      330 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/orval.config.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)   408504 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/package-lock.json
--rw-r--r--   0 izeigerman   (501) staff       (20)     2395 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/package.json
--rw-r--r--   0 izeigerman   (501) staff       (20)     1642 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/playwright.config.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)       82 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/postcss.config.js
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.317195 sqlmesh-0.4.2.dev9/web/client/public/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.377287 sqlmesh-0.4.2.dev9/web/client/public/favicons/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2473 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.377655 sqlmesh-0.4.2.dev9/web/client/src/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.378069 sqlmesh-0.4.2.dev9/web/client/src/api/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1220 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/api/channels.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     4473 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/api/index.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3247 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/api/instance.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.317427 sqlmesh-0.4.2.dev9/web/client/src/assets/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.317535 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.379470 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74500 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74524 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74368 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    73964 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    68940 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    67284 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    74116 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    73916 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.382391 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    55004 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    56384 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    57104 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    62320 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    56652 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    61688 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    57680 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    53148 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    57060 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    56836 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    61460 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    52820 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    59176 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    63876 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    60768 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    81732 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    60992 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 izeigerman   (501) staff       (20)    64792 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383040 sqlmesh-0.4.2.dev9/web/client/src/context/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4198 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/context/context.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3385 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/context/editor.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      923 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/context/fileTree.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     2661 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/context/plan.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1562 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/context/theme.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383262 sqlmesh-0.4.2.dev9/web/client/src/hooks/
--rw-r--r--   0 izeigerman   (501) staff       (20)      308 2023-03-02 00:19:27.000000 sqlmesh-0.4.2.dev9/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      817 2023-02-27 20:28:04.000000 sqlmesh-0.4.2.dev9/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     9237 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/web/client/src/index.css
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.317774 sqlmesh-0.4.2.dev9/web/client/src/library/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.318969 sqlmesh-0.4.2.dev9/web/client/src/library/components/
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383377 sqlmesh-0.4.2.dev9/web/client/src/library/components/banner/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1295 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383500 sqlmesh-0.4.2.dev9/web/client/src/library/components/button/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4517 2023-03-25 06:07:32.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383621 sqlmesh-0.4.2.dev9/web/client/src/library/components/button/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)     3516 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383737 sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/
--rw-r--r--   0 izeigerman   (501) staff       (20)      856 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.383856 sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)      632 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.384996 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1388 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 izeigerman   (501) staff       (20)     4897 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     8064 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     2718 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     9819 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     8190 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     3527 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.385303 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 izeigerman   (501) staff       (20)     5880 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3987 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1538 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.385863 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/
--rw-r--r--   0 izeigerman   (501) staff       (20)    10852 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     6045 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     2997 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      562 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.386140 sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2961 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     3146 2023-04-09 02:39:12.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.386571 sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4342 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     6011 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    22356 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.386829 sqlmesh-0.4.2.dev9/web/client/src/library/components/input/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2087 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      688 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.387203 sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/
--rw-r--r--   0 izeigerman   (501) staff       (20)     2292 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     4637 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     8042 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.387575 sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1560 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1953 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1447 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.391353 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/
--rw-r--r--   0 izeigerman   (501) staff       (20)     7538 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     6775 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1312 2023-03-29 18:25:45.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    10448 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1178 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    15001 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     9926 2023-03-28 05:23:20.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)    10478 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     3444 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     2155 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     2634 2023-04-09 02:39:18.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.391515 sqlmesh-0.4.2.dev9/web/client/src/library/components/progress/
--rw-r--r--   0 izeigerman   (501) staff       (20)      713 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.392026 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/
--rw-r--r--   0 izeigerman   (501) staff       (20)      526 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1921 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)      443 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.392281 sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/
--rw-r--r--   0 izeigerman   (501) staff       (20)      788 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.392425 sqlmesh-0.4.2.dev9/web/client/src/library/components/tasksOverview/
--rw-r--r--   0 izeigerman   (501) staff       (20)    11713 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/tasksOverview/TasksOverview.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.392554 sqlmesh-0.4.2.dev9/web/client/src/library/components/toggle/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1453 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 izeigerman   (501) staff       (20)     1197 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/main.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.393344 sqlmesh-0.4.2.dev9/web/client/src/models/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1647 2023-04-02 22:26:52.000000 sqlmesh-0.4.2.dev9/web/client/src/models/artifact.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     3472 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/models/directory.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     4190 2023-03-16 22:35:40.000000 sqlmesh-0.4.2.dev9/web/client/src/models/environment.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1760 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/src/models/file.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      173 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/src/models/index.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      766 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/src/models/initial.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      200 2023-02-14 21:38:27.000000 sqlmesh-0.4.2.dev9/web/client/src/routes.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.393603 sqlmesh-0.4.2.dev9/web/client/src/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)       35 2023-01-20 18:11:03.000000 sqlmesh-0.4.2.dev9/web/client/src/tests/setup.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.4.2.dev9/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.393855 sqlmesh-0.4.2.dev9/web/client/src/types/
--rw-r--r--   0 izeigerman   (501) staff       (20)      467 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/types/enum.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)      137 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/types/index.d.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.394105 sqlmesh-0.4.2.dev9/web/client/src/utils/
--rw-r--r--   0 izeigerman   (501) staff       (20)     4102 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/client/src/utils/index.spec.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     5245 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/utils/index.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.394232 sqlmesh-0.4.2.dev9/web/client/src/workers/
--rw-r--r--   0 izeigerman   (501) staff       (20)      113 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/workers/index.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.394473 sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/
--rw-r--r--   0 izeigerman   (501) staff       (20)     1105 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1578 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     5842 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/tailwind.config.js
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.394596 sqlmesh-0.4.2.dev9/web/client/tests/
--rw-r--r--   0 izeigerman   (501) staff       (20)      170 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/tests/initial.spec.ts
--rw-r--r--   0 izeigerman   (501) staff       (20)     1141 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/client/tsconfig.json
--rw-r--r--   0 izeigerman   (501) staff       (20)     1297 2023-04-17 20:03:35.000000 sqlmesh-0.4.2.dev9/web/client/vite.config.ts
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.395495 sqlmesh-0.4.2.dev9/web/server/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.4.2.dev9/web/server/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.395616 sqlmesh-0.4.2.dev9/web/server/api/
--rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.4.2.dev9/web/server/api/__init__.py
-drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-18 04:12:59.396842 sqlmesh-0.4.2.dev9/web/server/api/endpoints/
--rw-r--r--   0 izeigerman   (501) staff       (20)      784 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/__init__.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     4864 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/commands.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      819 2023-02-27 20:28:04.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/context.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1858 2023-02-17 22:23:25.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/directories.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      708 2023-03-01 20:53:43.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/environments.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      637 2023-02-15 19:33:57.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/events.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5528 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/files.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1834 2023-04-17 20:03:31.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/lineage.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      969 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/models.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3806 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/api/endpoints/plan.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     3381 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/console.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     1374 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/main.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     5724 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/models.py
--rw-r--r--   0 izeigerman   (501) staff       (20)      260 2023-04-07 21:24:23.000000 sqlmesh-0.4.2.dev9/web/server/openapi.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2401 2023-03-09 19:19:03.000000 sqlmesh-0.4.2.dev9/web/server/settings.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2114 2023-02-04 22:32:08.000000 sqlmesh-0.4.2.dev9/web/server/sse.py
--rw-r--r--   0 izeigerman   (501) staff       (20)     2419 2023-03-24 20:30:10.000000 sqlmesh-0.4.2.dev9/web/server/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.959057 sqlmesh-0.5.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.867058 sqlmesh-0.5.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1872 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4414 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/.circleci/continue_config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1900 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/Dockerfile.api
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/Dockerfile.app
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11346 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1855 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1994 2023-04-19 01:51:19.959057 sqlmesh-0.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.871058 sqlmesh-0.5.0/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.851058 sqlmesh-0.5.0/docs/_readthedocs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.871058 sqlmesh-0.5.0/docs/_readthedocs/html/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/_readthedocs/html/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9965 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/comparisons.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.871058 sqlmesh-0.5.0/docs/concepts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.871058 sqlmesh-0.5.0/docs/concepts/architecture/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6689 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/audits.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3866 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5952 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/glossary.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/hooks.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/macros.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.871058 sqlmesh-0.5.0/docs/concepts/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7606 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/models/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/models/python_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4938 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/models/seed_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5356 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/models/sql_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6637 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/overview.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.871058 sqlmesh-0.5.0/docs/concepts/plans/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43124 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8973 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/plans.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5699 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/concepts/tests.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/development.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.875058 sqlmesh-0.5.0/docs/guides/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1953 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/guides/connections.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1309 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/guides/migrations.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/guides/models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/guides/multi_repo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/guides/projects.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.875058 sqlmesh-0.5.0/docs/guides/scheduling/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   740917 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   379880 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5648 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/guides/scheduling.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1854 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/guides/testing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5517 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/installation.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.875058 sqlmesh-0.5.0/docs/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/integrations/airflow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7309 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/integrations/dbt.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23739 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/integrations/engines.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      925 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/integrations/github.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/integrations/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/prerequisites.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10781 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/quick_start.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.875058 sqlmesh-0.5.0/docs/reference/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6032 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/reference/cli.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13240 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/reference/configuration.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4091 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/reference/notebook.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/reference/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/reference/python.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/release_notes.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3249 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/docs/sqlmesh.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.875058 sqlmesh-0.5.0/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/airflow/Dockerfile.template
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/airflow/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      942 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/airflow/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/airflow/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/airflow/dags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3515 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/airflow/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/airflow/spark_conf/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.855058 sqlmesh-0.5.0/examples/multi/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_1/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_1/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_1/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_1/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_1/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_1/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_1/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_1/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_1/models/a.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_1/models/b.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_1/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_2/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_2/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_2/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_2/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_2/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_2/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_2/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_2/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_2/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_2/models/c.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_2/models/d.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/multi/repo_2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/multi/repo_2/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/sushi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/sushi/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/audits/items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      829 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.879058 sqlmesh-0.5.0/examples/sushi/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/data/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.883058 sqlmesh-0.5.0/examples/sushi/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.883058 sqlmesh-0.5.0/examples/sushi/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      702 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.883058 sqlmesh-0.5.0/examples/sushi/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/order_items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1646 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/orders.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      197 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.883058 sqlmesh-0.5.0/examples/sushi/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.883058 sqlmesh-0.5.0/examples/sushi/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1459 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.883058 sqlmesh-0.5.0/examples/sushi_dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.883058 sqlmesh-0.5.0/examples/sushi_dbt/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.883058 sqlmesh-0.5.0/examples/sushi_dbt/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      752 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.855058 sqlmesh-0.5.0/examples/sushi_dbt/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      783 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/sushi_dbt/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/wursthall/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.855058 sqlmesh-0.5.0/examples/wursthall/audits/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/wursthall/audits/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/wursthall/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/wursthall/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.887058 sqlmesh-0.5.0/examples/wursthall/models/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3145 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.891058 sqlmesh-0.5.0/examples/wursthall/models/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      120 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3419 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.855058 sqlmesh-0.5.0/examples/wursthall/seeds/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.891058 sqlmesh-0.5.0/examples/wursthall/seeds/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7416 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.891058 sqlmesh-0.5.0/examples/wursthall/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/mkdocs.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.891058 sqlmesh-0.5.0/pdoc/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1153 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/pdoc/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.891058 sqlmesh-0.5.0/pdoc/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.891058 sqlmesh-0.5.0/posts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.891058 sqlmesh-0.5.0/posts/virtual_data_environments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   318753 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/posts/virtual_data_environments/change_categorization.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   274526 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/posts/virtual_data_environments/isolated_rigid_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   163619 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/posts/virtual_data_environments/partial_breaking.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   298971 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/posts/virtual_data_environments/stateful_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   366545 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/posts/virtual_data_environments/virtual_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1344487 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/posts/virtual_data_environments/virtual_envs_end_to_end.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18696 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/posts/virtual_data_environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-04-19 01:51:19.959057 sqlmesh-0.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3113 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.895058 sqlmesh-0.5.0/sqlmesh/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        3 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/.airflowignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3676 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-04-19 01:51:19.000000 sqlmesh-0.5.0/sqlmesh/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.895058 sqlmesh-0.5.0/sqlmesh/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      821 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4314 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/cli/example_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9176 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/cli/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1433 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/cli/options.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.899058 sqlmesh-0.5.0/sqlmesh/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/_typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.899058 sqlmesh-0.5.0/sqlmesh/core/audit/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8136 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.899058 sqlmesh-0.5.0/sqlmesh/core/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      668 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/config/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/config/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19724 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/config/connection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3351 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/config/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/config/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5611 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/config/root.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8421 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29242 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34599 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8612 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/context_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17626 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/dialect.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.903058 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28960 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3100 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4238 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10243 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1939 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1971 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6650 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2658 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4131 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1815 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10026 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18920 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.903058 sqlmesh-0.5.0/sqlmesh/core/model/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1300 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/model/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2417 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47553 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/model/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7382 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/model/kind.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12622 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/model/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2017 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/model/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2314 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.903058 sqlmesh-0.5.0/sqlmesh/core/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24778 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8075 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12174 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/renderer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15386 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20418 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.903058 sqlmesh-0.5.0/sqlmesh/core/snapshot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31868 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19093 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.903058 sqlmesh-0.5.0/sqlmesh/core/state_sync/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13080 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12222 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20048 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10834 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/core/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.907058 sqlmesh-0.5.0/sqlmesh/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9390 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15659 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11226 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1969 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4749 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5143 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3089 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9298 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12656 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/package.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3561 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4779 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11880 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/dbt/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.907058 sqlmesh-0.5.0/sqlmesh/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/engines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4437 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/engines/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.907058 sqlmesh-0.5.0/sqlmesh/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.907058 sqlmesh-0.5.0/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.907058 sqlmesh-0.5.0/sqlmesh/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.911058 sqlmesh-0.5.0/sqlmesh/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/integrations/github/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2210 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/integrations/github/notification_operator_provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/integrations/github/notification_target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1829 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/integrations/github/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13647 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/magics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.911058 sqlmesh-0.5.0/sqlmesh/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/migrations/v0002_remove_identify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.911058 sqlmesh-0.5.0/sqlmesh/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.911058 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4020 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8053 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3830 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18799 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.911058 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2132 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8508 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.915058 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1341 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6307 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1340 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5222 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10922 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4400 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1292 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4139 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5213 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.915058 sqlmesh-0.5.0/sqlmesh/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4378 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8053 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7530 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/conversions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4329 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7549 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1244 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16084 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/rich.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6487 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.895058 sqlmesh-0.5.0/sqlmesh.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1994 2023-04-19 01:51:19.000000 sqlmesh-0.5.0/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21666 2023-04-19 01:51:19.000000 sqlmesh-0.5.0/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-19 01:51:19.000000 sqlmesh-0.5.0/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-04-19 01:51:19.000000 sqlmesh-0.5.0/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      808 2023-04-19 01:51:19.000000 sqlmesh-0.5.0/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-19 01:51:19.000000 sqlmesh-0.5.0/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21020 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/sqlmesh.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.915058 sqlmesh-0.5.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/common_fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3741 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.919058 sqlmesh-0.5.0/tests/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.919058 sqlmesh-0.5.0/tests/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27881 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1386 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/test_base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1270 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1253 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/test_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8036 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7073 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_audit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6611 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_connection_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10197 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_dialect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26783 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5880 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_macros.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24406 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15280 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3824 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4557 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32235 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_schema_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      857 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25072 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_snapshot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9870 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21852 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/core/test_state_sync.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.919058 sqlmesh-0.5.0/tests/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/dbt/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2537 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/dbt/test_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12939 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/dbt/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16951 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/dbt/test_transformation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.919058 sqlmesh-0.5.0/tests/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/engines/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/engines/spark/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.859058 sqlmesh-0.5.0/tests/fixtures/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.859058 sqlmesh-0.5.0/tests/fixtures/dbt/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.859058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1055 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10264 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.859058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.923058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/fixtures/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25229 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/integrations/github/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/integrations/github/fixtures/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/integrations/github/fixtures/pull_request_review.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      477 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/integrations/github/test_notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1414 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.927058 sqlmesh-0.5.0/tests/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3866 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4280 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9704 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1227 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6043 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5785 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.931058 sqlmesh-0.5.0/tests/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3580 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6430 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1818 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_filesystem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5516 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5790 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2501 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2911 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/utils/test_yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.931058 sqlmesh-0.5.0/tests/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/web/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15138 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/tests/web/test_main.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.931058 sqlmesh-0.5.0/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.931058 sqlmesh-0.5.0/web/client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/.eslintrc.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/.prettierignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/.prettierrc.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.931058 sqlmesh-0.5.0/web/client/dist/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.935057 sqlmesh-0.5.0/web/client/dist/assets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74500 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/CircularStd-Black-52659624.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74368 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74116 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1507068 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/Graph-2afdb6eb.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5980 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/Graph-34acea2c.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21344 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/Plan-317aab54.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    55004 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57104 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/Publico-Bold-c79acd56.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    56836 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/Publico-Medium-01b4a891.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1100002 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/index-0d5132a3.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35224 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/index-4452b6b5.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/assets/worker-e891d118.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.935057 sqlmesh-0.5.0/web/client/dist/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-04-19 01:51:06.000000 sqlmesh-0.5.0/web/client/dist/favicons/favicon.ico
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-04-19 01:51:07.000000 sqlmesh-0.5.0/web/client/dist/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36926 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/openapi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      330 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/orval.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   408504 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2395 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/playwright.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/postcss.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.863058 sqlmesh-0.5.0/web/client/public/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.935057 sqlmesh-0.5.0/web/client/public/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.939057 sqlmesh-0.5.0/web/client/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.939057 sqlmesh-0.5.0/web/client/src/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1220 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/api/channels.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4473 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/api/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3247 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/api/instance.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.863058 sqlmesh-0.5.0/web/client/src/assets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.863058 sqlmesh-0.5.0/web/client/src/assets/fonts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.939057 sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74500 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74524 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74368 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73964 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    68940 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    67284 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74116 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73916 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.943057 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    55004 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56384 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57104 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    62320 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56652 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61688 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57680 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    53148 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57060 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56836 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61460 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    52820 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    59176 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    63876 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60768 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    81732 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60992 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    64792 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.943057 sqlmesh-0.5.0/web/client/src/context/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4198 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/context/context.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3385 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/context/editor.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      923 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/context/fileTree.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2661 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/context/plan.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1562 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/context/theme.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.943057 sqlmesh-0.5.0/web/client/src/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9237 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/index.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.863058 sqlmesh-0.5.0/web/client/src/library/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.867058 sqlmesh-0.5.0/web/client/src/library/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.943057 sqlmesh-0.5.0/web/client/src/library/components/banner/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1295 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.943057 sqlmesh-0.5.0/web/client/src/library/components/button/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4517 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.943057 sqlmesh-0.5.0/web/client/src/library/components/button/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3516 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.943057 sqlmesh-0.5.0/web/client/src/library/components/divider/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.947057 sqlmesh-0.5.0/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.947057 sqlmesh-0.5.0/web/client/src/library/components/editor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1388 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4897 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8064 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2718 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9819 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8190 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3527 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.947057 sqlmesh-0.5.0/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5880 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3987 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1538 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.947057 sqlmesh-0.5.0/web/client/src/library/components/fileTree/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10852 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6045 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.947057 sqlmesh-0.5.0/web/client/src/library/components/graph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2961 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3146 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.947057 sqlmesh-0.5.0/web/client/src/library/components/ide/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/ide/ActivePlan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6011 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/ide/IDE.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22356 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/ide/RunPlan.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.947057 sqlmesh-0.5.0/web/client/src/library/components/input/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2087 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.947057 sqlmesh-0.5.0/web/client/src/library/components/logo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4637 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8042 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.951057 sqlmesh-0.5.0/web/client/src/library/components/modal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1953 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.951057 sqlmesh-0.5.0/web/client/src/library/components/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7538 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10448 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1178 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15001 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9926 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10478 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3444 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2155 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2634 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.951057 sqlmesh-0.5.0/web/client/src/library/components/progress/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.951057 sqlmesh-0.5.0/web/client/src/library/components/root/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/root/Footer.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1921 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/root/Header.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/root/Main.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/root/Root.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.951057 sqlmesh-0.5.0/web/client/src/library/components/splitPane/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.951057 sqlmesh-0.5.0/web/client/src/library/components/tasksOverview/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11713 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.951057 sqlmesh-0.5.0/web/client/src/library/components/toggle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1453 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/library/components/toggle/Toggle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1197 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/main.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.955057 sqlmesh-0.5.0/web/client/src/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1647 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/models/artifact.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3472 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/models/directory.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4190 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/models/environment.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1760 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/models/file.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/models/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/models/initial.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/routes.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.955057 sqlmesh-0.5.0/web/client/src/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/tests/setup.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.955057 sqlmesh-0.5.0/web/client/src/types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/types/enum.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/types/index.d.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.955057 sqlmesh-0.5.0/web/client/src/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5245 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/utils/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.955057 sqlmesh-0.5.0/web/client/src/workers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/workers/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.955057 sqlmesh-0.5.0/web/client/src/workers/sqlglot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1578 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5842 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/tailwind.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.955057 sqlmesh-0.5.0/web/client/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/tests/initial.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/tsconfig.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1297 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/client/vite.config.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.955057 sqlmesh-0.5.0/web/server/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.955057 sqlmesh-0.5.0/web/server/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 01:51:19.959057 sqlmesh-0.5.0/web/server/api/endpoints/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4871 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      819 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/directories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/environments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5229 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/files.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1834 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/lineage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      969 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3628 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/api/endpoints/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1374 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5724 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/openapi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2421 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/sse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2461 2023-04-19 01:51:15.000000 sqlmesh-0.5.0/web/server/utils.py
```

### Comparing `sqlmesh-0.4.2.dev9/.circleci/config.yml` & `sqlmesh-0.5.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/.circleci/continue_config.yml` & `sqlmesh-0.5.0/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/.gitignore` & `sqlmesh-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/.pre-commit-config.yaml` & `sqlmesh-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/LICENSE` & `sqlmesh-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/Makefile` & `sqlmesh-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/PKG-INFO` & `sqlmesh-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.4.2.dev9
-Summary: UNKNOWN
+Version: 0.5.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: web
-Provides-Extra: snowflake
 Provides-Extra: bigquery
 Provides-Extra: databricks
-Provides-Extra: redshift
+Provides-Extra: dev
 Provides-Extra: dbt
+Provides-Extra: postgres
+Provides-Extra: redshift
+Provides-Extra: snowflake
+Provides-Extra: web
 License-File: LICENSE
 
 ![SQLMesh logo](sqlmesh.svg)
 
 SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
 
 For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
@@ -41,9 +40,7 @@
 
 * Join the [Tobiko Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) to ask questions, or just to say hi!
 * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
 * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
 
 ## Contribution
 Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-
-
```

### Comparing `sqlmesh-0.4.2.dev9/README.md` & `sqlmesh-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docker-compose.yml` & `sqlmesh-0.5.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/comparisons.md` & `sqlmesh-0.5.0/docs/comparisons.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 The first part of running a data transformation system is repeatedly iterating through three steps: create or modify model code, execute the models, evaluate the outputs. Practitioners may repeat these steps many times in a day's work.
 
 These steps incur costs to organizations: compute costs to run the models and staff time spent waiting on them to run. Inefficiencies compound rapidly because the steps are repeated so frequently.
 dbt's default full refresh approach leads to the most costly version of this loop: recomputing every model every time.
 
 SQLMesh takes another approach. It examines the code modifications and the dependency structure among the models to determine which models are affected -- and executes only those models. This results in the least costly version of the loop: computing only what is required every time through.
 
-This enables SQLMesh to provide efficient isolated environments with [Virtual Data Marts](./concepts/plans.md#plan-application). Environments in dbt cost compute and storage, but creating a development environment in SQLMesh is free -- you can quickly access a full replica of any other environment with a single command.
+This enables SQLMesh to provide efficient isolated [Virtual Environments](./concepts/plans.md#plan-application). Environments in dbt cost compute and storage, but creating a development environment in SQLMesh is free -- you can quickly access a full replica of any other environment with a single command.
 
 Additionally, SQLMesh ensures that promotion of staging environments to production is predictable and consistent. There is no concept of promotion in dbt, so queries are all rerun when it's time to deploy something. In SQLMesh, promotions are simple pointer swaps so there is no wasted compute.
 
 ### Incremental models
 Implementing incremental models is difficult and error-prone in dbt because it does not keep track of state.
 
 #### Complexity
```

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/architecture/serialization.md` & `sqlmesh-0.5.0/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.5.0/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/audits.md` & `sqlmesh-0.5.0/docs/concepts/audits.md`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 ```
 
 ## Running audits
 ### The CLI audit command
 
 You can execute audits with the `sqlmesh audit` command as follows:
 ```bash
-$ sqlmesh --path project audit -start 2022-01-01 -end 2022-01-02
+$ sqlmesh -p project audit -start 2022-01-01 -end 2022-01-02
 Found 1 audit(s).
 assert_item_price_is_not_null FAIL.
 
 Finished with 1 audit error(s).
 
 Failure in audit assert_item_price_is_not_null for model sushi.items (audits/items.sql).
 Got 3 results, expected 0.
```

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/environments.md` & `sqlmesh-0.5.0/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/glossary.md` & `sqlmesh-0.5.0/docs/concepts/glossary.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 ## User-Defined Function (UDF)
 Functions that a user of a database server provides to extend its functionality, in contrast to built-in functions that are already provided. UDFs are typically written to satisfy the particular requirements of the user.
 
 ## View
 A view is the result of a SQL query on a database.
 
-## Virtual Data Marts
-Term used to describes SQLMesh's ability to share tables across environments to ensure tables are only built once while maintaining data integrity and environment isolation. See [plan application](plans.md#plan-application) for more information. 
+## Virtual Environments
+SQLMesh's unique approach to environment that allows it to provide both environment isolation and the ability to share tables across environments. This is done in a way to ensure data consistency and accuracy. See [plan application](plans.md#plan-application) for more information. 
 
 ## Virtual Update
 Term used to describe a plan that can be applied without having to load any additional data or build any additional tables. See [Virtual Update](plans.md#virtual-update) for more information.
 
 ## Virtual Preview
 Term used to describe the ability to create an environment without having to build any additional tables. By comparing the version of models in the repo against what currently exists, SQLMesh can create an environment that exactly represents what is in the repo without by just updating views.
```

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/macros.md` & `sqlmesh-0.5.0/docs/concepts/macros.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/models/model_kinds.md` & `sqlmesh-0.5.0/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/models/overview.md` & `sqlmesh-0.5.0/docs/concepts/models/overview.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Overview
 
-Models are comprised of metadata and queries that create tables and views, which can be used by other models or even outside of SQLMesh. They are defined in the `models/` directory of your SQLMesh project and live in `.sql` files. 
+Models are comprised of metadata and queries that create tables and views, which can be used by other models or even outside of SQLMesh. They are defined in the `models/` directory of your SQLMesh project and live in `.sql` files.
 
 SQLMesh will automatically determine the relationships among and lineage of your models by parsing SQL, so you don't have to worry about manually configuring dependencies.
 
 ## Example
 The following is an example of a model defined in SQL. Note the following aspects:
   - Models can include descriptive information as comments, such as the first line.
-  - The first non-comment statement of a `model.sql` file is the `MODEL` DDL. 
+  - The first non-comment statement of a `model.sql` file is the `MODEL` DDL.
   - The last non-comment statement should be a `SELECT` statement that defines the logic needed to create the table
 
 ```sql linenums="1"
 -- Customer revenue computed and stored daily.
 MODEL (
   name sushi.customer_total_revenue,
   owner toby,
@@ -22,35 +22,35 @@
   o.customer_id::TEXT,
   SUM(o.amount)::DOUBLE AS revenue
 FROM sushi.orders AS o
 GROUP BY o.customer_id;
 ```
 
 ## Conventions
-SQLMesh attempts to infer as much as possible about your pipelines through SQL alone to reduce the cognitive overhead of switching to another format such as YAML. 
+SQLMesh attempts to infer as much as possible about your pipelines through SQL alone to reduce the cognitive overhead of switching to another format such as YAML.
 
 The `SELECT` expression of a model must follow certain conventions for SQLMesh to detect the necessary metadata to operate.
 
 ### Unique column names
 The final `SELECT` of a model's query must contain unique column names.
 
 ### Explict types
-The columns in the final `SELECT` of a model's query must be explicitly cast to a type so SQLMesh can automatically create tables with the appropriate schema. 
+The columns in the final `SELECT` of a model's query must be explicitly cast to a type so SQLMesh can automatically create tables with the appropriate schema.
 
 SQLMesh uses the postgres `x::int` syntax for casting; the casts are automatically transpiled to the appropriate format for the execution engine.
 
 ```sql linenums="1"
 WITH cte AS (
 SELECT 1 AS foo -- don't need to cast here
 )
 SELECT foo::int -- need to cast here because it's in the final select statement
 ```
 
 ### Inferrable names
-The final `SELECT` of a model's query must have inferrable names or aliases. 
+The final `SELECT` of a model's query must have inferrable names or aliases.
 
 Explicit aliases are recommended, but not required. The SQLMesh formatter will automatically add aliases to columns without them when the model SQL is rendered.
 
 This example demonstrates non-inferrable, inferrable, and explicit aliases:
 
 ```sql linenums="1"
 SELECT
@@ -63,29 +63,32 @@
   SUM(x) as x, -- explicitly x
 ```
 
 ## Properties
 The `MODEL` DDL statement takes various properties, which are used for both metadata and controlling behavior.
 
 ### name
-`name` specifies the name of the model. This name represents the production view name that the model outputs, so it generally takes the form of `"schema"."view_name"`. The name of a model must be unique in a SQLMesh project. 
+`name` specifies the name of the model. This name represents the production view name that the model outputs, so it generally takes the form of `"schema"."view_name"`. The name of a model must be unique in a SQLMesh project.
 
 When models are used in non-production environments, SQLMesh automatically prefixes the names. For example, consider a model named `"sushi"."customers"`. In production its view is named `"sushi"."customers"`, and in dev its view is named `"dev__sushi"."customers"`.
 
 Name is ***required*** and must be ***unique***.
 
 ### kind
 - Kind specifies what [kind](model_kinds.md) a model is. A model's kind determines how it is computed and stored. The default kind is `VIEW`, which means a view is created and your query is run each time that view is accessed.
 
 ### dialect
 - Dialect defines the SQL dialect of the file. By default, this uses the dialect of the SQLMesh `sqlmesh.core.config`.
 
 ### owner
 - Owner specifies who the main point of contact is for the model. It is an important field for organizations that have many data collaborators.
 
+### stamp
+An optional arbitrary string sequence used to create new model versions without making changes to any of the functional components of the definition.
+
 ### start
 - Start is used to determine the earliest time needed to process the model. It can be an absolute date/time (`2022-01-01`), or a relative one (`1 year ago`).
 
 ### cron
 - Cron is used to schedule your model to process or refresh at a certain interval. It uses [croniter](https://github.com/kiorky/croniter) under the hood, so expressions such as `@daily` can be used. A model's `IntervalUnit` is determined implicity by the cron expression.
 
 ### batch_size
@@ -94,21 +97,21 @@
 ### storage_format
 - Storage format is a property for engines such as Spark or Hive that support storage formats such as  `parquet` and `orc`.
 
 ### time_column
 - Time column is a required property for incremental models. It is used to determine which records to overwrite when doing an incremental insert. Engines that support partitioning such as Spark and Hive also use it as the partition key. Additional partition key columns can be specified with the `partitioned_by` property (see below). Time column can have an optional format string. The format should be in the dialect of the model.
 
 ### partitioned_by
-- Partitioned by is an optional property for engines such as Spark or Hive that support partitioning. Use this to add additional columns to the time column partition key. 
+- Partitioned by is an optional property for engines such as Spark or Hive that support partitioning. Use this to add additional columns to the time column partition key.
 
 ## Macros
 Macros can be used for passing in paramaterized arguments such as dates, as well as for making SQL less repetitive. By default, SQLMesh provides several predefined macro variables that can be used. Macros are used by prefixing with the `@` symbol. For more information, refer to [macros](../macros.md).
 
 ## Statements
-Models can have additional statements that run before the main query. This can be useful for loading things such as [UDFs](../glossary.md#user-defined-function-udf). 
+Models can have additional statements that run before the main query. This can be useful for loading things such as [UDFs](../glossary.md#user-defined-function-udf).
 
 In general, such statements should only be used for preparing the main query. They should not be used for creating or altering tables, as this could lead to unpredictable behavior.
 
 ```sql linenums="1" hl_lines="5-7"
 MODEL (
 ...
 );
@@ -118,15 +121,15 @@
 CREATE TEMPORARY FUNCTION UDF AS 'my.jar.udf';
 
 SELECT UDF(x)::int AS x
 FROM y
 ```
 
 ## Time column
-Models that are loaded incrementally require a time column to partition data. 
+Models that are loaded incrementally require a time column to partition data.
 
 A time column is a column in a model with an optional format string in the dialect of the model; for example, `'%Y-%m-%d'` for DuckDB or `'yyyy-mm-dd'` for Snowflake. For more information, refer to [time column](./model_kinds.md#time-column).
 
 ## Advanced usage
 The column used as your model's time column is not limited to a text or date type. In the following example, the time column, `di`, is an integer:
 
 ```sql linenums="1" hl_lines="5"
```

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/models/python_models.md` & `sqlmesh-0.5.0/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/models/seed_models.md` & `sqlmesh-0.5.0/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/models/sql_models.md` & `sqlmesh-0.5.0/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/overview.md` & `sqlmesh-0.5.0/docs/concepts/overview.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 
 "Backfilling" is the process of updating existing data to align with your changed models. For example, if your model change alters a calculation, then all existing data based on the old calculation method will be inaccurate once the new model is deployed. Backfilling entails re-calculating the existing fields whose calculation method has now changed.
 
 Most business data is temporal &mdash; each data fact was collected at a specific moment in time. The scale of backfill computations is directly tied to how much historical data must be re-calculated.
 
 The SQLMesh plan automatically determines which models and dates require backfill due to your changes. Based on this information, you specify the dates for which backfills will occur before you apply the plan.
 
-#### Build a virtual data mart
+#### Build a Virtual Environment
 Development activities for complex data systems should occur in a non-production environment so that errors can be detected before being deployed in production systems.
 
 One challenge with using multiple data environments is that backfill and other computations must happen twice &mdash; once for the non-production, and again for the production environment. This process consumes time and computing resources, resulting in delays and extra costs.
 
 SQLMesh solves this problem by maintaining a record of all model versions and their changes. It uses this record to determine when computations executed in a non-production environment generate outputs identical to what they would generate in the production environment. 
 
-SQLMesh uses its knowledge of equivalent outputs to create a **virtual data mart**. It does this by replacing references to outdated tables in the production environment with references to newly computed tables in the non-production environment. It effectively promotes views and tables from non-production to production, but *without computation or data movement*.
+SQLMesh uses its knowledge of equivalent outputs to create a **Virtual Environment**. It does this by replacing references to outdated tables in the production environment with references to newly computed tables in the non-production environment. It effectively promotes views and tables from non-production to production, but *without computation or data movement*.
 
-Because SQLMesh uses virtual data marts instead of re-computing everything in the production environment, promoting changes to production is quick and has no downtime. 
+Because SQLMesh uses virtual environments instead of re-computing everything in the production environment, promoting changes to production is quick and has no downtime. 
 
 ## Test your code and data
 Bad data is worse than no data. The best way to keep bad data out of your system is by testing your transformation code and results.
 
 ### [Tests](./tests.md)
 SQLMesh "tests" are similar to unit tests in software development, where the unit is a single model. SQLMesh tests validate model *code* &mdash; you specify the input data and expected output, then SQLMesh runs the test and compares the expected and actual output.
```

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.5.0/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/plans.md` & `sqlmesh-0.5.0/docs/concepts/plans.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 When a plan is applied to an environment, that environment gets associated with a collection of model variants that are part of that plan. In other words, each environment is a collection of references to model variants and the physical tables associated with them.
 
 ![Each model variant gets its own physical table, while environments only contain references to these tables](plans/model_versioning.png)
 
 *Each model variant gets its own physical table while environments only contain references to these tables.*
 
-This unique approach to understanding and applying changes is what enables SQLMesh's virtual data mart technology. This technology allows SQLMesh to ensure complete isolation between environments while allowing it to share physical data assets between environments when appropriate and safe to do so. Additionally, since each model change is captured in a separate physical table, reverting to a previous version becomes a simple and quick operation (refer to [Virtual Update](#virtual-update)) as long as its physical table hasn't been garbage collected by the janitor process. SQLMesh makes it easy to be correct, and really hard to accidentally and irreversibly break things.
+This unique approach to understanding and applying changes is what enables SQLMesh's Virtual Environments. This technology allows SQLMesh to ensure complete isolation between environments while allowing it to share physical data assets between environments when appropriate and safe to do so. Additionally, since each model change is captured in a separate physical table, reverting to a previous version becomes a simple and quick operation (refer to [Virtual Update](#virtual-update)) as long as its physical table hasn't been garbage collected by the janitor process. SQLMesh makes it easy to be correct, and really hard to accidentally and irreversibly break things.
 
 ### Backfilling
 Despite all the benefits, the approach described above is not without trade-offs. When a new model version is just created, a physical table assigned to it is empty. Therefore, SQLMesh needs to re-apply the logic of the new model version to the entire date range of this model in order to populate the new version's physical table. This process is called backfilling.
 
 Despite the fact that backfilling happens incrementally, there is an extra cost associated with this operation due to additional runtime involved. If the runtime cost is a concern, a [forward-only plan](#forward-only-plans) can be used instead.
 
 ### Virtual Update
```

### Comparing `sqlmesh-0.4.2.dev9/docs/concepts/tests.md` & `sqlmesh-0.5.0/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/development.md` & `sqlmesh-0.5.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/guides/connections.md` & `sqlmesh-0.5.0/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/guides/models.md` & `sqlmesh-0.5.0/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/guides/projects.md` & `sqlmesh-0.5.0/docs/guides/projects.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
     ```bash
     cd my-project
     ```
 
     From here, you can create your project structure from scratch, or SQLMesh can scaffold one for you. For the purposes of this guide, we'll show you how to scaffold your project so that you can get up and running quickly.
 
-1. To scaffold a project, it is recommended that you use a virtual environment by running the following commands:
+1. To scaffold a project, it is recommended that you use a python virtual environment by running the following commands:
 
     ```bash
     python -m venv .env
     ```
 
     ```bash
     source .env/bin/activate
     ```
 
     ```bash
     pip install sqlmesh
     ```
 
-    **Note:** When using a virtual environment, you must ensure that it is activated first. You should see `(.env)` in your command line; if you don't, run `source .env/bin/activate` from your project directory to activate your environment.
+    **Note:** When using a python virtual environment, you must ensure that it is activated first. You should see `(.env)` in your command line; if you don't, run `source .env/bin/activate` from your project directory to activate your environment.
 
 1. Once you have activated your environment, run the following command and SQLMesh will build out your project:
 
     ```bash
     sqlmesh init
     ```
 
@@ -54,18 +54,18 @@
     - ./tests (unit tests)
     - ./macros
 
 ## Editing an existing project
 
 To edit an existing project, open the project file you wish to edit in your preferred editor.
 
-If using CLI or Notebook, you can open a file in your project for editing by using the `sqlmesh` command with the `--path` varaible, and pointing to your project's path as follows:
+If using CLI or Notebook, you can open a file in your project for editing by using the `sqlmesh` command with the `-p` varaible, and pointing to your project's path as follows:
 
 ```bash
-sqlmesh --path <your-project-path>
+sqlmesh -p <your-project-path>
 ```
 
 For more details, refer to [CLI](../reference/cli.md) and [Notebook](../reference/notebook.md).
 
 ## Importing a project
 
 ### dbt
```

### Comparing `sqlmesh-0.4.2.dev9/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.5.0/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.5.0/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/guides/scheduling.md` & `sqlmesh-0.5.0/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/guides/testing.md` & `sqlmesh-0.5.0/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/index.md` & `sqlmesh-0.5.0/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     * SQLMesh summarizes the impact of changes and provides automated guardrails empowering everyone to safely and quickly contribute.
 
 1. Efficiency without complexity
     * SQLMesh automatically optimizes your workloads by reusing tables and minimizing computation saving you time and money.
 
 ### Key features
 * Efficient dev/staging environments
-    * SQLMesh builds a virtual data mart using views, which allows you to seamlessly rollback or roll forward your changes. Any data computation you run for validation purposes is actually not wasted &mdash; with a cheap pointer swap, you re-use your “staging” data in production. This means you get unlimited copy-on-write environments that make data exploration and preview of changes fun and safe.
+    * SQLMesh builds a Virtual Data Environment using views, which allows you to seamlessly rollback or roll forward your changes. Any data computation you run for validation purposes is actually not wasted &mdash; with a cheap pointer swap, you re-use your “staging” data in production. This means you get unlimited copy-on-write environments that make data exploration and preview of changes fun and safe.
 
 * Automatic DAG generation by semantically parsing and understanding SQL or Python scripts
     * No need to manually tag dependencies &mdash; SQLMesh was built with the ability to understand your entire data warehouse’s dependency graph.
 
 * Informative change summaries
     * Before making changes, SQLMesh will determine what has changed and show the entire graph of affected jobs.
```

### Comparing `sqlmesh-0.4.2.dev9/docs/integrations/airflow.md` & `sqlmesh-0.5.0/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/integrations/dbt.md` & `sqlmesh-0.5.0/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/integrations/engines.md` & `sqlmesh-0.5.0/docs/integrations/engines.md`

 * *Files 12% similar despite different names*

```diff
@@ -138,14 +138,51 @@
 | Option     | Description                                                                  |  Type  | Required |
 |------------|------------------------------------------------------------------------------|:------:|:--------:|
 | `database` | The optional database name. If not specified, the in-memory database is used | string |    N     |
 
 ## DuckDB - Airflow
 DuckDB only works when running locally; therefore it does not support Airflow. 
 
+# Postgres
+## Postgres - Local/Built-in Scheduler
+| Option            | Description                                                                                                                          |  Type  | Required |
+|-------------------|--------------------------------------------------------------------------------------------------------------------------------------|:------:|:--------:|
+| `host`            | The hostname of the Postgres server                                                                                                  | string |    Y     |
+| `user`            | The username to use for authentication with the Postgres server                                                                      | string |    Y     |
+| `password`        | The password to use for authentication with the Postgres server                                                                      | string |    Y     |
+| `port`            | The port number of the Postgres server                                                                                               |  int   |    Y     |
+| `database`        | The name of the database instance to connect to                                                                                      | string |    Y     |
+| `keepalives_idle` | The number of seconds between each keepalive packet sent to the server. If set to 0, the system default will be used. (Default: `0`) |  int   |    N     |
+| `connect_timeout` | The number of seconds to wait for the connection to the server. (Default: `10`)                                                      |  int   |    N     |
+| `role`            | The role to use for authentication with the Postgres server                                                                          | string |    N     |
+| `sslmode`         | The security of the connection to the Postgres server.                                                                               | string |    N     |
+
+## Postgres - Airflow
+**Engine Name:** `postgres`
+
+The SQLMesh Postgres Operator is similar to the [PostgresOperator](https://airflow.apache.org/docs/apache-airflow-providers-postgres/stable/_api/airflow/providers/postgres/operators/postgres/index.html), and relies on the same [PostgresHook](https://airflow.apache.org/docs/apache-airflow-providers-postgres/stable/_api/airflow/providers/postgres/hooks/postgres/index.html) implementation.
+
+To enable support for this operator, the Airflow Postgres provider package should be installed on the target Airflow cluster along with SQLMesh with the Postgres extra:
+```
+pip install "apache-airflow-providers-postgres"
+pip install "sqlmesh[postgres]"
+```
+
+The operator requires an [Airflow connection](https://airflow.apache.org/docs/apache-airflow/stable/howto/connection.html) to determine the target Postgres account. Refer to [Postgres connection](https://airflow.apache.org/docs/apache-airflow-providers-postgres/stable/connections/postgres.html) for more details.
+
+By default, the connection ID is set to `postgres_default`, but can be overridden using the `engine_operator_args` parameter to the `SQLMeshAirflow` instance as in the example below:
+```python linenums="1"
+sqlmesh_airflow = SQLMeshAirflow(
+    "postgres",
+    engine_operator_args={
+        "postgres_conn_id": "<Connection ID>"
+    },
+)
+```
+
 # Redshift
 ## Redshift - Local/Built-in Scheduler
 | Option                  | Description                                                                                                 |  Type  | Required |
 |-------------------------|-------------------------------------------------------------------------------------------------------------|:------:|:--------:|
 | `user`                  | The username to use for authentication with the Amazon Redshift cluster                                     | string |    N     |
 | `password`              | The password to use for authentication with the Amazon Redshift cluster                                     | string |    N     |
 | `database`              | The name of the database instance to connect to                                                             | string |    N     |
```

### Comparing `sqlmesh-0.4.2.dev9/docs/integrations/github.md` & `sqlmesh-0.5.0/docs/integrations/github.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # GitHub Actions
 
 SQLMesh's Github Actions integration will allow you to add a SQLMesh CI/CD bot to any Github project using [Github Actions](https://github.com/features/actions). The bot will automatically run [plan/apply](../concepts/plans.md) to an [environment](../concepts/environments.md) based on the code in a pull request.
 
-This will be done without copying or rebuilding data using SQLMesh's [Virtual Data Mart technology](../concepts/glossary.md#virtual-data-marts). 
+This will be done without copying or rebuilding data using SQLMesh's [Virtual Data Environments](../concepts/glossary.md#virtual-environments). 
 Once approved, the CI/CD bot will automatically run [plan/apply](../concepts/plans.md) to the production environment and merge the PR upon completion.
 This allows you to always have your main branch and prod environments in sync.
 
 We will be launching this CI/CD bot soon &mdash; in the meantime, please leave any feedback or questions in [our Slack channel](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg)!
```

### Comparing `sqlmesh-0.4.2.dev9/docs/prerequisites.md` & `sqlmesh-0.5.0/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/quick_start.md` & `sqlmesh-0.5.0/docs/quick_start.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```bash
 mkdir sqlmesh-example
 ```
 ```bash
 cd sqlmesh-example
 ```
 
-When using a virtual environment, you must ensure it's activated first by running the `source .env/bin/activate` command from the folder used during [installation](installation.md).
+When using a python virtual environment, you must ensure it's activated first by running the `source .env/bin/activate` command from the folder used during [installation](installation.md).
 
 Create a SQLMesh scaffold by using the following command:
 
 ```bash
 sqlmesh init
 ```
```

### Comparing `sqlmesh-0.4.2.dev9/docs/reference/cli.md` & `sqlmesh-0.5.0/docs/reference/cli.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 ```
 Usage: sqlmesh [OPTIONS] COMMAND [ARGS]...
 
   SQLMesh command line tool.
 
 Options:
-  --path TEXT    Path to the models directory.
+  --paths TEXT   Path(s) to the models directory.
   --config TEXT  Name of the config object.
   --help         Show this message and exit.
 
 Commands:
   audit     Run audits.
   dag       Renders the dag using graphviz.
   diff      Show the diff between the current context and a given...
   evaluate  Evaluate a model and return a dataframe with a default limit...
   fetchdf   Runs a sql query and displays the results.
   format    Format all models in a given directory.
   init      Create a new SQLMesh repository.
+  migrate   Migrate SQLMesh to the current running version.
   plan      Plan a migration of the current context's models with the...
   render    Renders a model's query, optionally expanding referenced models.
   run       Evaluates the DAG of models using the built-in scheduler.
   test      Run model unit tests.
 ```
 
 ## plan
@@ -63,34 +64,34 @@
 ## evaluate
 ```
 Usage: sqlmesh evaluate [OPTIONS] MODEL
 
   Evaluate a model and return a dataframe with a default limit of 1000.
 
 Options:
-  -s, --start TEXT   The start datetime of the interval for which this 
+  -s, --start TEXT   The start datetime of the interval for which this
                      command will be applied.
-  -e, --end TEXT     The end datetime of the interval for which this 
+  -e, --end TEXT     The end datetime of the interval for which this
                      command will be applied.
   -l, --latest TEXT  The latest time used for non-incremental datasets
                      (defaults to now).
   --limit INTEGER    The number of rows the query should be limited to.
   --help             Show this message and exit.
 ```
 
 ## render
 ```
 Usage: sqlmesh render [OPTIONS] MODEL
 
   Renders a model's query, optionally expanding referenced models.
 
 Options:
-  -s, --start TEXT   The start datetime of the interval for which this 
+  -s, --start TEXT   The start datetime of the interval for which this
                      command will be applied.
-  -e, --end TEXT     The end datetime of the interval for which this 
+  -e, --end TEXT     The end datetime of the interval for which this
                      command will be applied.
   -l, --latest TEXT  The latest time used for non-incremental datasets
                      (defaults to now).
   --expand TEXT      Whether or not to expand materialized models (defaults to
                      False). If True, all referenced models are expanded as
                      raw queries. Multiple model names can also be specified,
                      in which case only they will be expanded as raw queries.
@@ -123,17 +124,17 @@
 ```
 Usage: sqlmesh audit [OPTIONS]
 
   Run audits.
 
 Options:
   --model TEXT       A model to audit. Multiple models can be audited.
-  -s, --start TEXT   The start datetime of the interval for which this 
+  -s, --start TEXT   The start datetime of the interval for which this
                      command will be applied.
-  -e, --end TEXT     The end datetime of the interval for which this 
+  -e, --end TEXT     The end datetime of the interval for which this
                      command will be applied.
   -l, --latest TEXT  The latest time used for non-incremental datasets
                      (defaults to now).
   --help             Show this message and exit.
 ```
 
 ## format
@@ -165,7 +166,16 @@
   This command requires a manual install of both the python and system
   graphviz package.
 
 Options:
   --file TEXT  The file to which the dag image should be written.
   --help       Show this message and exit.
 ```
+
+## migrate
+```
+Usage: sqlmesh migrate
+
+  Migrates SQLMesh to the current running version.
+
+  Please contact your SQLMesh administrator before doing this.
+```
```

### Comparing `sqlmesh-0.4.2.dev9/docs/reference/configuration.md` & `sqlmesh-0.5.0/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/reference/notebook.md` & `sqlmesh-0.5.0/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/reference/overview.md` & `sqlmesh-0.5.0/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/docs/sqlmesh.png` & `sqlmesh-0.5.0/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/airflow/Dockerfile.template` & `sqlmesh-0.5.0/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/airflow/Makefile` & `sqlmesh-0.5.0/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/airflow/README.md` & `sqlmesh-0.5.0/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.5.0/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.5.0/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi/config.py` & `sqlmesh-0.5.0/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi/helper.py` & `sqlmesh-0.5.0/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi/macros/macros.py` & `sqlmesh-0.5.0/examples/sushi/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.5.0/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi/models/items.py` & `sqlmesh-0.5.0/examples/sushi/models/items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi/models/order_items.py` & `sqlmesh-0.5.0/examples/sushi/models/order_items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi/models/orders.py` & `sqlmesh-0.5.0/examples/sushi/models/orders.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.5.0/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.5.0/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.5.0/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.5.0/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.5.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.5.0/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.5.0/examples/sushi_dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.5.0/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.5.0/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.5.0/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/wursthall/macros/macros.py` & `sqlmesh-0.5.0/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.5.0/examples/wursthall/models/db/order_f.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.5.0/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.5.0/examples/wursthall/models/src/customer_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.5.0/examples/wursthall/models/src/order_item_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/wursthall/models/src/shared.py` & `sqlmesh-0.5.0/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.5.0/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.5.0/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.5.0/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/mkdocs.yml` & `sqlmesh-0.5.0/mkdocs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,30 @@
     - quick_start.md
   - Guides:
     - guides/projects.md
     - guides/models.md
     - guides/testing.md
     - guides/scheduling.md
     - guides/connections.md
+    - guides/multi_repo.md
+    - guides/migrations.md
   - Concepts:
     - concepts/overview.md
     - Models:
       - concepts/models/overview.md
       - concepts/models/model_kinds.md
       - concepts/models/sql_models.md
       - concepts/models/python_models.md
       - concepts/models/seed_models.md
     - concepts/plans.md
     - concepts/environments.md
     - concepts/tests.md
     - concepts/audits.md
     - concepts/macros.md
     - concepts/hooks.md
-    - concepts/team_development.md
     - Architecture:
       - concepts/architecture/snapshots.md
       - concepts/architecture/serialization.md
     - concepts/glossary.md
   - Reference:
     - API:
       - reference/overview.md
```

### Comparing `sqlmesh-0.4.2.dev9/pdoc/cli.py` & `sqlmesh-0.5.0/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/posts/virtual_environments/change_categorization.png` & `sqlmesh-0.5.0/posts/virtual_data_environments/change_categorization.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/posts/virtual_environments/isolated_rigid_envs.png` & `sqlmesh-0.5.0/posts/virtual_data_environments/isolated_rigid_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/posts/virtual_environments/partial_breaking.png` & `sqlmesh-0.5.0/posts/virtual_data_environments/partial_breaking.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/posts/virtual_environments/stateful_envs.png` & `sqlmesh-0.5.0/posts/virtual_data_environments/stateful_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/posts/virtual_environments/virtual_envs.png` & `sqlmesh-0.5.0/posts/virtual_data_environments/virtual_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/posts/virtual_environments/virtual_envs_end_to_end.png` & `sqlmesh-0.5.0/posts/virtual_data_environments/virtual_envs_end_to_end.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/posts/virtual_environments.md` & `sqlmesh-0.5.0/posts/virtual_data_environments.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 Data teams have some of these benefits but lack key innovations to work at the level of efficiency and reliability that software engineers enjoy. **Virtual Data Environments** fill this gap.
 
 ### Current Landscape
 Environments are routinely used by data practitioners. For example, **dbt** allows its users to configure different *targets* — connections to different schemas within a Data Warehouse or even separate Data Warehouses instances altogether.
 
 **dbt**’s approach is sufficient for deploying data pipelines into separate environments for development / testing, staging, and production, while ensuring that changes are only applied to the target environment and leave datasets in other environments unaffected.
 
-![Figure 1: Isolated but rigid Data Warehouse environments](virtual_environments/isolated_rigid_envs.png)
+![Figure 1: Isolated but rigid Data Warehouse environments](virtual_data_environments/isolated_rigid_envs.png)
 *Figure 1: Isolated but rigid Data Warehouse environments*
 
 However, this development process becomes troublesome as an organization grows in size and multiple users begin to iterate and push changes (oftentimes concurrently). Some of the challenges include:
 
 1. Populating different environments with data is hard. Generally, there are four approaches:
 
     - Create a complete copy of data used in the production environment
@@ -45,15 +45,15 @@
 
 Some tools go one step further and allow their users to create snapshots of the current state of the environment based on the raw contents of source files of the pipelines deployed there.
 
 This approach helps determine which pipelines have been modified in the new environment and allows users to reuse the unmodified portion of production datasets as part of their development environment.
 
 Variations of this approach can be seen in dbt’s [state](https://docs.getdbt.com/docs/deploy/project-state) + [defer](https://docs.getdbt.com/reference/node-selection/defer) method and Fivetran’s [“smart runs”](https://www.fivetran.com/blog/how-we-execute-dbt-runs-faster-and-cheaper).
 
-![Figure 2: Detecting changes by comparing the raw contents of source files](virtual_environments/stateful_envs.png)
+![Figure 2: Detecting changes by comparing the raw contents of source files](virtual_data_environments/stateful_envs.png)
 *Figure 2: Detecting changes by comparing the raw contents of source files*
 
 This approach, though clearly an improvement, still has several shortcomings:
 - Users are not informed about the **indirect** impact their changes have on downstream datasets, so they are forced to rely on their judgment and choose to either recompute the entire dependency graph (correctness) or recompute modified datasets only (efficiency). Anything in between requires careful manual intervention on the user’s part, which is error-prone and doesn’t scale to large dependency graphs.
 - Existing datasets can be reused when creating new development environments, but not when deploying changes to production. As mentioned earlier, this leads to changes being recomputed all over again without any guarantee of yielding the same results. Meanwhile, existing production data and deployed code remain out of sync for the duration of the recomputation.
 - State is discarded once the changes are deployed to production, making it impossible to reuse previously built datasets when reverting applied changes.
 
@@ -77,15 +77,15 @@
 
 More generally, we're looking for a way to **reuse** existing data when appropriate to get an accurate **preview** of proposed changes in a fully **isolated** manner.
 
 SQLMesh’s Virtual Data Environments achieve exactly this thanks to the following aspects of the platform:
 - Each dataset managed by the platform is populated by a logic defined as a [model](https://sqlmesh.readthedocs.io/en/stable/concepts/models/overview/) using either SQL or Python. Every time a change to an existing model is made, a new [snapshot](https://sqlmesh.readthedocs.io/en/stable/concepts/architecture/snapshots/) of this model gets created and associated with a unique [fingerprint](https://sqlmesh.readthedocs.io/en/stable/concepts/architecture/snapshots/#fingerprinting). The fingerprint itself is a combination of hashes computed on the attributes that constitute a model. By default, each model snapshot writes into its own unique table (or updates its own unique view), so multiple versions of a model can exist at the same time without causing conflicts.
 - The platform doesn't expose datasets (physical tables or views) populated with model snapshots directly. Instead, it provides access to them through a layer of indirection implemented using [views](https://en.wikipedia.org/wiki/View_(SQL)). This way, updating a dataset version in production becomes the atomic and almost instantaneous operation of updating a view associated with it by swapping the source it points to. The best part is that this operation is completely transparent to downstream consumers who always refer to a view and never to an underlying physical table. I refer to the layer of indirection powered by views as the **virtual layer**, while the layer of tables and views populated directly with model snapshots is called the **physical layer**.
 
-![Figure 3: Environments managed through the virtual layer](virtual_environments/virtual_envs.png)
+![Figure 3: Environments managed through the virtual layer](virtual_data_environments/virtual_envs.png)
 *Figure 3: Environments managed through the virtual layer*
 
 These two properties combined constitute **Virtual Data Environments**.
 
 ### Model Snapshots
 As mentioned earlier, every time a model changes a new model snapshot is created to capture the change. Each snapshot represents the state of a model at the time the snapshot was generated. In SQLMesh, snapshots are generated automatically when a new [plan](https://sqlmesh.readthedocs.io/en/stable/concepts/plans/) is created and applied.
 
@@ -101,24 +101,24 @@
 #### Automatic Change Categorization
 The difference between **direct** and **indirect** modifications becomes relevant when [categorizing](https://sqlmesh.readthedocs.io/en/stable/concepts/plans/#change-categories) individual changes during plan creation.
 
 Every time a model is modified directly, SQLMesh automatically categorizes the change as “breaking” (downstream models are affected) or “non-breaking” (only the modified model is affected) based on the change’s impact on downstream models. This is possible due to the platform’s ability to understand SQL semantically, at the [AST](https://en.wikipedia.org/wiki/Abstract_syntax_tree) level. By comparing the current model version with the previous one we’re able to compute a [semantic diff](https://github.com/tobymao/sqlglot/blob/main/posts/sql_diff.md), which SQLMesh further analyzes to understand the impacts it would have on downstream models.
 
 For example, adding a new column is not considered to be a breaking change, but removing or modifying the existing one is.
 
-![Figure 4: Breaking vs. non-breaking changes](virtual_environments/change_categorization.png)
+![Figure 4: Breaking vs. non-breaking changes](virtual_data_environments/change_categorization.png)
 *Figure 4: Breaking vs. non-breaking changes*
 
 This way SQLMesh automatically reduces the amount of necessary recomputation to a minimum while guaranteeing correctness. No user intervention needed.
 
 Currently, this approach doesn’t extend beyond looking at each model as a whole. Soon, however, SQLMesh will categorize changes per *individual column* instead, thanks to its ability to determine column-level lineage.
 
 This will allow an even finer balance between correctness and efficiency, since changes like removing a column that is not referenced downstream will no longer be categorized as “breaking.”
 
-![Figure 5: Column-level change categorization](virtual_environments/partial_breaking.png)
+![Figure 5: Column-level change categorization](virtual_data_environments/partial_breaking.png)
 *Figure 5: Column-level change categorization*
 
 #### Physical Layer
 When a model is modified directly or indirectly, a new snapshot that captures the change gets associated with its own unique table (or view) in the **physical layer**, the name of which is based on the snapshot's fingerprint.
 
 This means different versions of the same model can coexist and be evaluated at the same time without overriding each others' outputs. The platform keeps track of missing data intervals for each individual snapshot and automatically [backfills](https://sqlmesh.readthedocs.io/en/stable/concepts/plans/#backfilling) data gaps during the plan application.
 
@@ -135,15 +135,15 @@
 
 Those versions/clones, however, are not tied in any way to underlying pipelines or a dependency graph that reference them, so users are responsible for correctly picking an appropriate copy. Additionally, the number of copies of the same dataset that can be created this way is rather limited.
 
 Unlike those tools, SQLMesh uses the virtual layer approach to create and manage entire dataset graphs (as opposed to individual datasets), while keeping the implementation completely agnostic to the underlying storage technology.
 
 Each [environment](https://sqlmesh.readthedocs.io/en/stable/concepts/environments/) in SQLMesh is just a collection of views, one per model, each pointing at a snapshot table in the **physical layer**. This works equally well with most Data Warehouse technologies, be it Iceberg, Delta Lake, Snowflake, BigQuery, or something else.
 
-![Figure 6: Virtual Data Environments end-to-end](virtual_environments/virtual_envs_end_to_end.png)
+![Figure 6: Virtual Data Environments end-to-end](virtual_data_environments/virtual_envs_end_to_end.png)
 *Figure 6: Virtual Data Environments end-to-end*
 
 Views that belong to environments other than production have an environment name attached as a suffix to the schema portion of their fully qualified names. For example, the `db.model_a` dataset is accessed using that name in the production environment, but in an environment named `test` the name `db__test.model_a` would be used instead. That's how changes can be **previewed** before making their way into production.
 
 When a new environment is created, it uses the same set of snapshot table pointers as the production environment. Once changes are applied to the new environment, new model snapshots are generated and only the affected views are updated. Views that are part of the production environment remain unaffected. This is how SQLMesh ensures environment **isolation**.
 
 Finally, if a model implementation hasn't changed in relation to production (either **directly** or **indirectly**), the platform can safely **reuse** the same snapshot table that is currently being used in the production environment. Similarly, new snapshot tables created during development can be safely reused when changes are promoted into production.
```

### Comparing `sqlmesh-0.4.2.dev9/pytest.ini` & `sqlmesh-0.5.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/setup.cfg` & `sqlmesh-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 
 [mypy-databricks_cli.*]
 ignore_missing_imports = True
 
 [mypy-fsspec]
 ignore_missing_imports = True
 
+[mypy-psycopg2.*]
+ignore_missing_imports = True
+
 [autoflake]
 in-place = True
 expand-star-imports = True
 remove-all-unused-imports = True
 ignore-init-module-imports = True
 remove-duplicate-keys = True
 remove-unused-variables = True
```

### Comparing `sqlmesh-0.4.2.dev9/setup.py` & `sqlmesh-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,18 +39,25 @@
         "hyperscript",
         "jinja2",
         "pandas",
         "pydantic>=1.9.1,<2.0.0",
         "requests",
         "rich",
         "ruamel.yaml",
-        "sqlglot~=11.5.3",
+        "sqlglot~=11.5.4",
         "fsspec",
     ],
     extras_require={
+        "bigquery": [
+            "google-cloud-bigquery[pandas]",
+        ],
+        "databricks": [
+            "databricks-sql-connector",
+            "databricks-cli",
+        ],
         "dev": [
             f"apache-airflow=={os.environ.get('AIRFLOW_VERSION', '2.3.3')}",
             "autoflake==1.7.7",
             "black==22.6.0",
             "dbt-core",
             "Faker",
             "google-auth",
@@ -72,35 +79,31 @@
             "sqlalchemy-stubs",
             "tenacity==8.1.0",
             "types-croniter",
             "types-dateparser",
             "types-pytz",
             "types-requests==2.28.8",
         ],
-        "web": [
-            "fastapi==0.95.0",
-            "hyperscript==0.0.1",
-            "pyarrow==11.0.0",
-            "uvicorn==0.21.1",
-        ],
-        "snowflake": [
-            "snowflake-connector-python[pandas]",
-        ],
-        "bigquery": [
-            "google-cloud-bigquery[pandas]",
+        "dbt": [
+            "dbt-core",
         ],
-        "databricks": [
-            "databricks-sql-connector",
-            "databricks-cli",
+        "postgres": [
+            "psycopg2",
         ],
         "redshift": [
             "redshift_connector",
         ],
-        "dbt": [
-            "dbt-core",
+        "snowflake": [
+            "snowflake-connector-python[pandas]",
+        ],
+        "web": [
+            "fastapi==0.95.0",
+            "hyperscript==0.0.1",
+            "pyarrow==11.0.0",
+            "uvicorn==0.21.1",
         ],
     },
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/__init__.py` & `sqlmesh-0.5.0/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/cli/__init__.py` & `sqlmesh-0.5.0/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/cli/example_project.py` & `sqlmesh-0.5.0/sqlmesh/cli/example_project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/cli/main.py` & `sqlmesh-0.5.0/sqlmesh/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from sqlmesh.cli.example_project import ProjectTemplate, init_example_project
 from sqlmesh.core.context import Context
 from sqlmesh.utils.date import TimeLike
 from sqlmesh.utils.errors import MissingDependencyError
 
 
 @click.group(no_args_is_help=True)
-@opt.path
+@opt.paths
 @opt.config
 @click.option(
     "--connection",
     type=str,
     help="The name of the connection.",
 )
 @click.option(
@@ -27,42 +27,43 @@
     type=str,
     help="The name of the connection to use for tests.",
 )
 @click.pass_context
 @error_handler
 def cli(
     ctx: click.Context,
-    path: str,
+    paths: t.List[str],
     config: t.Optional[str] = None,
     connection: t.Optional[str] = None,
     test_connection: t.Optional[str] = None,
 ) -> None:
     """SQLMesh command line tool."""
     if ctx.invoked_subcommand == "version":
         return
 
-    path = os.path.abspath(path)
-    if ctx.invoked_subcommand == "init":
-        ctx.obj = path
-        return
+    if len(paths) == 1:
+        path = os.path.abspath(paths[0])
+        if ctx.invoked_subcommand == "init":
+            ctx.obj = path
+            return
 
     # Delegates the execution of the --help option to the corresponding subcommand
     if "--help" in sys.argv:
         return
 
     context = Context(
-        path=path,
+        paths=paths,
         config=config,
         connection=connection,
         test_connection=test_connection,
     )
 
     if not context.models:
         raise click.ClickException(
-            f"`{path}` doesn't seem to have any models... cd into the proper directory or specify the path with --path."
+            f"`{paths}` doesn't seem to have any models... cd into the proper directory or specify the path(s) with -p."
         )
 
     ctx.obj = context
 
 
 @cli.command("init")
 @click.option(
@@ -337,9 +338,17 @@
 
     host = host or "127.0.0.1"
     port = 8000 if port is None else port
     os.environ["PROJECT_PATH"] = str(obj.path)
     uvicorn.run("web.server.main:app", host=host, port=port, log_level="info")
 
 
+@cli.command("migrate")
+@click.pass_context
+@error_handler
+def migrate(ctx: click.Context) -> None:
+    """Migrate SQLMesh to the current running version."""
+    ctx.obj.migrate()
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/cli/options.py` & `sqlmesh-0.5.0/sqlmesh/cli/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import os
 
 import click
 
-path = click.option(
-    "--path",
-    default=os.getcwd(),
-    help="Path to the models directory.",
+paths = click.option(
+    "-p",
+    "--paths",
+    multiple=True,
+    default=[os.getcwd()],
+    help="Path(s) to the SQLMesh config/project.",
 )
 
 config = click.option(
     "--config",
     help="Name of the config object. Only applicable to configuration defined using Python script.",
 )
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/_typing.py` & `sqlmesh-0.5.0/sqlmesh/core/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.5.0/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/audit/definition.py` & `sqlmesh-0.5.0/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/config/__init__.py` & `sqlmesh-0.5.0/sqlmesh/core/config/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from sqlmesh.core.config.connection import (
     BigQueryConnectionConfig,
     ConnectionConfig,
     DatabricksConnectionConfig,
     DatabricksSparkSessionConnectionConfig,
     DatabricksSQLConnectionConfig,
     DuckDBConnectionConfig,
+    PostgresConnectionConfig,
     RedshiftConnectionConfig,
     SnowflakeConnectionConfig,
 )
 from sqlmesh.core.config.loader import load_config_from_paths
 from sqlmesh.core.config.model import ModelDefaultsConfig
 from sqlmesh.core.config.root import Config
 from sqlmesh.core.config.scheduler import AirflowSchedulerConfig, BuiltInSchedulerConfig
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/config/base.py` & `sqlmesh-0.5.0/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.5.0/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/config/common.py` & `sqlmesh-0.5.0/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/config/connection.py` & `sqlmesh-0.5.0/sqlmesh/core/config/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -512,19 +512,60 @@
     @property
     def _connection_factory(self) -> t.Callable:
         from redshift_connector import connect
 
         return connect
 
 
+class PostgresConnectionConfig(_ConnectionConfig):
+    host: str
+    user: str
+    password: str
+    port: int
+    database: str
+    keepalives_idle: int = 0
+    connect_timeout: int = 10
+    role: t.Optional[str] = None
+    sslmode: t.Optional[str] = None
+
+    concurrent_tasks: int = 4
+
+    type_: Literal["postgres"] = Field(alias="type", default="postgres")
+
+    @property
+    def _connection_kwargs_keys(self) -> t.Set[str]:
+        return {
+            "host",
+            "user",
+            "password",
+            "port",
+            "database",
+            "keepalives_idle",
+            "connect_timeout",
+            "role",
+            "sslmode",
+        }
+
+    @property
+    def _engine_adapter(self) -> t.Type[EngineAdapter]:
+        return engine_adapter.PostgresEngineAdapter
+
+    @property
+    def _connection_factory(self) -> t.Callable:
+        from psycopg2 import connect
+
+        return connect
+
+
 ConnectionConfig = Annotated[
     t.Union[
-        DuckDBConnectionConfig,
-        SnowflakeConnectionConfig,
+        BigQueryConnectionConfig,
         DatabricksSQLConnectionConfig,
         DatabricksSparkSessionConnectionConfig,
         DatabricksConnectionConfig,
-        BigQueryConnectionConfig,
+        DuckDBConnectionConfig,
+        PostgresConnectionConfig,
         RedshiftConnectionConfig,
+        SnowflakeConnectionConfig,
     ],
     Field(discriminator="type_"),
 ]
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/config/loader.py` & `sqlmesh-0.5.0/sqlmesh/core/config/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 f"Unsupported config file extension '{extension}' in config file '{path}'."
             )
 
         config = config.update_with(next_config) if config is not None else next_config
 
     if config is None:
         raise ConfigError(
-            "SQLMesh config could not be found. Point the cli to the right path with `sqlmesh --path`. If you haven't set up SQLMesh, run `sqlmesh init`."
+            "SQLMesh config could not be found. Point the cli to the right path with `sqlmesh -p`. If you haven't set up SQLMesh, run `sqlmesh init`."
         )
 
     if load_from_env:
         config = config.update_with(load_config_from_env())
 
     return config
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/config/model.py` & `sqlmesh-0.5.0/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/config/root.py` & `sqlmesh-0.5.0/sqlmesh/core/config/root.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         default_connection: The name of a connection to use by default.
         test_connection: The connection settings for tests. Can be a name which refers to an existing configuration
             in `connections`.
         scheduler: The scheduler configuration.
         notification_targets: The notification targets to use.
         dialect: The default sql dialect of model queries. Default: same as engine dialect.
         physical_schema: The default schema used to store materialized tables.
+        project: The project name of this config. Used for multi-repo setups.
         snapshot_ttl: The period of time that a model snapshot that is not a part of any environment should exist before being deleted.
         environment_ttl: The period of time that a development environment should exist before being deleted.
         ignore_patterns: Files that match glob patterns specified in this list are ignored when scanning the project folder.
         time_column_format: The default format to use for all model time columns. Defaults to %Y-%m-%d.
             This time format uses python format codes. https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes.
         auto_categorize_changes: Indicates whether SQLMesh should attempt to automatically categorize model changes (breaking / non-breaking)
             during plan creation.
@@ -42,18 +43,19 @@
     connections: t.Union[t.Dict[str, ConnectionConfig], ConnectionConfig] = DuckDBConnectionConfig()
     default_connection: str = ""
     test_connection_: t.Union[ConnectionConfig, str] = Field(
         alias="test_connection", default=DuckDBConnectionConfig()
     )
     scheduler: SchedulerConfig = BuiltInSchedulerConfig()
     notification_targets: t.List[NotificationTarget] = []
-    physical_schema: str = ""
+    physical_schema: str = c.SQLMESH
+    project: str = ""
     snapshot_ttl: str = c.DEFAULT_SNAPSHOT_TTL
     environment_ttl: t.Optional[str] = c.DEFAULT_ENVIRONMENT_TTL
-    ignore_patterns: t.List[str] = []
+    ignore_patterns: t.List[str] = c.IGNORE_PATTERNS
     time_column_format: str = c.DEFAULT_TIME_COLUMN_FORMAT
     auto_categorize_changes: CategorizerConfig = CategorizerConfig()
     users: t.List[User] = []
     model_defaults: ModelDefaultsConfig = ModelDefaultsConfig()
     loader: t.Type[Loader] = SqlMeshLoader
 
     _FIELD_UPDATE_STRATEGY: t.ClassVar[t.Dict[str, UpdateStrategy]] = {
@@ -107,7 +109,11 @@
             return self.connections
 
     @property
     def test_connection(self) -> ConnectionConfig:
         if isinstance(self.test_connection_, str):
             return self.get_connection(self.test_connection_)
         return self.test_connection_
+
+    @property
+    def dialect(self) -> t.Optional[str]:
+        return self.model_defaults.dialect
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.5.0/sqlmesh/core/config/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 class BuiltInSchedulerConfig(_SchedulerConfig, BaseConfig):
     """The Built-In Scheduler configuration."""
 
     type_: Literal["builtin"] = Field(alias="type", default="builtin")
 
     def create_state_sync(self, context: Context) -> t.Optional[StateSync]:
-        return EngineAdapterStateSync(context.engine_adapter, context.physical_schema)
+        return EngineAdapterStateSync(context.engine_adapter)
 
     def create_plan_evaluator(self, context: Context) -> PlanEvaluator:
         return BuiltInPlanEvaluator(
             state_sync=context.state_sync,
             snapshot_evaluator=context.snapshot_evaluator,
             backfill_concurrent_tasks=context.concurrent_tasks,
             console=context.console,
@@ -103,18 +103,18 @@
     def create_plan_evaluator(self, context: Context) -> PlanEvaluator:
         return AirflowPlanEvaluator(
             airflow_client=self.get_client(context.console),
             dag_run_poll_interval_secs=self.dag_run_poll_interval_secs,
             dag_creation_poll_interval_secs=self.dag_creation_poll_interval_secs,
             dag_creation_max_retry_attempts=self.dag_creation_max_retry_attempts,
             console=context.console,
-            notification_targets=context.notification_targets,
+            notification_targets=context.config.notification_targets,
             backfill_concurrent_tasks=self.backfill_concurrent_tasks,
             ddl_concurrent_tasks=self.ddl_concurrent_tasks,
-            users=context.users,
+            users=context.config.users,
         )
 
 
 class AirflowSchedulerConfig(_BaseAirflowSchedulerConfig, BaseConfig):
     """The Airflow Scheduler configuration.
 
     Args:
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/console.py` & `sqlmesh-0.5.0/sqlmesh/core/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,17 @@
         """Displays the models with missing dates"""
         if not plan.missing_intervals:
             return
         backfill = Tree("[bold]Models needing backfill (missing dates):")
         for missing in plan.missing_intervals:
             snapshot = plan.context_diff.snapshots[missing.snapshot_name]
             view_name = snapshot.qualified_view_name.for_environment(plan.environment_name)
-            backfill.add(f"{view_name}: {missing.format_missing_range()}")
+            backfill.add(
+                f"{view_name}: {missing.format_missing_range(snapshot.model.interval_unit())}"
+            )
         self._print(backfill)
 
     def _prompt_backfill(self, plan: Plan, auto_apply: bool) -> None:
         is_forward_only_dev = plan.is_dev and plan.forward_only
         backfill_or_preview = "preview" if is_forward_only_dev else "backfill"
 
         if plan.is_start_and_end_allowed:
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/constants.py` & `sqlmesh-0.5.0/sqlmesh/core/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,7 +28,13 @@
 DEFAULT_TIME_COLUMN_FORMAT = "%Y-%m-%d"
 """Default time column format"""
 
 EPOCH = datetime.date(1970, 1, 1)
 
 DEFAULT_MAX_LIMIT = 1000
 """The default maximum row limit that is used when evaluating a model."""
+
+AUDITS = "audits"
+HOOKS = "hooks"
+MACROS = "macros"
+MODELS = "models"
+TESTS = "tests"
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/context.py` & `sqlmesh-0.5.0/sqlmesh/core/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,24 +52,25 @@
 from sqlmesh.core.dialect import format_model_expressions, pandas_to_sql, parse
 from sqlmesh.core.engine_adapter import EngineAdapter
 from sqlmesh.core.environment import Environment
 from sqlmesh.core.hooks import hook
 from sqlmesh.core.loader import Loader, SqlMeshLoader, update_model_schemas
 from sqlmesh.core.macros import ExecutableOrMacro
 from sqlmesh.core.model import Model
+from sqlmesh.core.model.definition import _Model
 from sqlmesh.core.plan import Plan
 from sqlmesh.core.scheduler import Scheduler
 from sqlmesh.core.snapshot import (
     Snapshot,
     SnapshotEvaluator,
     SnapshotFingerprint,
     to_table_mapping,
 )
 from sqlmesh.core.state_sync import StateReader, StateSync
-from sqlmesh.core.test import run_all_model_tests, run_model_tests
+from sqlmesh.core.test import get_all_model_tests, run_model_tests, run_tests
 from sqlmesh.core.user import User
 from sqlmesh.utils import UniqueKeyDict, sys_path
 from sqlmesh.utils.dag import DAG
 from sqlmesh.utils.date import TimeLike, yesterday_ds
 from sqlmesh.utils.errors import ConfigError, MissingDependencyError, PlanError
 
 if t.TYPE_CHECKING:
@@ -167,18 +168,15 @@
 
 class Context(BaseContext):
     """Encapsulates a SQLMesh environment supplying convenient functions to perform various tasks.
 
     Args:
         engine_adapter: The default engine adapter to use.
         notification_targets: The notification target to use. Defaults to what is defined in config.
-        dialect: Default dialect of the sql in models.
-        physical_schema: The schema used to store physical materialized tables.
-        snapshot_ttl: Duration before unpromoted snapshots are removed.
-        path: The directory containing SQLMesh files.
+        paths: The directories containing SQLMesh files.
         config: A Config object or the name of a Config object in config.py.
         connection: The name of the connection. If not specified the first connection as it appears
             in configuration will be used.
         test_connection: The name of the connection to use for tests. If not specified the first
             connection as it appears in configuration will be used.
         concurrent_tasks: The maximum number of tasks that can use the connection concurrently.
         load: Whether or not to automatically load all models and macros (default True).
@@ -187,69 +185,66 @@
     """
 
     def __init__(
         self,
         engine_adapter: t.Optional[EngineAdapter] = None,
         notification_targets: t.Optional[t.List[NotificationTarget]] = None,
         state_sync: t.Optional[StateSync] = None,
-        dialect: str = "",
-        physical_schema: str = "",
-        snapshot_ttl: str = "",
-        path: str = "",
+        paths: t.Union[str, t.Iterable[str]] = "",
         config: t.Optional[t.Union[Config, str]] = None,
         connection: t.Optional[str] = None,
         test_connection: t.Optional[str] = None,
         concurrent_tasks: t.Optional[int] = None,
         loader: t.Optional[t.Type[Loader]] = None,
         load: bool = True,
         console: t.Optional[Console] = None,
         users: t.Optional[t.List[User]] = None,
     ):
         self.console = console or get_console()
-        self.path = Path(path).absolute()
-        if not self.path.is_dir():
-            raise ConfigError(f"{path} is not a directory")
 
-        self.config = self._load_config(config or "config")
+        self._sqlmesh_path = Path.home() / ".sqlmesh"
 
-        self.physical_schema = physical_schema or self.config.physical_schema or "sqlmesh"
-        self.snapshot_ttl = snapshot_ttl or self.config.snapshot_ttl or c.DEFAULT_SNAPSHOT_TTL
-        self.dag: DAG[str] = DAG()
+        self.configs = self._load_configs(
+            config or "config",
+            [
+                Path(path).absolute()
+                for path in ([paths] if isinstance(paths, str) else list(paths))
+            ],
+        )
 
+        self.dag: DAG[str] = DAG()
         self._models: UniqueKeyDict[str, Model] = UniqueKeyDict("models")
         self._audits: UniqueKeyDict[str, Audit] = UniqueKeyDict("audits")
         self._macros: UniqueKeyDict[str, ExecutableOrMacro] = UniqueKeyDict("macros")
         self._hooks: UniqueKeyDict[str, hook] = UniqueKeyDict("hooks")
 
+        self.path, self.config = t.cast(t.Tuple[Path, Config], next(iter(self.configs.items())))
+        self._scheduler = self.config.scheduler
         self.connection = connection
+        self.environment_ttl = self.config.environment_ttl
+        self.auto_categorize_changes = self.config.auto_categorize_changes
         connection_config = self.config.get_connection(connection)
         self.concurrent_tasks = concurrent_tasks or connection_config.concurrent_tasks
         self._engine_adapter = engine_adapter or connection_config.create_engine_adapter()
 
         test_connection_config = (
             self.config.test_connection
             if test_connection is None
             else self.config.get_connection(test_connection)
         )
         self._test_engine_adapter = test_connection_config.create_engine_adapter()
 
-        self.dialect = dialect or self.config.model_defaults.dialect or self._engine_adapter.dialect
-
         self.snapshot_evaluator = SnapshotEvaluator(
             self.engine_adapter, ddl_concurrent_tasks=self.concurrent_tasks
         )
 
-        self.notification_targets = self.config.notification_targets + (notification_targets or [])
-
         self._provided_state_sync: t.Optional[StateSync] = state_sync
         self._state_sync: t.Optional[StateSync] = None
         self._state_reader: t.Optional[StateReader] = None
 
-        self.users = self.config.users + (users or [])
-
         self._loader = (loader or self.config.loader or SqlMeshLoader)()
 
         if load:
             self.load()
 
     @property
     def engine_adapter(self) -> EngineAdapter:
@@ -274,15 +269,15 @@
         path = model._path  # type: ignore
         # model.copy() can't be used here due to a cached state that can be a part of a model instance.
         model = t.cast(Model, type(model)(**{**t.cast(Model, model).dict(), **kwargs}))
         model._path = path
         self._models.update({model.name: model})
 
         self._add_model_to_dag(model)
-        update_model_schemas(self.dialect, self.dag, self._models)
+        update_model_schemas(self.dag, self._models)
 
         return model
 
     def scheduler(self, environment: t.Optional[str] = None) -> Scheduler:
         """Returns the built-in scheduler.
 
         Args:
@@ -311,17 +306,15 @@
             max_workers=self.concurrent_tasks,
             console=self.console,
         )
 
     @property
     def state_sync(self) -> StateSync:
         if not self._state_sync:
-            self._state_sync = self._provided_state_sync or self.config.scheduler.create_state_sync(
-                self
-            )
+            self._state_sync = self._provided_state_sync or self._scheduler.create_state_sync(self)
             if not self._state_sync:
                 raise ConfigError(
                     "The operation is not supported when using a read-only state sync"
                 )
 
             if self._state_sync.get_versions(validate=False).schema_version == 0:
                 self._state_sync.migrate()
@@ -329,61 +322,29 @@
 
     @property
     def state_reader(self) -> StateReader:
         if not self._state_reader:
             try:
                 self._state_reader = self.state_sync
             except ConfigError:
-                self._state_reader = self.config.scheduler.create_state_reader(self)
+                self._state_reader = self._scheduler.create_state_reader(self)
             if not self._state_reader:
                 raise ConfigError(
                     "Invalid configuration: neither State Sync nor Reader has been configured"
                 )
         return self._state_reader
 
-    @property
-    def sqlmesh_path(self) -> Path:
-        """Path to the SQLMesh home directory."""
-        return Path.home() / ".sqlmesh"
-
-    @property
-    def models_directory_path(self) -> Path:
-        """Path to the directory where the models are defined"""
-        return self.path / "models"
-
-    @property
-    def macro_directory_path(self) -> Path:
-        """Path to the directory where macros are defined"""
-        return self.path / "macros"
-
-    @property
-    def hook_directory_path(self) -> Path:
-        """Path to the directory where hooks are defined"""
-        return self.path / "hooks"
-
-    @property
-    def test_directory_path(self) -> Path:
-        return self.path / "tests"
-
-    @property
-    def audits_directory_path(self) -> Path:
-        return self.path / "audits"
-
-    @property
-    def ignore_patterns(self) -> t.List[str]:
-        return c.IGNORE_PATTERNS + self.config.ignore_patterns
-
     def refresh(self) -> None:
         """Refresh all models that have been updated."""
         if self._loader.reload_needed():
             self.load()
 
     def load(self) -> Context:
         """Load all files in the context's path."""
-        with sys_path(self.path):
+        with sys_path(*self.configs):
             project = self._loader.load(self)
             self._hooks = project.hooks
             self._macros = project.macros
             self._models = project.models
             self._audits = project.audits
             self.dag = project.dag
 
@@ -413,14 +374,28 @@
         if not skip_janitor:
             self._run_janitor()
 
     def get_model(self, name: str) -> t.Optional[Model]:
         """Returns a model with the given name or None if a model with such name doesn't exist."""
         return self._models.get(name)
 
+    def config_for_path(self, path: Path) -> Config:
+        for config_path, config in self.configs.items():
+            try:
+                path.relative_to(config_path)
+                return config
+            except ValueError:
+                pass
+        return self.config
+
+    def config_for_model(self, model: str | Model) -> Config:
+        return self.config_for_path(
+            (model if isinstance(model, _Model) else self._models[model])._path
+        )
+
     @property
     def models(self) -> MappingProxyType[str, Model]:
         """Returns all registered models in this context."""
         return MappingProxyType(self._models)
 
     @property
     def macros(self) -> MappingProxyType[str, ExecutableOrMacro]:
@@ -435,40 +410,67 @@
     @property
     def snapshots(self) -> t.Dict[str, Snapshot]:
         """Generates and returns snapshots based on models registered in this context.
 
         If one of the snapshots has been previosly stored in the persisted state, the stored
         instance will be returned.
         """
-        local_snapshots = self.local_snapshots
-
-        stored_snapshots = self.state_reader.get_snapshots(
-            [s.snapshot_id for s in local_snapshots.values()]
+        prod = self.state_reader.get_environment(c.PROD)
+        remote_snapshots = (
+            {
+                snapshot.name: snapshot
+                for snapshot in self.state_reader.get_snapshots(prod.snapshots).values()
+            }
+            if prod
+            else {}
         )
 
-        return {name: stored_snapshots.get(s.snapshot_id, s) for name, s in local_snapshots.items()}
-
-    @property
-    def local_snapshots(self) -> t.Dict[str, Snapshot]:
-        """Generates and returns snapshots based on models registered in this context without reconciling them
-        with the persisted state.
-        """
-        local_snapshots = {}
         fingerprint_cache: t.Dict[str, SnapshotFingerprint] = {}
-        for model in self._models.values():
+        models = self._models.copy()
+        audits = self._audits.copy()
+        projects = {config.project for config in self.configs.values()}
+
+        for name, snapshot in remote_snapshots.items():
+            if name not in models and snapshot.project not in projects:
+                models[name] = snapshot.model
+
+                for audit in snapshot.audits:
+                    if name not in audits:
+                        audits[name] = audit
+
+        snapshots = {}
+
+        for model in models.values():
+            if model.name in remote_snapshots:
+                snapshot = remote_snapshots[model.name]
+                physical_schema = snapshot.physical_schema
+                ttl = snapshot.ttl
+                project = snapshot.project
+            else:
+                config = self.config_for_model(model)
+                physical_schema = config.physical_schema
+                ttl = config.snapshot_ttl
+                project = config.project
+
             snapshot = Snapshot.from_model(
                 model,
-                physical_schema=self.physical_schema,
-                models=self._models,
-                ttl=self.snapshot_ttl,
-                audits=self._audits,
+                models=models,
+                audits=audits,
                 cache=fingerprint_cache,
+                physical_schema=physical_schema,
+                ttl=ttl,
+                project=project,
             )
-            local_snapshots[model.name] = snapshot
-        return local_snapshots
+            snapshots[model.name] = snapshot
+
+        stored_snapshots = self.state_reader.get_snapshots(
+            [s.snapshot_id for s in snapshots.values() if not s.version]
+        )
+
+        return {name: stored_snapshots.get(s.snapshot_id, s) for name, s in snapshots.items()}
 
     def render(
         self,
         model_or_snapshot: ModelOrSnapshot,
         *,
         start: t.Optional[TimeLike] = None,
         end: t.Optional[TimeLike] = None,
@@ -557,15 +559,17 @@
 
     def format(self) -> None:
         """Format all models in a given directory."""
         for model in self._models.values():
             if not model.is_sql:
                 continue
             with open(model._path, "r+", encoding="utf-8") as file:
-                expressions = parse(file.read(), default_dialect=self.dialect)
+                expressions = parse(
+                    file.read(), default_dialect=self.config_for_model(model).dialect
+                )
                 file.seek(0)
                 file.write(format_model_expressions(expressions, model.dialect))
                 file.truncate()
 
     def plan(
         self,
         environment: t.Optional[str] = None,
@@ -624,26 +628,25 @@
                 "When targeting the production enviornment either the backfill should not be skipped or the lack of data gaps should be enforced (--no-gaps flag)."
             )
 
         self._run_plan_tests(skip_tests)
 
         plan = Plan(
             context_diff=self._context_diff(environment or c.PROD, create_from=create_from),
-            dag=self.dag,
             state_reader=self.state_reader,
             start=start,
             end=end,
             apply=self.apply,
             restate_models=restate_models,
             no_gaps=no_gaps,
             skip_backfill=skip_backfill,
             is_dev=environment != c.PROD,
             forward_only=forward_only,
-            environment_ttl=self.config.environment_ttl,
-            categorizer_config=self.config.auto_categorize_changes,
+            environment_ttl=self.environment_ttl,
+            categorizer_config=self.auto_categorize_changes,
             auto_categorization_enabled=not no_auto_categorization,
         )
 
         if not no_prompts:
             self.console.plan(plan, auto_apply)
         elif auto_apply:
             self.apply(plan)
@@ -659,15 +662,15 @@
         Args:
             plan: The plan to apply.
         """
         if not plan.context_diff.has_changes and not plan.requires_backfill:
             return
         if plan.uncategorized:
             raise PlanError("Can't apply a plan with uncategorized changes.")
-        self.config.scheduler.create_plan_evaluator(self).evaluate(plan)
+        self._scheduler.create_plan_evaluator(self).evaluate(plan)
 
     def diff(self, environment: t.Optional[str] = None, detailed: bool = False) -> None:
         """Show a diff of the current context with a given environment.
 
         Args:
             environment: The environment to diff against.
             detailed: Show the actual SQL differences if True.
@@ -734,32 +737,41 @@
         self,
         match_patterns: t.Optional[t.List[str]] = None,
         tests: t.Optional[t.List[str]] = None,
         verbose: bool = False,
     ) -> unittest.result.TestResult:
         """Discover and run model tests"""
         verbosity = 2 if verbose else 1
+
         try:
             if tests:
                 result = run_model_tests(
                     tests=tests,
-                    snapshots=self.local_snapshots,
+                    models=self._models,
                     engine_adapter=self._test_engine_adapter,
                     verbosity=verbosity,
                     patterns=match_patterns,
-                    ignore_patterns=self.ignore_patterns,
                 )
             else:
-                result = run_all_model_tests(
-                    path=self.test_directory_path,
-                    snapshots=self.local_snapshots,
+                test_meta = []
+
+                for path, config in self.configs.items():
+                    test_meta.extend(
+                        get_all_model_tests(
+                            path / c.TESTS,
+                            patterns=match_patterns,
+                            ignore_patterns=config.ignore_patterns,
+                        )
+                    )
+
+                result = run_tests(
+                    test_meta,
+                    models=self._models,
                     engine_adapter=self._test_engine_adapter,
                     verbosity=verbosity,
-                    patterns=match_patterns,
-                    ignore_patterns=self.ignore_patterns,
                 )
         finally:
             self._test_engine_adapter.close()
         return result
 
     def audit(
         self,
@@ -860,29 +872,35 @@
         self,
         environment: str | Environment,
         snapshots: t.Optional[t.Dict[str, Snapshot]] = None,
         create_from: t.Optional[str] = None,
     ) -> ContextDiff:
         environment = Environment.normalize_name(environment)
         return ContextDiff.create(
-            environment, snapshots or self.snapshots, create_from or c.PROD, self.state_reader
+            environment,
+            snapshots=snapshots or self.snapshots,
+            create_from=create_from or c.PROD,
+            state_reader=self.state_reader,
         )
 
-    def _load_config(self, config: t.Union[str, Config]) -> Config:
+    def _load_configs(
+        self, config: t.Union[str, Config], paths: t.List[Path]
+    ) -> t.Dict[Path, Config]:
         if isinstance(config, Config):
-            return config
+            return {path: config for path in paths}
+
+        lookup_paths = [self._sqlmesh_path / "config.yml", self._sqlmesh_path / "config.yaml"]
 
-        lookup_paths = [
-            self.sqlmesh_path / "config.yml",
-            self.sqlmesh_path / "config.yaml",
-            self.path / "config.py",
-            self.path / "config.yml",
-            self.path / "config.yaml",
-        ]
-        return load_config_from_paths(*lookup_paths, config_name=config)
+        return {
+            path: load_config_from_paths(
+                *(lookup_paths + [path / "config.py", path / "config.yml", path / "config.yaml"]),
+                config_name=config,
+            )
+            for path in paths
+        }
 
     def _add_model_to_dag(self, model: Model) -> None:
         self.dag.graph[model.name] = set()
 
         self.dag.add(model.name, model.depends_on)
 
     def _run_janitor(self) -> None:
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/context_diff.py` & `sqlmesh-0.5.0/sqlmesh/core/context_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/dialect.py` & `sqlmesh-0.5.0/sqlmesh/core/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,24 @@
     "databricks": DatabricksSparkSessionEngineAdapter,
     "redshift": RedshiftEngineAdapter,
     "postgres": PostgresEngineAdapter,
     "mysql": EngineAdapterWithIndexSupport,
     "mssql": EngineAdapterWithIndexSupport,
 }
 
+DIALECT_ALIASES = {
+    "postgresql": "postgres",
+}
+
 
 def create_engine_adapter(
     connection_factory: t.Callable[[], t.Any], dialect: str, multithreaded: bool = False
 ) -> EngineAdapter:
     dialect = dialect.lower()
-    if dialect == "postgresql":
-        dialect = "postgres"
+    dialect = DIALECT_ALIASES.get(dialect, dialect)
     if dialect == "databricks":
         try:
             from pyspark.sql import SparkSession
 
             spark = SparkSession.getActiveSession()
             if spark:
                 engine_adapter: t.Optional[
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         multithreaded: Indicates whether this adapter will be used by more than one thread.
     """
 
     DIALECT = ""
     DEFAULT_BATCH_SIZE = 10000
     DEFAULT_SQL_GEN_KWARGS: t.Dict[str, str | bool | int] = {}
     ESCAPE_JSON = False
+    SUPPORTS_INDEXES = False
     SCHEMA_DIFFER = SchemaDiffer()
 
     def __init__(
         self,
         connection_factory: t.Callable[[], t.Any],
         dialect: str = "",
         sql_gen_kwargs: t.Optional[t.Dict[str, Dialect | bool | str]] = None,
@@ -106,81 +107,93 @@
             columns_to_types: Only used if a dataframe is provided. A mapping between the column name and its data type.
                 Expected to be ordered to match the order of values in the dataframe.
         """
         table = exp.to_table(table_name)
         if isinstance(query_or_df, pd.DataFrame):
             if not columns_to_types:
                 raise ValueError("columns_to_types must be provided for dataframes")
-            expression = next(
-                self._pandas_to_sql(
-                    query_or_df,
-                    alias=table.alias_or_name,
-                    columns_to_types=columns_to_types,
-                )
-            )
-            create = exp.Create(
-                this=table,
-                kind="TABLE",
-                replace=True,
-                expression=expression,
-            )
+            return self._create_table_from_df(table, query_or_df, columns_to_types, replace=True)
         else:
-            create = exp.Create(
-                this=table,
-                kind="TABLE",
-                replace=True,
-                expression=query_or_df,
-            )
-        self.execute(create)
+            query_or_df = t.cast(Query, query_or_df)
+            return self._create_table_from_query(table, query_or_df, replace=True)
 
     def create_index(
         self,
         table_name: TableName,
         index_name: str,
         columns: t.Tuple[str, ...],
         exists: bool = True,
     ) -> None:
-        """Creates a new index for the given table.
+        """Creates a new index for the given table if supported
 
         Args:
             table_name: The name of the target table.
             index_name: The name of the index.
             columns: The list of columns that constitute the index.
             exists: Indicates whether to include the IF NOT EXISTS check.
         """
+        if not self.SUPPORTS_INDEXES:
+            return
+        expression = exp.Create(
+            this=exp.Index(
+                this=exp.to_identifier(index_name),
+                table=exp.to_table(table_name),
+                columns=exp.Tuple(
+                    expressions=[exp.to_column(c) for c in columns],
+                ),
+            ),
+            kind="INDEX",
+            exists=exists,
+        )
+        self.execute(expression)
 
     def create_table(
         self,
         table_name: TableName,
-        query_or_columns_to_types: Query | t.Dict[str, exp.DataType],
+        columns_to_types: t.Dict[str, exp.DataType],
         primary_key: t.Optional[t.Tuple[str, ...]] = None,
         exists: bool = True,
         **kwargs: t.Any,
     ) -> None:
-        """Create a table using a DDL statement or a CTAS.
-
-        If a query is passed in instead of column type map, CREATE TABLE AS will be used.
+        """Create a table using a DDL statement
 
         Args:
             table_name: The name of the table to create. Can be fully qualified or just table name.
-            query_or_columns_to_types: A query or mapping between the column name and its data type.
+            columns_to_types: A mapping between the column name and its data type.
             primary_key: Determines the table primary key.
             exists: Indicates whether to include the IF NOT EXISTS check.
             kwargs: Optional create table properties.
         """
-        if isinstance(query_or_columns_to_types, dict):
-            expression = self._create_table_from_columns(
-                table_name, query_or_columns_to_types, primary_key, exists, **kwargs
-            )
+        self._create_table_from_columns(table_name, columns_to_types, primary_key, exists, **kwargs)
+
+    def ctas(
+        self,
+        table_name: TableName,
+        query_or_df: QueryOrDF,
+        columns_to_types: t.Optional[t.Dict[str, exp.DataType]] = None,
+        exists: bool = True,
+        **kwargs: t.Any,
+    ) -> None:
+        """Create a table using a CTAS statement
+
+        Args:
+            table_name: The name of the table to create. Can be fully qualified or just table name.
+            query_or_df: The SQL query to run or a dataframe for the CTAS.
+            columns_to_types: A mapping between the column name and its data type. Required if using a DataFrame.
+            exists: Indicates whether to include the IF NOT EXISTS check.
+            kwargs: Optional create table properties.
+        """
+        if isinstance(query_or_df, QUERY_TYPES):
+            query_or_df = t.cast(Query, query_or_df)
+            self._create_table_from_query(table_name, query_or_df, exists, **kwargs)
         else:
-            expression = self._create_table_from_query(
-                table_name, query_or_columns_to_types, exists, **kwargs
-            )
-        if expression is not None:
-            self.execute(expression)
+            if not columns_to_types:
+                raise SQLMeshError("Must provide a column type map to do a CTAS with a DataFrame.")
+            query_or_df = t.cast(pd.DataFrame, query_or_df)
+            self._create_table_from_df(table_name, query_or_df, columns_to_types, exists, **kwargs)
 
     def create_state_table(
         self,
         table_name: str,
         columns_to_types: t.Dict[str, exp.DataType],
         primary_key: t.Optional[t.Tuple[str, ...]] = None,
     ) -> None:
@@ -200,66 +213,97 @@
     def _create_table_from_columns(
         self,
         table_name: TableName,
         columns_to_types: t.Dict[str, exp.DataType],
         primary_key: t.Optional[t.Tuple[str, ...]] = None,
         exists: bool = True,
         **kwargs: t.Any,
-    ) -> t.Optional[exp.Create]:
+    ) -> None:
         """
         Create a table using a DDL statement.
 
         Args:
             table_name: The name of the table to create. Can be fully qualified or just table name.
             columns_to_types: Mapping between the column name and its data type.
             exists: Indicates whether to include the IF NOT EXISTS check.
             kwargs: Optional create table properties.
         """
-        properties = self._create_table_properties(**kwargs)
-        schema: t.Optional[exp.Schema | exp.Table] = exp.to_table(table_name)
+        table = exp.to_table(table_name)
+        primary_key_expression = (
+            [exp.PrimaryKey(expressions=[exp.to_column(k) for k in primary_key])]
+            if primary_key and self.SUPPORTS_INDEXES
+            else []
+        )
         schema = exp.Schema(
-            this=schema,
+            this=table,
             expressions=[
                 exp.ColumnDef(this=exp.to_identifier(column), kind=kind)
                 for column, kind in columns_to_types.items()
-            ],
-        )
-        return exp.Create(
-            this=schema,
-            kind="TABLE",
-            exists=exists,
-            properties=properties,
-            expression=None,
+            ]
+            + primary_key_expression,
         )
+        self._create_table(schema, None, exists=exists, **kwargs)
 
     def _create_table_from_query(
         self,
         table_name: TableName,
         query: Query,
         exists: bool = True,
+        replace: bool = False,
         **kwargs: t.Any,
-    ) -> t.Optional[exp.Create]:
-        """
-        Create a table using a DDL statement.
+    ) -> None:
+        table = exp.to_table(table_name)
+        self._create_table(table, query, exists=exists, replace=replace, **kwargs)
 
-        Args:
-            table_name: The name of the table to create. Can be fully qualified or just table name.
-            query: The query to use for creating the table
-            exists: Indicates whether to include the IF NOT EXISTS check.
-            kwargs: Optional create table properties.
-        """
-        properties = self._create_table_properties(**kwargs)
-        schema: t.Optional[exp.Schema | exp.Table] = exp.to_table(table_name)
-        return exp.Create(
-            this=schema,
+    def _create_table_from_df(
+        self,
+        table_name: TableName,
+        df: DF,
+        columns_to_types: t.Dict[str, exp.DataType],
+        exists: bool = True,
+        replace: bool = False,
+        **kwargs: t.Any,
+    ) -> None:
+        table = exp.to_table(table_name)
+        if not columns_to_types:
+            raise ValueError("columns_to_types must be provided for dataframes")
+        if not isinstance(df, pd.DataFrame):
+            raise ValueError("df must be a pandas DataFrame")
+        expression = next(
+            self._pandas_to_sql(
+                df,
+                alias=table.alias_or_name,
+                columns_to_types=columns_to_types,
+            )
+        )
+        self._create_table(table_name, expression, exists=exists, replace=replace, **kwargs)
+
+    def _create_table(
+        self,
+        table_name_or_schema: t.Union[exp.Schema, TableName],
+        expression: t.Optional[exp.Expression],
+        exists: bool = True,
+        replace: bool = False,
+        properties: t.Optional[exp.Properties] = None,
+        **kwargs: t.Any,
+    ) -> None:
+        exists = False if replace else exists
+        if not isinstance(table_name_or_schema, exp.Schema):
+            table_name_or_schema = exp.to_table(table_name_or_schema)
+        if not properties and kwargs:
+            properties = self._create_table_properties(**kwargs)
+        create = exp.Create(
+            this=table_name_or_schema,
             kind="TABLE",
+            replace=replace,
             exists=exists,
+            expression=expression,
             properties=properties,
-            expression=query,
         )
+        self.execute(create)
 
     def create_table_like(
         self,
         target_table_name: TableName,
         source_table_name: TableName,
         exists: bool = True,
     ) -> None:
@@ -276,22 +320,22 @@
                 expressions=[
                     exp.LikeProperty(this=source_table),
                 ]
             ),
         )
         self.execute(create_expression)
 
-    def drop_table(self, table_name: str, exists: bool = True) -> None:
+    def drop_table(self, table_name: TableName, exists: bool = True) -> None:
         """Drops a table.
 
         Args:
             table_name: The name of the table to drop.
             exists: If exists, defaults to True.
         """
-        drop_expression = exp.Drop(this=table_name, kind="TABLE", exists=exists)
+        drop_expression = exp.Drop(this=exp.to_table(table_name), kind="TABLE", exists=exists)
         self.execute(drop_expression)
 
     def alter_table(
         self,
         current_table_name: TableName,
         target_table_name: TableName,
     ) -> None:
@@ -729,15 +773,14 @@
         kwargs defined for the given dialect, and then kwargs provided by the user when defining the engine
         adapter, and then finally kwargs provided by the user when calling this method.
         """
         sql_gen_kwargs = {
             "dialect": self.dialect,
             "pretty": False,
             "comments": False,
-            "identify": True,
             **self.DEFAULT_SQL_GEN_KWARGS,
             **self.sql_gen_kwargs,
             **kwargs,
         }
         return e.sql(**sql_gen_kwargs)  # type: ignore
 
     def _get_data_objects(
@@ -747,47 +790,8 @@
         Returns all the data objects that exist in the given schema and optionally catalog.
         """
 
         raise NotImplementedError()
 
 
 class EngineAdapterWithIndexSupport(EngineAdapter):
-    def create_index(
-        self,
-        table_name: TableName,
-        index_name: str,
-        columns: t.Tuple[str, ...],
-        exists: bool = True,
-    ) -> None:
-        expression = exp.Create(
-            this=exp.Index(
-                this=exp.to_identifier(index_name),
-                table=exp.to_table(table_name),
-                columns=exp.Tuple(
-                    expressions=[exp.to_column(c) for c in columns],
-                ),
-            ),
-            kind="INDEX",
-            exists=exists,
-        )
-        self.execute(expression)
-
-    def _create_table_from_columns(
-        self,
-        table_name: TableName,
-        columns_to_types: t.Dict[str, exp.DataType],
-        primary_key: t.Optional[t.Tuple[str, ...]] = None,
-        exists: bool = True,
-        **kwargs: t.Any,
-    ) -> t.Optional[exp.Create]:
-        expression = super()._create_table_from_columns(
-            table_name, columns_to_types, primary_key, exists, **kwargs
-        )
-        if expression is None or primary_key is None:
-            return expression
-
-        schema = expression.this
-        schema.append(
-            "expressions",
-            exp.Anonymous(this="PRIMARY KEY", expressions=[exp.to_column(k) for k in primary_key]),
-        )
-        return expression
+    SUPPORTS_INDEXES = True
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class DatabricksSQLEngineAdapter(BaseSparkEngineAdapter):
     DIALECT = "databricks"
     SCHEMA_DIFFER = SchemaDiffer(
         support_positional_add=True,
         support_nested_operations=True,
-        array_suffix=".element",
+        array_element_selector="element",
     )
 
     def _fetch_native_df(self, query: t.Union[exp.Expression, str]) -> DF:
         """
         Returns a Pandas DataFrame from a query or expression.
         """
         self.execute(query)
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/redshift.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 import uuid
 
 import pandas as pd
 from sqlglot import exp
 
 from sqlmesh.core.dialect import pandas_to_sql
 from sqlmesh.core.engine_adapter._typing import DF_TYPES, Query
-from sqlmesh.core.engine_adapter.postgres import PostgresBaseEngineAdapter
-from sqlmesh.core.engine_adapter.shared import DataObject
+from sqlmesh.core.engine_adapter.base_postgres import BasePostgresEngineAdapter
 
 if t.TYPE_CHECKING:
     from sqlmesh.core._typing import TableName
     from sqlmesh.core.engine_adapter._typing import QueryOrDF
 
 
-class RedshiftEngineAdapter(PostgresBaseEngineAdapter):
+class RedshiftEngineAdapter(BasePostgresEngineAdapter):
     DIALECT = "redshift"
     DEFAULT_BATCH_SIZE = 1000
 
     @property
     def cursor(self) -> t.Any:
         connection = self._connection_pool.get()
         # The SQLMesh implementation relies on autocommit being set to True
@@ -64,27 +63,28 @@
         return self.cursor.fetch_dataframe()
 
     def _create_table_from_query(
         self,
         table_name: TableName,
         query: Query,
         exists: bool = True,
+        replace: bool = False,
         **kwargs: t.Any,
-    ) -> t.Optional[exp.Create]:
+    ) -> None:
         """
         Redshift doesn't support `CREATE TABLE IF NOT EXISTS AS...` but does support `CREATE TABLE AS...` so
         we check if the exists check exists and if not then we can use the base implementation. Otherwise we
         manually check if it exists and if it does then this is a no-op anyways so we return and if it doesn't
         then we run the query with exists set to False since we just confirmed it doesn't exist.
         """
         if not exists:
             return super()._create_table_from_query(table_name, query, exists, **kwargs)
         if self.table_exists(table_name):
-            return None
-        return self._create_table_from_query(table_name, query, exists=False, **kwargs)
+            return
+        super()._create_table_from_query(table_name, query, exists=False, **kwargs)
 
     @classmethod
     def _pandas_to_sql(
         cls,
         df: pd.DataFrame,
         columns_to_types: t.Dict[str, exp.DataType],
         batch_size: int = 0,
@@ -102,23 +102,25 @@
     def replace_query(
         self,
         table_name: TableName,
         query_or_df: QueryOrDF,
         columns_to_types: t.Optional[t.Dict[str, exp.DataType]] = None,
     ) -> None:
         """
-        Redshift doesn't support `CREATE OR REPLACE TABLE...` with `VALUES` expression so we need to specially
+        Redshift doesn't support `CREATE OR REPLACE TABLE...` and it also doesn't support `VALUES` expression so we need to specially
         handle DataFrame replacements.
 
         If the table doesn't exist then we just create it and load it with insert statements
         If it does exist then we need to do the:
             `CREATE TABLE...`, `INSERT INTO...`, `RENAME TABLE...`, `RENAME TABLE...`, DROP TABLE...`  dance.
         """
         if not isinstance(query_or_df, pd.DataFrame):
-            return super().replace_query(table_name, query_or_df, columns_to_types)
+            with self.transaction():
+                self.drop_table(table_name, exists=True)
+                return self.ctas(table_name, query_or_df, columns_to_types)
         if not columns_to_types:
             raise ValueError("columns_to_types must be provided for dataframes")
         target_table = exp.to_table(table_name)
         target_exists = self.table_exists(target_table)
         if target_exists:
             with self.transaction():
                 temp_table_name = f"{target_table.alias_or_name}_temp_{self._short_hash()}"
@@ -140,39 +142,7 @@
             for expression in self._pandas_to_sql(
                 query_or_df, columns_to_types, self.DEFAULT_BATCH_SIZE
             ):
                 self._insert_append_query(target_table, expression, columns_to_types)
 
     def _short_hash(self) -> str:
         return uuid.uuid4().hex[:8]
-
-    def _get_data_objects(
-        self, schema_name: str, catalog_name: t.Optional[str] = None
-    ) -> t.List[DataObject]:
-        """
-        Returns all the data objects that exist in the given schema and optionally catalog.
-        """
-        catalog_name = f"'{catalog_name}'" if catalog_name else "NULL"
-        query = f"""
-            SELECT
-                {catalog_name} AS catalog_name,
-                tablename AS name,
-                schemaname AS schema_name,
-                'TABLE' AS type
-            FROM pg_tables
-            WHERE schemaname ILIKE '{schema_name}'
-            UNION ALL
-            SELECT
-                {catalog_name} AS catalog_name,
-                viewname AS name,
-                schemaname AS schema_name,
-                'VIEW' AS type
-            FROM pg_views
-            WHERE schemaname ILIKE '{schema_name}'
-        """
-        df = self.fetchdf(query)
-        return [
-            DataObject(
-                catalog=row.catalog_name, schema=row.schema_name, name=row.name, type=row.type  # type: ignore
-            )
-            for row in df.itertuples()
-        ]
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.5.0/sqlmesh/core/engine_adapter/spark.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,14 +83,28 @@
         if isinstance(table_name, exp.Table):
             table_name = table_name.sql(dialect=self.dialect)
 
         df.select(*self.spark.table(table_name).columns).write.insertInto(  # type: ignore
             table_name, overwrite=overwrite
         )
 
+    def _create_table_from_df(
+        self,
+        table_name: TableName,
+        df: DF,
+        columns_to_types: t.Dict[str, exp.DataType],
+        exists: bool = True,
+        replace: bool = True,
+        **kwargs: t.Any,
+    ) -> None:
+        df = self._ensure_pyspark_df(df)
+        if isinstance(table_name, exp.Table):
+            table_name = table_name.sql(dialect=self.dialect)
+        df.write.saveAsTable(table_name, mode="overwrite")
+
     def _get_data_objects(
         self, schema_name: str, catalog_name: t.Optional[str] = None
     ) -> t.List[DataObject]:
         target = nullsafe_join(".", catalog_name, schema_name)
         df = self.fetch_pyspark_df(f"SHOW TABLE EXTENDED IN {target} LIKE '*'")
         return [
             DataObject(
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/environment.py` & `sqlmesh-0.5.0/sqlmesh/core/environment.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/hooks.py` & `sqlmesh-0.5.0/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/loader.py` & `sqlmesh-0.5.0/sqlmesh/core/loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from __future__ import annotations
 
 import abc
 import importlib
+import itertools
 import linecache
 import os
 import sys
 import types
 import typing as t
 from dataclasses import dataclass
 from pathlib import Path
 
 from sqlglot.errors import SqlglotError
 from sqlglot.schema import MappingSchema
 
+from sqlmesh.core import constants as c
 from sqlmesh.core.audit import Audit
 from sqlmesh.core.dialect import parse
 from sqlmesh.core.hooks import HookRegistry, hook
 from sqlmesh.core.macros import MacroRegistry, macro
 from sqlmesh.core.model import Model, SeedModel, load_model
 from sqlmesh.core.model import model as model_registry
 from sqlmesh.utils import UniqueKeyDict
 from sqlmesh.utils.dag import DAG
 from sqlmesh.utils.errors import ConfigError
 
 if t.TYPE_CHECKING:
+    from sqlmesh.core.config import Config
     from sqlmesh.core.context import Context
 
 
-def update_model_schemas(dialect: str, dag: DAG[str], models: UniqueKeyDict[str, Model]) -> None:
-    schema = MappingSchema(dialect=dialect)
+def update_model_schemas(dag: DAG[str], models: UniqueKeyDict[str, Model]) -> None:
+    schema = MappingSchema()
     for name in dag.sorted():
         model = models.get(name)
 
         # External models don't exist in the context, so we need to skip them
         if not model:
             continue
 
@@ -76,15 +79,15 @@
         self._path_mtimes.clear()
         self._dag = DAG()
 
         macros, hooks = self._load_scripts()
         models = self._load_models(macros, hooks)
         for model in models.values():
             self._add_model_to_dag(model)
-        update_model_schemas(self._context.dialect, self._dag, models)
+        update_model_schemas(self._dag, models)
 
         audits = self._load_audits()
 
         project = LoadedProject(
             macros=macros, hooks=hooks, models=models, audits=audits, dag=self._dag
         )
         return project
@@ -128,19 +131,21 @@
 
     def _load_scripts(self) -> t.Tuple[MacroRegistry, HookRegistry]:
         """Loads all user defined hooks and macros."""
         # Store a copy of the macro registry
         standard_hooks = hook.get_registry()
         standard_macros = macro.get_registry()
 
-        for path in tuple(self._glob_path(self._context.macro_directory_path, ".py")) + tuple(
-            self._glob_path(self._context.hook_directory_path, ".py")
-        ):
-            if self._import_python_file(path.relative_to(self._context.path)):
-                self._track_file(path)
+        for context_path, config in self._context.configs.items():
+            for path in itertools.chain(
+                self._glob_paths(context_path / c.MACROS, config=config, extension=".py"),
+                self._glob_paths(context_path / c.HOOKS, config=config, extension=".py"),
+            ):
+                if self._import_python_file(path, context_path):
+                    self._track_file(path)
 
         hooks = hook.get_registry()
         macros = macro.get_registry()
 
         hook.set_registry(standard_hooks)
         macro.set_registry(standard_macros)
 
@@ -157,98 +162,106 @@
         return models
 
     def _load_sql_models(
         self, macros: MacroRegistry, hooks: HookRegistry
     ) -> UniqueKeyDict[str, Model]:
         """Loads the sql models into a Dict"""
         models: UniqueKeyDict = UniqueKeyDict("models")
-        for path in self._glob_path(self._context.models_directory_path, ".sql"):
-            self._track_file(path)
-            with open(path, "r", encoding="utf-8") as file:
-                try:
-                    expressions = parse(file.read(), default_dialect=self._context.dialect)
-                except SqlglotError as ex:
-                    raise ConfigError(f"Failed to parse a model definition at '{path}': {ex}")
-                model = load_model(
-                    expressions,
-                    defaults=self._context.config.model_defaults.dict(),
-                    macros=macros,
-                    hooks=hooks,
-                    path=Path(path).absolute(),
-                    module_path=self._context.path,
-                    dialect=self._context.dialect,
-                    time_column_format=self._context.config.time_column_format,
-                )
-                models[model.name] = model
-
-                if isinstance(model, SeedModel):
-                    seed_path = model.seed_path
-                    self._track_file(seed_path)
+        for context_path, config in self._context.configs.items():
+            for path in self._glob_paths(context_path / c.MODELS, config=config, extension=".sql"):
+                self._track_file(path)
+                with open(path, "r", encoding="utf-8") as file:
+                    try:
+                        expressions = parse(
+                            file.read(), default_dialect=config.model_defaults.dialect
+                        )
+                    except SqlglotError as ex:
+                        raise ConfigError(f"Failed to parse a model definition at '{path}': {ex}")
+                    model = load_model(
+                        expressions,
+                        defaults=config.model_defaults.dict(),
+                        macros=macros,
+                        hooks=hooks,
+                        path=Path(path).absolute(),
+                        module_path=context_path,
+                        dialect=config.model_defaults.dialect,
+                        time_column_format=config.time_column_format,
+                    )
+                    models[model.name] = model
+
+                    if isinstance(model, SeedModel):
+                        seed_path = model.seed_path
+                        self._track_file(seed_path)
 
         return models
 
     def _load_python_models(self) -> UniqueKeyDict[str, Model]:
         """Loads the python models into a Dict"""
         models: UniqueKeyDict = UniqueKeyDict("models")
         registry = model_registry.registry()
         registry.clear()
         registered: t.Set[str] = set()
 
-        for path in self._glob_path(self._context.models_directory_path, ".py"):
-            self._track_file(path)
-            self._import_python_file(path.relative_to(self._context.path))
-            new = registry.keys() - registered
-            registered |= new
-            for name in new:
-                model = registry[name].model(
-                    path=path,
-                    module_path=self._context.path,
-                    defaults=self._context.config.model_defaults.dict(),
-                    time_column_format=self._context.config.time_column_format,
-                )
-                models[model.name] = model
+        for context_path, config in self._context.configs.items():
+            for path in self._glob_paths(context_path / c.MODELS, config=config, extension=".py"):
+                self._track_file(path)
+                self._import_python_file(path, context_path)
+                new = registry.keys() - registered
+                registered |= new
+                for name in new:
+                    model = registry[name].model(
+                        path=path,
+                        module_path=context_path,
+                        defaults=config.model_defaults.dict(),
+                        time_column_format=config.time_column_format,
+                    )
+                    models[model.name] = model
 
         return models
 
     def _load_audits(self) -> UniqueKeyDict[str, Audit]:
         """Loads all the model audits."""
         audits_by_name: UniqueKeyDict[str, Audit] = UniqueKeyDict("audits")
-        for path in self._glob_path(self._context.audits_directory_path, ".sql"):
-            self._track_file(path)
-            with open(path, "r", encoding="utf-8") as file:
-                expressions = parse(file.read(), default_dialect=self._context.dialect)
-                audits = Audit.load_multiple(
-                    expressions=expressions,
-                    path=path,
-                    dialect=self._context.dialect,
-                )
-                for audit in audits:
-                    audits_by_name[audit.name] = audit
+        for context_path, config in self._context.configs.items():
+            for path in self._glob_paths(context_path / c.AUDITS, config=config, extension=".sql"):
+                self._track_file(path)
+                with open(path, "r", encoding="utf-8") as file:
+                    expressions = parse(file.read(), default_dialect=config.model_defaults.dialect)
+                    audits = Audit.load_multiple(
+                        expressions=expressions,
+                        path=path,
+                        dialect=config.model_defaults.dialect,
+                    )
+                    for audit in audits:
+                        audits_by_name[audit.name] = audit
         return audits_by_name
 
-    def _import_python_file(self, relative_path: Path) -> types.ModuleType:
+    def _import_python_file(self, file: Path, context_path: Path) -> types.ModuleType:
+        relative_path = file.relative_to(context_path)
         module_name = str(relative_path.with_suffix("")).replace(os.path.sep, ".")
         # remove the entire module hierarchy in case they were already loaded
         parts = module_name.split(".")
         for i in range(len(parts)):
             sys.modules.pop(".".join(parts[0 : i + 1]), None)
 
         return importlib.import_module(module_name)
 
-    def _glob_path(self, path: Path, file_extension: str) -> t.Generator[Path, None, None]:
+    def _glob_paths(
+        self, path: Path, config: Config, extension: str
+    ) -> t.Generator[Path, None, None]:
         """
         Globs the provided path for the file extension but also removes any filepaths that match an ignore
         pattern either set in constants or provided in config
 
         Args:
             path: The filepath to glob
-            file_extension: The extension to check for in that path (checks recursively in zero or more subdirectories)
+            extension: The extension to check for in that path (checks recursively in zero or more subdirectories)
 
         Returns:
             Matched paths that are not ignored
         """
-        for filepath in path.glob(f"**/*{file_extension}"):
-            for ignore_pattern in self._context.ignore_patterns:
+        for filepath in path.glob(f"**/*{extension}"):
+            for ignore_pattern in config.ignore_patterns:
                 if filepath.match(ignore_pattern):
                     break
             else:
                 yield filepath
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/macros.py` & `sqlmesh-0.5.0/sqlmesh/core/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/model/__init__.py` & `sqlmesh-0.5.0/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/model/common.py` & `sqlmesh-0.5.0/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/model/decorator.py` & `sqlmesh-0.5.0/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/model/definition.py` & `sqlmesh-0.5.0/sqlmesh/core/model/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/model/kind.py` & `sqlmesh-0.5.0/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/model/meta.py` & `sqlmesh-0.5.0/sqlmesh/core/model/meta.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/model/seed.py` & `sqlmesh-0.5.0/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/notification_target.py` & `sqlmesh-0.5.0/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/plan/definition.py` & `sqlmesh-0.5.0/sqlmesh/core/plan/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from sqlmesh.utils.date import (
     TimeLike,
     make_inclusive,
     make_inclusive_end,
     now,
     to_date,
     to_datetime,
+    to_ds,
     to_timestamp,
     validate_date_range,
     yesterday_ds,
 )
 from sqlmesh.utils.errors import PlanError, SQLMeshError
 from sqlmesh.utils.pydantic import PydanticModel
 
@@ -38,15 +39,14 @@
 
 
 class Plan:
     """Plan is the main class to represent user choices on how they want to backfill and version their models.
 
     Args:
         context_diff: The context diff that the plan is based on.
-        dag: The dag object to determine relationships.
         state_reader: The state_reader to get metadata with.
         start: The start time to backfill data.
         end: The end time to backfill data.
         apply: The callback to apply the plan.
         restate_models: A list of models for which the data should be restated for the time range
             specified in this plan. Note: models defined outside SQLMesh (external) won't be a part
             of the restatement.
@@ -60,15 +60,14 @@
         categorizer_config: Auto categorization settings.
         auto_categorization_enabled: Whether to apply auto categorization.
     """
 
     def __init__(
         self,
         context_diff: ContextDiff,
-        dag: DAG,
         state_reader: StateReader,
         start: t.Optional[TimeLike] = None,
         end: t.Optional[TimeLike] = None,
         apply: t.Optional[t.Callable[[Plan], None]] = None,
         restate_models: t.Optional[t.Iterable[str]] = None,
         no_gaps: bool = False,
         skip_backfill: bool = False,
@@ -88,15 +87,20 @@
         self.forward_only = forward_only
         self.environment_ttl = environment_ttl
         self.categorizer_config = categorizer_config or CategorizerConfig()
         self.auto_categorization_enabled = auto_categorization_enabled
         self._start = start if start or not (is_dev and forward_only) else yesterday_ds()
         self._end = end if end or not is_dev else now()
         self._apply = apply
-        self._dag = dag
+        self._dag: DAG[str] = DAG()
+
+        for name, snapshot in self.context_diff.snapshots.items():
+            self._dag.graph[name] = set()
+            self._dag.add(name, snapshot.model.depends_on)
+
         self._state_reader = state_reader
         self.__missing_intervals: t.Optional[t.Dict[str, Intervals]] = None
         self._restatements: t.Set[str] = set()
 
         if restate_models and context_diff.new_snapshots:
             raise PlanError(
                 "Model changes and restatements can't be a part of the same plan. "
@@ -572,16 +576,19 @@
     snapshot_name: str
     intervals: Intervals
 
     @property
     def merged_intervals(self) -> Intervals:
         return merge_intervals(self.intervals)
 
-    def format_missing_range(self) -> str:
+    def format_missing_range(self, unit: t.Optional[IntervalUnit] = None) -> str:
         intervals = [make_inclusive(start, end) for start, end in self.merged_intervals]
         return ", ".join(
-            f"({_format_date_time(start)}, {_format_date_time(end)})" for start, end in intervals
+            f"({_format_date_time(start, unit)}, {_format_date_time(end, unit)})"
+            for start, end in intervals
         )
 
 
-def _format_date_time(time_like: TimeLike) -> str:
+def _format_date_time(time_like: TimeLike, unit: t.Optional[IntervalUnit]) -> str:
+    if unit is None or unit == IntervalUnit.DAY:
+        return to_ds(time_like)
     return to_datetime(time_like).isoformat()[:19]
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.5.0/sqlmesh/core/plan/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/renderer.py` & `sqlmesh-0.5.0/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/scheduler.py` & `sqlmesh-0.5.0/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/schema_diff.py` & `sqlmesh-0.5.0/sqlmesh/core/schema_diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,81 +28,105 @@
 
 
 class TableAlterColumn(PydanticModel):
     name: str
     is_struct: bool
     is_array_of_struct: bool
     is_array_of_primitive: bool
+    quoted: bool = False
 
     @classmethod
-    def primitive(self, name: str) -> TableAlterColumn:
+    def primitive(self, name: str, quoted: bool = False) -> TableAlterColumn:
         return self(
-            name=name, is_struct=False, is_array_of_struct=False, is_array_of_primitive=False
+            name=name,
+            is_struct=False,
+            is_array_of_struct=False,
+            is_array_of_primitive=False,
+            quoted=quoted,
         )
 
     @classmethod
-    def struct(self, name: str) -> TableAlterColumn:
+    def struct(self, name: str, quoted: bool = False) -> TableAlterColumn:
         return self(
-            name=name, is_struct=True, is_array_of_struct=False, is_array_of_primitive=False
+            name=name,
+            is_struct=True,
+            is_array_of_struct=False,
+            is_array_of_primitive=False,
+            quoted=quoted,
         )
 
     @classmethod
-    def array_of_struct(self, name: str) -> TableAlterColumn:
+    def array_of_struct(self, name: str, quoted: bool = False) -> TableAlterColumn:
         return self(
-            name=name, is_struct=False, is_array_of_struct=True, is_array_of_primitive=False
+            name=name,
+            is_struct=False,
+            is_array_of_struct=True,
+            is_array_of_primitive=False,
+            quoted=quoted,
         )
 
     @classmethod
-    def array_of_primitive(self, name: str) -> TableAlterColumn:
+    def array_of_primitive(self, name: str, quoted: bool = False) -> TableAlterColumn:
         return self(
-            name=name, is_struct=False, is_array_of_struct=False, is_array_of_primitive=True
+            name=name,
+            is_struct=False,
+            is_array_of_struct=False,
+            is_array_of_primitive=True,
+            quoted=quoted,
         )
 
     @classmethod
     def from_struct_kwarg(self, struct: exp.StructKwarg) -> TableAlterColumn:
         name = struct.alias_or_name
+        quoted = struct.this.quoted
         if struct.expression.is_type(exp.DataType.Type.STRUCT):
-            return self.struct(name)
+            return self.struct(name, quoted=quoted)
         elif struct.expression.is_type(exp.DataType.Type.ARRAY):
             if struct.expression.expressions[0].is_type(exp.DataType.Type.STRUCT):
-                return self.array_of_struct(name)
+                return self.array_of_struct(name, quoted=quoted)
             else:
-                return self.array_of_primitive(name)
+                return self.array_of_primitive(name, quoted=quoted)
         else:
-            return self.primitive(name)
+            return self.primitive(name, quoted=quoted)
 
     @property
     def is_array(self) -> bool:
         return self.is_array_of_struct or self.is_array_of_primitive
 
     @property
     def is_primitive(self) -> bool:
         return not self.is_struct and not self.is_array
 
     @property
     def is_nested(self) -> bool:
         return not self.is_primitive
 
+    @property
+    def identifier(self) -> exp.Identifier:
+        return exp.to_identifier(self.name, quoted=self.quoted)
+
 
 class TableAlterColumnPosition(PydanticModel):
     is_first: bool
     is_last: bool
-    after: t.Optional[str] = None
+    after: t.Optional[exp.Identifier] = None
 
     @classmethod
     def first(self) -> TableAlterColumnPosition:
         return self(is_first=True, is_last=False, after=None)
 
     @classmethod
-    def last(self, after: t.Optional[str] = None) -> TableAlterColumnPosition:
-        return self(is_first=False, is_last=True, after=after)
+    def last(
+        self, after: t.Optional[t.Union[str, exp.Identifier]] = None
+    ) -> TableAlterColumnPosition:
+        return self(is_first=False, is_last=True, after=exp.to_identifier(after) if after else None)
 
     @classmethod
-    def middle(self, after: str) -> TableAlterColumnPosition:
-        return self(is_first=False, is_last=False, after=after)
+    def middle(self, after: t.Union[str, exp.Identifier]) -> TableAlterColumnPosition:
+        return self(is_first=False, is_last=False, after=exp.to_identifier(after))
 
     @classmethod
     def create(
         self,
         pos: int,
         current_kwargs: t.List[exp.StructKwarg],
         replacing_col: bool = False,
@@ -113,15 +137,15 @@
         if not is_first:
             prior_kwarg = current_kwargs[pos - 1]
             after, _ = _get_name_and_type(prior_kwarg)
         return self(is_first=is_first, is_last=is_last, after=after)
 
     @property
     def column_position_node(self) -> t.Optional[exp.ColumnPosition]:
-        column = exp.column(self.after) if self.after and not self.is_last else None
+        column = self.after if not self.is_last else None
         position = None
         if self.is_first:
             position = "FIRST"
         elif column and not self.is_last:
             position = "AFTER"
         return exp.ColumnPosition(this=column, position=position)
 
@@ -191,53 +215,57 @@
     def is_drop(self) -> bool:
         return self.op.is_drop
 
     @property
     def is_alter_type(self) -> bool:
         return self.op.is_alter_type
 
-    def full_column_path(self, array_suffix: str) -> str:
+    def column_identifiers(self, array_element_selector: str) -> t.List[exp.Identifier]:
         results = []
         for column in self.columns:
-            if column.is_array_of_struct and len(self.columns) > 1:
-                results.append(column.name + array_suffix)
-            else:
-                results.append(column.name)
-        return ".".join(results)
-
-    def column(self, array_suffix: str) -> exp.Column:
-        return exp.column(self.full_column_path(array_suffix))
+            results.append(column.identifier)
+            if column.is_array_of_struct and len(self.columns) > 1 and array_element_selector:
+                results.append(exp.to_identifier(array_element_selector))
+        return results
+
+    def column(self, array_element_selector: str) -> t.Union[exp.Dot, exp.Identifier]:
+        columns = self.column_identifiers(array_element_selector)
+        if len(columns) == 1:
+            return columns[0]
+        return exp.Dot.build(columns)
 
-    def column_def(self, array_suffix: str) -> exp.ColumnDef:
+    def column_def(self, array_element_selector: str) -> exp.ColumnDef:
         return exp.ColumnDef(
-            this=exp.to_identifier(self.full_column_path(array_suffix)),
+            this=self.column(array_element_selector),
             kind=self.column_type,
         )
 
-    def expression(self, table_name: t.Union[str, exp.Table], array_suffix: str) -> exp.AlterTable:
+    def expression(
+        self, table_name: t.Union[str, exp.Table], array_element_selector: str
+    ) -> exp.AlterTable:
         if self.is_alter_type:
             return exp.AlterTable(
                 this=exp.to_table(table_name),
                 actions=[
                     exp.AlterColumn(
-                        this=self.column(array_suffix),
+                        this=self.column(array_element_selector),
                         dtype=self.column_type,
                     )
                 ],
             )
         elif self.is_add:
             alter_table = exp.AlterTable(this=exp.to_table(table_name))
-            column = self.column_def(array_suffix)
+            column = self.column_def(array_element_selector)
             alter_table.set("actions", [column])
             if self.add_position:
                 column.set("position", self.add_position.column_position_node)
             return alter_table
         elif self.is_drop:
             alter_table = exp.AlterTable(this=exp.to_table(table_name))
-            drop_column = exp.Drop(this=self.column(array_suffix), kind="COLUMN")
+            drop_column = exp.Drop(this=self.column(array_element_selector), kind="COLUMN")
             alter_table.set("actions", [drop_column])
             return alter_table
         else:
             raise ValueError(f"Unknown operation {self.op}")
 
 
 class SchemaDiffer(PydanticModel):
@@ -256,15 +284,15 @@
     Potential future improvements:
     1. Support precision changes on columns like VARCHAR and DECIMAL. Each engine has different rules on what is allowed
     2. Support column moves. Databricks Delta supports moves and would allow exact matches.
     """
 
     support_positional_add: bool = False
     support_nested_operations: bool = False
-    array_suffix: str = ""
+    array_element_selector: str = ""
     compatible_types: t.Dict[exp.DataType, t.Set[exp.DataType]] = {}
 
     @classmethod
     def _dict_to_struct(cls, value: t.Dict[str, exp.DataType]) -> exp.DataType:
         return exp.DataType(
             this=exp.DataType.Type.STRUCT,
             expressions=[
@@ -283,28 +311,28 @@
     def _get_matching_kwarg(
         self,
         current_kwarg: t.Union[str, exp.StructKwarg],
         new_struct: exp.DataType,
         current_pos: int,
     ) -> t.Tuple[t.Optional[int], t.Optional[exp.StructKwarg]]:
         current_name = (
-            current_kwarg
+            exp.to_identifier(current_kwarg)
             if isinstance(current_kwarg, str)
             else _get_name_and_type(current_kwarg)[0]
         )
         # First check if we have the same column in the same position to get O(1) complexity
         new_kwarg = seq_get(new_struct.expressions, current_pos)
         if new_kwarg:
             new_name, new_type = _get_name_and_type(new_kwarg)
-            if current_name == new_name:
+            if current_name.this == new_name.this:
                 return current_pos, new_kwarg
         # If not, check if we have the same column in all positions with O(n) complexity
         for i, new_kwarg in enumerate(new_struct.expressions):
             new_name, new_type = _get_name_and_type(new_kwarg)
-            if current_name == new_name:
+            if current_name.this == new_name.this:
                 return i, new_kwarg
         return None, None
 
     def _drop_operation(
         self,
         columns: t.Union[TableAlterColumn, t.List[TableAlterColumn]],
         struct: exp.DataType,
@@ -495,15 +523,16 @@
             current: The current schema.
             new: The new schema.
 
         Returns:
             The list of table alter operations.
         """
         return [
-            op.expression(table_name, self.array_suffix) for op in self._from_structs(current, new)
+            op.expression(table_name, self.array_element_selector)
+            for op in self._from_structs(current, new)
         ]
 
     def compare_columns(
         self,
         table_name: t.Union[str, exp.Table],
         current: t.Dict[str, exp.DataType],
         new: t.Dict[str, exp.DataType],
@@ -519,9 +548,9 @@
             The list of schema deltas.
         """
         return self.compare_structs(
             table_name, self._dict_to_struct(current), self._dict_to_struct(new)
         )
 
 
-def _get_name_and_type(struct: exp.StructKwarg) -> t.Tuple[str, exp.DataType]:
-    return struct.alias_or_name, struct.expression
+def _get_name_and_type(struct: exp.StructKwarg) -> t.Tuple[exp.Identifier, exp.DataType]:
+    return struct.this, struct.expression
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.5.0/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.5.0/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.5.0/sqlmesh/core/snapshot/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,16 @@
 
         fingerprint: A unique hash of the model definition so that models can be reused across environments.
         physical_schema: The physical schema that the snapshot is stored in.
         model: Model object that the snapshot encapsulates.
         parents: The list of parent snapshots (upstream dependencies).
         audits: The list of audits used by the model.
         intervals: List of [start, end) intervals showing which time ranges a snapshot has data for.
+        dev_intervals: List of [start, end) intervals showing development intervals (forward-only).
+        project: The name of the project this snapshot is associated with.
         created_ts: Epoch millis timestamp when a snapshot was first created.
         updated_ts: Epoch millis timestamp when a snapshot was last updated.
         ttl: The time-to-live of a snapshot determines when it should be deleted after it's no longer referenced
             in any environment.
         previous: The snapshot data version that this snapshot was based on. If this snapshot is new, then previous will be None.
         version: User specified version for a snapshot that is used for physical storage.
             By default, the version is the fingerprint, but not all changes to models require a backfill.
@@ -282,14 +284,15 @@
     fingerprint: SnapshotFingerprint
     physical_schema: str
     model: Model
     parents: t.Tuple[SnapshotId, ...]
     audits: t.Tuple[Audit, ...]
     intervals: Intervals
     dev_intervals: Intervals
+    project: str = ""
     created_ts: int
     updated_ts: int
     ttl: str
     previous_versions: t.Tuple[SnapshotDataVersion, ...] = ()
     indirect_versions: t.Dict[str, t.Tuple[SnapshotDataVersion, ...]] = {}
     version: t.Optional[str] = None
     change_category: t.Optional[SnapshotChangeCategory] = None
@@ -342,17 +345,18 @@
         return merged
 
     @classmethod
     def from_model(
         cls,
         model: Model,
         *,
-        physical_schema: str,
         models: t.Dict[str, Model],
+        physical_schema: str = c.SQLMESH,
         ttl: str = c.DEFAULT_SNAPSHOT_TTL,
+        project: str = "",
         version: t.Optional[str] = None,
         audits: t.Optional[t.Dict[str, Audit]] = None,
         cache: t.Optional[t.Dict[str, SnapshotFingerprint]] = None,
     ) -> Snapshot:
         """Creates a new snapshot for a model.
 
         Args:
@@ -395,14 +399,15 @@
                     ).to_identifier(),
                 )
                 for name in _parents_from_model(model, models)
             ),
             audits=tuple(model.referenced_audits(audits)),
             intervals=[],
             dev_intervals=[],
+            project=project,
             created_ts=created_ts,
             updated_ts=created_ts,
             ttl=ttl,
             version=version,
         )
 
     def __eq__(self, other: t.Any) -> bool:
@@ -444,22 +449,34 @@
             start: Start interval to remove.
             end: End interval to remove.
         """
         interval = self._inclusive_exclusive(start, end)
         self.intervals = remove_interval(self.intervals, *interval)
         self.dev_intervals = remove_interval(self.dev_intervals, *interval)
 
-    def _inclusive_exclusive(self, start: TimeLike, end: TimeLike) -> t.Tuple[int, int]:
+    def _inclusive_exclusive(
+        self, start: TimeLike, end: TimeLike, strict: bool = True
+    ) -> t.Tuple[int, int]:
+        """Transform the inclusive start and end into a [start, end) pair.
+
+        Args:
+            start: The start date/time of the interval (inclusive)
+            end: The end date/time of the interval (inclusive)
+            strict: Whether to fail when the inclusive start is the same as the exclusive end.
+
+        Returns:
+            A [start, end) pair.
+        """
         start_ts = to_timestamp(self.model.cron_floor(start))
         end_ts = to_timestamp(
             self.model.cron_next(end) if is_date(end) else self.model.cron_floor(end)
         )
 
-        if start_ts > end_ts:
-            raise ValueError("`end` must be > `start`")
+        if (strict and start_ts >= end_ts) or (start_ts > end_ts):
+            raise ValueError("`end` must be greater than `start`")
         return (start_ts, end_ts)
 
     def merge_intervals(self, other: Snapshot) -> None:
         """Inherits intervals from the target snapshot.
 
         Args:
             other: The target snapshot to inherit intervals from.
@@ -484,15 +501,17 @@
         Returns:
             A list of all the missing intervals as epoch timestamps.
         """
         if self.is_embedded_kind:
             return []
 
         missing = []
-        start_dt, end_dt = (to_datetime(ts) for ts in self._inclusive_exclusive(start, end))
+        start_dt, end_dt = (
+            to_datetime(ts) for ts in self._inclusive_exclusive(start, end, strict=False)
+        )
         dates = tuple(croniter_range(start_dt, end_dt, self.model.normalized_cron()))
         size = len(dates) - 1
 
         for i in range(size):
             current_ts = to_timestamp(dates[i])
             end_ts = (
                 to_timestamp(dates[i + 1])
@@ -710,36 +729,33 @@
         for hook in hooks:
             if isinstance(hook, exp.Expression):
                 serialized.append(hook.sql())
             else:
                 name, args = hook
                 serialized.append(
                     f"{name}:"
-                    + ",".join(
-                        f"{k}={v.sql(identify=True, comments=False)}"
-                        for k, v in sorted(args.items())
-                    )
+                    + ",".join(f"{k}={v.sql(comments=False)}" for k, v in sorted(args.items()))
                 )
         return serialized
 
     data = [
         str(model.sorted_python_env),
         model.kind.name,
         model.cron,
         model.storage_format,
         physical_schema,
         *(model.partitioned_by or []),
-        *(expression.sql(identify=True, comments=False) for expression in model.expressions or []),
+        *(expression.sql(comments=False) for expression in model.expressions or []),
         *serialize_hooks(model.pre),
         *serialize_hooks(model.post),
         model.stamp,
     ]
 
     if isinstance(model, SqlModel):
-        data.append(model.query.sql(identify=True, comments=False))
+        data.append(model.query.sql(comments=False))
 
         for macro_name, macro in sorted(model.jinja_macros.root_macros.items(), key=lambda x: x[0]):
             data.append(macro_name)
             data.append(macro.definition)
 
         for package in model.jinja_macros.packages.values():
             for macro_name, macro in sorted(package.items(), key=lambda x: x[0]):
@@ -777,21 +793,21 @@
 
     for audit_name, audit_args in sorted(model.audits, key=lambda a: a[0]):
         metadata.append(audit_name)
 
         if audit_name in BUILT_IN_AUDITS:
             for arg_name, arg_value in audit_args.items():
                 metadata.append(arg_name)
-                metadata.append(arg_value.sql(identify=True, comments=True))
+                metadata.append(arg_value.sql(comments=True))
         elif audit_name in audits:
             audit = audits[audit_name]
             metadata.extend(
                 [
                     audit.render_query(model, **t.cast(t.Dict[str, t.Any], audit_args)).sql(
-                        identify=True, comments=True
+                        comments=True
                     ),
                     audit.dialect,
                     str(audit.skip),
                     str(audit.blocking),
                 ]
             )
         else:
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.5.0/sqlmesh/core/snapshot/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,15 +322,15 @@
                 latest=latest,
                 snapshots=snapshots,
                 is_dev=is_dev,
                 engine_adapter=self.adapter,
                 **audit_args,
                 **kwargs,
             )
-            count, *_ = self.adapter.fetchone(select("COUNT(*)").from_(query.subquery()))
+            count, *_ = self.adapter.fetchone(select("COUNT(*)").from_(query.subquery("audit")))
             if count and raise_exception:
                 message = f"Audit '{audit_name}' for model '{snapshot.model.name}' failed.\nGot {count} results, expected 0.\n{query}"
                 if audit.blocking:
                     raise AuditError(message)
                 else:
                     logger.warning(f"{message}\nAudit is warn only so proceeding with execution.")
             results.append(AuditResult(audit=audit, count=count, query=query))
@@ -377,23 +377,31 @@
             logger.info("Creating view '%s'", table_name)
             self.adapter.create_view(
                 table_name,
                 snapshot.model.render_query(snapshots=parent_snapshots_by_name, is_dev=is_dev),
             )
         else:
             logger.info("Creating table '%s'", table_name)
-            self.adapter.create_table(
-                table_name,
-                query_or_columns_to_types=snapshot.model.columns_to_types
-                if snapshot.model.annotated
-                else snapshot.model.ctas_query(parent_snapshots_by_name, is_dev=is_dev),
-                storage_format=snapshot.model.storage_format,
-                partitioned_by=snapshot.model.partitioned_by,
-                partition_interval_unit=snapshot.model.interval_unit(),
-            )
+            if snapshot.model.annotated:
+                self.adapter.create_table(
+                    table_name,
+                    columns_to_types=snapshot.model.columns_to_types,
+                    storage_format=snapshot.model.storage_format,
+                    partitioned_by=snapshot.model.partitioned_by,
+                    partition_interval_unit=snapshot.model.interval_unit(),
+                )
+            else:
+                self.adapter.ctas(
+                    table_name,
+                    snapshot.model.ctas_query(parent_snapshots_by_name, is_dev=is_dev),
+                    snapshot.model.columns_to_types,
+                    storage_format=snapshot.model.storage_format,
+                    partitioned_by=snapshot.model.partitioned_by,
+                    partition_interval_unit=snapshot.model.interval_unit(),
+                )
 
     def _migrate_snapshot(self, snapshot: SnapshotInfoLike) -> None:
         if not snapshot.is_materialized or snapshot.is_new_version:
             return
 
         tmp_table_name = snapshot.table_name(is_dev=True)
         target_table_name = snapshot.table_name()
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.5.0/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.5.0/sqlmesh/core/state_sync/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.5.0/sqlmesh/core/state_sync/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.5.0/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import logging
 import typing as t
 from copy import deepcopy
 
 from sqlglot import __version__ as SQLGLOT_VERSION
 from sqlglot import exp
 
+from sqlmesh.core import constants as c
 from sqlmesh.core.audit import Audit
 from sqlmesh.core.dialect import select_from_values
 from sqlmesh.core.engine_adapter import EngineAdapter, TransactionType
 from sqlmesh.core.environment import Environment
 from sqlmesh.core.model import Model
 from sqlmesh.core.snapshot import (
     Snapshot,
@@ -57,15 +58,15 @@
         engine_adapter: The EngineAdapter to use to store and fetch snapshots.
         schema: The schema to store state metadata in.
     """
 
     def __init__(
         self,
         engine_adapter: EngineAdapter,
-        schema: str,
+        schema: str = c.SQLMESH,
     ):
         self.schema = schema
         self.engine_adapter = engine_adapter
         self.snapshots_table = f"{schema}._snapshots"
         self.environments_table = f"{schema}._environments"
         self.versions_table = f"{schema}._versions"
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/test.py` & `sqlmesh-0.5.0/sqlmesh/core/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import unittest
 
 import pandas as pd
 import ruamel
 from sqlglot import Expression, exp, parse_one
 
 from sqlmesh.core.engine_adapter import EngineAdapter
-from sqlmesh.core.snapshot import Snapshot
+from sqlmesh.core.model import Model
 from sqlmesh.utils import unique
 from sqlmesh.utils.errors import SQLMeshError
 from sqlmesh.utils.pydantic import PydanticModel
 from sqlmesh.utils.yaml import load as yaml_load
 
 
 class ModelTestMetadata(PydanticModel):
@@ -38,24 +38,24 @@
 class ModelTest(unittest.TestCase):
     view_names: t.List[str] = []
 
     def __init__(
         self,
         body: t.Dict[str, t.Any],
         test_name: str,
-        snapshots: t.Dict[str, Snapshot],
+        models: t.Dict[str, Model],
         engine_adapter: EngineAdapter,
         path: t.Optional[pathlib.Path],
     ) -> None:
         """ModelTest encapsulates a unit test for a model.
 
         Args:
             body: A dictionary that contains test metadata like inputs and outputs.
             test_name: The name of the test.
-            snapshots: All snapshots to use for expansion and mapping of physical locations.
+            models: All models to use for expansion and mapping of physical locations.
             engine_adapter: The engine adapter to use.
             path: An optional path to the test definition yaml file
         """
         self.body = body
         self.path = path
 
         self.test_name = test_name
@@ -64,38 +64,38 @@
         if "model" not in body:
             self._raise_error("Incomplete test, missing model name")
 
         if "outputs" not in body:
             self._raise_error("Incomplete test, missing outputs")
 
         self.model_name = body["model"]
-        if self.model_name not in snapshots:
+        if self.model_name not in models:
             self._raise_error(f"Model '{self.model_name}' was not found")
 
-        self.snapshot = snapshots[self.model_name]
+        self.model = models[self.model_name]
 
         inputs = self.body.get("inputs", {})
-        for snapshot_id in self.snapshot.parents:
-            if snapshot_id.name not in inputs:
-                self._raise_error(f"Incomplete test, missing input for table {snapshot_id.name}")
+        for depends_on in self.model.depends_on:
+            if depends_on not in inputs:
+                self._raise_error(f"Incomplete test, missing input for table {depends_on}")
 
-        self.query = self.snapshot.model.render_query(**self.body.get("vars", {}))
+        self.query = self.model.render_query(**self.body.get("vars", {}))
         # For tests we just use the model name for the table reference and we don't want to expand
-        mapping = {name: _test_fixture_name(name) for name in snapshots}
+        mapping = {name: _test_fixture_name(name) for name in models}
         if mapping:
             self.query = exp.replace_tables(self.query, mapping)
 
         self.ctes = {cte.alias: cte for cte in self.query.ctes}
 
         super().__init__()
 
     def setUp(self) -> None:
         """Load all input tables"""
         inputs = {name: table["rows"] for name, table in self.body.get("inputs", {}).items()}
-        self.engine_adapter.create_schema(self.snapshot.physical_schema)
+
         for table, rows in inputs.items():
             df = pd.DataFrame.from_records(rows)  # noqa
             columns_to_types: t.Dict[str, exp.DataType] = {}
             for i, v in rows[0].items():
                 # convert ruamel into python
                 v = v.real if hasattr(v, "real") else v
                 columns_to_types[i] = parse_one(type(v).__name__, into=exp.DataType)  # type: ignore
@@ -193,15 +193,15 @@
             path=path, test_name=test_name, body=value
         )
     return model_test_metadata
 
 
 def discover_model_tests(
     path: pathlib.Path, ignore_patterns: t.Optional[t.List[str]] = None
-) -> t.Generator[ModelTestMetadata, None, None]:
+) -> t.Iterator[ModelTestMetadata]:
     """Discover model tests.
 
     Model tests are defined in YAML files and contain the inputs and outputs used to test model queries.
 
     Args:
         path: A path to search for tests.
         ignore_patterns: An optional list of patterns to ignore.
@@ -241,103 +241,77 @@
         if ("*" in pattern and fnmatch.fnmatchcase(test.fully_qualified_test_name, pattern))
         or pattern in test.fully_qualified_test_name
     )
 
 
 def run_tests(
     model_test_metadata: t.List[ModelTestMetadata],
-    snapshots: t.Dict[str, Snapshot],
+    models: t.Dict[str, Model],
     engine_adapter: EngineAdapter,
     verbosity: int = 1,
 ) -> unittest.result.TestResult:
     """Create a test suite of ModelTest objects and run it.
 
     Args:
         model_test_metadata: A list of ModelTestMetadata named tuples.
-        snapshots: All snapshots to use for expansion and mapping of physical locations.
+        models: All models to use for expansion and mapping of physical locations.
         engine_adapter: The engine adapter to use.
         patterns: A list of patterns to match against.
         verbosity: The verbosity level.
     """
     suite = unittest.TestSuite(
         ModelTest(
             body=metadata.body,
             test_name=metadata.test_name,
-            snapshots=snapshots,
+            models=models,
             engine_adapter=engine_adapter,
             path=metadata.path,
         )
         for metadata in model_test_metadata
     )
     return unittest.TextTestRunner(verbosity=verbosity, resultclass=ModelTextTestResult).run(suite)
 
 
 def get_all_model_tests(
-    path: pathlib.Path,
+    *paths: pathlib.Path,
     patterns: t.Optional[t.List[str]] = None,
     ignore_patterns: t.Optional[t.List[str]] = None,
 ) -> t.List[ModelTestMetadata]:
-    model_test_metadatas = list(discover_model_tests(pathlib.Path(path), ignore_patterns))
+    model_test_metadatas = [
+        meta for path in paths for meta in discover_model_tests(pathlib.Path(path), ignore_patterns)
+    ]
     if patterns:
         model_test_metadatas = filter_tests_by_patterns(model_test_metadatas, patterns)
     return model_test_metadatas
 
 
-def run_all_model_tests(
-    path: pathlib.Path,
-    snapshots: t.Dict[str, Snapshot],
-    engine_adapter: EngineAdapter,
-    verbosity: int = 1,
-    patterns: t.Optional[t.List[str]] = None,
-    ignore_patterns: t.Optional[t.List[str]] = None,
-) -> unittest.result.TestResult:
-    """Discover and run all model tests found in path.
-
-    Args:
-        path: A path to search for tests.
-        snapshots: All snapshots to use for expansion and mapping of physical locations.
-        engine_adapter: The engine adapter to use.
-        verbosity: The verbosity level.
-        patterns: A list of patterns to match against.
-        ignore_patterns: An optional list of patterns to ignore.
-    """
-    model_tests = get_all_model_tests(path, patterns, ignore_patterns)
-    return run_tests(model_tests, snapshots, engine_adapter, verbosity)
-
-
 def run_model_tests(
     tests: t.List[str],
-    snapshots: t.Dict[str, Snapshot],
+    models: t.Dict[str, Model],
     engine_adapter: EngineAdapter,
     verbosity: int = 1,
     patterns: t.Optional[t.List[str]] = None,
-    ignore_patterns: t.Optional[t.List[str]] = None,
 ) -> unittest.result.TestResult:
     """Load and run tests.
 
     Args
         tests: A list of tests to run, e.g. [tests/test_orders.yaml::test_single_order]
-        snapshots: All snapshots to use for expansion and mapping of physical locations.
+        models: All models to use for expansion and mapping of physical locations.
         engine_adapter: The engine adapter to use.
         patterns: A list of patterns to match against.
         verbosity: The verbosity level.
-        ignore_patterns: An optional list of patterns to ignore.
     """
     loaded_tests = []
     for test in tests:
         filename, test_name = test.split("::", maxsplit=1) if "::" in test else (test, "")
         path = pathlib.Path(filename)
-        for ignore_pattern in ignore_patterns or []:
-            if path.match(ignore_pattern):
-                break
+        if test_name:
+            loaded_tests.append(load_model_test_file(path)[test_name])
         else:
-            if test_name:
-                loaded_tests.append(load_model_test_file(path)[test_name])
-            else:
-                loaded_tests.extend(load_model_test_file(path).values())
+            loaded_tests.extend(load_model_test_file(path).values())
     if patterns:
         loaded_tests = filter_tests_by_patterns(loaded_tests, patterns)
-    return run_tests(loaded_tests, snapshots, engine_adapter, verbosity)
+    return run_tests(loaded_tests, models, engine_adapter, verbosity)
 
 
 def _test_fixture_name(name: str) -> str:
     return f"{name}__fixture"
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/core/user.py` & `sqlmesh-0.5.0/sqlmesh/core/user.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/adapter.py` & `sqlmesh-0.5.0/sqlmesh/dbt/adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.5.0/sqlmesh/dbt/basemodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from sqlmesh.dbt.adapter import ParsetimeAdapter
 from sqlmesh.dbt.column import (
     ColumnConfig,
     column_descriptions_to_sqlmesh,
     column_types_to_sqlmesh,
     yaml_to_columns,
 )
-from sqlmesh.dbt.common import DbtContext, GeneralConfig, SqlStr
+from sqlmesh.dbt.common import GeneralConfig, QuotingConfig, SqlStr
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.utils import AttributeDict
 from sqlmesh.utils.conversions import ensure_bool
 from sqlmesh.utils.date import date_dict
 from sqlmesh.utils.errors import ConfigError
 from sqlmesh.utils.jinja import MacroReference, extract_macro_references
 from sqlmesh.utils.pydantic import PydanticModel
 
@@ -84,14 +85,15 @@
         schema: Custom schema name added to the model schema name
         alias: Relation identifier for this model instead of the filename
         pre-hook: List of SQL statements to run before the model is built
         post-hook: List of SQL statements to run after the model is built
         full_refresh: Forces the model to always do a full refresh or never do a full refresh
         grants: Set or revoke permissions to the database object for this model
         columns: Column information for the model
+        quoting: Define which components of the qualified name (database, schema, identifier) to quote when resolving the ref() method
     """
 
     # sqlmesh fields
     owner: t.Optional[str] = None
     stamp: t.Optional[str] = None
     storage_format: t.Optional[str] = None
     path: Path = Path()
@@ -104,14 +106,15 @@
     schema_: t.Optional[str] = Field(None, alias="schema")
     alias: t.Optional[str] = None
     pre_hook: t.List[SqlStr] = Field([], alias="pre-hook")
     post_hook: t.List[SqlStr] = Field([], alias="post-hook")
     full_refresh: t.Optional[bool] = None
     grants: t.Dict[str, t.List[str]] = {}
     columns: t.Dict[str, ColumnConfig] = {}
+    quoting: QuotingConfig = Field(default_factory=QuotingConfig)
 
     @validator("pre_hook", "post_hook", pre=True)
     def _validate_hooks(cls, v: t.Union[str, t.List[t.Union[SqlStr, str]]]) -> t.List[SqlStr]:
         return [SqlStr(val) for val in ensure_list(v)]
 
     @validator("full_refresh", pre=True)
     def _validate_bool(cls, v: str) -> bool:
@@ -192,14 +195,15 @@
 
         return AttributeDict(
             {
                 "database": self.database,
                 "schema": self.table_schema,
                 "identifier": self.table_name,
                 "type": relation_type.value,
+                "quote_policy": AttributeDict(self.quoting.dict()),
             }
         )
 
     def attribute_dict(self) -> AttributeDict[str, t.Any]:
         return AttributeDict(self.dict())
 
     def sqlmesh_model_kwargs(self, model_context: DbtContext) -> t.Dict[str, t.Any]:
@@ -251,23 +255,35 @@
         """Convert DBT model into sqlmesh Model"""
 
     def _context_for_dependencies(
         self, context: DbtContext, dependencies: Dependencies
     ) -> DbtContext:
         model_context = context.copy()
 
-        model_context.sources = {
-            name: value for name, value in context.sources.items() if name in dependencies.sources
-        }
-        model_context.seeds = {
-            name: value for name, value in context.seeds.items() if name in dependencies.refs
-        }
-        model_context.models = {
-            name: value for name, value in context.models.items() if name in dependencies.refs
-        }
+        models = {}
+        seeds = {}
+        sources = {}
+
+        for ref in self._dependencies.refs:
+            if ref in context.seeds:
+                seeds[ref] = context.seeds[ref]
+            elif ref in context.models:
+                models[ref] = context.models[ref]
+            else:
+                raise ConfigError(f"Model '{ref}' was not found for model '{self.table_name}'.")
+
+        for source in self._dependencies.sources:
+            if source in context.sources:
+                sources[source] = context.sources[source]
+            else:
+                raise ConfigError(f"Source '{source}' was not found for model '{self.table_name}'.")
+
+        model_context.sources = sources
+        model_context.seeds = seeds
+        model_context.models = models
         model_context.variables = {
             name: value
             for name, value in context.variables.items()
             if name in dependencies.variables
         }
 
         return model_context
@@ -357,41 +373,29 @@
             config = config.update_with(
                 {kwarg.key: _extract_value(kwarg.value) for kwarg in call.kwargs}
             )
 
         return config
 
     def _ref(self, package_name: str, model_name: t.Optional[str] = None) -> BaseRelation:
-        if package_name in self.context.models:
-            relation = BaseRelation.create(**self.context.models[package_name].relation_info)
-        elif package_name in self.context.seeds:
-            relation = BaseRelation.create(**self.context.seeds[package_name].relation_info)
-        else:
-            raise ConfigError(
-                f"Model '{package_name}' was not found for model '{self.config.table_name}'."
-            )
         self._captured_dependencies.refs.add(package_name)
-        return relation
+        return BaseRelation.create()
 
     def _var(self, name: str, default: t.Optional[str] = None) -> t.Any:
         if default is None and name not in self.context.variables:
             raise ConfigError(
                 f"Variable '{name}' was not found for model '{self.config.table_name}'."
             )
         self._captured_dependencies.variables.add(name)
         return self.context.variables.get(name, default)
 
     def _source(self, source_name: str, table_name: str) -> BaseRelation:
         full_name = ".".join([source_name, table_name])
-        if full_name not in self.context.sources:
-            raise ConfigError(
-                f"Source '{full_name}' was not found for model '{self.config.table_name}'."
-            )
         self._captured_dependencies.sources.add(full_name)
-        return BaseRelation.create(**self.context.sources[full_name].relation_info)
+        return BaseRelation.create()
 
     class TrackingAdapter(ParsetimeAdapter):
         def __init__(self, outer_self: ModelSqlRenderer, *args: t.Any, **kwargs: t.Any):
             super().__init__(*args, **kwargs)
             self.outer_self = outer_self
             self.context = outer_self.context
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/builtin.py` & `sqlmesh-0.5.0/sqlmesh/dbt/builtin.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import jinja2
 from dbt.adapters.base import BaseRelation
 from dbt.contracts.relation import Policy
 from ruamel.yaml import YAMLError
 
 from sqlmesh.core.engine_adapter import EngineAdapter
 from sqlmesh.dbt.adapter import ParsetimeAdapter, RuntimeAdapter
-from sqlmesh.dbt.common import DbtContext
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.package import PackageLoader
 from sqlmesh.utils import AttributeDict, yaml
 from sqlmesh.utils.errors import ConfigError, MacroEvalError
 from sqlmesh.utils.jinja import JinjaMacroRegistry, MacroReturnVal
 
 
 class Exceptions:
@@ -157,28 +157,28 @@
 def generate_ref(refs: t.Dict[str, t.Any]) -> t.Callable:
 
     # TODO suport package name
     def ref(package: str, name: t.Optional[str] = None) -> t.Optional[BaseRelation]:
         name = name or package
         relation_info = refs.get(name)
         if relation_info is None:
-            return relation_info
+            return None
 
-        return BaseRelation.create(**relation_info, quote_policy=quote_policy())
+        return BaseRelation.create(**relation_info)
 
     return ref
 
 
 def generate_source(sources: t.Dict[str, t.Any]) -> t.Callable:
     def source(package: str, name: str) -> t.Optional[BaseRelation]:
         relation_info = sources.get(f"{package}.{name}")
         if relation_info is None:
-            return relation_info
+            return None
 
-        return BaseRelation.create(**relation_info, quote_policy=quote_policy())
+        return BaseRelation.create(**relation_info)
 
     return source
 
 
 def quote_policy() -> Policy:
     return Policy(database=False, schema=False, identifier=False)
 
@@ -308,15 +308,15 @@
 ) -> t.Dict[str, t.Any]:
     builtin_globals = BUILTIN_GLOBALS.copy()
     jinja_globals = jinja_globals.copy()
 
     this = jinja_globals.pop("this", None)
     if this is not None:
         if not isinstance(this, BaseRelation):
-            builtin_globals["this"] = BaseRelation.create(**this, quote_policy=quote_policy())
+            builtin_globals["this"] = BaseRelation.create(**this)
         else:
             builtin_globals["this"] = this
 
     sources = jinja_globals.pop("sources", None)
     if sources is not None:
         builtin_globals["source"] = generate_source(sources)
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/column.py` & `sqlmesh-0.5.0/sqlmesh/dbt/column.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/loader.py` & `sqlmesh-0.5.0/sqlmesh/dbt/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sqlmesh.core.audit import Audit
 from sqlmesh.core.config import Config
 from sqlmesh.core.hooks import HookRegistry
 from sqlmesh.core.loader import Loader
 from sqlmesh.core.macros import MacroRegistry
 from sqlmesh.core.model import Model
 from sqlmesh.dbt.basemodel import BaseModelConfig
-from sqlmesh.dbt.common import DbtContext
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.profile import Profile
 from sqlmesh.dbt.project import Project
 from sqlmesh.utils import UniqueKeyDict
 
 
 def sqlmesh_config(project_root: t.Optional[Path] = None, **kwargs: t.Any) -> Config:
     project_root = project_root or Path()
@@ -52,17 +52,14 @@
         )
         for path in project.project_files:
             self._track_file(path)
 
         context = project.context.copy()
 
         for package_name, package in project.packages.items():
-            context.add_sources(package.sources)
-            context.add_seeds(package.seeds)
-            context.add_models(package.models)
             context.jinja_macros.add_macros(
                 package.macros,
                 package=package_name if package_name != context.project_name else None,
             )
 
         # First render all the config and discover dependencies
         for package in project.packages.values():
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/model.py` & `sqlmesh-0.5.0/sqlmesh/dbt/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     IncrementalByUniqueKeyKind,
     Model,
     ModelKind,
     ModelKindName,
     create_sql_model,
 )
 from sqlmesh.dbt.basemodel import BaseModelConfig, Materialization
-from sqlmesh.dbt.common import DbtContext, SqlStr
+from sqlmesh.dbt.common import SqlStr
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.target import TargetConfig
 from sqlmesh.utils.errors import ConfigError
 
 INCREMENTAL_BY_TIME_STRATEGIES = set(["delete+insert", "insert_overwrite"])
 INCREMENTAL_BY_UNIQUE_KEY_STRATEGIES = set(["merge"])
 
 
@@ -65,15 +66,15 @@
     dialect: t.Optional[str] = None
     batch_size: t.Optional[int]
 
     # DBT configuration fields
     start: t.Optional[str] = None
     cluster_by: t.Optional[t.List[str]] = None
     incremental_strategy: t.Optional[str] = None
-    materialized: Materialization = Materialization.VIEW
+    materialized: str = Materialization.VIEW.value
     sql_header: t.Optional[str] = None
     unique_key: t.Optional[t.List[str]] = None
 
     # redshift
     bind: t.Optional[bool] = None
 
     # Private fields
@@ -89,41 +90,37 @@
     def _validate_list(cls, v: t.Union[str, t.List[str]]) -> t.List[str]:
         return ensure_list(v)
 
     @validator("sql", pre=True)
     def _validate_sql(cls, v: t.Union[str, SqlStr]) -> SqlStr:
         return SqlStr(v)
 
-    @validator("materialized", pre=True)
-    def _validate_materialization(cls, v: str) -> Materialization:
-        return Materialization(v.lower())
-
     _FIELD_UPDATE_STRATEGY: t.ClassVar[t.Dict[str, UpdateStrategy]] = {
         **BaseModelConfig._FIELD_UPDATE_STRATEGY,
         **{
             "sql": UpdateStrategy.IMMUTABLE,
             "time_column": UpdateStrategy.IMMUTABLE,
         },
     }
 
     @property
     def model_dialect(self) -> t.Optional[str]:
         return self.dialect or self.meta.get("dialect", None)
 
     @property
     def model_materialization(self) -> Materialization:
-        return self.materialized
+        return Materialization(self.materialized.lower())
 
     def model_kind(self, target: TargetConfig) -> ModelKind:
         """
         Get the sqlmesh ModelKind
         Returns:
             The sqlmesh ModelKind
         """
-        materialization = self.materialized
+        materialization = self.model_materialization
         if materialization == Materialization.TABLE:
             return ModelKind(name=ModelKindName.FULL)
         if materialization == Materialization.VIEW:
             return ModelKind(name=ModelKindName.VIEW)
         if materialization == Materialization.INCREMENTAL:
             if self.time_column:
                 strategy = self.incremental_strategy or target.default_incremental_strategy(
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/package.py` & `sqlmesh-0.5.0/sqlmesh/dbt/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 import typing as t
 from pathlib import Path
 
 from sqlmesh.dbt.common import (
     PROJECT_FILENAME,
     BaseConfig,
-    DbtContext,
+    QuotingConfig,
     SqlStr,
     load_yaml,
 )
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.model import ModelConfig
 from sqlmesh.dbt.seed import SeedConfig
 from sqlmesh.dbt.source import SourceConfig
 from sqlmesh.utils.errors import ConfigError
 from sqlmesh.utils.jinja import MacroExtractor, MacroInfo
 from sqlmesh.utils.pydantic import PydanticModel
 
@@ -130,26 +131,31 @@
             scoped_configs[scope] = config
             for key, value in nested_config.items():
                 nested_scope = (*scope, key)
                 load_config(value, config, nested_scope, scoped_configs)
 
             return scoped_configs
 
+        if "quoting" in yaml:
+            quoting = QuotingConfig(**yaml["quoting"])
+        else:
+            quoting = self._context.target.quoting
+
         scope = ()
         self.project_config.source_config = load_config(
-            yaml.get("sources", {}), SourceConfig(), scope
+            yaml.get("sources", {}), SourceConfig(quoting=quoting), scope
         )
         self.project_config.seed_config = load_config(
             yaml.get("seeds", {}),
-            SeedConfig(target_schema=self._context.target.schema_),
+            SeedConfig(target_schema=self._context.target.schema_, quoting=quoting),
             scope,
         )
         self.project_config.model_config = load_config(
             yaml.get("models", {}),
-            ModelConfig(target_schema=self._context.target.schema_),
+            ModelConfig(target_schema=self._context.target.schema_, quoting=quoting),
             scope,
         )
 
     def _load_models(
         self, models_dirs: t.List[Path]
     ) -> t.Tuple[t.Dict[str, ModelConfig], t.Dict[str, SourceConfig]]:
         """
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/profile.py` & `sqlmesh-0.5.0/sqlmesh/dbt/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import typing as t
 from pathlib import Path
 
-from sqlmesh.dbt.common import PROJECT_FILENAME, DbtContext, load_yaml
+from sqlmesh.dbt.common import PROJECT_FILENAME, load_yaml
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.target import TargetConfig
 from sqlmesh.utils.errors import ConfigError
 from sqlmesh.utils.yaml import dumps as dump_yaml
 
 
 class Profile:
     """
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/project.py` & `sqlmesh-0.5.0/sqlmesh/dbt/project.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
+import logging
 import typing as t
 from pathlib import Path
 
-from sqlmesh.dbt.common import PROJECT_FILENAME, DbtContext, load_yaml
+from sqlmesh.dbt.common import PROJECT_FILENAME, load_yaml
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.package import Package, PackageLoader, ProjectConfig
 from sqlmesh.dbt.profile import Profile
 from sqlmesh.utils.errors import ConfigError
 
+logger = logging.getLogger(__name__)
+
 
 class Project:
     """Configuration for a DBT project"""
 
     def __init__(
         self,
         context: DbtContext,
@@ -59,14 +63,21 @@
         context.profile_name = (
             context.render(project_yaml.get("profile", "")) or context.project_name
         )
 
         profile = Profile.load(context, context.target_name)
         context.target = profile.target
 
+        extra_fields = profile.target.extra
+        if extra_fields:
+            extra_str = ",".join(f"'{field}'" for field in extra_fields)
+            logger.warning(
+                f"Warning: {profile.target.type} adapter does not currently support {extra_str}."
+            )
+
         packages = {}
         root_loader = PackageLoader(context, ProjectConfig())
 
         packages[context.project_name] = root_loader.load()
         project_config = root_loader.project_config
 
         packages_dir = Path(
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/seed.py` & `sqlmesh-0.5.0/sqlmesh/dbt/seed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from sqlmesh.core.model import Model, SeedKind, create_seed_model
 from sqlmesh.dbt.basemodel import BaseModelConfig
-from sqlmesh.dbt.common import DbtContext, SqlStr
+from sqlmesh.dbt.common import SqlStr
+from sqlmesh.dbt.context import DbtContext
 
 
 class SeedConfig(BaseModelConfig):
     """
     seedConfig contains all config parameters available to DBT seeds
 
     See https://docs.getdbt.com/reference/configs-and-properties for
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/source.py` & `sqlmesh-0.5.0/sqlmesh/dbt/source.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import typing as t
 
 from dbt.contracts.relation import RelationType
 from pydantic import Field, validator
 
 from sqlmesh.core.config.base import UpdateStrategy
 from sqlmesh.dbt.column import ColumnConfig, yaml_to_columns
-from sqlmesh.dbt.common import GeneralConfig
-from sqlmesh.utils.conversions import ensure_bool
+from sqlmesh.dbt.common import GeneralConfig, QuotingConfig
+from sqlmesh.utils import AttributeDict
 
 
 class SourceConfig(GeneralConfig):
     """
     Args:
         config_name: The schema.table_name names declared in source config
         name: The name of the source or table
         database: Name of the database where the table is stored. By default, the project's target database is used.
         schema: The scehma name as stored in the database. If not specified, the source name is used.
         identifier: The table name as stored in the database. If not specified, the source table name is used
         loader: Describes the tool that loads the source into the warehouse
         overrides: Override a source defined in the specified package
         freshness: Dictionary specifying maximum time, since the most recent record, to consider the source fresh
         loaded_at_field: Column name or expression that returns a timestamp indicating freshness
-        quoting: Dictionary of what to quote (database, schema, identifier) when resolving the source() method
+        quoting: Define which components of the qualified name (database, schema, identifier) to quote when resolving the source() method
         external: Dictionary of metadata properties specific to sources that point to external tables
         columns: Columns within the source
     """
 
     # sqlmesh fields
     config_name: str = ""
 
@@ -36,22 +36,18 @@
     database: t.Optional[str] = None
     schema_: t.Optional[str] = Field(None, alias="schema")
     identifier: t.Optional[str] = None
     loader: t.Optional[str] = None
     overrides: t.Optional[str] = None
     freshness: t.Optional[t.Dict[str, t.Any]] = {}
     loaded_at_field: t.Optional[str] = None
-    quoting: t.Optional[t.Dict[str, bool]] = {}
+    quoting: QuotingConfig = Field(default_factory=QuotingConfig)
     external: t.Optional[t.Dict[str, t.Any]] = {}
     columns: t.Dict[str, ColumnConfig] = {}
 
-    @validator("quoting", pre=True)
-    def _validate_quoting(cls, v: t.Dict[str, t.Any]) -> t.Dict[str, bool]:
-        return {key: ensure_bool(val) for key, val in v.items()}
-
     @validator("columns", pre=True)
     def _validate_columns(cls, v: t.Any) -> t.Dict[str, ColumnConfig]:
         if not isinstance(v, dict) or all(isinstance(col, ColumnConfig) for col in v.values()):
             return v
 
         return yaml_to_columns(v)
 
@@ -65,14 +61,17 @@
         return self.identifier or self.name
 
     @property
     def source_name(self) -> str:
         return ".".join(part for part in (self.schema_, self.table_name) if part)
 
     @property
-    def relation_info(self) -> t.Dict[str, t.Any]:
-        return {
-            "database": self.database,
-            "schema": self.schema_,
-            "identifier": self.table_name,
-            "type": RelationType.External.value,
-        }
+    def relation_info(self) -> AttributeDict:
+        return AttributeDict(
+            {
+                "database": self.database,
+                "schema": self.schema_,
+                "identifier": self.table_name,
+                "type": RelationType.External.value,
+                "quote_policy": AttributeDict(self.quoting.dict()),
+            }
+        )
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/dbt/target.py` & `sqlmesh-0.5.0/sqlmesh/dbt/target.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 
 from sqlmesh.core.config.connection import (
     BigQueryConnectionConfig,
     BigQueryConnectionMethod,
     ConnectionConfig,
     DatabricksSQLConnectionConfig,
     DuckDBConnectionConfig,
+    PostgresConnectionConfig,
     RedshiftConnectionConfig,
     SnowflakeConnectionConfig,
 )
 from sqlmesh.core.model import IncrementalByTimeRangeKind, IncrementalByUniqueKeyKind
+from sqlmesh.dbt.common import DbtConfig, QuotingConfig
 from sqlmesh.utils import AttributeDict
 from sqlmesh.utils.errors import ConfigError
-from sqlmesh.utils.pydantic import PydanticModel
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 IncrementalKind = t.Union[t.Type[IncrementalByUniqueKeyKind], t.Type[IncrementalByTimeRangeKind]]
 
 
-class TargetConfig(abc.ABC, PydanticModel):
+class TargetConfig(abc.ABC, DbtConfig):
     """
     Configuration for DBT profile target
 
     Args:
         name: The name of this target
         type: The type of the data warehouse
         schema_: The target schema for this project
@@ -83,14 +84,22 @@
 
     def target_jinja(self, profile_name: str) -> AttributeDict:
         fields = self.dict().copy()
         fields["profile_name"] = profile_name
         fields["target_name"] = self.name
         return AttributeDict(fields)
 
+    @property
+    def quoting(self) -> QuotingConfig:
+        return QuotingConfig()
+
+    @property
+    def extra(self) -> t.Set[str]:
+        return self.extra_fields(set(self.dict()))
+
 
 class DuckDbConfig(TargetConfig):
     """
     Connection config for DuckDb target
 
     Args:
         path: Location of the database file. If not specified, an in memory database is used.
@@ -150,14 +159,18 @@
             account=self.account,
             warehouse=self.warehouse,
             database=self.database,
             role=self.role,
             concurrent_tasks=self.threads,
         )
 
+    @property
+    def quoting(self) -> QuotingConfig:
+        return QuotingConfig(database=False, schema=False, identifier=False)
+
 
 class PostgresConfig(TargetConfig):
     """
     Project connection and operational configuration for the Postgres target
 
     Args:
         host: The Postgres host to connect to
@@ -177,24 +190,35 @@
     host: str
     user: str
     password: str
     port: int
     dbname: str
     keepalives_idle: int = 0
     connect_timeout: int = 10
-    retries: int = 1
-    search_path: t.Optional[str] = None
+    retries: int = 1  # Currently Unsupported by SQLMesh
+    search_path: t.Optional[str] = None  # Currently Unsupported by SQLMesh
     role: t.Optional[str] = None
     sslmode: t.Optional[str] = None
 
     def default_incremental_strategy(self, kind: IncrementalKind) -> str:
         return "delete+insert" if kind is IncrementalByUniqueKeyKind else "append"
 
     def to_sqlmesh(self) -> ConnectionConfig:
-        raise ConfigError("PostgreSQL is not supported by SQLMesh yet.")
+        return PostgresConnectionConfig(
+            host=self.host,
+            user=self.user,
+            password=self.password,
+            port=self.port,
+            database=self.schema_,
+            keepalives_idle=self.keepalives_idle,
+            concurrent_tasks=self.threads,
+            connect_timeout=self.connect_timeout,
+            role=self.role,
+            sslmode=self.sslmode,
+        )
 
 
 class RedshiftConfig(TargetConfig):
     """
     Project connection and operational configuration for the Redshift target
 
     Args:
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/engines/commands.py` & `sqlmesh-0.5.0/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/app.py` & `sqlmesh-0.5.0/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.5.0/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/notification_operator_provider.py` & `sqlmesh-0.5.0/sqlmesh/integrations/github/notification_operator_provider.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/notification_target.py` & `sqlmesh-0.5.0/sqlmesh/integrations/github/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/integrations/github/shared.py` & `sqlmesh-0.5.0/sqlmesh/integrations/github/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/magics.py` & `sqlmesh-0.5.0/sqlmesh/magics.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from collections import defaultdict
 
 from IPython.core.display import HTML, display
 from IPython.core.magic import Magics, line_cell_magic, line_magic, magics_class
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 from ruamel.yaml import YAML
 
+from sqlmesh.core import constants as c
 from sqlmesh.core.console import get_console
 from sqlmesh.core.context import Context
 from sqlmesh.core.dialect import format_model_expressions, parse
 from sqlmesh.core.model import load_model
 from sqlmesh.core.test import ModelTestMetadata, get_all_model_tests
 from sqlmesh.utils.errors import MagicError, MissingContextException, SQLMeshError
 from sqlmesh.utils.yaml import dumps as yaml_dumps
@@ -42,19 +43,22 @@
             if context:
                 return context
         raise MissingContextException(
             f"Context must be defined and initialized with one of these names: {', '.join(CONTEXT_VARIABLE_NAMES)}"
         )
 
     @magic_arguments()
-    @argument("path", type=str, help="The path to the SQLMesh project.")
+    @argument(
+        "--paths", "-p", type=str, nargs="+", default="", help="The path to the SQLMesh project."
+    )
     @line_magic
-    def context(self, path: str) -> None:
+    def context(self, line: str) -> None:
         """Sets the context in the user namespace."""
-        self._shell.user_ns["context"] = Context(path=path)
+        args = parse_argstring(self.context, line)
+        self._shell.user_ns["context"] = Context(paths=args.paths)
 
     @magic_arguments()
     @argument("model", type=str, help="The model.")
     @argument("--start", "-s", type=str, help="Start date to render.")
     @argument("--end", "-e", type=str, help="End date to render.")
     @argument("--latest", "-l", type=str, help="Latest date to render.")
     @argument("--dialect", "-d", type=str, help="The rendered dialect.")
@@ -64,21 +68,22 @@
         args = parse_argstring(self.model, line)
         model = self._context.get_model(args.model)
 
         if not model:
             raise SQLMeshError(f"Cannot find {model}")
 
         if sql:
+            config = self._context.config_for_model(model)
             loaded = load_model(
-                parse(sql, default_dialect=self._context.dialect),
+                parse(sql, default_dialect=config.dialect),
                 macros=self._context._macros,
                 hooks=self._context._hooks,
                 path=model._path,
-                dialect=self._context.dialect,
-                time_column_format=self._context.config.time_column_format,
+                dialect=config.dialect,
+                time_column_format=config.time_column_format,
             )
 
             if loaded.name == args.model:
                 model = loaded
 
         self._context.upsert_model(model)
         expressions = model.render_definition(include_python=False)
@@ -115,20 +120,26 @@
     @line_cell_magic
     def test(self, line: str, test_def_raw: t.Optional[str] = None) -> None:
         """Allow the user to list tests for a model, output a specific test, and then write their changes back"""
         args = parse_argstring(self.test, line)
         if not args.test_name and not args.ls:
             raise MagicError("Must provide either test name or `--ls` to list tests")
 
-        model_test_metadatas = get_all_model_tests(
-            self._context.test_directory_path,
-            ignore_patterns=self._context.ignore_patterns,
-        )
+        test_meta = []
+
+        for path, config in self._context.configs.items():
+            test_meta.extend(
+                get_all_model_tests(
+                    path / c.TESTS,
+                    ignore_patterns=config.ignore_patterns,
+                )
+            )
+
         tests: t.Dict[str, t.Dict[str, ModelTestMetadata]] = defaultdict(dict)
-        for model_test_metadata in model_test_metadatas:
+        for model_test_metadata in test_meta:
             model = model_test_metadata.body.get("model")
             if not model:
                 self._context.console.log_error(
                     f"Test found that does not have `model` defined: {model_test_metadata.path}"
                 )
             tests[model][model_test_metadata.test_name] = model_test_metadata
         if args.ls:
@@ -343,14 +354,21 @@
     @line_magic
     def dag(self, line: str) -> None:
         """Displays the dag"""
         self._context.refresh()
         dag = self._context.get_dag()
         self.display(HTML(dag.pipe().decode("utf-8")))
 
+    @magic_arguments()
+    @line_magic
+    def migrate(self, line: str) -> None:
+        """Migrate SQLMesh to the current running version."""
+        self._context.migrate()
+        self.display("Migration complete")
+
     @property
     def _shell(self) -> t.Any:
         # Make mypy happy.
         if not self.shell:
             raise RuntimeError("IPython Magics are in invalid state")
         return self.shell
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.5.0/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.5.0/sqlmesh/schedulers/airflow/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 @contextlib.contextmanager
 def scoped_state_sync() -> t.Generator[StateSync, None, None]:
     dialect = settings.engine.dialect.name
     engine_adapter = create_engine_adapter(
         settings.engine.raw_connection, dialect, multithreaded=True
     )
     try:
-        yield EngineAdapterStateSync(engine_adapter, "sqlmesh")
+        yield EngineAdapterStateSync(engine_adapter)
     finally:
         engine_adapter.close()
 
 
 @provide_session
 def get_snapshot_dag_ids(session: Session = PROVIDED_SESSION) -> t.List[str]:
     dag_tags = session.query(DagTag).filter(DagTag.name == common.SNAPSHOT_AIRFLOW_TAG).all()
@@ -135,11 +135,17 @@
             return SQLMeshBigQueryOperator
         if name == "redshift":
             from sqlmesh.schedulers.airflow.operators.redshift import (
                 SQLMeshRedshiftOperator,
             )
 
             return SQLMeshRedshiftOperator
+        if name in ("postgres", "postgresql"):
+            from sqlmesh.schedulers.airflow.operators.postgres import (
+                SQLMeshPostgresOperator,
+            )
+
+            return SQLMeshPostgresOperator
     except ImportError:
         raise SQLMeshError(f"Failed to automatically discover an operator for '{name}'.'")
 
     raise ValueError(f"Unsupported engine name '{name}'.")
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/__init__.py` & `sqlmesh-0.5.0/sqlmesh/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,28 +99,29 @@
     @classmethod
     def set_registry(cls, registry: UniqueKeyDict) -> None:
         """Set the registry."""
         cls._registry = registry
 
 
 @contextmanager
-def sys_path(path: Path) -> t.Generator[None, None, None]:
+def sys_path(*paths: Path) -> t.Generator[None, None, None]:
     """A context manager to temporarily add a path to 'sys.path'."""
-    path_str = str(path.absolute())
+    inserted = set()
 
-    if path_str in sys.path:
-        inserted = False
-    else:
-        sys.path.insert(0, path_str)
-        inserted = True
+    for path in paths:
+        path_str = str(path.absolute())
+
+        if path_str not in sys.path:
+            sys.path.insert(0, path_str)
+            inserted.add(path_str)
 
     try:
         yield
     finally:
-        if inserted:
+        for path_str in inserted:
             sys.path.remove(path_str)
 
 
 def format_exception(exception: BaseException) -> t.List[str]:
     if sys.version_info < (3, 10):
         return traceback.format_exception(
             type(exception), exception, exception.__traceback__
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/concurrency.py` & `sqlmesh-0.5.0/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.5.0/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/dag.py` & `sqlmesh-0.5.0/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/date.py` & `sqlmesh-0.5.0/sqlmesh/utils/date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/errors.py` & `sqlmesh-0.5.0/sqlmesh/utils/errors.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/jinja.py` & `sqlmesh-0.5.0/sqlmesh/utils/jinja.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,21 @@
     create_builtins_module: t.Optional[str] = None
 
     _parser_cache: t.Dict[t.Tuple[t.Optional[str], str], Template] = {}
     __environment: t.Optional[Environment] = None
 
     @validator("global_objs", pre=True)
     def _validate_attribute_dict(cls, value: t.Any) -> t.Any:
+        def _attribute_dict(val: t.Dict[str, t.Any]) -> AttributeDict:
+            return AttributeDict(
+                {k: _attribute_dict(v) if isinstance(v, dict) else v for k, v in val.items()}
+            )
+
         if isinstance(value, t.Dict):
-            return {k: AttributeDict(v) if isinstance(v, dict) else v for k, v in value.items()}
+            return _attribute_dict(value)
         return value
 
     def add_macros(self, macros: t.Dict[str, MacroInfo], package: t.Optional[str] = None) -> None:
         """Adds macros to the target package.
 
         Args:
             macros: Macros that should be added.
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.5.0/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/pandas.py` & `sqlmesh-0.5.0/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/pydantic.py` & `sqlmesh-0.5.0/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/rich.py` & `sqlmesh-0.5.0/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/transactional_file.py` & `sqlmesh-0.5.0/sqlmesh/utils/transactional_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,39 +26,45 @@
 
 class TransactionalFile:
     """A transaction handler which wraps a file path."""
 
     mtime_dispatch = {
         "s3": lambda f: datetime.strptime(f["LastModified"], "%Y-%m-%d %H:%M:%S%z"),
         "gcs": lambda f: datetime.strptime(f["updated"], "%Y-%m-%dT%H:%M:%S.%fZ"),
-        "azure": lambda f: datetime.strptime(f["LastModified"], "%Y-%m-%d %H:%M:%S%z"),
+        "adl": lambda f: datetime.strptime(f["LastModified"], "%Y-%m-%d %H:%M:%S%z"),
         "file": lambda f: datetime.fromtimestamp(f["mtime"]),
     }
+    # Support aliases
+    mtime_dispatch["gs"] = mtime_dispatch["gcs"]
+    mtime_dispatch["s3a"] = mtime_dispatch["s3"]
+    mtime_dispatch["azure"] = mtime_dispatch["adl"]
 
     def __init__(self, path: str, fs: fsspec.AbstractFileSystem) -> None:
         """Creates a new FileTransactionHandler.
 
         Args:
             path: The path to lock.
             fs: The fsspec file system.
         """
         self.path = path
         self.lock_prefix = f"{self.path}.lock"
         self.lock_path = f"{self.lock_prefix}.{lock_id()}"
+        proto = fs.protocol[0] if isinstance(fs.protocol, (list, tuple)) else fs.protocol
+        self.get_mtime = self.mtime_dispatch.get(proto, self.mtime_dispatch["file"])
         self._fs = fs
         self._original_contents: t.Optional[bytes] = None
         self._is_locked = False
 
     def _sync_locks(self) -> t.Dict[str, t.Tuple[float, str]]:
         """Gets a map of lock paths to their last modified times and removes stale locks."""
         output = {}
         now = datetime.now()
 
         for lock in self._fs.glob(self.lock_prefix + ".*", refresh=True, detail=True).values():
-            mtime = self.mtime_dispatch[self._fs.protocol](lock)
+            mtime = self.get_mtime(lock)
             name = lock["name"]
             if now - mtime > timedelta(seconds=LOCK_TTL_SECONDS):
                 # Manage stale locks
                 self._fs.rm(name)
                 continue
             # this creates a sortable key
             # the mtime of the file, followed by the name, which is also time sortable
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh/utils/yaml.py` & `sqlmesh-0.5.0/sqlmesh/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.5.0/sqlmesh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.4.2.dev9
-Summary: UNKNOWN
+Version: 0.5.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: web
-Provides-Extra: snowflake
 Provides-Extra: bigquery
 Provides-Extra: databricks
-Provides-Extra: redshift
+Provides-Extra: dev
 Provides-Extra: dbt
+Provides-Extra: postgres
+Provides-Extra: redshift
+Provides-Extra: snowflake
+Provides-Extra: web
 License-File: LICENSE
 
 ![SQLMesh logo](sqlmesh.svg)
 
 SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
 
 For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
@@ -41,9 +40,7 @@
 
 * Join the [Tobiko Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) to ask questions, or just to say hi!
 * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
 * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
 
 ## Contribution
 Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-
-
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.5.0/sqlmesh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,27 @@
 docs/concepts/audits.md
 docs/concepts/environments.md
 docs/concepts/glossary.md
 docs/concepts/hooks.md
 docs/concepts/macros.md
 docs/concepts/overview.md
 docs/concepts/plans.md
-docs/concepts/team_development.md
 docs/concepts/tests.md
 docs/concepts/architecture/serialization.md
 docs/concepts/architecture/snapshots.md
 docs/concepts/models/model_kinds.md
 docs/concepts/models/overview.md
 docs/concepts/models/python_models.md
 docs/concepts/models/seed_models.md
 docs/concepts/models/sql_models.md
 docs/concepts/plans/model_versioning.png
 docs/guides/connections.md
+docs/guides/migrations.md
 docs/guides/models.md
+docs/guides/multi_repo.md
 docs/guides/projects.md
 docs/guides/scheduling.md
 docs/guides/testing.md
 docs/guides/scheduling/airflow_successful_plan_apply.png
 docs/guides/scheduling/airflow_successful_setup.png
 docs/integrations/airflow.md
 docs/integrations/dbt.md
@@ -65,14 +66,30 @@
 examples/airflow/README.md
 examples/airflow/__init__.py
 examples/airflow/docker_compose_decorator.py
 examples/airflow/requirements.txt
 examples/airflow/dags/sqlmesh_integration.py
 examples/airflow/spark_conf/hive-site.xml
 examples/airflow/spark_conf/spark-defaults.conf
+examples/multi/repo_1/config.yaml
+examples/multi/repo_1/audits/.gitkeep
+examples/multi/repo_1/macros/.gitkeep
+examples/multi/repo_1/macros/__init__.py
+examples/multi/repo_1/models/.gitkeep
+examples/multi/repo_1/models/a.sql
+examples/multi/repo_1/models/b.sql
+examples/multi/repo_1/tests/.gitkeep
+examples/multi/repo_2/config.yaml
+examples/multi/repo_2/audits/.gitkeep
+examples/multi/repo_2/macros/.gitkeep
+examples/multi/repo_2/macros/__init__.py
+examples/multi/repo_2/models/.gitkeep
+examples/multi/repo_2/models/c.sql
+examples/multi/repo_2/models/d.sql
+examples/multi/repo_2/tests/.gitkeep
 examples/sushi/__init__.py
 examples/sushi/config.py
 examples/sushi/helper.py
 examples/sushi/audits/items.sql
 examples/sushi/audits/order_items.sql
 examples/sushi/data/.keep
 examples/sushi/hooks/__init__.py
@@ -138,21 +155,21 @@
 examples/wursthall/models/src/order_item_details.py
 examples/wursthall/models/src/shared.py
 examples/wursthall/seeds/src/menu_item_details.csv
 examples/wursthall/tests/test_customer_d.yaml
 examples/wursthall/tests/test_order_item_f.yaml
 pdoc/cli.py
 pdoc/templates/module.html.jinja2
-posts/virtual_environments.md
-posts/virtual_environments/change_categorization.png
-posts/virtual_environments/isolated_rigid_envs.png
-posts/virtual_environments/partial_breaking.png
-posts/virtual_environments/stateful_envs.png
-posts/virtual_environments/virtual_envs.png
-posts/virtual_environments/virtual_envs_end_to_end.png
+posts/virtual_data_environments.md
+posts/virtual_data_environments/change_categorization.png
+posts/virtual_data_environments/isolated_rigid_envs.png
+posts/virtual_data_environments/partial_breaking.png
+posts/virtual_data_environments/stateful_envs.png
+posts/virtual_data_environments/virtual_envs.png
+posts/virtual_data_environments/virtual_envs_end_to_end.png
 sqlmesh/.airflowignore
 sqlmesh/__init__.py
 sqlmesh/_version.py
 sqlmesh/magics.py
 sqlmesh/py.typed
 sqlmesh.egg-info/PKG-INFO
 sqlmesh.egg-info/SOURCES.txt
@@ -192,26 +209,26 @@
 sqlmesh/core/config/loader.py
 sqlmesh/core/config/model.py
 sqlmesh/core/config/root.py
 sqlmesh/core/config/scheduler.py
 sqlmesh/core/engine_adapter/__init__.py
 sqlmesh/core/engine_adapter/_typing.py
 sqlmesh/core/engine_adapter/base.py
+sqlmesh/core/engine_adapter/base_postgres.py
 sqlmesh/core/engine_adapter/base_spark.py
 sqlmesh/core/engine_adapter/bigquery.py
 sqlmesh/core/engine_adapter/databricks.py
 sqlmesh/core/engine_adapter/databricks_api.py
 sqlmesh/core/engine_adapter/duckdb.py
 sqlmesh/core/engine_adapter/postgres.py
 sqlmesh/core/engine_adapter/redshift.py
 sqlmesh/core/engine_adapter/shared.py
 sqlmesh/core/engine_adapter/snowflake.py
 sqlmesh/core/engine_adapter/spark.py
 sqlmesh/core/model/__init__.py
-sqlmesh/core/model/cache.py
 sqlmesh/core/model/common.py
 sqlmesh/core/model/decorator.py
 sqlmesh/core/model/definition.py
 sqlmesh/core/model/kind.py
 sqlmesh/core/model/meta.py
 sqlmesh/core/model/seed.py
 sqlmesh/core/plan/__init__.py
@@ -227,14 +244,15 @@
 sqlmesh/core/state_sync/engine_adapter.py
 sqlmesh/dbt/__init__.py
 sqlmesh/dbt/adapter.py
 sqlmesh/dbt/basemodel.py
 sqlmesh/dbt/builtin.py
 sqlmesh/dbt/column.py
 sqlmesh/dbt/common.py
+sqlmesh/dbt/context.py
 sqlmesh/dbt/loader.py
 sqlmesh/dbt/model.py
 sqlmesh/dbt/package.py
 sqlmesh/dbt/profile.py
 sqlmesh/dbt/project.py
 sqlmesh/dbt/seed.py
 sqlmesh/dbt/source.py
@@ -250,14 +268,15 @@
 sqlmesh/integrations/__init__.py
 sqlmesh/integrations/github/__init__.py
 sqlmesh/integrations/github/notification_operator_provider.py
 sqlmesh/integrations/github/notification_target.py
 sqlmesh/integrations/github/shared.py
 sqlmesh/migrations/__init__.py
 sqlmesh/migrations/v0001_init.py
+sqlmesh/migrations/v0002_remove_identify.py
 sqlmesh/schedulers/__init__.py
 sqlmesh/schedulers/airflow/__init__.py
 sqlmesh/schedulers/airflow/api.py
 sqlmesh/schedulers/airflow/client.py
 sqlmesh/schedulers/airflow/common.py
 sqlmesh/schedulers/airflow/dag_generator.py
 sqlmesh/schedulers/airflow/integration.py
@@ -269,14 +288,15 @@
 sqlmesh/schedulers/airflow/hooks/bigquery.py
 sqlmesh/schedulers/airflow/hooks/redshift.py
 sqlmesh/schedulers/airflow/operators/__init__.py
 sqlmesh/schedulers/airflow/operators/bigquery.py
 sqlmesh/schedulers/airflow/operators/databricks.py
 sqlmesh/schedulers/airflow/operators/hwm_sensor.py
 sqlmesh/schedulers/airflow/operators/notification.py
+sqlmesh/schedulers/airflow/operators/postgres.py
 sqlmesh/schedulers/airflow/operators/redshift.py
 sqlmesh/schedulers/airflow/operators/snowflake.py
 sqlmesh/schedulers/airflow/operators/spark_submit.py
 sqlmesh/schedulers/airflow/operators/targets.py
 sqlmesh/utils/__init__.py
 sqlmesh/utils/concurrency.py
 sqlmesh/utils/connection_pool.py
@@ -310,18 +330,20 @@
 tests/core/test_schema_diff.py
 tests/core/test_seed.py
 tests/core/test_snapshot.py
 tests/core/test_snapshot_evaluator.py
 tests/core/test_state_sync.py
 tests/core/engine_adapter/__init__.py
 tests/core/engine_adapter/test_base.py
+tests/core/engine_adapter/test_base_postgres.py
 tests/core/engine_adapter/test_base_spark.py
 tests/core/engine_adapter/test_bigquery.py
 tests/core/engine_adapter/test_databricks.py
 tests/core/engine_adapter/test_duckdb.py
+tests/core/engine_adapter/test_postgres.py
 tests/core/engine_adapter/test_redshift.py
 tests/core/engine_adapter/test_spark.py
 tests/dbt/__init__.py
 tests/dbt/conftest.py
 tests/dbt/test_adapter.py
 tests/dbt/test_config.py
 tests/dbt/test_transformation.py
@@ -403,14 +425,28 @@
 web/client/package-lock.json
 web/client/package.json
 web/client/playwright.config.ts
 web/client/postcss.config.js
 web/client/tailwind.config.js
 web/client/tsconfig.json
 web/client/vite.config.ts
+web/client/dist/index.html
+web/client/dist/assets/CircularStd-Black-52659624.otf
+web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+web/client/dist/assets/Graph-2afdb6eb.js
+web/client/dist/assets/Graph-34acea2c.css
+web/client/dist/assets/Plan-317aab54.js
+web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+web/client/dist/assets/Publico-Bold-c79acd56.otf
+web/client/dist/assets/Publico-Medium-01b4a891.otf
+web/client/dist/assets/index-0d5132a3.js
+web/client/dist/assets/index-4452b6b5.css
+web/client/dist/assets/worker-e891d118.js
+web/client/dist/favicons/favicon.ico
 web/client/public/favicons/favicon.ico
 web/client/src/index.css
 web/client/src/main.tsx
 web/client/src/routes.tsx
 web/client/src/api/channels.ts
 web/client/src/api/index.ts
 web/client/src/api/instance.ts
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.5.0/sqlmesh.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 hyperscript
 jinja2
 pandas
 pydantic<2.0.0,>=1.9.1
 requests
 rich
 ruamel.yaml
-sqlglot~=11.5.3
+sqlglot~=11.5.4
 fsspec
 
 [bigquery]
 google-cloud-bigquery[pandas]
 
 [databricks]
 databricks-sql-connector
@@ -48,14 +48,17 @@
 sqlalchemy-stubs
 tenacity==8.1.0
 types-croniter
 types-dateparser
 types-pytz
 types-requests==2.28.8
 
+[postgres]
+psycopg2
+
 [redshift]
 redshift_connector
 
 [snowflake]
 snowflake-connector-python[pandas]
 
 [web]
```

### Comparing `sqlmesh-0.4.2.dev9/sqlmesh.svg` & `sqlmesh-0.5.0/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/conftest.py` & `sqlmesh-0.5.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from sqlmesh.utils.date import TimeLike
 
 pytest_plugins = ["tests.common_fixtures"]
 
 
 @pytest.fixture
 def context(tmpdir) -> Context:
-    return Context(path=str(tmpdir))
+    return Context(paths=str(tmpdir))
 
 
 @pytest.fixture
 def duck_conn() -> duckdb.DuckDBPyConnection:
     return duckdb.connect()
 
 
@@ -31,65 +31,63 @@
     plan_evaluator = BuiltInPlanEvaluator(context.state_sync, context.snapshot_evaluator)
     plan_evaluator._push(plan)
     plan_evaluator._promote(plan)
 
 
 @pytest.fixture()
 def sushi_context_pre_scheduling(mocker: MockerFixture) -> Context:
-    context, plan = init_and_plan_sushi_context("examples/sushi", mocker)
+    context, plan = init_and_plan_context("examples/sushi", mocker)
     push_plan(context, plan)
     return context
 
 
 @pytest.fixture()
 def sushi_context_fixed_date(mocker: MockerFixture) -> Context:
-    context, plan = init_and_plan_sushi_context("examples/sushi", mocker)
+    context, plan = init_and_plan_context("examples/sushi", mocker)
 
     for model in context.models.values():
         if model.start:
             context.upsert_model(model.name, start="2022-01-01")
 
     plan = context.plan("prod")
     plan.set_start("1 week ago")
     push_plan(context, plan)
     return context
 
 
 @pytest.fixture()
 def sushi_context(mocker: MockerFixture) -> Context:
-    context, plan = init_and_plan_sushi_context("examples/sushi", mocker)
+    context, plan = init_and_plan_context("examples/sushi", mocker)
     context.apply(plan)
     return context
 
 
 @pytest.fixture()
 def sushi_dbt_context(mocker: MockerFixture) -> Context:
-    context, plan = init_and_plan_sushi_context("examples/sushi_dbt", mocker, "Jan 1 2022")
+    context, plan = init_and_plan_context("examples/sushi_dbt", mocker, "Jan 1 2022")
 
     context.apply(plan)
     return context
 
 
 @pytest.fixture()
 def sushi_test_dbt_context(mocker: MockerFixture) -> Context:
     from tests.fixtures.dbt.sushi_test.seed_sources import init_raw_schema
 
-    context, plan = init_and_plan_sushi_context(
-        "tests/fixtures/dbt/sushi_test", mocker, "Jan 1 2022"
-    )
+    context, plan = init_and_plan_context("tests/fixtures/dbt/sushi_test", mocker, "Jan 1 2022")
     init_raw_schema(context.engine_adapter)
 
     context.apply(plan)
     return context
 
 
-def init_and_plan_sushi_context(
-    path: str, mocker: MockerFixture, start: TimeLike = "1 week ago"
+def init_and_plan_context(
+    paths: str | t.List[str], mocker: MockerFixture, start: TimeLike = "1 week ago"
 ) -> t.Tuple[Context, Plan]:
-    sushi_context = Context(path=path, config="test_config")
+    sushi_context = Context(paths=paths, config="test_config")
     confirm = mocker.patch("sqlmesh.core.console.Confirm")
     confirm.ask.return_value = False
 
     plan = sushi_context.plan("prod")
     plan.set_start(start)
 
     return (sushi_context, plan)
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.5.0/tests/core/engine_adapter/test_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     adapter.create_view("test_view", parse_one("SELECT a FROM tbl"))
     adapter.create_view("test_view", parse_one("SELECT a FROM tbl"), replace=False)
 
     cursor_mock.execute.assert_has_calls(
         [
-            call('CREATE OR REPLACE VIEW "test_view" AS SELECT "a" FROM "tbl"'),
-            call('CREATE VIEW "test_view" AS SELECT "a" FROM "tbl"'),
+            call("CREATE OR REPLACE VIEW test_view AS SELECT a FROM tbl"),
+            call("CREATE VIEW test_view AS SELECT a FROM tbl"),
         ]
     )
 
 
 def test_create_schema(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
@@ -36,16 +36,16 @@
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     adapter.create_schema("test_schema")
     adapter.create_schema("test_schema", ignore_if_exists=False)
 
     cursor_mock.execute.assert_has_calls(
         [
-            call('CREATE SCHEMA IF NOT EXISTS "test_schema"'),
-            call('CREATE SCHEMA "test_schema"'),
+            call("CREATE SCHEMA IF NOT EXISTS test_schema"),
+            call("CREATE SCHEMA test_schema"),
         ]
     )
 
 
 def test_columns(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
@@ -65,36 +65,36 @@
     assert adapter.columns("test_table") == {
         "id": exp.DataType.build("int"),
         "name": exp.DataType.build("string"),
         "price": exp.DataType.build("double"),
         "ds": exp.DataType.build("string"),
     }
 
-    cursor_mock.execute.assert_called_once_with('DESCRIBE "test_table"')
+    cursor_mock.execute.assert_called_once_with("DESCRIBE test_table")
 
 
 def test_table_exists(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     assert adapter.table_exists("test_table")
     cursor_mock.execute.assert_called_once_with(
-        'DESCRIBE "test_table"',
+        "DESCRIBE test_table",
     )
 
     cursor_mock = mocker.Mock()
     cursor_mock.execute.side_effect = RuntimeError("error")
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     assert not adapter.table_exists("test_table")
     cursor_mock.execute.assert_called_once_with(
-        'DESCRIBE "test_table"',
+        "DESCRIBE test_table",
     )
 
 
 def test_insert_overwrite_by_time_partition(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
@@ -108,16 +108,16 @@
     )
 
     cursor_mock.begin.assert_called_once()
     cursor_mock.commit.assert_called_once()
 
     cursor_mock.execute.assert_has_calls(
         [
-            call("DELETE FROM \"test_table\" WHERE \"b\" BETWEEN '2022-01-01' AND '2022-01-02'"),
-            call('INSERT INTO "test_table" ("a") SELECT "a" FROM "tbl"'),
+            call("DELETE FROM test_table WHERE b BETWEEN '2022-01-01' AND '2022-01-02'"),
+            call("INSERT INTO test_table (a) SELECT a FROM tbl"),
         ]
     )
 
 
 def test_insert_append_query(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
@@ -126,17 +126,15 @@
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     adapter.insert_append(
         "test_table",
         parse_one("SELECT a FROM tbl"),
         columns_to_types={"a": exp.DataType.build("INT")},
     )
 
-    cursor_mock.execute.assert_called_once_with(
-        'INSERT INTO "test_table" ("a") SELECT "a" FROM "tbl"'
-    )
+    cursor_mock.execute.assert_called_once_with("INSERT INTO test_table (a) SELECT a FROM tbl")
 
 
 def test_insert_append_pandas(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
@@ -153,15 +151,15 @@
 
     cursor_mock.begin.assert_called_once()
     cursor_mock.commit.assert_called_once()
 
     cursor_mock.execute.assert_has_calls(
         [
             call(
-                'INSERT INTO "test_table" ("a", "b") SELECT CAST("a" AS INT) AS "a", CAST("b" AS INT) AS "b" FROM (VALUES (CAST(1 AS INT), CAST(4 AS INT)), (2, 5), (3, 6)) AS "t"("a", "b")'
+                "INSERT INTO test_table (a, b) SELECT CAST(a AS INT) AS a, CAST(b AS INT) AS b FROM (VALUES (CAST(1 AS INT), CAST(4 AS INT)), (2, 5), (3, 6)) AS t(a, b)"
             ),
         ]
     )
 
 
 def test_create_table(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
@@ -173,15 +171,15 @@
         "colb": exp.DataType.build("TEXT"),
     }
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     adapter.create_table("test_table", columns_to_types)
 
     cursor_mock.execute.assert_called_once_with(
-        'CREATE TABLE IF NOT EXISTS "test_table" ("cola" INT, "colb" TEXT)'
+        "CREATE TABLE IF NOT EXISTS test_table (cola INT, colb TEXT)"
     )
 
 
 def test_create_table_properties(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
@@ -196,26 +194,26 @@
         "test_table",
         columns_to_types,
         partitioned_by=["colb"],
         storage_format="ICEBERG",
     )
 
     cursor_mock.execute.assert_called_once_with(
-        'CREATE TABLE IF NOT EXISTS "test_table" ("cola" INT, "colb" TEXT)'
+        "CREATE TABLE IF NOT EXISTS test_table (cola INT, colb TEXT)"
     )
 
 
 @pytest.mark.parametrize(
     "schema_differ_config, current_table, target_table, expected_final_structure, expected",
     [
         (
             {
                 "support_positional_add": True,
                 "support_nested_operations": True,
-                "array_suffix": ".element",
+                "array_element_selector": "element",
             },
             {
                 "a": "INT",
                 "b": "TEXT",
                 "c": "INT",
                 "d": "INT",
                 "nested": "STRUCT<nested_a INT, nested_c INT>",
@@ -234,26 +232,26 @@
                 "a": "INT",
                 "e": "TEXT",
                 "b": "TEXT",
                 "nested": "STRUCT<nested_a INT, nested_b INT, nested_c INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_b INT, array_c INT>>",
             },
             [
-                """ALTER TABLE "test_table" DROP COLUMN "c\"""",
-                """ALTER TABLE "test_table" DROP COLUMN "d\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "f" VARCHAR(100) FIRST""",
-                """ALTER TABLE "test_table" ADD COLUMN "e" TEXT AFTER "a\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested.nested_b" INT AFTER "nested_a\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col.element.array_b" INT AFTER "array_a\"""",
+                """ALTER TABLE test_table DROP COLUMN c""",
+                """ALTER TABLE test_table DROP COLUMN d""",
+                """ALTER TABLE test_table ADD COLUMN f VARCHAR(100) FIRST""",
+                """ALTER TABLE test_table ADD COLUMN e TEXT AFTER a""",
+                """ALTER TABLE test_table ADD COLUMN nested.nested_b INT AFTER nested_a""",
+                """ALTER TABLE test_table ADD COLUMN array_col.element.array_b INT AFTER array_a""",
             ],
         ),
         (
             {
                 "support_nested_operations": True,
-                "array_suffix": ".element",
+                "array_element_selector": "element",
             },
             {
                 "a": "INT",
                 "b": "TEXT",
                 "c": "INT",
                 "d": "INT",
                 "nested": "STRUCT<nested_a INT, nested_c INT>",
@@ -272,25 +270,25 @@
                 "b": "TEXT",
                 "nested": "STRUCT<nested_a INT, nested_c INT, nested_b INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_c INT, array_b INT>>",
                 "f": "VARCHAR(100)",
                 "e": "TEXT",
             },
             [
-                """ALTER TABLE "test_table" DROP COLUMN "c\"""",
-                """ALTER TABLE "test_table" DROP COLUMN "d\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "f" VARCHAR(100)""",
-                """ALTER TABLE "test_table" ADD COLUMN "e" TEXT""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested.nested_b" INT""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col.element.array_b" INT""",
+                """ALTER TABLE test_table DROP COLUMN c""",
+                """ALTER TABLE test_table DROP COLUMN d""",
+                """ALTER TABLE test_table ADD COLUMN f VARCHAR(100)""",
+                """ALTER TABLE test_table ADD COLUMN e TEXT""",
+                """ALTER TABLE test_table ADD COLUMN nested.nested_b INT""",
+                """ALTER TABLE test_table ADD COLUMN array_col.element.array_b INT""",
             ],
         ),
         (
             {
-                "array_suffix": ".element",
+                "array_element_selector": "element",
             },
             {
                 "a": "INT",
                 "b": "TEXT",
                 "c": "INT",
                 "d": "INT",
                 "nested": "STRUCT<nested_a INT, nested_c INT>",
@@ -309,27 +307,27 @@
                 "b": "TEXT",
                 "f": "VARCHAR(100)",
                 "e": "TEXT",
                 "nested": "STRUCT<nested_a INT, nested_b INT, nested_c INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_b INT, array_c INT>>",
             },
             [
-                """ALTER TABLE "test_table" DROP COLUMN "c\"""",
-                """ALTER TABLE "test_table" DROP COLUMN "d\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "f" VARCHAR(100)""",
-                """ALTER TABLE "test_table" ADD COLUMN "e" TEXT""",
-                """ALTER TABLE "test_table" DROP COLUMN "nested\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested" STRUCT<"nested_a" INT, "nested_b" INT, "nested_c" INT>""",
-                """ALTER TABLE "test_table" DROP COLUMN "array_col\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col" ARRAY<STRUCT<"array_a" INT, "array_b" INT, "array_c" INT>>""",
+                """ALTER TABLE test_table DROP COLUMN c""",
+                """ALTER TABLE test_table DROP COLUMN d""",
+                """ALTER TABLE test_table ADD COLUMN f VARCHAR(100)""",
+                """ALTER TABLE test_table ADD COLUMN e TEXT""",
+                """ALTER TABLE test_table DROP COLUMN nested""",
+                """ALTER TABLE test_table ADD COLUMN nested STRUCT<nested_a INT, nested_b INT, nested_c INT>""",
+                """ALTER TABLE test_table DROP COLUMN array_col""",
+                """ALTER TABLE test_table ADD COLUMN array_col ARRAY<STRUCT<array_a INT, array_b INT, array_c INT>>""",
             ],
         ),
         (
             {
-                "array_suffix": ".element",
+                "array_element_selector": "element",
             },
             {
                 "a": "INT",
                 "b": "TEXT",
                 "c": "INT",
                 "d": "INT",
                 "nested": "STRUCT<nested_a INT, nested_c INT>",
@@ -348,87 +346,87 @@
                 "b": "TEXT",
                 "f": "VARCHAR(100)",
                 "e": "TEXT",
                 "nested": "STRUCT<nested_a INT, nested_b INT, nested_c INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_b INT, array_c INT>>",
             },
             [
-                """ALTER TABLE "test_table" DROP COLUMN "c\"""",
-                """ALTER TABLE "test_table" DROP COLUMN "d\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "f" VARCHAR(100)""",
-                """ALTER TABLE "test_table" ADD COLUMN "e" TEXT""",
-                """ALTER TABLE "test_table" DROP COLUMN "nested\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested" STRUCT<"nested_a" INT, "nested_b" INT, "nested_c" INT>""",
-                """ALTER TABLE "test_table" DROP COLUMN "array_col\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col" ARRAY<STRUCT<"array_a" INT, "array_b" INT, "array_c" INT>>""",
+                """ALTER TABLE test_table DROP COLUMN c""",
+                """ALTER TABLE test_table DROP COLUMN d""",
+                """ALTER TABLE test_table ADD COLUMN f VARCHAR(100)""",
+                """ALTER TABLE test_table ADD COLUMN e TEXT""",
+                """ALTER TABLE test_table DROP COLUMN nested""",
+                """ALTER TABLE test_table ADD COLUMN nested STRUCT<nested_a INT, nested_b INT, nested_c INT>""",
+                """ALTER TABLE test_table DROP COLUMN array_col""",
+                """ALTER TABLE test_table ADD COLUMN array_col ARRAY<STRUCT<array_a INT, array_b INT, array_c INT>>""",
             ],
         ),
         # Test multiple operations on a column with positional and nested features enabled
         (
             {
                 "support_positional_add": True,
                 "support_nested_operations": True,
-                "array_suffix": ".element",
+                "array_element_selector": "element",
             },
             {
-                "nested": "STRUCT<nested_a INT, nested_c INT, nested_e INT>",
-                "array_col": "ARRAY<STRUCT<array_a INT, array_c INT, array_e INT>>",
+                "nested": """STRUCT<nested_a INT, "nested_c" INT, nested_e INT>""",
+                "array_col": """ARRAY<STRUCT<array_a INT, "array_c" INT, array_e INT>>""",
             },
             {
-                "nested": "STRUCT<nested_a INT, nested_b INT, nested_d INT, nested_e INT>",
-                "array_col": "ARRAY<STRUCT<array_a INT, array_b INT, array_d INT, array_e INT>>",
+                "nested": """STRUCT<nested_a INT, "nested_b" INT, nested_d INT, nested_e INT>""",
+                "array_col": """ARRAY<STRUCT<array_a INT, "array_b" INT, array_d INT, array_e INT>>""",
             },
             {
-                "nested": "STRUCT<nested_a INT, nested_b INT, nested_d INT, nested_e INT>",
-                "array_col": "ARRAY<STRUCT<array_a INT, array_b INT, array_d INT, array_e INT>>",
+                "nested": """STRUCT<nested_a INT, "nested_b" INT, nested_d INT, nested_e INT>""",
+                "array_col": """ARRAY<STRUCT<array_a INT, "array_b" INT, array_d INT, array_e INT>>""",
             },
             [
-                """ALTER TABLE "test_table" DROP COLUMN "nested.nested_c\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested.nested_b" INT AFTER "nested_a\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested.nested_d" INT AFTER "nested_b\"""",
-                """ALTER TABLE "test_table" DROP COLUMN "array_col.element.array_c\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col.element.array_b" INT AFTER "array_a\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col.element.array_d" INT AFTER "array_b\"""",
+                """ALTER TABLE test_table DROP COLUMN nested."nested_c\"""",
+                """ALTER TABLE test_table ADD COLUMN nested."nested_b" INT AFTER nested_a""",
+                """ALTER TABLE test_table ADD COLUMN nested.nested_d INT AFTER "nested_b\"""",
+                """ALTER TABLE test_table DROP COLUMN array_col.element."array_c\"""",
+                """ALTER TABLE test_table ADD COLUMN array_col.element."array_b" INT AFTER array_a""",
+                """ALTER TABLE test_table ADD COLUMN array_col.element.array_d INT AFTER "array_b\"""",
             ],
         ),
         # Test multiple operations on a column with positional and nested features enabled and that when adding
         # last we don't include position since it is not needed
         (
             {
                 "support_positional_add": True,
                 "support_nested_operations": True,
-                "array_suffix": ".element",
+                "array_element_selector": "element",
             },
             {
                 "nested": "STRUCT<nested_a INT, nested_c INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_c INT>>",
             },
             {
                 "nested": "STRUCT<nested_a INT, nested_b INT, nested_d INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_b INT, array_d INT>>",
             },
             {
                 "nested": "STRUCT<nested_a INT, nested_b INT, nested_d INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_b INT, array_d INT>>",
             },
             [
-                """ALTER TABLE "test_table" DROP COLUMN "nested.nested_c\"""",
+                """ALTER TABLE test_table DROP COLUMN nested.nested_c""",
                 # Position is not included since we are adding to last so we don't need to specify position
-                """ALTER TABLE "test_table" ADD COLUMN "nested.nested_b" INT""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested.nested_d" INT""",
-                """ALTER TABLE "test_table" DROP COLUMN "array_col.element.array_c\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col.element.array_b" INT""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col.element.array_d" INT""",
+                """ALTER TABLE test_table ADD COLUMN nested.nested_b INT""",
+                """ALTER TABLE test_table ADD COLUMN nested.nested_d INT""",
+                """ALTER TABLE test_table DROP COLUMN array_col.element.array_c""",
+                """ALTER TABLE test_table ADD COLUMN array_col.element.array_b INT""",
+                """ALTER TABLE test_table ADD COLUMN array_col.element.array_d INT""",
             ],
         ),
         # Test multiple operations on a column with positional and no nested features enabled
         (
             {
                 "support_positional_add": True,
-                "array_suffix": ".element",
+                "array_element_selector": "element",
             },
             {
                 "nested": "STRUCT<nested_a INT, nested_c INT, nested_e INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_c INT, array_e INT>>",
                 "col_c": "INT",
             },
             {
@@ -438,25 +436,25 @@
             },
             {
                 "nested": "STRUCT<nested_a INT, nested_b INT, nested_d INT, nested_e INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_b INT, array_d INT, array_e INT>>",
                 "col_c": "INT",
             },
             [
-                """ALTER TABLE "test_table" DROP COLUMN "nested\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested" STRUCT<"nested_a" INT, "nested_b" INT, "nested_d" INT, "nested_e" INT> FIRST""",
-                """ALTER TABLE "test_table" DROP COLUMN "array_col\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col" ARRAY<STRUCT<"array_a" INT, "array_b" INT, "array_d" INT, "array_e" INT>> AFTER "nested\"""",
+                """ALTER TABLE test_table DROP COLUMN nested""",
+                """ALTER TABLE test_table ADD COLUMN nested STRUCT<nested_a INT, nested_b INT, nested_d INT, nested_e INT> FIRST""",
+                """ALTER TABLE test_table DROP COLUMN array_col""",
+                """ALTER TABLE test_table ADD COLUMN array_col ARRAY<STRUCT<array_a INT, array_b INT, array_d INT, array_e INT>> AFTER nested""",
             ],
         ),
         # Test multiple operations on a column with no positional and nested features enabled
         (
             {
                 "support_nested_operations": True,
-                "array_suffix": ".element",
+                "array_element_selector": "element",
             },
             {
                 "nested": "STRUCT<nested_a INT, nested_c INT, nested_e INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_c INT, nested_e INT>>",
                 "col_c": "INT",
             },
             {
@@ -466,26 +464,26 @@
             },
             {
                 "nested": "STRUCT<nested_a INT, nested_e INT, nested_b INT, nested_d INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, nested_e INT, array_b INT, array_d INT>>",
                 "col_c": "INT",
             },
             [
-                """ALTER TABLE "test_table" DROP COLUMN "nested.nested_c\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested.nested_b" INT""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested.nested_d" INT""",
-                """ALTER TABLE "test_table" DROP COLUMN "array_col.element.array_c\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col.element.array_b" INT""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col.element.array_d" INT""",
+                """ALTER TABLE test_table DROP COLUMN nested.nested_c""",
+                """ALTER TABLE test_table ADD COLUMN nested.nested_b INT""",
+                """ALTER TABLE test_table ADD COLUMN nested.nested_d INT""",
+                """ALTER TABLE test_table DROP COLUMN array_col.element.array_c""",
+                """ALTER TABLE test_table ADD COLUMN array_col.element.array_b INT""",
+                """ALTER TABLE test_table ADD COLUMN array_col.element.array_d INT""",
             ],
         ),
         # Test multiple operations on a column with no positional or nested features enabled
         (
             {
-                "array_suffix": ".element",
+                "array_element_selector": "element",
             },
             {
                 "nested": "STRUCT<nested_a INT, nested_c INT, nested_e INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_c INT, array_e INT>>",
                 "col_c": "INT",
             },
             {
@@ -495,18 +493,37 @@
             },
             {
                 "col_c": "INT",
                 "nested": "STRUCT<nested_a INT, nested_b INT, nested_d INT, nested_e INT>",
                 "array_col": "ARRAY<STRUCT<array_a INT, array_b INT, array_d INT, array_e INT>>",
             },
             [
-                """ALTER TABLE "test_table" DROP COLUMN "nested\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "nested" STRUCT<"nested_a" INT, "nested_b" INT, "nested_d" INT, "nested_e" INT>""",
-                """ALTER TABLE "test_table" DROP COLUMN "array_col\"""",
-                """ALTER TABLE "test_table" ADD COLUMN "array_col" ARRAY<STRUCT<"array_a" INT, "array_b" INT, "array_d" INT, "array_e" INT>>""",
+                """ALTER TABLE test_table DROP COLUMN nested""",
+                """ALTER TABLE test_table ADD COLUMN nested STRUCT<nested_a INT, nested_b INT, nested_d INT, nested_e INT>""",
+                """ALTER TABLE test_table DROP COLUMN array_col""",
+                """ALTER TABLE test_table ADD COLUMN array_col ARRAY<STRUCT<array_a INT, array_b INT, array_d INT, array_e INT>>""",
+            ],
+        ),
+        # Test deeply nested structures
+        (
+            {
+                "support_nested_operations": True,
+                "array_element_selector": "element",
+            },
+            {
+                "nested": """STRUCT<nested_1_a STRUCT<"nested_2_a" ARRAY<STRUCT<nested_3_a STRUCT<nested_4_a ARRAY<STRUCT<"nested_5_a" ARRAY<STRUCT<nested_6_a INT>>>>>>>>>""",
+            },
+            {
+                "nested": """STRUCT<nested_1_a STRUCT<"nested_2_a" ARRAY<STRUCT<nested_3_a STRUCT<nested_4_a ARRAY<STRUCT<"nested_5_a" ARRAY<STRUCT<nested_6_a INT, nested_6_b INT>>>>>>>>>""",
+            },
+            {
+                "nested": """STRUCT<nested_1_a STRUCT<"nested_2_a" ARRAY<STRUCT<nested_3_a STRUCT<nested_4_a ARRAY<STRUCT<"nested_5_a" ARRAY<STRUCT<nested_6_a INT, nested_6_b INT>>>>>>>>>""",
+            },
+            [
+                """ALTER TABLE test_table ADD COLUMN nested.nested_1_a."nested_2_a".element.nested_3_a.nested_4_a.element."nested_5_a".element.nested_6_b INT""",
             ],
         ),
     ],
 )
 def test_alter_table(
     mocker: MockerFixture,
     schema_differ_config: t.Dict[str, t.Any],
@@ -565,70 +582,70 @@
     adapter.merge(
         target_table="target",
         source_table="SELECT id, ts, val FROM source",
         column_names=["id", "ts", "val"],
         unique_key=["id"],
     )
     cursor_mock.execute.assert_called_once_with(
-        'MERGE INTO "target" AS "__MERGE_TARGET__" USING (SELECT id, ts, val FROM source) AS __MERGE_SOURCE__ ON "__MERGE_TARGET__"."id" = "__MERGE_SOURCE__"."id" '
-        'WHEN MATCHED THEN UPDATE SET "__MERGE_TARGET__"."id" = "__MERGE_SOURCE__"."id", "__MERGE_TARGET__"."ts" = "__MERGE_SOURCE__"."ts", "__MERGE_TARGET__"."val" = "__MERGE_SOURCE__"."val" '
-        'WHEN NOT MATCHED THEN INSERT ("id", "ts", "val") VALUES ("__MERGE_SOURCE__"."id", "__MERGE_SOURCE__"."ts", "__MERGE_SOURCE__"."val")'
+        "MERGE INTO target AS __MERGE_TARGET__ USING (SELECT id, ts, val FROM source) AS __MERGE_SOURCE__ ON __MERGE_TARGET__.id = __MERGE_SOURCE__.id "
+        "WHEN MATCHED THEN UPDATE SET __MERGE_TARGET__.id = __MERGE_SOURCE__.id, __MERGE_TARGET__.ts = __MERGE_SOURCE__.ts, __MERGE_TARGET__.val = __MERGE_SOURCE__.val "
+        "WHEN NOT MATCHED THEN INSERT (id, ts, val) VALUES (__MERGE_SOURCE__.id, __MERGE_SOURCE__.ts, __MERGE_SOURCE__.val)"
     )
 
     cursor_mock.reset_mock()
     adapter.merge(
         target_table="target",
         source_table="SELECT id, ts, val FROM source",
         column_names=["id", "ts", "val"],
         unique_key=["id", "ts"],
     )
     cursor_mock.execute.assert_called_once_with(
-        'MERGE INTO "target" AS "__MERGE_TARGET__" USING (SELECT id, ts, val FROM source) AS __MERGE_SOURCE__ ON "__MERGE_TARGET__"."id" = "__MERGE_SOURCE__"."id" AND "__MERGE_TARGET__"."ts" = "__MERGE_SOURCE__"."ts" '
-        'WHEN MATCHED THEN UPDATE SET "__MERGE_TARGET__"."id" = "__MERGE_SOURCE__"."id", "__MERGE_TARGET__"."ts" = "__MERGE_SOURCE__"."ts", "__MERGE_TARGET__"."val" = "__MERGE_SOURCE__"."val" '
-        'WHEN NOT MATCHED THEN INSERT ("id", "ts", "val") VALUES ("__MERGE_SOURCE__"."id", "__MERGE_SOURCE__"."ts", "__MERGE_SOURCE__"."val")'
+        "MERGE INTO target AS __MERGE_TARGET__ USING (SELECT id, ts, val FROM source) AS __MERGE_SOURCE__ ON __MERGE_TARGET__.id = __MERGE_SOURCE__.id AND __MERGE_TARGET__.ts = __MERGE_SOURCE__.ts "
+        "WHEN MATCHED THEN UPDATE SET __MERGE_TARGET__.id = __MERGE_SOURCE__.id, __MERGE_TARGET__.ts = __MERGE_SOURCE__.ts, __MERGE_TARGET__.val = __MERGE_SOURCE__.val "
+        "WHEN NOT MATCHED THEN INSERT (id, ts, val) VALUES (__MERGE_SOURCE__.id, __MERGE_SOURCE__.ts, __MERGE_SOURCE__.val)"
     )
 
 
 def test_replace_query(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     adapter.replace_query("test_table", parse_one("SELECT a FROM tbl"), {"a": "int"})
 
     cursor_mock.execute.assert_called_once_with(
-        'CREATE OR REPLACE TABLE "test_table" AS SELECT "a" FROM "tbl"'
+        "CREATE OR REPLACE TABLE test_table AS SELECT a FROM tbl"
     )
 
 
 def test_replace_query_pandas(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     df = pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
     adapter.replace_query("test_table", df, {"a": "int", "b": "int"})
 
     cursor_mock.execute.assert_called_once_with(
-        'CREATE OR REPLACE TABLE "test_table" AS SELECT CAST("a" AS INT) AS "a", CAST("b" AS INT) AS "b" FROM (VALUES (CAST(1 AS INT), CAST(4 AS INT)), (2, 5), (3, 6)) AS "test_table"("a", "b")'
+        "CREATE OR REPLACE TABLE test_table AS SELECT CAST(a AS INT) AS a, CAST(b AS INT) AS b FROM (VALUES (CAST(1 AS INT), CAST(4 AS INT)), (2, 5), (3, 6)) AS test_table(a, b)"
     )
 
 
 def test_create_table_like(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     adapter.create_table_like("target_table", "source_table")
 
     cursor_mock.execute.assert_called_once_with(
-        'CREATE TABLE IF NOT EXISTS "target_table" LIKE "source_table"'
+        "CREATE TABLE IF NOT EXISTS target_table LIKE source_table"
     )
 
 
 def test_create_table_primary_key(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
@@ -638,33 +655,33 @@
         "colb": exp.DataType.build("TEXT"),
     }
 
     adapter = EngineAdapterWithIndexSupport(lambda: connection_mock, "")  # type: ignore
     adapter.create_table("test_table", columns_to_types, primary_key=("cola", "colb"))
 
     cursor_mock.execute.assert_called_once_with(
-        'CREATE TABLE IF NOT EXISTS "test_table" ("cola" INT, "colb" TEXT, PRIMARY KEY("cola", "colb"))'
+        "CREATE TABLE IF NOT EXISTS test_table (cola INT, colb TEXT, PRIMARY KEY (cola, colb))"
     )
 
 
 def test_create_index(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = EngineAdapterWithIndexSupport(lambda: connection_mock, "")  # type: ignore
     adapter.create_index("test_table", "test_index", ("cola", "colb"))
 
     cursor_mock.execute.assert_called_once_with(
-        'CREATE INDEX IF NOT EXISTS "test_index" ON "test_table" ("cola", "colb")'
+        "CREATE INDEX IF NOT EXISTS test_index ON test_table (cola, colb)"
     )
 
 
 def test_rename_table(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = EngineAdapter(lambda: connection_mock, "")  # type: ignore
     adapter.rename_table("old_table", "new_table")
 
-    cursor_mock.execute.assert_called_once_with('ALTER TABLE "old_table" RENAME TO "new_table"')
+    cursor_mock.execute.assert_called_once_with("ALTER TABLE old_table RENAME TO new_table")
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.5.0/tests/core/engine_adapter/test_databricks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # type: ignore
 import pandas as pd
 from pytest_mock.plugin import MockerFixture
 from sqlglot import parse_one
 
-from sqlmesh.core.engine_adapter.base_spark import BaseSparkEngineAdapter
+from sqlmesh.core.engine_adapter import DatabricksSQLEngineAdapter
 
 
 def test_replace_query(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
-    adapter = BaseSparkEngineAdapter(lambda: connection_mock, "spark")
+    adapter = DatabricksSQLEngineAdapter(lambda: connection_mock)
     adapter.replace_query("test_table", parse_one("SELECT a FROM tbl"), {"a": "int"})
 
     cursor_mock.execute.assert_called_once_with(
-        "INSERT OVERWRITE TABLE `test_table` (`a`) SELECT `a` FROM `tbl`"
+        "INSERT OVERWRITE TABLE test_table (a) SELECT a FROM tbl"
     )
 
 
 def test_replace_query_pandas(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
-    adapter = BaseSparkEngineAdapter(lambda: connection_mock, "spark")
+    adapter = DatabricksSQLEngineAdapter(lambda: connection_mock)
     df = pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
     adapter.replace_query("test_table", df, {"a": "int", "b": "int"})
 
     cursor_mock.execute.assert_called_once_with(
-        "INSERT OVERWRITE TABLE `test_table` (`a`, `b`) SELECT CAST(`a` AS INT) AS `a`, CAST(`b` AS INT) AS `b` FROM VALUES (CAST(1 AS INT), CAST(4 AS INT)), (2, 5), (3, 6) AS `test_table`(`a`, `b`)"
+        "INSERT OVERWRITE TABLE test_table (a, b) SELECT CAST(a AS INT) AS a, CAST(b AS INT) AS b FROM VALUES (CAST(1 AS INT), CAST(4 AS INT)), (2, 5), (3, 6) AS test_table(a, b)"
     )
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.5.0/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.5.0/tests/core/engine_adapter/test_base_postgres.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # type: ignore
-import pandas as pd
 from pytest_mock.plugin import MockerFixture
-from sqlglot import parse_one
+from sqlglot import exp
 
-from sqlmesh.core.engine_adapter import DatabricksSQLEngineAdapter
+from sqlmesh.core.engine_adapter.base_postgres import BasePostgresEngineAdapter
 
 
-def test_replace_query(mocker: MockerFixture):
+def test_columns(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
+    cursor_mock.fetchall.return_value = [("col", "INT")]
 
-    adapter = DatabricksSQLEngineAdapter(lambda: connection_mock)
-    adapter.replace_query("test_table", parse_one("SELECT a FROM tbl"), {"a": "int"})
+    adapter = BasePostgresEngineAdapter(lambda: connection_mock, "postgres")
 
+    resp = adapter.columns("db.table")
     cursor_mock.execute.assert_called_once_with(
-        "INSERT OVERWRITE TABLE `test_table` (`a`) SELECT `a` FROM `tbl`"
+        """SELECT column_name, data_type FROM information_schema.columns WHERE table_name = 'table' AND table_schema = 'db'"""
     )
+    assert resp == {"col": exp.DataType.build("INT")}
 
 
-def test_replace_query_pandas(mocker: MockerFixture):
+def test_table_exists(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
+    cursor_mock.fetchone.return_value = (1,)
 
-    adapter = DatabricksSQLEngineAdapter(lambda: connection_mock)
-    df = pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
-    adapter.replace_query("test_table", df, {"a": "int", "b": "int"})
+    adapter = BasePostgresEngineAdapter(lambda: connection_mock, "postgres")
 
+    resp = adapter.table_exists("db.table")
     cursor_mock.execute.assert_called_once_with(
-        "INSERT OVERWRITE TABLE `test_table` (`a`, `b`) SELECT CAST(`a` AS INT) AS `a`, CAST(`b` AS INT) AS `b` FROM VALUES (CAST(1 AS INT), CAST(4 AS INT)), (2, 5), (3, 6) AS `test_table`(`a`, `b`)"
+        """SELECT 1 FROM information_schema.tables WHERE table_name = 'table' AND table_schema = 'db'"""
     )
+    assert resp
+    cursor_mock.fetchone.return_value = None
+    resp = adapter.table_exists("db.table")
+    assert not resp
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.5.0/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.5.0/tests/core/engine_adapter/test_redshift.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,69 +22,89 @@
         adapter.create_view,
         view_name="test_view",
         query_or_df=df,
         columns_to_types={"a": "int", "b": "int"},
     )
 
 
-def test_create_table_from_query_no_exists(mocker: MockerFixture):
+def test_create_table_from_query_exists_no_if_not_exists(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = RedshiftEngineAdapter(lambda: connection_mock)
-    adapter.create_table(
+    mocker.patch(
+        "sqlmesh.core.engine_adapter.redshift.RedshiftEngineAdapter.table_exists",
+        return_value=True,
+    )
+
+    adapter.ctas(
         table_name="test_table",
-        query_or_columns_to_types=parse_one("SELECT cola FROM table"),
+        query_or_df=parse_one("SELECT cola FROM table"),
         exists=False,
     )
 
-    cursor_mock.execute.assert_called_once_with(
-        'CREATE TABLE "test_table" AS SELECT "cola" FROM "table"'
+    cursor_mock.execute.assert_called_once_with("CREATE TABLE test_table AS SELECT cola FROM table")
+
+
+def test_create_table_from_query_exists_and_if_not_exists(mocker: MockerFixture):
+    connection_mock = mocker.NonCallableMock()
+    cursor_mock = mocker.Mock()
+    connection_mock.cursor.return_value = cursor_mock
+
+    adapter = RedshiftEngineAdapter(lambda: connection_mock)
+    mocker.patch(
+        "sqlmesh.core.engine_adapter.redshift.RedshiftEngineAdapter.table_exists",
+        return_value=True,
+    )
+    adapter.ctas(
+        table_name="test_table",
+        query_or_df=parse_one("SELECT cola FROM table"),
+        exists=True,
     )
 
+    cursor_mock.execute.assert_not_called()
+
 
-def test_create_table_from_query_exists(mocker: MockerFixture):
+def test_create_table_from_query_not_exists_if_not_exists(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = RedshiftEngineAdapter(lambda: connection_mock)
     mocker.patch(
         "sqlmesh.core.engine_adapter.redshift.RedshiftEngineAdapter.table_exists",
         return_value=False,
     )
-    adapter.create_table(
+    adapter.ctas(
         table_name="test_table",
-        query_or_columns_to_types=parse_one("SELECT cola FROM table"),
+        query_or_df=parse_one("SELECT cola FROM table"),
         exists=True,
     )
 
-    cursor_mock.execute.assert_called_once_with(
-        'CREATE TABLE "test_table" AS SELECT "cola" FROM "table"'
-    )
+    cursor_mock.execute.assert_called_once_with("CREATE TABLE test_table AS SELECT cola FROM table")
 
 
-def test_create_table_from_query_already_exists(mocker: MockerFixture):
+def test_create_table_from_query_not_exists_no_if_not_exists(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = RedshiftEngineAdapter(lambda: connection_mock)
     mocker.patch(
         "sqlmesh.core.engine_adapter.redshift.RedshiftEngineAdapter.table_exists",
-        return_value=True,
+        return_value=False,
     )
-    adapter.create_table(
+    adapter.ctas(
         table_name="test_table",
-        query_or_columns_to_types=parse_one("SELECT cola FROM table"),
-        exists=True,
+        query_or_df=parse_one("SELECT cola FROM table"),
+        exists=False,
     )
 
-    assert not cursor_mock.execute.called
+    cursor_mock.execute.assert_called_once_with("CREATE TABLE test_table AS SELECT cola FROM table")
 
 
 def test_pandas_to_sql(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
@@ -100,18 +120,25 @@
 
 def test_replace_query_with_query(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = RedshiftEngineAdapter(lambda: connection_mock)
+    mocker.patch(
+        "sqlmesh.core.engine_adapter.redshift.RedshiftEngineAdapter.table_exists",
+        return_value=False,
+    )
     adapter.replace_query(table_name="test_table", query_or_df=parse_one("SELECT cola FROM table"))
 
-    cursor_mock.execute.assert_called_once_with(
-        'CREATE OR REPLACE TABLE "test_table" AS SELECT "cola" FROM "table"'
+    cursor_mock.execute.assert_has_calls(
+        [
+            mocker.call("DROP TABLE IF EXISTS test_table"),
+            mocker.call("CREATE TABLE test_table AS SELECT cola FROM table"),
+        ]
     )
 
 
 def test_replace_query_with_df_table_exists(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
@@ -136,21 +163,21 @@
     )
 
     cursor_mock.begin.assert_called_once()
     cursor_mock.commit.assert_called_once()
 
     cursor_mock.execute.assert_has_calls(
         [
-            call('CREATE TABLE "test_table_temp_1234" ("a" INTEGER, "b" INTEGER)'),
+            call("CREATE TABLE test_table_temp_1234 (a INTEGER, b INTEGER)"),
             call(
-                'INSERT INTO "test_table_temp_1234" ("a", "b") VALUES (CAST(1 AS INTEGER), CAST(4 AS INTEGER)), (2, 5), (3, 6)'
+                "INSERT INTO test_table_temp_1234 (a, b) VALUES (CAST(1 AS INTEGER), CAST(4 AS INTEGER)), (2, 5), (3, 6)"
             ),
-            call('ALTER TABLE "test_table" RENAME TO "test_table_old_1234"'),
-            call('ALTER TABLE "test_table_temp_1234" RENAME TO "test_table"'),
-            call('DROP TABLE IF EXISTS "test_table_old_1234"'),
+            call("ALTER TABLE test_table RENAME TO test_table_old_1234"),
+            call("ALTER TABLE test_table_temp_1234 RENAME TO test_table"),
+            call("DROP TABLE IF EXISTS test_table_old_1234"),
         ]
     )
 
 
 def test_replace_query_with_df_table_not_exists(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
@@ -169,17 +196,17 @@
             "a": exp.DataType.build("int"),
             "b": exp.DataType.build("int"),
         },
     )
 
     cursor_mock.execute.assert_has_calls(
         [
-            call('CREATE TABLE "test_table" ("a" INTEGER, "b" INTEGER)'),
+            call("CREATE TABLE test_table (a INTEGER, b INTEGER)"),
             call(
-                'INSERT INTO "test_table" ("a", "b") VALUES (CAST(1 AS INTEGER), CAST(4 AS INTEGER)), (2, 5), (3, 6)'
+                "INSERT INTO test_table (a, b) VALUES (CAST(1 AS INTEGER), CAST(4 AS INTEGER)), (2, 5), (3, 6)"
             ),
         ]
     )
 
 
 def test_table_exists_db_table(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
@@ -187,23 +214,23 @@
     connection_mock.cursor.return_value = cursor_mock
     connection_mock.cursor.return_value.fetchone.return_value = (1,)
 
     adapter = RedshiftEngineAdapter(lambda: connection_mock)
     assert adapter.table_exists(table_name=exp.to_table("some_db.some_table"))
 
     cursor_mock.execute.assert_called_once_with(
-        """SELECT 1 FROM "information_schema"."tables" WHERE "table_name" = 'some_table' AND "table_schema" = 'some_db'"""
+        "SELECT 1 FROM information_schema.tables WHERE table_name = 'some_table' AND table_schema = 'some_db'"
     )
 
 
 def test_table_exists_table_only(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
     connection_mock.cursor.return_value.fetchone.return_value = None
 
     adapter = RedshiftEngineAdapter(lambda: connection_mock)
     assert not adapter.table_exists(table_name=exp.to_table("some_table"))
 
     cursor_mock.execute.assert_called_once_with(
-        """SELECT 1 FROM "information_schema"."tables" WHERE "table_name" = 'some_table'"""
+        "SELECT 1 FROM information_schema.tables WHERE table_name = 'some_table'"
     )
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.5.0/tests/core/engine_adapter/test_spark.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "test_table",
         columns_to_types,
         partitioned_by=["colb"],
         storage_format="ICEBERG",
     )
 
     cursor_mock.execute.assert_called_once_with(
-        "CREATE TABLE IF NOT EXISTS `test_table` (`cola` INT, `colb` STRING) USING ICEBERG PARTITIONED BY (`colb`)"
+        "CREATE TABLE IF NOT EXISTS test_table (cola INT, colb STRING) USING ICEBERG PARTITIONED BY (colb)"
     )
 
 
 def test_alter_table(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
@@ -60,31 +60,31 @@
 
     adapter.columns = table_columns
 
     adapter.alter_table(current_table_name, target_table_name)
 
     cursor_mock.execute.assert_has_calls(
         [
-            call("""ALTER TABLE `test_table` DROP COLUMN `b`"""),
-            call("""ALTER TABLE `test_table` DROP COLUMN `id`"""),
-            call("""ALTER TABLE `test_table` ADD COLUMN `id` LONG"""),
-            call("""ALTER TABLE `test_table` DROP COLUMN `a`"""),
-            call("""ALTER TABLE `test_table` ADD COLUMN `a` STRING"""),
-            call("""ALTER TABLE `test_table` DROP COLUMN `complex`"""),
-            call("""ALTER TABLE `test_table` ADD COLUMN `complex` STRUCT<`complex_a`: INT>"""),
-            call("""ALTER TABLE `test_table` DROP COLUMN `ds`"""),
-            call("""ALTER TABLE `test_table` ADD COLUMN `ds` INT"""),
+            call("""ALTER TABLE test_table DROP COLUMN b"""),
+            call("""ALTER TABLE test_table DROP COLUMN id"""),
+            call("""ALTER TABLE test_table ADD COLUMN id LONG"""),
+            call("""ALTER TABLE test_table DROP COLUMN a"""),
+            call("""ALTER TABLE test_table ADD COLUMN a STRING"""),
+            call("""ALTER TABLE test_table DROP COLUMN complex"""),
+            call("""ALTER TABLE test_table ADD COLUMN complex STRUCT<complex_a: INT>"""),
+            call("""ALTER TABLE test_table DROP COLUMN ds"""),
+            call("""ALTER TABLE test_table ADD COLUMN ds INT"""),
         ]
     )
 
 
 def test_replace_query(mocker: MockerFixture):
     connection_mock = mocker.NonCallableMock()
     cursor_mock = mocker.Mock()
     connection_mock.cursor.return_value = cursor_mock
 
     adapter = SparkEngineAdapter(lambda: connection_mock, "spark")
     adapter.replace_query("test_table", parse_one("SELECT a FROM tbl"), {"a": "int"})
 
     cursor_mock.execute.assert_called_once_with(
-        "INSERT OVERWRITE TABLE `test_table` (`a`) SELECT `a` FROM `tbl`"
+        "INSERT OVERWRITE TABLE test_table (a) SELECT a FROM tbl"
     )
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_audit.py` & `sqlmesh-0.5.0/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_config.py` & `sqlmesh-0.5.0/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_connection_config.py` & `sqlmesh-0.5.0/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_context.py` & `sqlmesh-0.5.0/tests/core/test_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,62 +13,50 @@
 from sqlmesh.core.plan import BuiltInPlanEvaluator, Plan
 from sqlmesh.utils.date import yesterday_ds
 from sqlmesh.utils.errors import ConfigError
 from tests.utils.test_filesystem import create_temp_file
 
 
 def test_global_config():
-    context = Context(path="examples/sushi")
-    assert context.dialect == "duckdb"
-    assert context.physical_schema == "sqlmesh"
+    context = Context(paths="examples/sushi")
+    assert context.config.dialect is None
+    assert context.config.physical_schema == "sqlmesh"
 
 
 def test_named_config():
-    context = Context(path="examples/sushi", config="local_config")
-    assert context.dialect == "duckdb"
+    context = Context(paths="examples/sushi", config="local_config")
+    assert len(context.config.connections) == 1
 
 
 def test_invalid_named_config():
     with pytest.raises(
         ConfigError,
         match="Config 'blah' was not found.",
     ):
-        Context(path="examples/sushi", config="blah")
+        Context(paths="examples/sushi", config="blah")
 
 
 def test_missing_named_config():
     with pytest.raises(ConfigError, match=r"Config 'imaginary_config' was not found."):
-        Context(path="examples/sushi", config="imaginary_config")
-
-
-def test_config_precedence():
-    context = Context(path="examples/sushi", dialect="spark", physical_schema="test")
-    assert context.dialect == "spark"
-    assert context.physical_schema == "test"
-
-    # Context parameters take precedence over config
-    config = Config(model_defaults=ModelDefaultsConfig(dialect="presto"), physical_schema="dev")
-    context = Context(path="examples/sushi", dialect="spark", physical_schema="test", config=config)
-    assert context.dialect == "spark"
-    assert context.physical_schema == "test"
+        Context(paths="examples/sushi", config="imaginary_config")
 
 
 def test_config_parameter():
     config = Config(model_defaults=ModelDefaultsConfig(dialect="presto"), physical_schema="dev")
-    context = Context(path="examples/sushi", config=config)
-    assert context.dialect == "presto"
-    assert context.physical_schema == "dev"
+    context = Context(paths="examples/sushi", config=config)
+    assert context.config.dialect == "presto"
+    assert context.config.physical_schema == "dev"
 
 
 def test_config_not_found():
     with pytest.raises(
         ConfigError,
-        match=r"^nonexistent/directory is not a directory.*",
+        match=r".*config could not be found.*",
     ):
-        Context(path="nonexistent/directory", config="local_config")
+        Context(paths="nonexistent/directory", config="local_config")
 
 
 def test_custom_macros(sushi_context):
     assert "add_one" in sushi_context.macros
 
 
 def test_dag(sushi_context):
@@ -160,15 +148,15 @@
           o.ds
         HAVING
           CAST(o.ds AS TEXT) <= '2021-01-01' AND CAST(o.ds AS TEXT) >= '2021-01-01'
         """,
     )
 
     # unpushed render still works
-    unpushed = Context(path="examples/sushi")
+    unpushed = Context(paths="examples/sushi")
     assert_exp_eq(
         unpushed.render(snapshot.name),
         f"""
         SELECT
           CAST(o.waiter_id AS INT) AS waiter_id, /* Waiter id */
           CAST(SUM(oi.quantity * i.price) AS DOUBLE) AS revenue, /* Revenue from orders taken by this waiter */
           CAST(o.ds AS TEXT) AS ds /* Date */
@@ -223,15 +211,14 @@
 
     plan_evaluator = BuiltInPlanEvaluator(
         sushi_context.state_sync, sushi_context.snapshot_evaluator
     )
     plan_evaluator._promote(
         Plan(
             context_diff=sushi_context._context_diff("prod"),
-            dag=sushi_context.dag,
             state_reader=sushi_context.state_reader,
         )
     )
 
     sushi_context.upsert_model("sushi.customers", query=parse_one("select 1"))
     sushi_context.diff("test")
     assert mock_console.show_model_difference_summary.called
@@ -312,16 +299,18 @@
 from sqlmesh.core.macros import macro
 
 @macro()
 def test():
     return "test"
 """,
     )
-    config = Config(ignore_patterns=["models/ignore/*.sql", "macro_ignore.py"])
-    context = Context(path=str(tmpdir), config=config)
+    config = Config(
+        ignore_patterns=["models/ignore/*.sql", "macro_ignore.py", ".ipynb_checkpoints/*"]
+    )
+    context = Context(paths=str(tmpdir), config=config)
 
     assert ["db.actual_test"] == list(context.models)
     assert "test" == list(context.macros)[-1]
 
 
 def test_plan_apply(sushi_context) -> None:
     plan = sushi_context.plan(
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_dialect.py` & `sqlmesh-0.5.0/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_integration.py` & `sqlmesh-0.5.0/tests/core/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -606,29 +606,50 @@
     )
 
 
 @pytest.mark.integration
 @pytest.mark.core_integration
 def test_auto_categorization(sushi_context: Context):
     environment = "dev"
-    sushi_context.config.auto_categorize_changes.sql = AutoCategorizationMode.FULL
+    for config in sushi_context.configs.values():
+        config.auto_categorize_changes.sql = AutoCategorizationMode.FULL
     initial_add(sushi_context, environment)
 
     version = sushi_context.snapshots["sushi.waiter_as_customer_by_day"].version
     fingerprint = sushi_context.snapshots["sushi.waiter_as_customer_by_day"].fingerprint
 
     model = t.cast(SqlModel, sushi_context.models["sushi.waiters"])
     sushi_context.upsert_model("sushi.waiters", query=model.query.select("'foo' AS foo"))  # type: ignore
     apply_to_environment(sushi_context, environment)
 
     assert sushi_context.snapshots["sushi.waiter_as_customer_by_day"].change_category is None
     assert sushi_context.snapshots["sushi.waiter_as_customer_by_day"].fingerprint != fingerprint
     assert sushi_context.snapshots["sushi.waiter_as_customer_by_day"].version == version
 
 
+@pytest.mark.integration
+@pytest.mark.core_integration
+def test_multi(mocker):
+    context = Context(paths=["examples/multi/repo_1", "examples/multi/repo_2"])
+    context.state_sync.reset()
+    plan = context.plan()
+    assert len(plan.new_snapshots) == 4
+    context.apply(plan)
+
+    context = Context(paths=["examples/multi/repo_1"])
+    model = context.models["bronze.a"]
+    model.query.select("'c' AS c", copy=False)
+    plan = context.plan()
+    assert set(snapshot.name for snapshot in plan.directly_modified) == {"bronze.a"}
+    assert list(plan.indirectly_modified.values())[0] == {"bronze.b", "silver.c", "silver.d"}
+    assert len(plan.missing_intervals) == 1
+    context.apply(plan)
+    validate_apply_basics(context, c.PROD, plan.snapshots)
+
+
 def initial_add(context: Context, environment: str):
     assert not context.state_reader.get_environment(environment)
 
     plan = context.plan(environment, start=start(context), create_from="nonexistent_env")
     validate_plan_changes(plan, added=context.models)
 
     context.apply(plan)
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_macros.py` & `sqlmesh-0.5.0/tests/core/test_macros.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,19 @@
     ) == exp.table_("y")
 
 
 @pytest.mark.parametrize(
     "sql, expected, args",
     [
         (
+            """select @EACH(['a', 'b'], x -> x)""",
+            "SELECT 'a', 'b'",
+            {},
+        ),
+        (
             """@FILTER_COUNTRY(@'continent = ''NA''', 'USA')""",
             "continent = 'NA' AND country = 'USA'",
             {},
         ),
         ("""@SQL(@REDUCE([100, 200, 300, 400], (x,y) -> x + y))""", "1000", {}),
         (
             """select @EACH([a, b, c], x -> x and @SQL('@y'))""",
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_model.py` & `sqlmesh-0.5.0/tests/core/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -876,40 +876,34 @@
                 (4, 1, '2020-01-04'),
                 (5, 1, '2020-01-05'),
                 (6, 1, '2020-01-06'),
                 (7, 1, '2020-01-07')
             ) AS t (id, item_id, ds)
         """
         ),
-        path=context.path,
-        dialect=context.dialect,
     )
 
     model2 = load_model(
         d.parse(
             """
         MODEL (name db.model2, kind full);
 
         SELECT * FROM db.model1 AS model1
 		"""
         ),
-        path=context.path,
-        dialect=context.dialect,
     )
 
     model3 = load_model(
         d.parse(
             """
             MODEL(name db.model3, kind full);
 
             SELECT * FROM db.model2 AS model2
         """
         ),
-        path=context.path,
-        dialect=context.dialect,
     )
 
     context.upsert_model(model1)
     context.upsert_model(model2)
     context.upsert_model(model3)
 
     assert_exp_eq(
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_plan.py` & `sqlmesh-0.5.0/tests/core/test_plan.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from sqlmesh.core.model.seed import Seed
 from sqlmesh.core.plan import Plan
 from sqlmesh.core.snapshot import (
     SnapshotChangeCategory,
     SnapshotDataVersion,
     SnapshotFingerprint,
 )
-from sqlmesh.utils.dag import DAG
 from sqlmesh.utils.date import to_date, to_datetime, to_timestamp
 from sqlmesh.utils.errors import PlanError
 
 
 def test_forward_only_plan_sets_version(make_snapshot, mocker: MockerFixture):
     snapshot_a = make_snapshot(SqlModel(name="a", query=parse_one("select 1, ds")))
     snapshot_a.set_version()
@@ -30,26 +29,24 @@
                 metadata_hash="test_metadata_hash",
             ),
             version="test_version",
         ),
     )
     assert not snapshot_b.version
 
-    dag = DAG[str]({"b": {"a"}})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a, "b": snapshot_b}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {"b": (snapshot_b, snapshot_b)}
     context_diff_mock.new_snapshots = {snapshot_b.snapshot_id: snapshot_b}
 
     state_reader_mock = mocker.Mock()
 
-    plan = Plan(context_diff_mock, dag, state_reader_mock, forward_only=True)
+    plan = Plan(context_diff_mock, state_reader_mock, forward_only=True)
 
     assert snapshot_b.version == "test_version"
 
     # Make sure that the choice can't be set manually.
     with pytest.raises(PlanError, match="Choice setting is not supported by a forward-only plan."):
         plan.set_choice(snapshot_b, SnapshotChangeCategory.BREAKING)
 
@@ -62,16 +59,14 @@
             kind=IncrementalByTimeRangeKind(time_column="ds"),
         )
     )
 
     expected_start = to_datetime("2022-01-01")
     expected_end = to_datetime("2022-01-02")
 
-    dag = DAG[str]({"a": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {}
     context_diff_mock.new_snapshots = {snapshot_a.snapshot_id: snapshot_a}
 
@@ -80,43 +75,41 @@
     yesterday_ds_mock = mocker.patch("sqlmesh.core.scheduler.yesterday")
     yesterday_ds_mock.return_value = expected_start
 
     now_ds_mock = mocker.patch("sqlmesh.core.plan.definition.now")
     now_ds_mock.return_value = expected_end
     state_reader_mock.missing_intervals.return_value = {}
 
-    plan = Plan(context_diff_mock, dag, state_reader_mock, forward_only=True, is_dev=True)
+    plan = Plan(context_diff_mock, state_reader_mock, forward_only=True, is_dev=True)
 
     assert plan.restatements == {"a"}
     assert plan.start == expected_start
     assert plan.end == expected_end
 
     yesterday_ds_mock.assert_called_once()
     now_ds_mock.call_count == 2
 
 
 def test_forward_only_plan_new_models_not_allowed(make_snapshot, mocker: MockerFixture):
     snapshot_a = make_snapshot(SqlModel(name="a", query=parse_one("select 1, ds")))
     snapshot_a.set_version()
 
-    dag = DAG[str]({"a": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a}
     context_diff_mock.added = {"a"}
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {}
     context_diff_mock.new_snapshots = {}
 
     state_reader_mock = mocker.Mock()
 
     with pytest.raises(
         PlanError, match="New models can't be added as part of the forward-only plan."
     ):
-        Plan(context_diff_mock, dag, state_reader_mock, forward_only=True)
+        Plan(context_diff_mock, state_reader_mock, forward_only=True)
 
 
 def test_paused_forward_only_parent(make_snapshot, mocker: MockerFixture):
     snapshot_a = make_snapshot(SqlModel(name="a", query=parse_one("select 1, ds")))
     snapshot_a.previous_versions = (
         SnapshotDataVersion(
             fingerprint=SnapshotFingerprint(
@@ -125,33 +118,31 @@
             ),
             version="test_version",
             change_category=None,
         ),
     )
     snapshot_a.set_version(snapshot_a.previous_version)
 
-    snapshot_b = make_snapshot(SqlModel(name="b", query=parse_one("select 2, ds")))
+    snapshot_b = make_snapshot(SqlModel(name="b", query=parse_one("select 2, ds from a")))
     assert not snapshot_b.version
 
-    dag = DAG[str]({"b": {"a"}})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a, "b": snapshot_b}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {"b": (snapshot_b, snapshot_b)}
     context_diff_mock.new_snapshots = {snapshot_b.snapshot_id: snapshot_b}
 
     state_reader_mock = mocker.Mock()
 
     with pytest.raises(
         PlanError,
         match=r"Model 'b' depends on a paused version of model 'a'.*",
     ):
-        Plan(context_diff_mock, dag, state_reader_mock, forward_only=False)
+        Plan(context_diff_mock, state_reader_mock, forward_only=False)
 
 
 def test_restate_models(sushi_context_pre_scheduling: Context):
     plan = sushi_context_pre_scheduling.plan(
         restate_models=["sushi.waiter_revenue_by_day"], no_prompts=True
     )
     assert plan.restatements == {"sushi.waiter_revenue_by_day"}
@@ -166,100 +157,93 @@
         SqlModel(
             name="a",
             query=parse_one("select 1, key"),
             kind="VIEW",
         )
     )
 
-    dag = DAG[str]({"a": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {}
     context_diff_mock.new_snapshots = {}
 
     state_reader_mock = mocker.Mock()
 
     with pytest.raises(
         PlanError,
         match=r"Cannot restate from 'a'. Either such model doesn't exist or no other model references it.",
     ):
-        Plan(context_diff_mock, dag, state_reader_mock, restate_models=["a"])
+        Plan(context_diff_mock, state_reader_mock, restate_models=["a"])
 
 
 def test_new_snapshots_with_restatements(make_snapshot, mocker: MockerFixture):
     snapshot_a = make_snapshot(SqlModel(name="a", query=parse_one("select 1, ds")))
 
-    dag = DAG[str]({"a": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {}
     context_diff_mock.new_snapshots = {snapshot_a.snapshot_id: snapshot_a}
 
     state_reader_mock = mocker.Mock()
 
     with pytest.raises(
         PlanError,
         match=r"Model changes and restatements can't be a part of the same plan.*",
     ):
-        Plan(context_diff_mock, dag, state_reader_mock, restate_models=["a"])
+        Plan(context_diff_mock, state_reader_mock, restate_models=["a"])
 
 
 def test_end_validation(make_snapshot, mocker: MockerFixture):
     snapshot_a = make_snapshot(
         SqlModel(
             name="a",
             query=parse_one("select 1, ds"),
             kind=IncrementalByTimeRangeKind(time_column="ds"),
         )
     )
 
-    dag = DAG[str]({"a": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {}
     context_diff_mock.new_snapshots = {snapshot_a.snapshot_id: snapshot_a}
 
     state_reader_mock = mocker.Mock()
 
-    dev_plan = Plan(context_diff_mock, dag, state_reader_mock, end="2022-01-03", is_dev=True)
+    dev_plan = Plan(context_diff_mock, state_reader_mock, end="2022-01-03", is_dev=True)
     assert dev_plan.end == "2022-01-03"
     dev_plan.end = "2022-01-04"
     assert dev_plan.end == "2022-01-04"
 
     start_end_not_allowed_message = (
         "The start and end dates can't be set for a production plan without restatements."
     )
 
     with pytest.raises(PlanError, match=start_end_not_allowed_message):
-        Plan(context_diff_mock, dag, state_reader_mock, end="2022-01-03")
+        Plan(context_diff_mock, state_reader_mock, end="2022-01-03")
 
     with pytest.raises(PlanError, match=start_end_not_allowed_message):
-        Plan(context_diff_mock, dag, state_reader_mock, start="2022-01-03")
+        Plan(context_diff_mock, state_reader_mock, start="2022-01-03")
 
-    prod_plan = Plan(context_diff_mock, dag, state_reader_mock)
+    prod_plan = Plan(context_diff_mock, state_reader_mock)
 
     with pytest.raises(PlanError, match=start_end_not_allowed_message):
         prod_plan.end = "2022-01-03"
 
     with pytest.raises(PlanError, match=start_end_not_allowed_message):
         prod_plan.start = "2022-01-03"
 
     context_diff_mock.new_snapshots = {}
     restatement_prod_plan = Plan(
         context_diff_mock,
-        dag,
         state_reader_mock,
         end="2022-01-03",
         restate_models=["a"],
     )
     assert restatement_prod_plan.end == "2022-01-03"
     restatement_prod_plan.end = "2022-01-04"
     assert restatement_prod_plan.end == "2022-01-04"
@@ -270,39 +254,37 @@
     snapshot.set_version()
     assert not snapshot.is_forward_only
 
     forward_only_snapshot = make_snapshot(SqlModel(name="a", query=parse_one("select 2, ds")))
     forward_only_snapshot.set_version(snapshot.version)
     assert forward_only_snapshot.is_forward_only
 
-    dag = DAG[str]({"a": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {"a": (snapshot, forward_only_snapshot)}
     context_diff_mock.new_snapshots = {}
 
     state_reader_mock = mocker.Mock()
 
     with pytest.raises(
         PlanError,
         match=r"Detected an existing version of model 'a' that has been previously superseded by a forward-only change.*",
     ):
-        Plan(context_diff_mock, dag, state_reader_mock, forward_only=True)
+        Plan(context_diff_mock, state_reader_mock, forward_only=True)
 
     # Make sure the plan can be created if a new snapshot version was enforced.
     new_version_snapshot = make_snapshot(
         SqlModel(name="a", query=parse_one("select 1, ds"), stamp="test_stamp")
     )
     new_version_snapshot.set_version()
     context_diff_mock.modified_snapshots = {"a": (new_version_snapshot, forward_only_snapshot)}
     context_diff_mock.new_snapshots = {new_version_snapshot.snapshot_id: new_version_snapshot}
-    Plan(context_diff_mock, dag, state_reader_mock, forward_only=True)
+    Plan(context_diff_mock, state_reader_mock, forward_only=True)
 
 
 def test_forward_only_plan_seed_models(make_snapshot, mocker: MockerFixture):
     snapshot_a = make_snapshot(
         SeedModel(
             name="a",
             kind=SeedKind(path="./path/to/seed"),
@@ -319,78 +301,72 @@
             seed=Seed(content="new_content"),
             depends_on=set(),
         )
     )
     assert snapshot_a_updated.version is None
     assert snapshot_a_updated.change_category is None
 
-    dag = DAG[str]({"a": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a_updated}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {"a": (snapshot_a_updated, snapshot_a)}
     context_diff_mock.new_snapshots = {snapshot_a_updated.snapshot_id: snapshot_a_updated}
 
     state_reader_mock = mocker.Mock()
 
-    Plan(context_diff_mock, dag, state_reader_mock, forward_only=True)
+    Plan(context_diff_mock, state_reader_mock, forward_only=True)
     assert snapshot_a_updated.version == snapshot_a_updated.fingerprint.to_version()
     assert snapshot_a_updated.change_category == SnapshotChangeCategory.NON_BREAKING
 
 
 def test_start_inference(make_snapshot, mocker: MockerFixture):
     snapshot_a = make_snapshot(
         SqlModel(name="a", query=parse_one("select 1, ds"), start="2022-01-01")
     )
     snapshot_a.set_version()
 
     snapshot_b = make_snapshot(SqlModel(name="b", query=parse_one("select 2, ds")))
     snapshot_b.set_version()
 
-    dag = DAG[str]({"a": set(), "b": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a, "b": snapshot_b}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {}
     context_diff_mock.new_snapshots = {snapshot_b.snapshot_id: snapshot_b}
 
     state_reader_mock = mocker.Mock()
     state_reader_mock.missing_intervals.return_value = {
         snapshot_b: [(to_timestamp("2022-01-01"), to_timestamp("2023-01-01"))]
     }
 
-    plan = Plan(context_diff_mock, dag, state_reader_mock)
+    plan = Plan(context_diff_mock, state_reader_mock)
     assert len(plan._missing_intervals) == 1
     assert snapshot_b.version_get_or_generate() in plan._missing_intervals
 
     assert plan.start == to_timestamp("2022-01-01")
 
 
 def test_auto_categorization(make_snapshot, mocker: MockerFixture):
     snapshot = make_snapshot(SqlModel(name="a", query=parse_one("select 1, ds")))
     snapshot.set_version()
 
     updated_snapshot = make_snapshot(SqlModel(name="a", query=parse_one("select 2, ds")))
 
-    dag = DAG[str]({"a": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": updated_snapshot}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {"a": (updated_snapshot, snapshot)}
     context_diff_mock.new_snapshots = {updated_snapshot.snapshot_id: updated_snapshot}
 
     state_reader_mock = mocker.Mock()
 
-    Plan(context_diff_mock, dag, state_reader_mock)
+    Plan(context_diff_mock, state_reader_mock)
 
     assert updated_snapshot.version == updated_snapshot.fingerprint.to_version()
     assert updated_snapshot.change_category == SnapshotChangeCategory.BREAKING
 
 
 def test_end_from_missing_instead_of_now(make_snapshot, mocker: MockerFixture):
     snapshot_a = make_snapshot(
@@ -402,16 +378,14 @@
     )
 
     expected_start = to_datetime("2022-01-01")
     end_date = to_datetime("2022-01-03")
     expected_end = to_date(end_date) - timedelta(days=1)
     now = to_datetime("2022-01-30")
 
-    dag = DAG[str]({"a": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"a": snapshot_a}
     context_diff_mock.added = set()
     context_diff_mock.removed = set()
     context_diff_mock.modified_snapshots = {}
     context_diff_mock.new_snapshots = {snapshot_a.snapshot_id: snapshot_a}
 
@@ -419,33 +393,31 @@
 
     now_ds_mock = mocker.patch("sqlmesh.core.scheduler.now")
     now_ds_mock.return_value = now
     state_reader_mock.missing_intervals.return_value = {
         snapshot_a: [(to_timestamp(expected_start), to_timestamp(end_date))]
     }
 
-    plan = Plan(context_diff_mock, dag, state_reader_mock, is_dev=True)
+    plan = Plan(context_diff_mock, state_reader_mock, is_dev=True)
 
     assert plan.start == to_timestamp(expected_start)
     assert plan.end == expected_end
 
 
 def test_broken_references(make_snapshot, mocker: MockerFixture):
     snapshot_b = make_snapshot(SqlModel(name="b", query=parse_one("select 2, ds FROM a")))
     snapshot_b.set_version()
 
-    dag = DAG[str]({"b": set()})
-
     context_diff_mock = mocker.Mock()
     context_diff_mock.snapshots = {"b": snapshot_b}
     context_diff_mock.added = set()
     context_diff_mock.removed = {"a"}
     context_diff_mock.modified_snapshots = {}
     context_diff_mock.new_snapshots = {}
 
     state_reader_mock = mocker.Mock()
 
     with pytest.raises(
         PlanError,
         match=r"Removed models {'a'} are referenced in model 'b'.*",
     ):
-        Plan(context_diff_mock, dag, state_reader_mock)
+        Plan(context_diff_mock, state_reader_mock)
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_plan_evaluator.py` & `sqlmesh-0.5.0/tests/core/test_plan_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 def sushi_plan(sushi_context: Context, mocker: MockerFixture) -> Plan:
     mock_prompt = mocker.Mock()
     mock_prompt.ask.return_value = "2022-01-01"
     mocker.patch("sqlmesh.core.console.Prompt", mock_prompt)
 
     return Plan(
         sushi_context._context_diff("dev"),
-        dag=sushi_context.dag,
         state_reader=sushi_context.state_reader,
         is_dev=True,
     )
 
 
 def test_builtin_evaluator_push(sushi_context: Context, make_snapshot):
     new_model = SqlModel(
@@ -47,15 +46,14 @@
     new_view_model_snapshot = snapshots[new_view_model.name]
 
     new_model_snapshot.version = new_model_snapshot.fingerprint.to_version()
     new_view_model_snapshot.version = new_view_model_snapshot.fingerprint.to_version()
 
     plan = Plan(
         sushi_context._context_diff("prod"),
-        dag=sushi_context.dag,
         state_reader=sushi_context.state_reader,
     )
 
     evaluator = BuiltInPlanEvaluator(
         sushi_context.state_sync,
         sushi_context.snapshot_evaluator,
         console=sushi_context.console,
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_scheduler.py` & `sqlmesh-0.5.0/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_schema_diff.py` & `sqlmesh-0.5.0/tests/core/test_schema_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def test_schema_diff_calculate():
     alter_expressions = SchemaDiffer(
         **{
             "support_positional_add": False,
             "support_nested_operations": False,
-            "array_suffix": "",
+            "array_element_selector": "",
             "compatible_types": {
                 exp.DataType.build("STRING"): {exp.DataType.build("INT")},
             },
         }
     ).compare_columns(
         "apply_to_table",
         {
@@ -46,15 +46,15 @@
 
 
 def test_schema_diff_calculate_type_transitions():
     alter_expressions = SchemaDiffer(
         **{
             "support_positional_add": False,
             "support_nested_operations": False,
-            "array_suffix": "",
+            "array_element_selector": "",
             "compatible_types": {
                 exp.DataType.build("STRING"): {exp.DataType.build("INT")},
             },
         }
     ).compare_columns(
         "apply_to_table",
         {
@@ -732,7 +732,68 @@
     engine_adapter.alter_table("apply_to_table", "schema_from_table")
     assert engine_adapter.columns("apply_to_table") == {
         "id": exp.DataType.build("int"),
         "ds": exp.DataType.build("varchar"),
         "new_column": exp.DataType.build("double"),
         "name": exp.DataType.build("int"),
     }
+
+
+def test_schema_diff_alter_op_column():
+    nested = TableAlterOperation.add(
+        [
+            TableAlterColumn.array_of_struct("nested"),
+            TableAlterColumn.primitive("col_a"),
+        ],
+        "INT",
+        expected_table_struct="STRUCT<id INT, nested ARRAY<STRUCT<col_a INT>>>",
+        position=TableAlterColumnPosition.last("id"),
+    )
+    assert nested.column("").sql() == "nested.col_a"
+    nested_complete_column = TableAlterOperation.add(
+        [
+            TableAlterColumn.array_of_struct("nested_1", quoted=True),
+            TableAlterColumn.struct("nested_2"),
+            TableAlterColumn.array_of_struct("nested_3"),
+            TableAlterColumn.primitive("col_a", quoted=True),
+        ],
+        "INT",
+        expected_table_struct="""STRUCT<id INT, "nested_1" ARRAY<STRUCT<nested_2 STRUCT<nested_3 ARRAY<STRUCT<"col_a" INT>>>>>>""",
+        position=TableAlterColumnPosition.last("id"),
+    )
+    assert nested_complete_column.column("").sql() == '"nested_1".nested_2.nested_3."col_a"'
+    nested_one_more_complete_column = TableAlterOperation.add(
+        [
+            TableAlterColumn.array_of_struct("nested_1", quoted=True),
+            TableAlterColumn.struct("nested_2"),
+            TableAlterColumn.array_of_struct("nested_3"),
+            TableAlterColumn.struct("nested_4"),
+            TableAlterColumn.primitive("col_a", quoted=True),
+        ],
+        "INT",
+        expected_table_struct="""STRUCT<id INT, "nested_1" ARRAY<STRUCT<nested_2 STRUCT<nested_3 ARRAY<STRUCT<nested_4 STRUCT<"col_a" INT>>>>>>>""",
+        position=TableAlterColumnPosition.last("id"),
+    )
+    assert (
+        nested_one_more_complete_column.column("").sql()
+        == '"nested_1".nested_2.nested_3.nested_4."col_a"'
+    )
+    super_nested = TableAlterOperation.add(
+        [
+            TableAlterColumn.array_of_struct("nested_1", quoted=True),
+            TableAlterColumn.struct("nested_2"),
+            TableAlterColumn.array_of_struct("nested_3"),
+            TableAlterColumn.struct("nested_4"),
+            TableAlterColumn.struct("nested_5"),
+            TableAlterColumn.struct("nested_6", quoted=True),
+            TableAlterColumn.struct("nested_7"),
+            TableAlterColumn.array_of_struct("nested_8"),
+            TableAlterColumn.primitive("col_a", quoted=True),
+        ],
+        "INT",
+        expected_table_struct="""STRUCT<id INT, "nested_1" ARRAY<STRUCT<nested_2 STRUCT<nested_3 ARRAY<STRUCT<nested_4 STRUCT<nested_5 STRUCT<"nested_6" STRUCT<nested_7 STRUCT<nested_8 ARRAY<STRUCT<"col_a" INT>>>>>>>>>>>>""",
+        position=TableAlterColumnPosition.last("id"),
+    )
+    assert (
+        super_nested.column("element").sql()
+        == '"nested_1".element.nested_2.nested_3.element.nested_4.nested_5."nested_6".nested_7.nested_8.element."col_a"'
+    )
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_seed.py` & `sqlmesh-0.5.0/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_snapshot.py` & `sqlmesh-0.5.0/tests/core/test_snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
             },
             "source_type": "sql",
         },
         "audits": [],
         "name": "name",
         "parents": [{"name": "parent.tbl", "identifier": snapshot.parents[0].identifier}],
         "previous_versions": [],
+        "project": "",
         "indirect_versions": {},
         "updated_ts": 1663891973000,
         "version": snapshot.fingerprint.dict(),
     }
 
 
 def test_add_interval(snapshot: Snapshot, make_snapshot):
@@ -279,15 +280,15 @@
 each_macro = lambda: "test"
 
 
 def test_fingerprint(model: Model, parent_model: Model):
     fingerprint = fingerprint_from_model(model, models={})
 
     original_fingerprint = SnapshotFingerprint(
-        data_hash="3042895307",
+        data_hash="596551453",
         metadata_hash="2417444816",
     )
 
     assert fingerprint == original_fingerprint
     assert fingerprint_from_model(model, physical_schema="x", models={}) != fingerprint
 
     with_parent_fingerprint = fingerprint_from_model(model, models={"parent.tbl": parent_model})
@@ -358,15 +359,15 @@
                 }
             ),
         }
     )
     fingerprint = fingerprint_from_model(model, models={})
 
     original_fingerprint = SnapshotFingerprint(
-        data_hash="2665680291",
+        data_hash="2038703918",
         metadata_hash="2417444816",
     )
 
     fingerprint = fingerprint_from_model(model, models={})
     assert fingerprint == original_fingerprint
 
     model.jinja_macros.root_macros["test_macro"] = MacroInfo(
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.5.0/tests/core/test_snapshot_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         [
             call("physical_schema"),
         ]
     )
 
     adapter_mock.create_table.assert_called_once_with(
         snapshot.table_name(),
-        query_or_columns_to_types={"a": exp.DataType.build("int")},
+        columns_to_types={"a": exp.DataType.build("int")},
         storage_format="parquet",
         partitioned_by=["a"],
         partition_interval_unit=IntervalUnit.DAY,
     )
 
 
 def test_evaluate_paused_forward_only_upstream(mocker: MockerFixture, make_snapshot):
@@ -236,18 +236,16 @@
     )
     snapshot = make_snapshot(model, physical_schema="physical_schema", version="1")
 
     evaluator.migrate([snapshot])
 
     cursor_mock.execute.assert_has_calls(
         [
-            call("""ALTER TABLE "physical_schema"."test_schema__test_model__1" DROP COLUMN "b\""""),
-            call(
-                """ALTER TABLE "physical_schema"."test_schema__test_model__1" ADD COLUMN "a" INT"""
-            ),
+            call("""ALTER TABLE physical_schema.test_schema__test_model__1 DROP COLUMN b"""),
+            call("""ALTER TABLE physical_schema.test_schema__test_model__1 ADD COLUMN a INT"""),
         ]
     )
 
 
 def test_evaluate_creation_duckdb(
     snapshot: Snapshot,
     duck_conn,
```

### Comparing `sqlmesh-0.4.2.dev9/tests/core/test_state_sync.py` & `sqlmesh-0.5.0/tests/core/test_state_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,15 @@
 from sqlmesh.core.state_sync.base import SCHEMA_VERSION, SQLGLOT_VERSION, Versions
 from sqlmesh.utils.date import now_timestamp, to_datetime, to_ds, to_timestamp
 from sqlmesh.utils.errors import SQLMeshError
 
 
 @pytest.fixture
 def state_sync(duck_conn):
-    state_sync = EngineAdapterStateSync(
-        create_engine_adapter(lambda: duck_conn, "duckdb"),
-        "sqlmesh",
-    )
+    state_sync = EngineAdapterStateSync(create_engine_adapter(lambda: duck_conn, "duckdb"))
     state_sync.migrate()
     return state_sync
 
 
 @pytest.fixture
 def snapshots(make_snapshot: t.Callable) -> t.List[Snapshot]:
     return [
@@ -562,15 +559,15 @@
     )
 
     # old install does not have this table / row
     delete_versions(state_sync)
 
     with pytest.raises(
         SQLMeshError,
-        match=r"SQLMesh \(local\) is using version '1' which is ahead of '0'",
+        match=r"SQLMesh \(local\) is using version '2' which is ahead of '0'",
     ):
         state_sync.get_versions()
 
     state_sync.migrate()
 
     # migration version is behind, always raise
     state_sync._update_versions(schema_version=SCHEMA_VERSION + 1)
```

### Comparing `sqlmesh-0.4.2.dev9/tests/dbt/conftest.py` & `sqlmesh-0.5.0/tests/dbt/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 import pytest
 from pytest_mock.plugin import MockerFixture
 
-from sqlmesh.dbt.common import DbtContext
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.project import Project
 
 
 @pytest.fixture()
 def sushi_test_project(mocker: MockerFixture) -> Project:
     project = Project.load(DbtContext(project_root=Path("tests/fixtures/dbt/sushi_test")))
     for package_name, package in project.packages.items():
```

### Comparing `sqlmesh-0.4.2.dev9/tests/dbt/test_adapter.py` & `sqlmesh-0.5.0/tests/dbt/test_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     context = sushi_test_project.context
     assert context.engine_adapter
 
     engine_adapter = context.engine_adapter
     engine_adapter.create_schema("foo")
     engine_adapter.create_schema("ignored")
     engine_adapter.create_table(
-        table_name="foo.bar", query_or_columns_to_types={"baz": exp.DataType.build("int")}
+        table_name="foo.bar", columns_to_types={"baz": exp.DataType.build("int")}
     )
     engine_adapter.create_table(
-        table_name="foo.another", query_or_columns_to_types={"col": exp.DataType.build("int")}
+        table_name="foo.another", columns_to_types={"col": exp.DataType.build("int")}
     )
     engine_adapter.create_table(
-        table_name="ignored.ignore", query_or_columns_to_types={"col": exp.DataType.build("int")}
+        table_name="ignored.ignore", columns_to_types={"col": exp.DataType.build("int")}
     )
 
     assert (
         context.render("{{ adapter.get_relation(database=None, schema='foo', identifier='bar') }}")
         == '"foo"."bar"'
     )
     assert context.render(
```

### Comparing `sqlmesh-0.4.2.dev9/tests/dbt/test_config.py` & `sqlmesh-0.5.0/tests/dbt/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing as t
 from pathlib import Path
 
 import pytest
+from dbt.adapters.base import BaseRelation
 
 from sqlmesh.core.model import SqlModel
-from sqlmesh.dbt.common import DbtContext
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.model import Materialization, ModelConfig
 from sqlmesh.dbt.project import Project
 from sqlmesh.dbt.source import SourceConfig
 from sqlmesh.dbt.target import (
     BigQueryConfig,
     DatabricksConfig,
     DuckDbConfig,
@@ -254,14 +255,28 @@
     }
     actual_config = {k: getattr(raw_items_seed, k) for k, v in expected_config.items()}
     assert actual_config == expected_config
 
     assert raw_items_seed.model_name == "sushi.waiter_names"
 
 
+def test_quoting():
+    model = ModelConfig(alias="bar", schema="foo")
+    assert str(BaseRelation.create(**model.relation_info)) == '"foo"."bar"'
+
+    model.quoting.identifier = False
+    assert str(BaseRelation.create(**model.relation_info)) == '"foo".bar'
+
+    source = SourceConfig(identifier="bar", schema="foo")
+    assert str(BaseRelation.create(**source.relation_info)) == '"foo"."bar"'
+
+    source.quoting.schema_ = False
+    assert str(BaseRelation.create(**source.relation_info)) == 'foo."bar"'
+
+
 def _test_warehouse_config(config_yaml: str, config_model: t.Type[TargetConfig], *params_path: str):
     config_dict = yaml_load(config_yaml)
     for path in params_path:
         config_dict = config_dict[path]
 
     config = config_model(**config_dict)
```

### Comparing `sqlmesh-0.4.2.dev9/tests/dbt/test_transformation.py` & `sqlmesh-0.5.0/tests/dbt/test_transformation.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 )
 from sqlmesh.dbt.builtin import create_builtin_globals
 from sqlmesh.dbt.column import (
     ColumnConfig,
     column_descriptions_to_sqlmesh,
     column_types_to_sqlmesh,
 )
-from sqlmesh.dbt.common import DbtContext
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.model import Materialization, ModelConfig
 from sqlmesh.dbt.project import Project
 from sqlmesh.dbt.seed import SeedConfig
 from sqlmesh.dbt.source import SourceConfig
 from sqlmesh.dbt.target import DuckDbConfig
 from sqlmesh.utils.errors import ConfigError, MacroEvalError
 
@@ -206,32 +206,33 @@
     assert rendered.target_schema != model.target_schema
     assert rendered.target_schema == "foo"
     assert rendered.columns["zipcode"] != model.columns["zipcode"]
     assert rendered.columns["zipcode"].data_type == "varchar(5)"
 
     sqlmesh_model = rendered.to_sqlmesh(context)
     assert str(sqlmesh_model.query) == model.sql
-    assert str(sqlmesh_model.render_query()) == "SELECT * FROM raw.baz AS baz"
+    assert str(sqlmesh_model.render_query()) == 'SELECT * FROM "raw"."baz" AS baz'
     assert sqlmesh_model.columns_to_types == column_types_to_sqlmesh(rendered.columns)
 
 
 def test_config_containing_missing_dependency():
     context = DbtContext()
     model = ModelConfig(sql="{{ config(pre_hook=\"{{ print(ref('bar')) }}\") }} SELECT 1 FROM a")
     with pytest.raises(ConfigError, match="'bar' was not found"):
-        model.render_config(context)
+        model.render_config(context).to_sqlmesh(context)
 
     model = ModelConfig(sql='{{ config(pre_hook="{{ get_table_name() }}") }} SELECT 1 FROM a')
     with pytest.raises(ConfigError, match="get_table_name"):
-        model.render_config(context)
+        model.render_config(context).to_sqlmesh(context)
 
     model = ModelConfig(sql="{{ config(alias='{{ get_table_name() }}') }} SELECT 1 FROM a")
     rendered = model.render_config(context)
     assert rendered.alias == "{{ get_table_name() }}"
     assert "get_table_name" not in [macro.name for macro in rendered._dependencies.macros]
+    rendered.to_sqlmesh(context)
 
 
 def test_config_containing_method():
     context = DbtContext()
     context.jinja_macros.global_objs.update({"get_table_name": lambda: "foo"})
     model = ModelConfig(sql="{{ config(alias=get_table_name()) }} SELECT 1 FROM a")
 
@@ -269,14 +270,24 @@
 
 def test_schema_jinja(sushi_test_project: Project):
     model_config = ModelConfig(target_schema="sushi", sql="SELECT 1 AS one FROM {{ schema }}")
     context = sushi_test_project.context
     model_config.to_sqlmesh(context).render_query().sql() == "SELECT 1 AS one FROM sushi AS sushi"
 
 
+def test_materialized_jinja(sushi_test_project: Project):
+    model_config = ModelConfig(
+        materialized="{{ 'table' if target.type in ['duckdb'] else 'view' }}",
+        sql="SELECT 1 AS one FROM {{ schema }}",
+    )
+    context = sushi_test_project.context
+    rendered = model_config.render_config(context)
+    assert rendered.materialized == "table"
+
+
 def test_this(assert_exp_eq, sushi_test_project: Project):
     model_config = ModelConfig(alias="test", sql="SELECT 1 AS one FROM {{ this.identifier }}")
     context = sushi_test_project.context
     assert_exp_eq(
         model_config.to_sqlmesh(context).render_query().sql(), "SELECT 1 AS one FROM test AS test"
     )
```

### Comparing `sqlmesh-0.4.2.dev9/tests/engines/spark/test_db_api.py` & `sqlmesh-0.5.0/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pathlib import Path
 
 from sqlmesh.core.config import DuckDBConnectionConfig
 from sqlmesh.core.engine_adapter import EngineAdapter
-from sqlmesh.dbt.common import DbtContext
+from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.profile import Profile
 from sqlmesh.utils.errors import ConfigError
 
 DATA_DIR = os.path.join(os.path.dirname(__file__), "source_data")
 
 
 def _add_csv_file(conn: EngineAdapter, table_name: str, path: str) -> None:
```

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.5.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/migrations/environments.json` & `sqlmesh-0.5.0/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.5.0/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/integrations/github/fixtures/pull_request_review.json` & `sqlmesh-0.5.0/tests/integrations/github/fixtures/pull_request_review.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.5.0/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.5.0/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.5.0/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.5.0/tests/schedulers/airflow/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
                     },
                     "source_type": "sql",
                 },
                 "audits": [],
                 "name": "test_model",
                 "parents": [],
                 "previous_versions": [],
+                "project": "",
                 "physical_schema": "physical_schema",
                 "updated_ts": 1665014400000,
                 "version": snapshot.version,
             }
         ],
         "environment": {
             "name": "test_env",
```

### Comparing `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.5.0/tests/schedulers/airflow/test_end_to_end.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 @pytest.mark.integration
 @pytest.mark.airflow_integration
 def test_sushi(mocker: MockerFixture, is_docker: bool):
     start = yesterday_ds()
 
     airflow_config = "airflow_config_docker" if is_docker else "airflow_config"
-    context = Context(path="./examples/sushi", config=airflow_config)
+    context = Context(paths="./examples/sushi", config=airflow_config)
 
     context.plan(
         environment="test_dev",
         start=start,
         skip_tests=True,
         no_prompts=True,
         auto_apply=True,
```

### Comparing `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.5.0/tests/schedulers/airflow/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.5.0/tests/schedulers/airflow/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_concurrency.py` & `sqlmesh-0.5.0/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_connection_pool.py` & `sqlmesh-0.5.0/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_dag.py` & `sqlmesh-0.5.0/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_date.py` & `sqlmesh-0.5.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_filesystem.py` & `sqlmesh-0.5.0/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_jinja.py` & `sqlmesh-0.5.0/tests/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_metaprogramming.py` & `sqlmesh-0.5.0/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_pandas.py` & `sqlmesh-0.5.0/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_pydantic.py` & `sqlmesh-0.5.0/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_transactional_file.py` & `sqlmesh-0.5.0/tests/utils/test_transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/utils/test_yaml.py` & `sqlmesh-0.5.0/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/tests/web/test_main.py` & `sqlmesh-0.5.0/tests/web/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     app.dependency_overrides[get_settings] = get_settings_override
     return tmp_path
 
 
 @pytest.fixture
 def project_context(project_tmp_path: Path) -> Context:
-    context = Context(path=str(project_tmp_path), console=api_console)
+    context = Context(paths=str(project_tmp_path), console=api_console)
 
     def get_loaded_context_override() -> Context:
         return context
 
     app.dependency_overrides[get_loaded_context] = get_loaded_context_override
     return context
```

### Comparing `sqlmesh-0.4.2.dev9/web/client/.eslintrc.js` & `sqlmesh-0.5.0/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/index.html` & `sqlmesh-0.5.0/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/openapi.json` & `sqlmesh-0.5.0/web/client/openapi.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/package-lock.json` & `sqlmesh-0.5.0/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/package.json` & `sqlmesh-0.5.0/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/playwright.config.ts` & `sqlmesh-0.5.0/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/public/favicons/favicon.ico` & `sqlmesh-0.5.0/web/client/dist/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/api/channels.ts` & `sqlmesh-0.5.0/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/api/index.ts` & `sqlmesh-0.5.0/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/api/instance.ts` & `sqlmesh-0.5.0/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.5.0/web/client/dist/assets/CircularStd-Black-52659624.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.5.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.5.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.5.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.5.0/web/client/dist/assets/Publico-Bold-c79acd56.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.5.0/web/client/dist/assets/Publico-Medium-01b4a891.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.5.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/context/context.ts` & `sqlmesh-0.5.0/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/context/editor.ts` & `sqlmesh-0.5.0/web/client/src/context/editor.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/context/fileTree.ts` & `sqlmesh-0.5.0/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/context/plan.ts` & `sqlmesh-0.5.0/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/context/theme.tsx` & `sqlmesh-0.5.0/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.5.0/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/index.css` & `sqlmesh-0.5.0/web/client/src/index.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/button/Button.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.5.0/web/client/src/library/components/editor/Editor.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/Editor.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/editor/Editor.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.5.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/extensions/index.ts` & `sqlmesh-0.5.0/web/client/src/library/components/editor/extensions/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.5.0/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.5.0/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/Graph.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/graph/Graph.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.5.0/web/client/src/library/components/graph/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/ide/ActivePlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/ide/IDE.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/ide/RunPlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/input/Input.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/plan/Plan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.5.0/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.5.0/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.5.0/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.5.0/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/tasksOverview/TasksOverview.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.5.0/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/main.tsx` & `sqlmesh-0.5.0/web/client/src/main.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/models/artifact.ts` & `sqlmesh-0.5.0/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/models/directory.ts` & `sqlmesh-0.5.0/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/models/environment.ts` & `sqlmesh-0.5.0/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/models/file.ts` & `sqlmesh-0.5.0/web/client/src/models/file.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/models/initial.ts` & `sqlmesh-0.5.0/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/tests/utils.tsx` & `sqlmesh-0.5.0/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/utils/index.spec.ts` & `sqlmesh-0.5.0/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/utils/index.ts` & `sqlmesh-0.5.0/web/client/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.5.0/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.5.0/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/tailwind.config.js` & `sqlmesh-0.5.0/web/client/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/tsconfig.json` & `sqlmesh-0.5.0/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/client/vite.config.ts` & `sqlmesh-0.5.0/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/__init__.py` & `sqlmesh-0.5.0/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/commands.py` & `sqlmesh-0.5.0/web/server/api/endpoints/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,9 +141,9 @@
     rendered = context.render(
         snapshot,
         start=options.start,
         end=options.end,
         latest=options.latest,
         expand=options.expand,
     )
-    dialect = options.dialect or context.dialect
+    dialect = options.dialect or context.config.dialect
     return models.Query(sql=rendered.sql(pretty=options.pretty, dialect=dialect))
```

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/context.py` & `sqlmesh-0.5.0/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/directories.py` & `sqlmesh-0.5.0/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/environments.py` & `sqlmesh-0.5.0/web/server/api/endpoints/environments.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from sqlmesh.core.environment import Environment
 from web.server.settings import get_loaded_context
 
 router = APIRouter()
 
 
 @router.get("")
-def get_environments(context: Context = Depends(get_loaded_context)) -> t.Dict[str, Environment]:
+async def get_environments(
+    context: Context = Depends(get_loaded_context),
+) -> t.Dict[str, Environment]:
     """Get the environments"""
     environments = {env.name: env for env in context.state_reader.get_environments()}
     if c.PROD not in environments:
         environments[c.PROD] = Environment(
             name=c.PROD,
             snapshots=[],
             start_at=0,
```

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/events.py` & `sqlmesh-0.5.0/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/files.py` & `sqlmesh-0.5.0/web/server/api/endpoints/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,24 +19,18 @@
 @router.get("", response_model=models.Directory)
 def get_files(
     context: t.Optional[Context] = Depends(get_context),
     settings: Settings = Depends(get_settings),
     path_mapping: t.Dict[Path, models.FileType] = Depends(get_path_mapping),
 ) -> models.Directory:
     """Get all project files."""
-    if context:
-        ignore_patterns = context.ignore_patterns
-        hook_directory_path = context.hook_directory_path.relative_to(context.path)
-        macro_directory_path = context.macro_directory_path.relative_to(context.path)
-        test_directory_path = context.test_directory_path.relative_to(context.path)
-    else:
-        ignore_patterns = c.IGNORE_PATTERNS
-        hook_directory_path = Path("hooks")
-        macro_directory_path = Path("macros")
-        test_directory_path = Path("tests")
+    ignore_patterns = context.config.ignore_patterns if context else c.IGNORE_PATTERNS
+    hook_directory_path = Path(c.HOOKS)
+    macro_directory_path = Path(c.MACROS)
+    test_directory_path = Path(c.TESTS)
 
     def walk_path(
         path: str | Path,
     ) -> tuple[list[models.Directory], list[models.File]]:
         directories = []
         files = []
```

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/lineage.py` & `sqlmesh-0.5.0/web/server/api/endpoints/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/models.py` & `sqlmesh-0.5.0/web/server/api/endpoints/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/api/endpoints/plan.py` & `sqlmesh-0.5.0/web/server/api/endpoints/plan.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from __future__ import annotations
 
-import asyncio
-import functools
 import typing as t
 
 from fastapi import APIRouter, Body, Depends, HTTPException, Request, Response, status
 from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY
 
 from sqlmesh.core.context import Context
 from sqlmesh.utils.date import make_inclusive, to_ds
 from sqlmesh.utils.errors import PlanError
 from web.server import models
 from web.server.settings import get_loaded_context
-from web.server.utils import run_in_executor
 
 router = APIRouter()
 
 
 @router.post(
     "",
     response_model=models.ContextEnvironment,
@@ -35,31 +32,28 @@
         raise HTTPException(
             status_code=HTTP_422_UNPROCESSABLE_ENTITY,
             detail="Plan/apply is already running.",
         )
 
     context.refresh()
 
-    plan_func = functools.partial(
-        context.plan,
-        environment=environment,
-        no_prompts=True,
-        start=plan_dates.start if plan_dates else None,
-        end=plan_dates.end if plan_dates else None,
-        create_from=plan_options.create_from,
-        skip_tests=plan_options.skip_tests,
-        restate_models=plan_options.restate_models,
-        no_gaps=plan_options.no_gaps,
-        skip_backfill=plan_options.skip_backfill,
-        forward_only=plan_options.forward_only,
-        no_auto_categorization=plan_options.no_auto_categorization,
-    )
-    request.app.state.task = asyncio.create_task(run_in_executor(plan_func))
     try:
-        plan = await request.app.state.task
+        plan = context.plan(
+            environment=environment,
+            no_prompts=True,
+            start=plan_dates.start if plan_dates else None,
+            end=plan_dates.end if plan_dates else None,
+            create_from=plan_options.create_from,
+            skip_tests=plan_options.skip_tests,
+            restate_models=plan_options.restate_models,
+            no_gaps=plan_options.no_gaps,
+            skip_backfill=plan_options.skip_backfill,
+            forward_only=plan_options.forward_only,
+            no_auto_categorization=plan_options.no_auto_categorization,
+        )
     except PlanError as e:
         raise HTTPException(
             status_code=HTTP_422_UNPROCESSABLE_ENTITY,
             detail=str(e),
         )
 
     payload = models.ContextEnvironment(
```

### Comparing `sqlmesh-0.4.2.dev9/web/server/console.py` & `sqlmesh-0.5.0/web/server/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/main.py` & `sqlmesh-0.5.0/web/server/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/models.py` & `sqlmesh-0.5.0/web/server/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/settings.py` & `sqlmesh-0.5.0/web/server/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 
 @lru_cache()
 def get_settings() -> Settings:
     return Settings()
 
 
 @lru_cache()
-def _get_context(path: str, config: str) -> Context:
+def _get_context(path: str | Path, config: str) -> Context:
     from web.server.main import api_console
 
-    return Context(path=path, config=config, console=api_console, load=False)
+    return Context(paths=str(path), config=config, console=api_console, load=False)
 
 
 @lru_cache()
-def _get_loaded_context(path: str, config: str) -> Context:
+def _get_loaded_context(path: str | Path, config: str) -> Context:
     context = _get_context(path, config)
     context.load()
     return context
 
 
 @lru_cache()
 def _get_path_mappings(context: Context) -> dict[Path, FileType]:
```

### Comparing `sqlmesh-0.4.2.dev9/web/server/sse.py` & `sqlmesh-0.5.0/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.4.2.dev9/web/server/utils.py` & `sqlmesh-0.5.0/web/server/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     resolved_path = context.path.resolve()
     full_path = (resolved_path / path).resolve()
     try:
         full_path.relative_to(resolved_path)
     except ValueError:
         raise HTTPException(status_code=HTTP_404_NOT_FOUND)
 
-    if any(full_path.match(pattern) for pattern in context.ignore_patterns):
+    if any(
+        full_path.match(pattern) for pattern in context.config_for_path(Path(path)).ignore_patterns
+    ):
         raise HTTPException(status_code=HTTP_404_NOT_FOUND)
 
     return path
 
 
 def replace_file(src: Path, dst: Path) -> None:
     """Move a file or directory at src to dst."""
```

