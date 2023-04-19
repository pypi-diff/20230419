# Comparing `tmp/python_auditor-0.0.7.tar.gz` & `tmp/python_auditor-0.1.0.tar.gz`

## Comparing `python_auditor-0.0.7.tar` & `python_auditor-0.1.0.tar`

### file list

```diff
@@ -1,68 +1,73 @@
--rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 python_auditor-0.0.7/local_dependencies/auditor/Cargo.toml
--rw-r--r--   0     1001      123       67 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/.env
--rw-r--r--   0     1001      123      535 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/build.rs
--rw-r--r--   0     1001      123      296 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/configuration/base.yaml
--rw-r--r--   0     1001      123       62 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/configuration/local.yaml
--rw-r--r--   0     1001      123      367 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/configuration/priority-plugin/base.yml
--rw-r--r--   0     1001      123       59 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/configuration/production.yaml
--rw-r--r--   0     1001      123       68 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/configuration/slurm-epilog-collector/base.yml
--rw-r--r--   0     1001      123    19241 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/sqlx-data.json
--rw-r--r--   0     1001      123    13949 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/client/mod.rs
--rw-r--r--   0     1001      123     5134 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/configuration.rs
--rw-r--r--   0     1001      123      543 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/constants.rs
--rw-r--r--   0     1001      123     5335 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/domain/component.rs
--rw-r--r--   0     1001      123     5398 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/domain/meta.rs
--rw-r--r--   0     1001      123     1343 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/domain/mod.rs
--rw-r--r--   0     1001      123    13105 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/domain/record.rs
--rw-r--r--   0     1001      123     5986 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/domain/score.rs
--rw-r--r--   0     1001      123     3252 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/domain/validamount.rs
--rw-r--r--   0     1001      123     4327 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/domain/validname.rs
--rw-r--r--   0     1001      123     3175 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/domain/validvalue.rs
--rw-r--r--   0     1001      123      655 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/error.rs
--rw-r--r--   0     1001      123      728 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/lib.rs
--rw-r--r--   0     1001      123     1591 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/macros.rs
--rw-r--r--   0     1001      123     1771 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/main.rs
--rw-r--r--   0     1001      123     8434 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/metrics/database.rs
--rw-r--r--   0     1001      123     1695 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/metrics/mod.rs
--rw-r--r--   0     1001      123     6163 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/routes/add.rs
--rw-r--r--   0     1001      123     3323 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/routes/get.rs
--rw-r--r--   0     1001      123     6732 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/routes/get_since.rs
--rw-r--r--   0     1001      123      449 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/routes/health_check.rs
--rw-r--r--   0     1001      123      501 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/routes/mod.rs
--rw-r--r--   0     1001      123     2960 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/routes/update.rs
--rw-r--r--   0     1001      123     1718 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/startup.rs
--rw-r--r--   0     1001      123     1393 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/src/telemetry.rs
--rw-r--r--   0     1001      123     5192 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/tests/api/add.rs
--rw-r--r--   0     1001      123    21112 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/tests/api/client.rs
--rw-r--r--   0     1001      123     2667 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/tests/api/get.rs
--rw-r--r--   0     1001      123     7793 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/tests/api/get_since.rs
--rw-r--r--   0     1001      123      258 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/tests/api/health_check.rs
--rw-r--r--   0     1001      123     4019 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/tests/api/helpers.rs
--rw-r--r--   0     1001      123       88 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/tests/api/main.rs
--rw-r--r--   0     1001      123     3672 2023-02-13 10:02:41.000000 python_auditor-0.0.7/local_dependencies/auditor/tests/api/update.rs
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 python_auditor-0.0.7/Cargo.toml
--rw-r--r--   0     1001      123       28 2023-02-13 10:02:41.000000 python_auditor-0.0.7/.cargo/config.toml
--rw-r--r--   0     1001      123      241 2023-02-13 10:02:41.000000 python_auditor-0.0.7/.readthedocs.yaml
--rw-r--r--   0     1001      123     1865 2023-02-13 10:02:41.000000 python_auditor-0.0.7/README.md
--rw-r--r--   0     1001      123      634 2023-02-13 10:02:41.000000 python_auditor-0.0.7/docs/Makefile
--rw-r--r--   0     1001      123      128 2023-02-13 10:02:41.000000 python_auditor-0.0.7/docs/api.rst
--rw-r--r--   0     1001      123       84 2023-02-13 10:02:41.000000 python_auditor-0.0.7/docs/changelog.rst
--rw-r--r--   0     1001      123     1212 2023-02-13 10:02:41.000000 python_auditor-0.0.7/docs/conf.py
--rw-r--r--   0     1001      123     6303 2023-02-13 10:02:41.000000 python_auditor-0.0.7/docs/examples.rst
--rw-r--r--   0     1001      123      916 2023-02-13 10:02:41.000000 python_auditor-0.0.7/docs/index.rst
--rw-r--r--   0     1001      123      800 2023-02-13 10:02:41.000000 python_auditor-0.0.7/docs/make.bat
--rw-r--r--   0     1001      123      669 2023-02-13 10:02:41.000000 python_auditor-0.0.7/pyproject.toml
--rwxr-xr-x   0     1001      123     1894 2023-02-13 10:02:41.000000 python_auditor-0.0.7/scripts/test_add_update.py
--rwxr-xr-x   0     1001      123     2211 2023-02-13 10:02:41.000000 python_auditor-0.0.7/scripts/test_components.py
--rwxr-xr-x   0     1001      123     1297 2023-02-13 10:02:41.000000 python_auditor-0.0.7/scripts/test_eq.py
--rwxr-xr-x   0     1001      123     2118 2023-02-13 10:02:41.000000 python_auditor-0.0.7/scripts/test_get_since.py
--rwxr-xr-x   0     1001      123     1874 2023-02-13 10:02:41.000000 python_auditor-0.0.7/scripts/test_meta.py
--rw-r--r--   0     1001      123     3075 2023-02-13 10:02:41.000000 python_auditor-0.0.7/src/builder.rs
--rw-r--r--   0     1001      123     5862 2023-02-13 10:02:41.000000 python_auditor-0.0.7/src/client.rs
--rw-r--r--   0     1001      123     2607 2023-02-13 10:02:41.000000 python_auditor-0.0.7/src/domain/component.rs
--rw-r--r--   0     1001      123     1767 2023-02-13 10:02:41.000000 python_auditor-0.0.7/src/domain/meta.rs
--rw-r--r--   0     1001      123      464 2023-02-13 10:02:41.000000 python_auditor-0.0.7/src/domain/mod.rs
--rw-r--r--   0     1001      123     6069 2023-02-13 10:02:41.000000 python_auditor-0.0.7/src/domain/record.rs
--rw-r--r--   0     1001      123     2125 2023-02-13 10:02:41.000000 python_auditor-0.0.7/src/domain/score.rs
--rw-r--r--   0     1001      123      891 2023-02-13 10:02:41.000000 python_auditor-0.0.7/src/lib.rs
--rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 python_auditor-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2317 1970-01-01 00:00:00.000000 python_auditor-0.1.0/local_dependencies/auditor/Cargo.toml
+-rw-r--r--   0     1001      123       67 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/.env
+-rw-r--r--   0     1001      123      535 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/build.rs
+-rw-r--r--   0     1001      123      296 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/configuration/base.yaml
+-rw-r--r--   0     1001      123       62 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/configuration/local.yaml
+-rw-r--r--   0     1001      123      367 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/configuration/priority-plugin/base.yml
+-rw-r--r--   0     1001      123       59 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/configuration/production.yaml
+-rw-r--r--   0     1001      123       68 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/configuration/slurm-epilog-collector/base.yml
+-rw-r--r--   0     1001      123    19241 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/sqlx-data.json
+-rw-r--r--   0     1001      123    32603 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/client/mod.rs
+-rw-r--r--   0     1001      123     5134 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/configuration.rs
+-rw-r--r--   0     1001      123      600 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/constants.rs
+-rw-r--r--   0     1001      123     5335 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/domain/component.rs
+-rw-r--r--   0     1001      123     5398 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/domain/meta.rs
+-rw-r--r--   0     1001      123     1343 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/domain/mod.rs
+-rw-r--r--   0     1001      123    13105 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/domain/record.rs
+-rw-r--r--   0     1001      123     5986 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/domain/score.rs
+-rw-r--r--   0     1001      123     3252 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/domain/validamount.rs
+-rw-r--r--   0     1001      123     4327 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/domain/validname.rs
+-rw-r--r--   0     1001      123     3175 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/domain/validvalue.rs
+-rw-r--r--   0     1001      123      655 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/error.rs
+-rw-r--r--   0     1001      123      728 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/lib.rs
+-rw-r--r--   0     1001      123     1591 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/macros.rs
+-rw-r--r--   0     1001      123     1771 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/main.rs
+-rw-r--r--   0     1001      123     8434 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/metrics/database.rs
+-rw-r--r--   0     1001      123     1695 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/metrics/mod.rs
+-rw-r--r--   0     1001      123     6163 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/routes/add.rs
+-rw-r--r--   0     1001      123     3323 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/routes/get.rs
+-rw-r--r--   0     1001      123     6732 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/routes/get_since.rs
+-rw-r--r--   0     1001      123      449 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/routes/health_check.rs
+-rw-r--r--   0     1001      123      501 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/routes/mod.rs
+-rw-r--r--   0     1001      123     2960 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/routes/update.rs
+-rw-r--r--   0     1001      123     1718 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/startup.rs
+-rw-r--r--   0     1001      123     1393 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/src/telemetry.rs
+-rw-r--r--   0     1001      123     5192 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/tests/api/add.rs
+-rw-r--r--   0     1001      123    21377 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/tests/api/client.rs
+-rw-r--r--   0     1001      123     2667 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/tests/api/get.rs
+-rw-r--r--   0     1001      123     7793 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/tests/api/get_since.rs
+-rw-r--r--   0     1001      123      258 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/tests/api/health_check.rs
+-rw-r--r--   0     1001      123     4019 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/tests/api/helpers.rs
+-rw-r--r--   0     1001      123       88 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/tests/api/main.rs
+-rw-r--r--   0     1001      123     3672 2023-04-19 13:06:11.000000 python_auditor-0.1.0/local_dependencies/auditor/tests/api/update.rs
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 python_auditor-0.1.0/Cargo.toml
+-rw-r--r--   0     1001      123       28 2023-04-19 13:06:11.000000 python_auditor-0.1.0/.cargo/config.toml
+-rw-r--r--   0     1001      123      241 2023-04-19 13:06:11.000000 python_auditor-0.1.0/.readthedocs.yaml
+-rw-r--r--   0     1001      123     1865 2023-04-19 13:06:11.000000 python_auditor-0.1.0/README.md
+-rw-r--r--   0     1001      123      634 2023-04-19 13:06:11.000000 python_auditor-0.1.0/docs/Makefile
+-rw-r--r--   0     1001      123      128 2023-04-19 13:06:11.000000 python_auditor-0.1.0/docs/api.rst
+-rw-r--r--   0     1001      123       84 2023-04-19 13:06:11.000000 python_auditor-0.1.0/docs/changelog.rst
+-rw-r--r--   0     1001      123     1212 2023-04-19 13:06:11.000000 python_auditor-0.1.0/docs/conf.py
+-rw-r--r--   0     1001      123     6303 2023-04-19 13:06:11.000000 python_auditor-0.1.0/docs/examples.rst
+-rw-r--r--   0     1001      123      916 2023-04-19 13:06:11.000000 python_auditor-0.1.0/docs/index.rst
+-rw-r--r--   0     1001      123      800 2023-04-19 13:06:11.000000 python_auditor-0.1.0/docs/make.bat
+-rw-r--r--   0     1001      123      669 2023-04-19 13:06:11.000000 python_auditor-0.1.0/pyproject.toml
+-rwxr-xr-x   0     1001      123     1894 2023-04-19 13:06:11.000000 python_auditor-0.1.0/scripts/test_add_update.py
+-rwxr-xr-x   0     1001      123     1833 2023-04-19 13:06:11.000000 python_auditor-0.1.0/scripts/test_add_update_blocking.py
+-rwxr-xr-x   0     1001      123     2211 2023-04-19 13:06:11.000000 python_auditor-0.1.0/scripts/test_components.py
+-rwxr-xr-x   0     1001      123     2162 2023-04-19 13:06:11.000000 python_auditor-0.1.0/scripts/test_components_blocking.py
+-rwxr-xr-x   0     1001      123     1297 2023-04-19 13:06:11.000000 python_auditor-0.1.0/scripts/test_eq.py
+-rwxr-xr-x   0     1001      123     2118 2023-04-19 13:06:11.000000 python_auditor-0.1.0/scripts/test_get_since.py
+-rwxr-xr-x   0     1001      123     2057 2023-04-19 13:06:11.000000 python_auditor-0.1.0/scripts/test_get_since_blocking.py
+-rwxr-xr-x   0     1001      123     1874 2023-04-19 13:06:11.000000 python_auditor-0.1.0/scripts/test_meta.py
+-rwxr-xr-x   0     1001      123     1825 2023-04-19 13:06:11.000000 python_auditor-0.1.0/scripts/test_meta_blocking.py
+-rw-r--r--   0     1001      123     4834 2023-04-19 13:06:11.000000 python_auditor-0.1.0/src/blocking_client.rs
+-rw-r--r--   0     1001      123     3528 2023-04-19 13:06:11.000000 python_auditor-0.1.0/src/builder.rs
+-rw-r--r--   0     1001      123     5862 2023-04-19 13:06:11.000000 python_auditor-0.1.0/src/client.rs
+-rw-r--r--   0     1001      123     2607 2023-04-19 13:06:11.000000 python_auditor-0.1.0/src/domain/component.rs
+-rw-r--r--   0     1001      123     2000 2023-04-19 13:06:11.000000 python_auditor-0.1.0/src/domain/meta.rs
+-rw-r--r--   0     1001      123      464 2023-04-19 13:06:11.000000 python_auditor-0.1.0/src/domain/mod.rs
+-rw-r--r--   0     1001      123     6390 2023-04-19 13:06:11.000000 python_auditor-0.1.0/src/domain/record.rs
+-rw-r--r--   0     1001      123     2125 2023-04-19 13:06:11.000000 python_auditor-0.1.0/src/domain/score.rs
+-rw-r--r--   0     1001      123      981 2023-04-19 13:06:11.000000 python_auditor-0.1.0/src/lib.rs
+-rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 python_auditor-0.1.0/PKG-INFO
```

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/Cargo.toml` & `python_auditor-0.1.0/local_dependencies/auditor/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "auditor"
-version = "0.0.7"
+version = "0.1.0"
 authors = ["Stefan Kroboth <stefan.kroboth@gmail.com>"]
 edition = "2021"
 default-run = "auditor"
 license = "MIT OR Apache-2.0"
 description = "AccoUnting Data handlIng Toolbox for Opportunistic Resources"
 documentation = "https://docs.rs/auditor/"
 homepage = "https://alu-schumacher.github.io/AUDITOR/"
@@ -31,44 +31,44 @@
 name = "auditor"
 path = "src/main.rs"
 
 [profile.release]
 strip = true
 
 [dependencies]
-actix-web = "4.3.0"
+actix-web = "4.3.1"
 tokio = { version = "1", features = ["macros", "rt-multi-thread", "time"] }
 serde = { version = "1", features = ["derive"] }
 serde-aux = "4"
 serde_with = { version = "2", features = ["chrono_0_4"] }
 config = "0.13"
 uuid = { version = "1.3", features = ["v4"] }
-chrono = { version = "0.4.22", default-features = false, features = ["serde"] }
+chrono = { version = "0.4.24", default-features = false, features = ["serde"] }
 tracing = { version = "0.1", features = ["log"] }
 tracing-subscriber = { version = "0.3", features = ["registry", "env-filter"] }
 tracing-bunyan-formatter = "0.3"
 tracing-log = "0.1"
 tracing-actix-web = "0.7"
 secrecy = { version = "0.8", features = ["serde"] }
 unicode-segmentation = "1"
 fake = { version = "2.5", features = ["chrono"] }
 rand = "0.8"
-reqwest = { version = "0.11.14", default-features = false, features = ["json", "rustls-tls"] }
+reqwest = { version = "0.11.16", default-features = false, features = ["json", "rustls-tls", "blocking"] }
 anyhow = "1"
 regex = "1"
 num-traits = "^0.2"
 opentelemetry-prometheus = "0.10"
 opentelemetry = "0.17"
 actix-web-opentelemetry = { version = "0.12", features = ["metrics"] }
 thiserror = "1"
 prometheus = "0.13"
 itertools = "0.10.5"
 
 [dependencies.sqlx]
-version = "0.6.2"
+version = "0.6.3"
 default-features = false
 features = [
     "runtime-actix-rustls",
     "macros",
     "postgres",
     "uuid",
     "chrono",
```

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/build.rs` & `python_auditor-0.1.0/local_dependencies/auditor/build.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/sqlx-data.json` & `python_auditor-0.1.0/local_dependencies/auditor/sqlx-data.json`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/configuration.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/configuration.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/constants.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/constants.rs`

 * *Files 9% similar despite different names*

```diff
@@ -2,9 +2,10 @@
 //
 // Licensed under the Apache License, Version 2.0 <LICENSE-APACHE or
 // http://apache.org/licenses/LICENSE-2.0> or the MIT license <LICENSE-MIT or
 // http://opensource.org/licenses/MIT>, at your option. This file may not be
 // copied, modified, or distributed except according to those terms.
 
 pub const FORBIDDEN_CHARACTERS: [char; 9] = ['/', '(', ')', '"', '<', '>', '\\', '{', '}'];
+pub const ERR_INVALID_TIMEOUT: &str = "INVALID_TIMEOUT";
 pub const ERR_RECORD_EXISTS: &str = "RECORD_EXISTS";
 pub const ERR_UNEXPECTED_ERROR: &str = "UNEXPECTED_ERROR";
```

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/domain/component.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/domain/component.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/domain/meta.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/domain/meta.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/domain/mod.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/domain/mod.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/domain/record.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/domain/record.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/domain/score.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/domain/score.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/domain/validamount.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/domain/validamount.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/domain/validname.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/domain/validname.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/domain/validvalue.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/domain/validvalue.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/error.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/error.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/lib.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/lib.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/macros.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/macros.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/main.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/main.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/metrics/database.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/metrics/database.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/metrics/mod.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/routes/add.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/routes/add.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/routes/get.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/routes/get.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/routes/get_since.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/routes/get_since.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/routes/update.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/routes/update.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/startup.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/startup.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/src/telemetry.rs` & `python_auditor-0.1.0/local_dependencies/auditor/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/tests/api/add.rs` & `python_auditor-0.1.0/local_dependencies/auditor/tests/api/add.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/tests/api/client.rs` & `python_auditor-0.1.0/local_dependencies/auditor/tests/api/client.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 use crate::helpers::spawn_app;
-use auditor::client::AuditorClient;
+use auditor::client::AuditorClientBuilder;
 use auditor::domain::{Component, Record, RecordAdd, RecordDatabase, RecordTest, RecordUpdate};
 use chrono::{TimeZone, Utc};
 use fake::{Fake, Faker};
 
 #[tokio::test]
 async fn add_records() {
     // Arange
     let app = spawn_app().await;
-    let client = AuditorClient::from_connection_string(&app.address).unwrap();
+    let client = AuditorClientBuilder::new()
+        .connection_string(&app.address)
+        .build()
+        .unwrap();
 
     let mut test_cases_comp: Vec<RecordTest> =
         (0..100).map(|_| Faker.fake::<RecordTest>()).collect();
     let test_cases: Vec<RecordAdd> = test_cases_comp
         .iter()
         .cloned()
         .map(RecordAdd::try_from)
@@ -93,15 +96,18 @@
     }
 }
 
 #[tokio::test]
 async fn update_records() {
     // Arange
     let app = spawn_app().await;
-    let client = AuditorClient::from_connection_string(&app.address).unwrap();
+    let client = AuditorClientBuilder::new()
+        .connection_string(&app.address)
+        .build()
+        .unwrap();
 
     let mut test_cases_comp: Vec<RecordTest> =
         (0..100).map(|_| Faker.fake::<RecordTest>()).collect();
 
     let test_cases: Vec<RecordAdd> = test_cases_comp
         .iter()
         .cloned()
@@ -196,25 +202,31 @@
     }
 }
 
 #[tokio::test]
 async fn get_returns_empty_list_of_records() {
     // Arange
     let app = spawn_app().await;
-    let client = AuditorClient::from_connection_string(&app.address).unwrap();
+    let client = AuditorClientBuilder::new()
+        .connection_string(&app.address)
+        .build()
+        .unwrap();
 
     let records = client.get().await.unwrap();
 
     assert!(records.is_empty());
 }
 
 #[tokio::test]
 async fn get_returns_a_list_of_records() {
     let app = spawn_app().await;
-    let client = AuditorClient::from_connection_string(&app.address).unwrap();
+    let client = AuditorClientBuilder::new()
+        .connection_string(&app.address)
+        .build()
+        .unwrap();
 
     let mut test_cases: Vec<RecordTest> = (0..100).map(|_| Faker.fake::<RecordTest>()).collect();
 
     for record in test_cases.iter() {
         let runtime = (record.stop_time.unwrap() - record.start_time.unwrap()).num_seconds();
         let mut transaction = app.db_pool.begin().await.unwrap();
 
@@ -336,15 +348,18 @@
         );
     }
 }
 
 #[tokio::test]
 async fn get_started_since_returns_a_list_of_records() {
     let app = spawn_app().await;
-    let client = AuditorClient::from_connection_string(&app.address).unwrap();
+    let client = AuditorClientBuilder::new()
+        .connection_string(&app.address)
+        .build()
+        .unwrap();
 
     let mut test_cases: Vec<RecordTest> = (1..=31)
         .map(|i| {
             Faker
                 .fake::<RecordTest>()
                 .with_record_id(format!("r{i:0>2}"))
                 .with_start_time(format!("2022-03-{i:0>2}T12:00:00-00:00"))
@@ -482,15 +497,18 @@
         );
     }
 }
 
 #[tokio::test]
 async fn get_stopped_since_returns_a_list_of_records() {
     let app = spawn_app().await;
-    let client = AuditorClient::from_connection_string(&app.address).unwrap();
+    let client = AuditorClientBuilder::new()
+        .connection_string(&app.address)
+        .build()
+        .unwrap();
 
     let mut test_cases: Vec<RecordTest> = (1..=31)
         .map(|i| {
             Faker
                 .fake::<RecordTest>()
                 .with_record_id(format!("r{i:0>2}"))
                 .with_stop_time(format!("2022-03-{i:0>2}T12:00:00-00:00"))
```

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/tests/api/get.rs` & `python_auditor-0.1.0/local_dependencies/auditor/tests/api/get.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/tests/api/get_since.rs` & `python_auditor-0.1.0/local_dependencies/auditor/tests/api/get_since.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/tests/api/helpers.rs` & `python_auditor-0.1.0/local_dependencies/auditor/tests/api/helpers.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/local_dependencies/auditor/tests/api/update.rs` & `python_auditor-0.1.0/local_dependencies/auditor/tests/api/update.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/Cargo.toml` & `python_auditor-0.1.0/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "python-auditor"
-version = "0.0.7"
+version = "0.1.0"
 edition = "2021"
 authors = ["Stefan Kroboth <stefan.kroboth@gmail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python interface to AuditorClient"
 documentation = "https://docs.rs/pyauditor/"
 homepage = "https://alu-schumacher.github.io/AUDITOR/"
 repository = "https://github.com/alu-schumacher/AUDITOR"
@@ -21,14 +21,15 @@
 ]
 
 [lib]
 name = "pyauditor"
 crate-type = ["cdylib"]
 
 [dependencies]
-auditor = { path = "local_dependencies/auditor", version = "0.0.7", default-features = false, features = ["client"] }
+auditor = { path = "local_dependencies/auditor", version = "0.1.0", default-features = false, features = ["client"] }
 anyhow = "1"
 pyo3 = { version = "0.15.2", features = ["extension-module", "anyhow"] }
 pyo3-asyncio = { version = "0.15", features = ["attributes", "tokio-runtime"] }
 tokio = "1"
-chrono = { version = "0.4.22", features = ["serde"] }
+chrono = { version = "0.4.24", features = ["serde"] }
 pyo3-chrono = { version = "0.3.0", features = [] }
+serde_json = "1.0.96"
```

### Comparing `python_auditor-0.0.7/README.md` & `python_auditor-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/docs/Makefile` & `python_auditor-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/docs/conf.py` & `python_auditor-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/docs/examples.rst` & `python_auditor-0.1.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/docs/index.rst` & `python_auditor-0.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/docs/make.bat` & `python_auditor-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/pyproject.toml` & `python_auditor-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/scripts/test_add_update.py` & `python_auditor-0.1.0/scripts/test_add_update.py`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/scripts/test_components.py` & `python_auditor-0.1.0/scripts/test_components.py`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/scripts/test_eq.py` & `python_auditor-0.1.0/scripts/test_eq.py`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/scripts/test_get_since.py` & `python_auditor-0.1.0/scripts/test_get_since.py`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/scripts/test_meta.py` & `python_auditor-0.1.0/scripts/test_meta.py`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/src/builder.rs` & `python_auditor-0.1.0/src/builder.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright 2021-2022 AUDITOR developers
 //
 // Licensed under the Apache License, Version 2.0 <LICENSE-APACHE or
 // http://apache.org/licenses/LICENSE-2.0> or the MIT license <LICENSE-MIT or
 // http://opensource.org/licenses/MIT>, at your option. This file may not be
 // copied, modified, or distributed except according to those terms.
 
-use crate::client::AuditorClient;
+use crate::{blocking_client::AuditorClientBlocking, client::AuditorClient};
 use anyhow::Error;
 use pyo3::prelude::*;
 
 /// The ``AuditorClientBuilder`` class is used to build an instance of ``AuditorClient``.
 ///
 /// **Examples**
 ///
@@ -94,8 +94,17 @@
     pub fn build(&self) -> Result<AuditorClient, Error> {
         Ok(AuditorClient {
             // Must clone here because `build` moves the builder, but python
             // does not allow that. Doesn't matter, Python is slow anyways.
             inner: self.inner.clone().build()?,
         })
     }
+
+    /// Build an ``AuditorClientBlocking`` from ``AuditorClientBuilder``
+    pub fn build_blocking(&self) -> Result<AuditorClientBlocking, Error> {
+        Ok(AuditorClientBlocking {
+            // Must clone here because `build` moves the builder, but python
+            // does not allow that. Doesn't matter, Python is slow anyways.
+            inner: self.inner.clone().build_blocking()?,
+        })
+    }
 }
```

### Comparing `python_auditor-0.0.7/src/client.rs` & `python_auditor-0.1.0/src/client.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/src/domain/component.rs` & `python_auditor-0.1.0/src/domain/component.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/src/domain/meta.rs` & `python_auditor-0.1.0/src/domain/meta.rs`

 * *Files 8% similar despite different names*

```diff
@@ -25,21 +25,31 @@
     #[new]
     pub fn new() -> Self {
         Meta {
             inner: auditor::domain::Meta::new(),
         }
     }
 
+    /// insert(key: str, value: [str])
     /// Insert a key-value pair into Meta
+    ///
+    /// :param key: Key
+    /// :type key: str
+    /// :param value: Value
+    /// :type value: [str]
     fn insert(mut self_: PyRefMut<Self>, key: String, value: Vec<String>) -> PyRefMut<Self> {
         self_.inner.insert(key, value);
         self_
     }
 
+    /// get(key: str)
     /// Returns a list of string values matching the given key
+    ///
+    /// :param key: Key to get
+    /// :type key: str
     fn get(&self, key: String) -> Option<Vec<String>> {
         self.inner.get(&key).cloned()
     }
 }
 
 #[pyproto]
 impl PyObjectProtocol for Meta {
```

### Comparing `python_auditor-0.0.7/src/domain/record.rs` & `python_auditor-0.1.0/src/domain/record.rs`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,17 @@
     fn with_stop_time<'a>(
         mut self_: PyRefMut<'a, Self>,
         stop_time: &'a PyDateTime,
     ) -> Result<PyRefMut<'a, Self>, Error> {
         let stop_time: NaiveDateTime = stop_time.extract()?;
         let stop_time = Utc.from_utc_datetime(&stop_time.into());
         self_.inner.stop_time = Some(stop_time);
+        if let Some(start_time) = self_.inner.start_time.as_ref() {
+            self_.inner.runtime = Some((stop_time - *start_time).num_seconds())
+        }
         Ok(self_)
     }
 
     /// Returns the record_id
     #[getter]
     fn record_id(&self) -> String {
         self.inner.record_id.clone()
@@ -129,17 +132,17 @@
     fn components(&self) -> Option<Vec<Component>> {
         self.inner
             .components
             .as_ref()
             .map(|components| components.iter().cloned().map(Component::from).collect())
     }
 
-    /// Returns the meta dict
+    /// Returns the meta object
     ///
-    /// Returns None if no meta is available, otherwise returns a dict of meta information.
+    /// Returns None if no meta is available, otherwise returns a meta object.
     #[getter]
     fn meta(&self) -> Option<Meta> {
         self.inner.meta.clone().map(Meta::from)
     }
 
     /// Returns the start_time
     #[getter]
@@ -160,14 +163,19 @@
     }
 
     /// Returns the runtime of a record.
     #[getter]
     fn runtime(&self) -> Option<i64> {
         self.inner.runtime
     }
+
+    /// Output content of Record as JSON-encoded string
+    fn to_json(&self) -> Result<String, Error> {
+        Ok(format!("{}", serde_json::to_value(&self.inner)?))
+    }
 }
 
 #[pyproto]
 impl PyObjectProtocol for Record {
     fn __richcmp__(&self, other: PyRef<Record>, op: CompareOp) -> Py<PyAny> {
         let py = other.py();
         match op {
```

### Comparing `python_auditor-0.0.7/src/domain/score.rs` & `python_auditor-0.1.0/src/domain/score.rs`

 * *Files identical despite different names*

### Comparing `python_auditor-0.0.7/PKG-INFO` & `python_auditor-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-auditor
-Version: 0.0.7
+Version: 0.1.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-auditor Version: 0.0.7 Classifier:
+Metadata-Version: 2.1 Name: python-auditor Version: 0.1.0 Classifier:
 Programming Language :: Rust Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: MIT License Classifier: License :: OSI Approved :: Apache
 Software License Summary: Python interface to AuditorClient Keywords:
```

