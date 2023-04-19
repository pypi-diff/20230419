# Comparing `tmp/kestrel-lang-1.5.8.tar.gz` & `tmp/kestrel-lang-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-lang-1.5.8.tar", last modified: Thu Feb 16 16:09:24 2023, max compression
+gzip compressed data, was "kestrel-lang-1.5.9.tar", last modified: Fri Feb 17 22:47:08 2023, max compression
```

## Comparing `kestrel-lang-1.5.8.tar` & `kestrel-lang-1.5.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.645272 kestrel-lang-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-16 16:09:24.645272 kestrel-lang-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.633272 kestrel-lang-1.5.8/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/bin/kestrel
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-16 16:09:24.645272 kestrel-lang-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.629272 kestrel-lang-1.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.633272 kestrel-lang-1.5.8/src/kestrel/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.633272 kestrel-lang-1.5.8/src/kestrel/absinterface/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/absinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/absinterface/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.633272 kestrel-lang-1.5.8/src/kestrel/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/analytics/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/analytics/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.633272 kestrel-lang-1.5.8/src/kestrel/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/codegen/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/codegen/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/codegen/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/codegen/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/codegen/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/codegen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.637272 kestrel-lang-1.5.8/src/kestrel/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/datasource/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/datasource/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/datasource/retstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.637272 kestrel-lang-1.5.8/src/kestrel/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/semantics/completor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/semantics/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/semantics/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.637272 kestrel-lang-1.5.8/src/kestrel/symboltable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/symboltable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/symboltable/symtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/symboltable/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.637272 kestrel-lang-1.5.8/src/kestrel/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/syntax/ecgpattern.lark
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/syntax/ecgpattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/syntax/kestrel.lark
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/syntax/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/syntax/reference.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/syntax/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/syntax/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.637272 kestrel-lang-1.5.8/src/kestrel_analytics_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_analytics_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_analytics_docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_analytics_docker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.637272 kestrel-lang-1.5.8/src/kestrel_analytics_python/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_analytics_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_analytics_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_analytics_python/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.637272 kestrel-lang-1.5.8/src/kestrel_datasource_stixbundle/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_datasource_stixbundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_datasource_stixbundle/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.641272 kestrel-lang-1.5.8/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/src/kestrel_datasource_stixshifter/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.641272 kestrel-lang-1.5.8/src/kestrel_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-16 16:09:24.000000 kestrel-lang-1.5.8/src/kestrel_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-02-16 16:09:24.000000 kestrel-lang-1.5.8/src/kestrel_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 16:09:24.000000 kestrel-lang-1.5.8/src/kestrel_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-16 16:09:24.000000 kestrel-lang-1.5.8/src/kestrel_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-16 16:09:24.000000 kestrel-lang-1.5.8/src/kestrel_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:09:24.645272 kestrel-lang-1.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_find.py
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_command_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_python_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-02-16 16:09:06.000000 kestrel-lang-1.5.8/tests/test_timestamped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.207566 kestrel-lang-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-17 22:47:08.207566 kestrel-lang-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.183565 kestrel-lang-1.5.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/bin/kestrel
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-17 22:47:08.207566 kestrel-lang-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.183565 kestrel-lang-1.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.187565 kestrel-lang-1.5.9/src/kestrel/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.187565 kestrel-lang-1.5.9/src/kestrel/absinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/absinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/absinterface/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.187565 kestrel-lang-1.5.9/src/kestrel/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/analytics/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/analytics/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.191566 kestrel-lang-1.5.9/src/kestrel/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/codegen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.191566 kestrel-lang-1.5.9/src/kestrel/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/datasource/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/datasource/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/datasource/retstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.191566 kestrel-lang-1.5.9/src/kestrel/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/semantics/completor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/semantics/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/semantics/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.195566 kestrel-lang-1.5.9/src/kestrel/symboltable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/symboltable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/symboltable/symtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/symboltable/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.195566 kestrel-lang-1.5.9/src/kestrel/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/ecgpattern.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/ecgpattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/kestrel.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/reference.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/syntax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.195566 kestrel-lang-1.5.9/src/kestrel_analytics_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_docker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.199566 kestrel-lang-1.5.9/src/kestrel_analytics_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_analytics_python/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.199566 kestrel-lang-1.5.9/src/kestrel_datasource_stixbundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixbundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixbundle/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.199566 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.199566 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-17 22:47:08.000000 kestrel-lang-1.5.9/src/kestrel_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:47:08.207566 kestrel-lang-1.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_command_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_python_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-02-17 22:46:49.000000 kestrel-lang-1.5.9/tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.5.8/AUTHORS.rst` & `kestrel-lang-1.5.9/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/LICENSE.md` & `kestrel-lang-1.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/PKG-INFO` & `kestrel-lang-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.5.8
+Version: 1.5.9
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.5.8/README.rst` & `kestrel-lang-1.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/setup.cfg` & `kestrel-lang-1.5.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-lang
-version = 1.5.8
+version = 1.5.9
 description = Kestrel Threat Hunting Language
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
```

### Comparing `kestrel-lang-1.5.8/src/kestrel/__main__.py` & `kestrel-lang-1.5.9/src/kestrel/__main__.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/absinterface/manager.py` & `kestrel-lang-1.5.9/src/kestrel/absinterface/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/analytics/interface.py` & `kestrel-lang-1.5.9/src/kestrel/analytics/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/analytics/manager.py` & `kestrel-lang-1.5.9/src/kestrel/analytics/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/codegen/commands.py` & `kestrel-lang-1.5.9/src/kestrel/codegen/commands.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/codegen/data.py` & `kestrel-lang-1.5.9/src/kestrel/codegen/data.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/codegen/display.py` & `kestrel-lang-1.5.9/src/kestrel/codegen/display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/codegen/queries.py` & `kestrel-lang-1.5.9/src/kestrel/codegen/queries.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/codegen/relations.py` & `kestrel-lang-1.5.9/src/kestrel/codegen/relations.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/codegen/summary.py` & `kestrel-lang-1.5.9/src/kestrel/codegen/summary.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/config.py` & `kestrel-lang-1.5.9/src/kestrel/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/config.yaml` & `kestrel-lang-1.5.9/src/kestrel/config.yaml`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/datasource/interface.py` & `kestrel-lang-1.5.9/src/kestrel/datasource/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/datasource/manager.py` & `kestrel-lang-1.5.9/src/kestrel/datasource/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/datasource/retstruct.py` & `kestrel-lang-1.5.9/src/kestrel/datasource/retstruct.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/exceptions.py` & `kestrel-lang-1.5.9/src/kestrel/exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/semantics/completor.py` & `kestrel-lang-1.5.9/src/kestrel/semantics/completor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/semantics/processor.py` & `kestrel-lang-1.5.9/src/kestrel/semantics/processor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/semantics/reference.py` & `kestrel-lang-1.5.9/src/kestrel/semantics/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/session.py` & `kestrel-lang-1.5.9/src/kestrel/session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/symboltable/variable.py` & `kestrel-lang-1.5.9/src/kestrel/symboltable/variable.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/syntax/ecgpattern.py` & `kestrel-lang-1.5.9/src/kestrel/syntax/ecgpattern.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/syntax/kestrel.lark` & `kestrel-lang-1.5.9/src/kestrel/syntax/kestrel.lark`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/syntax/parser.py` & `kestrel-lang-1.5.9/src/kestrel/syntax/parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/syntax/reference.py` & `kestrel-lang-1.5.9/src/kestrel/syntax/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/syntax/utils.py` & `kestrel-lang-1.5.9/src/kestrel/syntax/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel/utils.py` & `kestrel-lang-1.5.9/src/kestrel/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel_analytics_docker/config.py` & `kestrel-lang-1.5.9/src/kestrel_analytics_docker/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel_analytics_docker/interface.py` & `kestrel-lang-1.5.9/src/kestrel_analytics_docker/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel_analytics_python/config.py` & `kestrel-lang-1.5.9/src/kestrel_analytics_python/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel_analytics_python/interface.py` & `kestrel-lang-1.5.9/src/kestrel_analytics_python/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel_datasource_stixbundle/interface.py` & `kestrel-lang-1.5.9/src/kestrel_datasource_stixbundle/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel_datasource_stixshifter/config.py` & `kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from kestrel.utils import update_nested_dict
 from kestrel.exceptions import InvalidDataSource
 
 PROFILE_PATH_DEFAULT = CONFIG_DIR_DEFAULT / "stixshifter.yaml"
 PROFILE_PATH_ENV_VAR = "KESTREL_STIXSHIFTER_CONFIG"
 STIXSHIFTER_DEBUG_ENV_VAR = "KESTREL_STIXSHIFTER_DEBUG"  # debug mode for stix-shifter if the environment variable exists
 ENV_VAR_PREFIX = "STIXSHIFTER_"
-RETRIEVAL_BATCH_SIZE = 10000
+RETRIEVAL_BATCH_SIZE = 512
 
 _logger = logging.getLogger(__name__)
 
 
 def set_stixshifter_logging_level():
     debug_mode = os.getenv(STIXSHIFTER_DEBUG_ENV_VAR, False)
     logging_level = logging.DEBUG if debug_mode else logging.INFO
```

### Comparing `kestrel-lang-1.5.8/src/kestrel_datasource_stixshifter/connector.py` & `kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/connector.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/src/kestrel_datasource_stixshifter/interface.py` & `kestrel-lang-1.5.9/src/kestrel_datasource_stixshifter/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
                             RETRIEVAL_BATCH_SIZE,
                             lastsortvalue,
                         )
                         if result_batch["success"]:
                             new_entries = result_batch["data"]
                             if new_entries:
                                 connector_results += new_entries
-                                result_retrieval_offset += RETRIEVAL_BATCH_SIZE
+                                result_retrieval_offset += len(new_entries)
                             else:
                                 has_remaining_results = False
                             if "lastsort" in result_batch:
                                 lastsortvalue = result_batch["lastsort"]
                         else:
                             stix_shifter_error_msg = (
                                 result_batch["error"]
```

### Comparing `kestrel-lang-1.5.8/src/kestrel_lang.egg-info/PKG-INFO` & `kestrel-lang-1.5.9/src/kestrel_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.5.8
+Version: 1.5.9
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.5.8/src/kestrel_lang.egg-info/SOURCES.txt` & `kestrel-lang-1.5.9/src/kestrel_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_assign.py` & `kestrel-lang-1.5.9/tests/test_command_assign.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_disp.py` & `kestrel-lang-1.5.9/tests/test_command_disp.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_find.py` & `kestrel-lang-1.5.9/tests/test_command_find.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_get.py` & `kestrel-lang-1.5.9/tests/test_command_get.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_group.py` & `kestrel-lang-1.5.9/tests/test_command_group.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_join.py` & `kestrel-lang-1.5.9/tests/test_command_join.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_load.py` & `kestrel-lang-1.5.9/tests/test_command_load.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_merge.py` & `kestrel-lang-1.5.9/tests/test_command_merge.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_new.py` & `kestrel-lang-1.5.9/tests/test_command_new.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_command_save.py` & `kestrel-lang-1.5.9/tests/test_command_save.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_completion.py` & `kestrel-lang-1.5.9/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_display.py` & `kestrel-lang-1.5.9/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_exceptions.py` & `kestrel-lang-1.5.9/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_expressions.py` & `kestrel-lang-1.5.9/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_parser.py` & `kestrel-lang-1.5.9/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_python_analytics.py` & `kestrel-lang-1.5.9/tests/test_python_analytics.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_session.py` & `kestrel-lang-1.5.9/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_stixshifter.py` & `kestrel-lang-1.5.9/tests/test_stixshifter.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.5.8/tests/test_timestamped.py` & `kestrel-lang-1.5.9/tests/test_timestamped.py`

 * *Files identical despite different names*

