# Comparing `tmp/fprime-tools-3.1.2a3.tar.gz` & `tmp/fprime-tools-3.1.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fprime-tools-3.1.2a3.tar", last modified: Tue Feb 28 22:43:11 2023, max compression
+gzip compressed data, was "fprime-tools-3.1.2a4.tar", last modified: Wed Apr 19 21:07:23 2023, max compression
```

## Comparing `fprime-tools-3.1.2a3.tar` & `fprime-tools-3.1.2a4.tar`

### file list

```diff
@@ -1,139 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/ISSUE_TEMPLATE/feature-request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.462801 fprime-tools-3.1.2a3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/.github/actions/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/actions/codeql/security-pack.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/.github/actions/spelling/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/actions/spelling/allow.txt
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/actions/spelling/excludes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/actions/spelling/expect.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/actions/spelling/patterns.txt
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/workflows/codeql-security-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/workflows/fprime-tools-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.github/workflows/spelling.yml
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.462801 fprime-tools-3.1.2a3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/docs/_static/css/rtd_width.css
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/docs/gendoc.bash
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/pylama.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.466801 fprime-tools-3.1.2a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/src/fprime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/src/fprime/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.470801 fprime-tools-3.1.2a3/src/fprime/common/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.474801 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/array_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/bool_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/enum_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/numerical_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/serializable_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/string_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/time_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/type_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/common/models/serialize/type_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.474801 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/CMakeLists_template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.474801 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.474801 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.474801 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.474801 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/sdd.md
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}ComponentAi.xml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/port_template.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.478801 fprime-tools-3.1.2a3/src/fprime/fbuild/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/cmake.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/gcovr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16976 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13426 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/target_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fbuild/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.478801 fprime-tools-3.1.2a3/src/fprime/fpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/fpp/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.478801 fprime-tools-3.1.2a3/src/fprime/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/util/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/util/build_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/util/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/util/code_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/util/help_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/util/string_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/src/fprime/util/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.478801 fprime-tools-3.1.2a3/src/fprime_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-28 22:43:11.000000 fprime-tools-3.1.2a3/src/fprime_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-02-28 22:43:11.000000 fprime-tools-3.1.2a3/src/fprime_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 22:43:11.000000 fprime-tools-3.1.2a3/src/fprime_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-28 22:43:11.000000 fprime-tools-3.1.2a3/src/fprime_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-28 22:43:11.000000 fprime-tools-3.1.2a3/src/fprime_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-28 22:43:11.000000 fprime-tools-3.1.2a3/src/fprime_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.466801 fprime-tools-3.1.2a3/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.466801 fprime-tools-3.1.2a3/test/fprime/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.466801 fprime-tools-3.1.2a3/test/fprime/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.466801 fprime-tools-3.1.2a3/test/fprime/common/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.478801 fprime-tools-3.1.2a3/test/fprime/common/models/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)    18469 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/common/models/serialize/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/common/models/serialize/time_type_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.478801 fprime-tools-3.1.2a3/test/fprime/fbuild/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.466801 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/external/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/external/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/grand-unified/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/grand-unified/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/subdir/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/CMakeCache.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/hashes.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/settings.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/subdir1/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/subdir1/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/subdir1/build-fprime-automatic-abcdefg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/subdir1/build-fprime-automatic-abcdefg/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.466801 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.466801 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/build-fprime-automatic-default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/build-fprime-automatic-default/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:43:11.482802 fprime-tools-3.1.2a3/test/fprime/fbuild/settings-data/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/settings-data/settings-custom-install.ini
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/settings-data/settings-custom-toolchain.ini
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/settings-data/settings-empty.ini
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/settings-data/settings-multi-line-default-options.ini
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/settings-data/settings-outside-cookiecutter.ini
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-02-28 22:42:51.000000 fprime-tools-3.1.2a3/test/fprime/fbuild/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.924112 fprime-tools-3.1.2a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/ISSUE_TEMPLATE/feature-request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.908112 fprime-tools-3.1.2a4/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/.github/actions/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/actions/codeql/security-pack.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/.github/actions/spelling/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/actions/spelling/allow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/actions/spelling/excludes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/actions/spelling/expect.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/actions/spelling/patterns.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/workflows/codeql-security-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/workflows/fprime-tools-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.github/workflows/spelling.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-19 21:07:23.924112 fprime-tools-3.1.2a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.908112 fprime-tools-3.1.2a4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/docs/_static/css/rtd_width.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/docs/gendoc.bash
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/pylama.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 21:07:23.924112 fprime-tools-3.1.2a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/array_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/bool_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/numerical_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/serializable_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/string_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/time_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/type_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/models/serialize/type_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/CMakeLists_template.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/sdd.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.fpp
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/instances.fpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/topology.fpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Packets.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}TopologyDefs.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/settings.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.916112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/project.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/port_template.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/src/fprime/fbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fbuild/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fbuild/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fbuild/cmake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fbuild/gcovr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fbuild/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fbuild/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fbuild/target_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fbuild/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/src/fprime/fpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/fpp/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/src/fprime/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/build_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/code_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17944 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/cookiecutter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18728 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/help_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/src/fprime/util/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/src/fprime_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-19 21:07:23.000000 fprime-tools-3.1.2a4/src/fprime_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-19 21:07:23.000000 fprime-tools-3.1.2a4/src/fprime_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:07:23.000000 fprime-tools-3.1.2a4/src/fprime_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 21:07:23.000000 fprime-tools-3.1.2a4/src/fprime_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-19 21:07:23.000000 fprime-tools-3.1.2a4/src/fprime_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 21:07:23.000000 fprime-tools-3.1.2a4/src/fprime_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/test/fprime/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/test/fprime/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/test/fprime/common/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/test/fprime/common/models/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)    18469 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/common/models/serialize/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/common/models/serialize/time_type_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/test/fprime/fbuild/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/external/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/grand-unified/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/grand-unified/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.920112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/subdir/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.924112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.924112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/CMakeCache.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/hashes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/settings.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.924112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/subdir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/subdir1/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.924112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/subdir1/build-fprime-automatic-abcdefg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/subdir1/build-fprime-automatic-abcdefg/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.912112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.924112 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/build-fprime-automatic-default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/build-fprime-automatic-default/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:07:23.924112 fprime-tools-3.1.2a4/test/fprime/fbuild/settings-data/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/settings-data/settings-custom-install.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/settings-data/settings-custom-toolchain.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/settings-data/settings-empty.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/settings-data/settings-multi-line-default-options.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/settings-data/settings-outside-cookiecutter.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-19 21:07:00.000000 fprime-tools-3.1.2a4/test/fprime/fbuild/test_settings.py
```

### Comparing `fprime-tools-3.1.2a3/.github/actions/spelling/expect.txt` & `fprime-tools-3.1.2a4/.github/actions/spelling/expect.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,43 @@
+argc
+atoi
 bak
+Callee
 cargs
+CDH
 cexc
 cfg
 ci
 cls
 cmake
 cmakelists
 cmp
 commonprefix
 config
 configparser
 configs
 confparse
 consts
-contextmanager
 contextlib
+contextmanager
 cookiecutter
+COOLDOWN
 cpp
 CPython
 css
+cstdlib
 ctor
 cwd
 CXX
 datetime
 dedent
 deduplicated
 deepcopy
+Deframer
+deframing
 DEPS
 deser
 deserialization
 deserialize
 deserialized
 deserializer
 deserializes
@@ -38,20 +46,22 @@
 dfl
 dinkel
 dirname
 dirone
 dirs
 distutils
 doctest
+Drv
 dumpable
 Dxyz
 elif
 endfor
 endif
 endswith
+entrypoint
 enum
 excinfo
 exe
 executables
 extlinks
 favicon
 fbuild
@@ -60,47 +70,52 @@
 filecmp
 FILEID
 fileobj
 filepath
 firest
 floordiv
 FPGA
-fprime
 fpp
+fprime
 fromkeys
 fromtimestamp
 func
 funcs
 functools
 gcda
 gcno
 gcov
 gcovr
 genex
 getattr
 getcwd
+getopt
 gh
 github
 gtest
 gui
 hasattr
 HJK
+hostname
 hpaulson
 hpp
 html
 http
 ifconfig
+ifndef
 impl
 importlib
 ini
+inlined
 intersphinx
 isdir
 isfile
 isinstance
 isnumeric
+Isr
 issubclass
 iterdir
 itertools
 itle
 IUF
 jishii
 joinpath
@@ -108,42 +123,53 @@
 jpl
 JSO
 json
 jsonable
 kevin
 kwargs
 len
+linux
 lld
 llvm
 locs
 lstrip
 lxml
 makedirs
+malloc
+mallocator
 maxdepth
 MEMB
+memset
 metadata
 mkdir
 mkdtemp
 mstarch
 mul
 MULTILINE
+Mutex
 namespace
+namespaced
 nargs
 nitpicky
 normpath
+nullptr
 openpty
+optarg
 optionxform
 oran
+Packetizer
 Paetz
 params
 pathlib
 Peet
 pexpect
+Pkts
 Popen
 postprocessed
+printf
 proj
 ptf
 py
 pydoc
 pyflakes
 pylama
 pylint
@@ -154,14 +180,15 @@
 radd
 raspberrypi
 rb
 readline
 README
 readthedocs
 recommonmark
+recv
 reder
 Refactor
 relpath
 restructuredtext
 returncode
 rfloordiv
 rmd
@@ -169,21 +196,25 @@
 rmul
 rpaetz
 rst
 rstrip
 rsub
 rtd
 rtruediv
+samefile
 sanitizers
-Sched
+sched
 SCLK
 scm
 sdd
 setuptools
 shutil
+SIGINT
+SIGTERM
+sizeof
 someotherpath
 sphinxcontrib
 splitlines
 src
 sset
 stackoverflow
 startswith
@@ -195,30 +226,33 @@
 strftime
 stylesheet
 subdir
 subparser
 Subproc
 sys
 tcanham
+Tcp
 td
 tempdir
 tempfile
 testbuild
 testimpl
 textwrap
 timebase
 toctree
 todo
 toolchain
 toolchains
+TOPOLOGYDEFS
 truediv
 typehints
 typename
 tz
 tzinfo
+Udp
 uint
 Uncomment
 undoc
 uninstall
 unittest
 unt
 url
@@ -228,13 +262,14 @@
 utf
 Utils
 valgrind
 vals
 venv
 versioning
 viewcode
+Website
 whitelist
 whitespaces
 workdir
 www
 wxgui
 xml
```

### Comparing `fprime-tools-3.1.2a3/.github/actions/spelling/patterns.txt` & `fprime-tools-3.1.2a4/.github/actions/spelling/patterns.txt`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/.github/pull_request_template.md` & `fprime-tools-3.1.2a4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/.github/workflows/codeql-security-scan.yml` & `fprime-tools-3.1.2a4/.github/workflows/codeql-security-scan.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/.github/workflows/fprime-tools-ci.yml` & `fprime-tools-3.1.2a4/.github/workflows/fprime-tools-ci.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/.github/workflows/integration-tests.yml` & `fprime-tools-3.1.2a4/.github/workflows/integration-tests.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/.github/workflows/publish.yml` & `fprime-tools-3.1.2a4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/.github/workflows/spelling.yml` & `fprime-tools-3.1.2a4/.github/workflows/spelling.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/LICENSE.txt` & `fprime-tools-3.1.2a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/NOTICE.txt` & `fprime-tools-3.1.2a4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/PKG-INFO` & `fprime-tools-3.1.2a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime-tools
-Version: 3.1.2a3
+Version: 3.1.2a4
 Summary: F Prime Flight Software core data types
 Home-page: https://github.com/nasa/fprime
 Author: Michael Starch
 Author-email: Michael.D.Starch@jpl.nasa.gov
 License: Apache 2.0 License
 Project-URL: Issue Tracker, https://github.com/nasa/fprime/issues
 Keywords: fprime,embedded,nasa
```

### Comparing `fprime-tools-3.1.2a3/README.md` & `fprime-tools-3.1.2a4/README.md`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/docs/_static/css/rtd_width.css` & `fprime-tools-3.1.2a4/docs/_static/css/rtd_width.css`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/docs/conf.py` & `fprime-tools-3.1.2a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/docs/index.rst` & `fprime-tools-3.1.2a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/pylama.cfg` & `fprime-tools-3.1.2a4/pylama.cfg`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/setup.py` & `fprime-tools-3.1.2a4/setup.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/__init__.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/array_type.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/array_type.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/bool_type.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/bool_type.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/enum_type.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/enum_type.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/numerical_types.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/numerical_types.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/serializable_type.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/serializable_type.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/string_type.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/string_type.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/time_type.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/time_type.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/type_base.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/type_base.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/common/models/serialize/type_exceptions.py` & `fprime-tools-3.1.2a4/src/fprime/common/models/serialize/type_exceptions.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/constants.py` & `fprime-tools-3.1.2a4/src/fprime/constants.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/pre_gen_project.py` & `fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/pre_gen_project.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fprime.fbuild.interaction import is_valid_name
+from fprime.util.cookiecutter_wrapper import is_valid_name
 
 # Check to ensure Component Name is valid
 def verify_inputs(component_name, commands, events, telemetry, parameters):
     if is_valid_name(component_name) != "valid":
         raise ValueError(
             "Unacceptable component name. Do not use spaces or special characters"
         )
@@ -10,12 +10,12 @@
         raise ValueError(
             "[ERROR] You must select at least one of the following options to have in your component: commands, events, telemetry, parameters"
         )
 
 
 verify_inputs(
     "{{ cookiecutter.component_name }}",
-    "{{ cookiecutter.commands }}",
-    "{{ cookiecutter.events }}",
-    "{{ cookiecutter.telemetry }}",
-    "{{ cookiecutter.parameters }}",
+    "{{ cookiecutter.enable_commands }}",
+    "{{ cookiecutter.enable_events }}",
+    "{{ cookiecutter.enable_telemetry }}",
+    "{{ cookiecutter.enable_parameters }}",
 )
```

### Comparing `fprime-tools-3.1.2a3/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/CMakeLists.txt` & `fprime-tools-3.1.2a4/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 #
 # SOURCE_FILES: combined list of source and autocoding files
 # MOD_DEPS: (optional) module dependencies
 # UT_SOURCE_FILES: list of source files for unit tests
 #
 ####
 set(SOURCE_FILES
-  "${CMAKE_CURRENT_LIST_DIR}/{{cookiecutter.component_name}}ComponentAi.xml"
+  "${CMAKE_CURRENT_LIST_DIR}/{{cookiecutter.component_name}}.fpp"
   "${CMAKE_CURRENT_LIST_DIR}/{{cookiecutter.component_name}}.cpp"
 )
 
 # Uncomment and add any modules that this component depends on, else
 # they might not be available when cmake tries to build this component.
 
 # set(MOD_DEPS
 #     Add your dependencies here
 # )
 
-register_fprime_module()
+register_fprime_module()
```

### Comparing `fprime-tools-3.1.2a3/src/fprime/fbuild/builder.py` & `fprime-tools-3.1.2a4/src/fprime/fbuild/builder.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/fbuild/cli.py` & `fprime-tools-3.1.2a4/src/fprime/fbuild/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 import argparse
 from pathlib import Path
 from typing import Dict, List, Tuple, Callable
 from fprime.fbuild.types import BuildType
 from fprime.fbuild.target import Target
 from fprime.fbuild.builder import Build
-from fprime.fbuild.interaction import confirm
+from fprime.common.utils import confirm
 
 
 def get_target(parsed: argparse.Namespace) -> Target:
     """Gets the target given the argparse namespace
 
     Takes the parsed namespace and processes it to a known matching target.
 
@@ -81,15 +81,23 @@
                 )
                 if parsed.force or confirm(
                     f"Purge installation directory at {install_dir} (yes/no)?"
                 ):
                     purge_build.purge_install()
     else:
         target = get_target(parsed)
-        target.execute(build, context=Path(parsed.path), args=(make_args, pass_through))
+        option_args = {
+            flag: getattr(parsed, flag.lstrip("-").replace("-", "_"), False)
+            for flag, _ in target.option_args()
+        }
+        target.execute(
+            build,
+            context=Path(parsed.path),
+            args=(make_args, pass_through, option_args),
+        )
 
 
 def add_target_parser(
     target: Target,
     subparsers,
     common: argparse.ArgumentParser,
     existing: Dict[str, Tuple[argparse.ArgumentParser, List[str]]],
@@ -146,14 +154,19 @@
         )
         parser.add_argument(
             f"--{flag}",
             action="store_true",
             default=False,
             help=f"{target.desc}{extra_help}",
         )
+    for flag, description in filter(
+        lambda flag_desc: flag_desc[0] not in flags, target.option_args()
+    ):
+        parser.add_argument(flag, action="store_true", help=f"{description}")
+        new_flags.append(flag)
     # Allow pass through arguments
     if target.pass_handler() and "--pass-through" not in flags:
         parser.add_argument(
             "--pass-through",
             nargs=argparse.REMAINDER,
             default=[],
             help="If specified, --pass-through must be the last argument. Remaining arguments passed to underlying executable",
```

### Comparing `fprime-tools-3.1.2a3/src/fprime/fbuild/cmake.py` & `fprime-tools-3.1.2a4/src/fprime/fbuild/cmake.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/fbuild/interaction.py` & `fprime-tools-3.1.2a4/src/fprime/util/cookiecutter_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,114 +1,109 @@
 """ Cookie cutter wrapper used to template out components
 """
 import os
 import glob
 import sys
-import textwrap
 from pathlib import Path
-from typing import Dict
 import re
 from contextlib import contextmanager
+import shutil
 
 from cookiecutter.main import cookiecutter
 from cookiecutter.exceptions import OutputDirExistsException
 from jinja2 import Environment, FileSystemLoader
 
+from fprime.common.utils import confirm
 from fprime.fbuild.builder import Build
 from fprime.fbuild.target import Target
 from fprime.fbuild.cmake import CMakeExecutionException
+from fprime.util.code_formatter import ClangFormatter
 
 
-def confirm(msg):
-    """Confirms the removal of the file with a yes or no input"""
-    # Loop "forever" intended
-    while True:
-        confirm_input = input(msg)
-        if confirm_input.lower() in ["y", "yes"]:
-            return True
-        if confirm_input.lower() in ["n", "no"]:
-            return False
-        print(f"{confirm_input} is invalid.  Please use 'yes' or 'no'")
-
-
-def replace_contents(filename, what, replacement, count=1):
-    changelog = Path(filename).read_text()
-    with open(filename, "w") as fh:
-        new_file = changelog.replace(what, replacement, count)
-        fh.write(new_file)
-        return new_file != changelog
-
-
-def run_impl(deployment: Path, path: Path, platform: str, verbose: bool):
-    """Run implementation of files one time"""
+def run_impl(build: Build, source_path: Path):
+    """Run implementation of files in source_path"""
     target = Target.get_target("impl", set())
-    build = Build(target.build_type, deployment, verbose=verbose)
-    build.load(platform)
 
-    hpp_files = glob.glob(f"{path}/*.hpp", recursive=False)
-    cpp_files = glob.glob(f"{path}/*.cpp", recursive=False)
+    hpp_files = glob.glob(f"{source_path}/*.hpp", recursive=False)
+    cpp_files = glob.glob(f"{source_path}/*.cpp", recursive=False)
     cpp_files.sort(key=len)
 
     # Check destinations
     if not hpp_files or not cpp_files:
         print(
             "[WARNING] Failed to find .cpp and .hpp destination files for implementation."
         )
         return False
 
     common = [name for name in cpp_files if "Common" in name] + []
     hpp_dest = hpp_files[0]
     cpp_dest = common[0] if common else cpp_files[0]
 
-    if not confirm(
-        f"Generate implementations and merge into {hpp_dest} and {cpp_dest}?"
-    ):
+    if not confirm(f"Generate implementation files (yes/no)? "):
         return False
-    print("Generating implementation files and merging...")
+    print(
+        "Refreshing cache and generating implementation files (ignore 'Stop' CMake warning)..."
+    )
     with suppress_stdout():
-        build.execute(target, context=path, make_args={})
+        target.execute(build, source_path, ({}, [], {}))
 
-    hpp_files_template = glob.glob(f"{path}/*.hpp-template", recursive=False)
-    cpp_files_template = glob.glob(f"{path}/*.cpp-template", recursive=False)
+    hpp_files_template = glob.glob(f"{source_path}/*.hpp-template", recursive=False)
+    cpp_files_template = glob.glob(f"{source_path}/*.cpp-template", recursive=False)
 
     if not hpp_files_template or not cpp_files_template:
         print("[WARNING] Failed to find generated .cpp-template or .hpp-template files")
         return False
 
     hpp_src = hpp_files_template[0]
     cpp_src = cpp_files_template[0]
 
-    # Copy files without headers
-    for src, dest in [(hpp_src, hpp_dest), (cpp_src, cpp_dest)]:
-        with open(src, "r") as file_handle:
-            lines = file_handle.readlines()
-        lines = lines[11:]  # Remove old header
-        with open(dest, "a") as file_handle:
-            file_handle.write("".join(lines))
-
-    removals = [Path(hpp_src), Path(cpp_src)]
-    for removal in removals:
-        os.remove(removal)
+    # Move (and overwrite) files from *.(c|h)pp-template to *.(c|h)pp
+    shutil.move(hpp_src, hpp_dest)
+    shutil.move(cpp_src, cpp_dest)
+
+    # Format files if clang-format is available
+    format_file = build.settings.get("framework_path", Path(".")) / ".clang-format"
+    if not format_file.is_file():
+        print(
+            f"[WARNING] .clang-format file not found at {format_file.resolve()}. Skipping formatting."
+        )
+        return True
+    clang_formatter = ClangFormatter("clang-format", format_file, {"backup": False})
+    if clang_formatter.is_supported():
+        clang_formatter.stage_file(Path(hpp_dest))
+        clang_formatter.stage_file(Path(cpp_dest))
+        clang_formatter.execute(None, None, ({}, []))
+    else:
+        print("[WARNING] clang-format not found in PATH. Skipping formatting.")
+
     return True
 
 
-def add_to_cmake(list_file: Path, comp_path: Path):
-    """Adds new component or port to CMakeLists.txt"""
-    print(f"[INFO] Found CMakeLists.txt at '{list_file}'")
+def add_to_cmake(list_file: Path, comp_path: Path, project_root: Path = None):
+    """Adds new component or port to CMakeLists.txt. If project_root is supplied,
+    the logged path will be relative to the project root instead of absolute"""
+    short_display_path = (
+        list_file
+        if project_root is None
+        else project_root.name / list_file.relative_to(project_root)
+    )
+    print(f"[INFO] Found CMake file at '{short_display_path}'")
     with open(list_file, "r") as f:
         lines = f.readlines()
 
     addition = (
         'add_fprime_subdirectory("${CMAKE_CURRENT_LIST_DIR}/' + str(comp_path) + '/")\n'
     )
     if addition in lines:
         print("Already added to CMakeLists.txt")
         return True
 
-    if not confirm(f"Add component {comp_path} to {list_file} at end of file?"):
+    if not confirm(
+        f"Add component {comp_path} to {short_display_path} at end of file (yes/no)? "
+    ):
         return False
 
     lines.append(addition)
     with open(list_file, "w") as f:
         f.write("".join(lines))
     return True
 
@@ -129,62 +124,14 @@
     with suppress_stdout():
         try:
             build.cmake.cmake_refresh_cache(build.get_build_cache())
         except CMakeExecutionException:
             build.cmake.cmake_refresh_cache(build.get_build_cache(), True)
 
 
-def add_unit_tests(deployment, comp_path, platform, verbose):
-    # Creates unit tests and moves them into test/ut directory
-    os.chdir(str(comp_path))
-    if confirm("Would you like to generate unit tests?: "):
-        test_path = Path("test", "ut")
-        test_path.mkdir(parents=True, exist_ok=True)
-        target = Target.get_target("impl", {"ut"})
-        build = Build(target.build_type, deployment, verbose=verbose)
-        build.load(platform)
-        print("Generating unit tests...")
-        with suppress_stdout():
-            build.execute(target, context=comp_path, make_args={})
-        test_files = [
-            "Tester.hpp",
-            "Tester.cpp",
-            "TesterBase.hpp",
-            "TesterBase.cpp",
-            "GTestBase.hpp",
-            "GTestBase.cpp",
-            "TestMain.cpp",
-        ]
-        for file in test_files:
-            if os.path.isfile(file):
-                new_name = test_path / file
-                os.rename(file, str(new_name))
-
-        with open("CMakeLists.txt", "r") as f:
-            cmakeFile = f.read()
-
-        with open("CMakeLists.txt", "w") as f:
-            cmakeFile = cmakeFile + textwrap.dedent(
-                """\n
-                set(UT_SOURCE_FILES
-                  "${CMAKE_CURRENT_LIST_DIR}/test/ut/TestMain.cpp"
-                  "${CMAKE_CURRENT_LIST_DIR}/test/ut/Tester.cpp"
-                )
-
-                register_fprime_ut()"""
-            )
-            f.write(cmakeFile)
-
-        if replace_contents(
-            Path("test", "ut", "Tester.hpp"), "ComponentImpl.hpp", ".hpp", -1
-        ):
-            print("[INFO] Fixed hpp include in Tester.hpp")
-        print("[INFO] Unit tests were generated.")
-
-
 def add_port_to_cmake(list_file: Path, comp_path: Path):
     """Adds new port to CMakeLists.txt in port directory"""
     print(f"[INFO] Found CMakeLists.txt at '{list_file}'")
     with open(list_file, "r") as file_handle:
         lines = file_handle.readlines()
     index = 0
     while re.search("set\(\s*SOURCE_FILES", lines[index]) is None:
@@ -198,14 +145,49 @@
     addition = '    "${{CMAKE_CURRENT_LIST_DIR}}/{}"\n'.format(comp_path)
     lines.insert(index, addition)
     with open(list_file, "w") as file_handle:
         file_handle.write("".join(lines))
     return True
 
 
+def find_nearest_cmake_file(component_dir: Path, deployment: Path, proj_root: Path):
+    """Find the nearest CMake file, i.e. CMakeLists.txt or project.cmake
+
+    The "nearest" file is defined as the closest parent that is not the project root CMakeLists.txt.
+    If none is found, the same procedure is run from the deployment directory and includes the project
+    root this time. If nothing is found, None is returned.
+
+    In short the following in order of preference:
+     - Any Component Parent
+     - Any Deployment Parent
+     - project.cmake
+     - None
+
+    Args:
+        component_dir: directory of new component
+        deployment: deployment directory
+        proj_root: project root directory
+
+    Returns:
+        path to CMakeLists.txt or None
+    """
+    test_path = component_dir.parent
+    # First iterate from where we are, then from the deployment to find the nearest CMakeList.txt nearby
+    for test_path, end_path in [(test_path, proj_root), (deployment, proj_root.parent)]:
+        while proj_root is not None and test_path != proj_root.parent:
+            project_file = test_path / "project.cmake"
+            if project_file.is_file():
+                return project_file
+            cmake_list_file = test_path / "CMakeLists.txt"
+            if cmake_list_file.is_file():
+                return cmake_list_file
+            test_path = test_path.parent
+    return None
+
+
 def find_nearest_cmake_lists(component_dir: Path, deployment: Path, proj_root: Path):
     """Find the nearest CMakeLists.txt file
 
     The "nearest" file is defined as the closes parent that is not the "project root" that contains a CMakeLists.txt. If
     none is found, the same procedure is run from the deployment directory and includes the project root this time. If
     nothing is found, None is returned.
 
@@ -230,18 +212,18 @@
             cmake_list_file = test_path / "CMakeLists.txt"
             if cmake_list_file.is_file():
                 return cmake_list_file
             test_path = test_path.parent
     return None
 
 
-def new_component(deployment: Path, platform: str, verbose: bool, build: Build):
+def new_component(build: Build):
     """Uses cookiecutter for making new components"""
     try:
-        print("[WARNING] **** fprime-util new is prototype functionality ****")
+        deployment = build.deployment
         proj_root = build.get_settings("project_root", None)
 
         # Checks if component_cookiecutter is set in settings.ini file, else uses local component_cookiecutter template as default
         if (
             build.get_settings("component_cookiecutter", None) is not None
             and build.get_settings("component_cookiecutter", None) != "default"
         ):
@@ -249,55 +231,50 @@
             print(f"[INFO] Cookiecutter source: {source}")
         else:
             source = (
                 os.path.dirname(__file__)
                 + "/../cookiecutter_templates/cookiecutter-fprime-component"
             )
             print("[INFO] Cookiecutter source: using builtin")
-        print()
+
+        # Use deployment name as default namespace if a deployment was found
+        extra_context = {}
+        if not proj_root.samefile(deployment):
+            extra_context["component_namespace"] = deployment.name
+
         final_component_dir = Path(
-            cookiecutter(source, extra_context={"component_namespace": deployment.name})
+            cookiecutter(source, extra_context=extra_context)
         ).resolve()
+
         if proj_root is None:
             print(
                 f"[INFO] Created component directory without adding to build system nor generating implementation {final_component_dir}"
             )
             return 0
+
         # Attempt to register to CMakeLists.txt
         proj_root = Path(proj_root)
-        cmake_lists_file = find_nearest_cmake_lists(
-            final_component_dir, deployment, proj_root
-        )
-        if cmake_lists_file is None or not add_to_cmake(
-            cmake_lists_file, final_component_dir.relative_to(cmake_lists_file.parent)
+        cmake_file = find_nearest_cmake_file(final_component_dir, deployment, proj_root)
+        if cmake_file is None or not add_to_cmake(
+            cmake_file,
+            final_component_dir.relative_to(cmake_file.parent),
+            proj_root,
         ):
             print(
                 f"[INFO] Could not register {final_component_dir} with build system. Please add it and generate implementations manually."
             )
             return 0
-        regenerate(build)
         # Attempt implementation
-        if not run_impl(deployment, final_component_dir, platform, verbose):
+        if not run_impl(build, final_component_dir):
             print(
-                "[INFO] Could not generate implementations. Please do so manually.".format(
-                    final_component_dir
-                )
+                f"[INFO] Did not generate implementations for {final_component_dir}. Please do so manually."
             )
             return 0
-        cpp_file = glob.glob(str(Path(deployment.name, final_component_dir, "*.cpp")))[
-            0
-        ]
-        print("[INFO] Created new component and created initial implementations.")
-        if replace_contents(cpp_file, "ComponentImpl.hpp", ".hpp", -1):
-            print("[INFO] Fixed hpp include in cpp file.")
 
-        add_unit_tests(deployment, final_component_dir, platform, verbose)
-        print(
-            f'[INFO] Next run `fprime-util build{"" if platform is None else f" {platform}"}` in {final_component_dir}'
-        )
+        print("[INFO] Created new component and generated initial implementations.")
         return 0
     except OutputDirExistsException as out_directory_error:
         print(f"{out_directory_error}", file=sys.stderr)
     except CMakeExecutionException as exc:
         print(f"[ERROR] Failed to create component. {exc}", file=sys.stderr)
     except OSError as ose:
         print(f"[ERROR] {ose}")
@@ -392,17 +369,18 @@
     # Fill in blank values with defaults
     for key in values:
         if values[key] == "":
             values[key] = defaults[key]
     return values
 
 
-def new_port(deployment: Path, build: Build):
+def new_port(build: Build):
     """Uses cookiecutter for making new ports"""
     try:
+        deployment = build.deployment
         proj_root = build.get_settings("project_root", None)
         if proj_root is not None:
             proj_root = Path(proj_root)
             proj_root_found = True
         else:
             proj_root_found = False
 
@@ -477,7 +455,57 @@
     except OutputDirExistsException as out_directory_error:
         print(f"{out_directory_error}", file=sys.stderr)
     except CMakeExecutionException as exc:
         print(f"[ERROR] Failed to create port. {exc}", file=sys.stderr)
     except OSError as ose:
         print(f"[ERROR] {ose}")
     return 1
+
+
+def new_deployment(parsed_args):
+    """Creates a new deployment using cookiecutter"""
+    source = (
+        os.path.dirname(__file__)
+        + "/../cookiecutter_templates/cookiecutter-fprime-deployment"
+    )
+    print(f"[INFO] Cookiecutter: using builtin template for new deployment")
+    try:
+        gen_path = cookiecutter(source, overwrite_if_exists=parsed_args.overwrite)
+    except OutputDirExistsException as out_directory_error:
+        print(
+            f"{out_directory_error}. Use --overwrite to overwrite (will not delete non-generated files).",
+            file=sys.stderr,
+        )
+        return 1
+    print(f"[INFO] New deployment successfully created: {gen_path}")
+    return 0
+
+
+def new_project(parsed_args):
+    """Creates a new F' project"""
+
+    # Check if Git is installed and available - needed for cloning F' as submodule
+    if not shutil.which("git"):
+        print(
+            "[ERROR] Git is not installed or in PATH. Please install Git and try again.",
+            file=sys.stderr,
+        )
+        return 1
+
+    source = (
+        os.path.dirname(__file__)
+        + "/../cookiecutter_templates/cookiecutter-fprime-project"
+    )
+    try:
+        gen_path = cookiecutter(
+            source,
+            overwrite_if_exists=parsed_args.overwrite,
+            output_dir=parsed_args.path,
+        )
+    except OutputDirExistsException as out_directory_error:
+        print(
+            f"{out_directory_error}. Use --overwrite to overwrite (will not delete non-generated files).",
+            file=sys.stderr,
+        )
+        return 1
+    print(f"[INFO] New project successfully created: {gen_path}")
+    return 0
```

### Comparing `fprime-tools-3.1.2a3/src/fprime/fbuild/settings.py` & `fprime-tools-3.1.2a4/src/fprime/fbuild/settings.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/fbuild/target.py` & `fprime-tools-3.1.2a4/src/fprime/fbuild/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Contains the supporting definitions for build targets. These targets are used to run various parts of the build and may
 contain build system targets (e.g. CMake target invokers), and miscellaneous targets that perform other actions.
 
 @author lestarch
 """
 import functools
+import itertools
 from abc import ABC, abstractmethod
 from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Set, Tuple
 from .types import BuildType, NoSuchTargetException
 
 
@@ -52,18 +53,36 @@
             True if supported false otherwise
         """
         # Always supported by targets, unless specifically overridden
         return True
 
     @abstractmethod
     def execute(
-        self, builder: "Build", context: Path, args: Tuple[Dict[str, str], List[str]]
+        self,
+        builder: "Build",
+        context: Path,
+        args: Tuple[Dict[str, str], List[str], Dict[str, bool]],
     ):
         """Executes the given target"""
 
+    def option_args(self) -> List[Tuple[str, str]]:
+        """List of option arguments handled by this target
+
+        Option flags are switches that are not allowed arguments. The current design defaults the value to False unless
+        the switch is supplied. This function is expected to return a list of pairs of switch flag and description help
+        text. e.g.
+        [
+            (--turn-on, "Turns on a switch"),
+        ]
+
+        Returns:
+            list of tuples containing the paired flag and description
+        """
+        return []
+
     def allows_pass_args(self):
         """Target allows pass-through arguments"""
         return False
 
     def pass_handler(self):
         """Handler of pass-through args"""
         return None
@@ -230,14 +249,24 @@
         # Supported only if all steps supported
         return functools.reduce(
             lambda sum, target: sum and target.is_supported(builder, context),
             self.targets,
             True,
         )
 
+    def option_args(self):
+        """Returns the set of option arguments"""
+        return list(
+            set(
+                itertools.chain.from_iterable(
+                    [target.option_args() for target in self.targets]
+                )
+            )
+        )
+
     def allows_pass_args(self):
         """Pass args allowed if any child allows it"""
         return functools.reduce(
             lambda sum, target: sum or target.allows_pass_args(), self.targets, False
         )
 
     def pass_handler(self):
@@ -264,26 +293,28 @@
 
     def __init__(self, build_target, *args, **kwargs):
         """Constructor setting child targets"""
         super().__init__(*args, **kwargs)
         self.build_target = build_target
 
     def execute(
-        self, builder: "Build", context: Path, args: Tuple[Dict[str, str], List[str]]
+        self,
+        builder: "Build",
+        context: Path,
+        args: Tuple[Dict[str, str], List[str], Dict[str, bool]],
     ):
         """Execute a build target
 
         Executes a target within the build system. This will execute the target by calling into the build system.
         Context is supplied such that the system can match local targets to the global target list.
 
         Args:
             builder: builder to execute target with
-            target: target to run
             context: context path for local targets
-            make_args: make system arguments directly supplied
+            args: make system arguments directly supplied
         """
         # Global targets with build target "" must be mapped to "arg"
         build_target = (
             self.build_target
             if self.build_target != "" or self.scope == TargetScope.LOCAL
             else "all"
         )
@@ -335,14 +366,18 @@
             context: contextual path to check
 
         Return:
             True if supported false otherwise
         """
         return self.delegate.is_supported(builder, context)
 
+    def option_args(self):
+        """Delegate the arguments"""
+        return self.delegate.option_args()
+
     def allows_pass_args(self):
         """Pass args allowed if any child allows it"""
         return self.delegate.allows_pass_args()
 
     def pass_handler(self):
         """Pass handler from delegate"""
         return self.delegate.pass_handler()
```

### Comparing `fprime-tools-3.1.2a3/src/fprime/fbuild/target_definitions.py` & `fprime-tools-3.1.2a4/src/fprime/fbuild/target_definitions.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/fbuild/types.py` & `fprime-tools-3.1.2a4/src/fprime/fbuild/types.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/fpp/cli.py` & `fprime-tools-3.1.2a4/src/fprime/fpp/cli.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/fpp/common.py` & `fprime-tools-3.1.2a4/src/fprime/fpp/common.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/util/build_helper.py` & `fprime-tools-3.1.2a4/src/fprime/util/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,115 +1,215 @@
-"""
-fprime.util.build_helper.py
+""" fprime.util.cli: CLI handling
 
-This script is defined to help users run standard make processes using CMake. This will support migrants from the old
-make system, as well as enable more efficient practices when developing in the CMake system. The following functions
-are supported herein:
-
- - build: build the current directory/module/deployment
- - impl: make implementation templates
- - testimpl: make testing templates
- - build_ut: build the current UTs
- - check: run modules unit tests
+Defines main entrypoint for fprime-util and sets up parsers for general CLI targets.
 
 @author mstarch
 """
 import argparse
-import os
-import re
 import sys
+import re
+import os
+
 from pathlib import Path
+from typing import Dict, Callable
+
+from fprime.fbuild.target import Target
+from fprime.fbuild.cli import add_fbuild_parsers
+from fprime.fbuild.builder import GenerateException, UnableToDetectDeploymentException
 
-from fprime.fbuild.types import InvalidBuildCacheException
-from fprime.fbuild.target import Target, NoSuchTargetException
-from fprime.fbuild.builder import (
-    Build,
-    BuildType,
-    GenerateException,
-    UnableToDetectDeploymentException,
-)
-from .help_text import HelpText
-from .versioning import get_version, VersionException
-from fprime.fbuild.cli import add_fbuild_parsers, get_target
 from fprime.fpp.cli import add_fpp_parsers
-from fprime.util.cli import add_special_parsers
 
-CMAKE_REG = re.compile(r"-D([a-zA-Z0-9_]+)=(.*)")
+from fprime.util.help_text import HelpText
+from fprime.util.build_helper import load_build
+from fprime.util.commands import run_hash_to_file, run_info, run_new, run_code_format
 
-# Attempt to get pkg_resources from "setuptools"
-try:
-    import pkg_resources
-except ImportError:
-    pkg_resources = None
 
+def utility_entry(args):
+    """Entrypoint for fprime-util, main interface to F' utility"""
+    parsed, cmake_args, make_args, parser, runners = parse_args(args)
 
-class ArgValidationException(Exception):
-    """An exception used for argument validation"""
+    try:
+        if skip_build_loading(parsed):
+            build = None
+        else:
+            build = load_build(parsed)
 
+        # runners is a Dict[str, Callable] of {command_name: handler_functions} pairs
+        return runners[parsed.command](
+            build, parsed, cmake_args, make_args, getattr(parsed, "pass_through", [])
+        )
 
-def package_version_check(package: str, requirement_path: Path):
-    """Checks the version of the packages installed match the expected packages of the fprime aggregate package"""
-    expected_version = get_version(package, requirement_path).lstrip(
-        "v"
-    )  # Python version
-    try:
-        version = pkg_resources.get_distribution(package).version
-        if version != expected_version:
-            print(
-                f"[WARNING] {package} has unexpected version. Expected: {expected_version} found {version}"
-            )
-    except pkg_resources.DistributionNotFound:
-        print(f"[WARNING] {package} is not installed")
-
-
-def validate_tools_from_requirements(build: Build):
-    """Uses build settings to find requirements file and validate the correct versions installed"""
-    # Find prioritized order of requirements.txt, ensuring that each member exists
-    possibilities = [
-        build.settings.get("project_root", None),
-        build.settings.get("framework_path", None),
-    ]
-    possibilities = [
-        Path(possible) / "requirements.txt"
-        for possible in possibilities
-        if possible is not None
-    ]
-    possibilities = [possible for possible in possibilities if possible.exists()]
-    # Skip tools check, as not requirements.txt found
-    if not possibilities:
+    except GenerateException as genex:
         print(
-            f"[WARNING] Could not find 'requirements.txt' in: {possibilities}. Will not check tool versions."
+            f"[ERROR] {genex}. Partial build cache remains. Run purge to clean-up.",
+            file=sys.stderr,
         )
-        return
-    # Pre-roll import errors from pkg_resources
-    if pkg_resources is None:
-        print("[WARNING] Cannot import 'pkg_resources'. Will not check tool versions.")
-        return
-
-    # Now check each required tool for fprime
-    tools = ["fprime-fpp", "fprime-tools", "fprime-gds"]
-    for tool in tools:
-        for possible in possibilities:
-            try:
-                package_version_check(tool, possible)
-                break
-            except (OSError, VersionException) as exc:
-                message = f"[WARNING] {exc}"
-        else:
-            print(message)
+    except UnableToDetectDeploymentException:
+        print(f"[ERROR] Could not detect deployment directory for: {parsed.path}")
+    except Exception as exc:
+        print(f"[ERROR] {exc}", file=sys.stderr)
+    return 1
+
+
+def skip_build_loading(parsed):
+    """Determines if the build load step should be skipped. Commands that do not require a build object
+    should manually be added here by the developer."""
+    if parsed.command == "new" and parsed.new_deployment:
+        return True
+    if parsed.command == "new" and parsed.new_project:
+        return True
+    return False
+
+
+def add_special_parsers(
+    subparsers, common: argparse.ArgumentParser, help_text: "HelpText"
+) -> Dict[str, Callable]:
+    """Adds in CLI parsers for other commands
+
+    Args:
+        subparsers: subparsers used to create new CLI subparsers
+        common: common parent parser
+
+    Returns:
+        Dictionary associating special command name to callable used to process it
+    """
+    # Add a search for hash function
+    hash_parser = subparsers.add_parser(
+        "hash-to-file",
+        description=help_text.long("hash-to-file"),
+        help=help_text.short("hash-to-file"),
+        parents=[common],
+        add_help=False,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    hash_parser.add_argument(
+        "hash",
+        type=lambda x: int(x, 0),
+        help="Assert hash value to convert to filename",
+    )
+
+    # Add a search for hash function
+    subparsers.add_parser(
+        "info",
+        description=help_text.long("info"),
+        help=help_text.short("info"),
+        parents=[common],
+        add_help=False,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+
+    # New functionality
+    new_parser = subparsers.add_parser(
+        "new",
+        description=help_text.long("new"),
+        help=help_text.short("new"),
+        parents=[common],
+        add_help=False,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    new_parser.add_argument(
+        "--overwrite",
+        default=False,
+        action="store_true",
+        help="Generated files will overwrite existing ones",
+    )
+    new_exclusive = new_parser.add_argument_group(
+        "'new' targets"
+    ).add_mutually_exclusive_group()
+    new_exclusive.add_argument(
+        "--component",
+        default=False,
+        action="store_true",
+        dest="new_component",
+        help="Tells the new command to generate a component",
+    )
+    new_exclusive.add_argument(
+        "--port",
+        default=False,
+        action="store_true",
+        dest="new_port",
+        help="Tells the new command to generate a port",
+    )
+    new_exclusive.add_argument(
+        "--deployment",
+        default=False,
+        action="store_true",
+        dest="new_deployment",
+        help="Tells the new command to generate a deployment",
+    )
+    new_exclusive.add_argument(
+        "--project",
+        default=False,
+        action="store_true",
+        dest="new_project",
+        help="Tells the new command to generate a project",
+    )
+
+    # Code formatting with clang-format
+    format_parser = subparsers.add_parser(
+        "format",
+        help=help_text.short("format"),
+        description=help_text.long("format"),
+        parents=[common],
+        add_help=False,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        conflict_handler="resolve",
+    ).add_argument_group("format utility arguments")
+    format_parser.add_argument(
+        "-x", "--no-backup", action="store_true", help="Disable backups"
+    )
+    format_parser.add_argument(
+        "-q", "--quiet", action="store_true", help="Disable clang-format verbose mode"
+    )
+    format_parser.add_argument(
+        "--force",
+        action="store_true",
+        help="Force all listed files to be passed to clang-format (no file extension check)",
+    )
+    format_parser.add_argument(
+        "--allow-extension",
+        action="append",
+        default=[],
+        help="Add a file extension to the allowed set",
+    )
+    format_parser.add_argument(
+        "-f",
+        "--files",
+        nargs="*",
+        default=[],
+        type=Path,
+        help="List of files to format",
+    )
+    format_parser.add_argument(
+        "--stdin", action="store_true", help="Read stdin for list of files to format"
+    )
+    format_parser.add_argument(
+        "--pass-through",
+        nargs=argparse.REMAINDER,
+        default=[],
+        help="If specified, --pass-through must be the last argument. Remaining arguments passed to underlying executable",
+    )
+    return {
+        "hash-to-file": run_hash_to_file,
+        "info": run_info,
+        "new": run_new,
+        "format": run_code_format,
+    }
 
 
 def validate(parsed, unknown):
     """
     Validate rules to ensure that the args are properly consistent. This will also generate a set of validated arguments
     to pass to CMake. This allows these values to be created, defaulted, and validated in one place
     :param parsed: args to validate
     :param unknown: unknown arguments
     :return: cmake arguments to pass to CMake
     """
+    # regex pattern to detect -D<CMAKE_ARGUMENT>=<VALUE> arguments for CMake
+    CMAKE_REG = re.compile(r"-D([a-zA-Z0-9_]+)=(.*)")
     cmake_args = {}
     make_args = {}
     # Check platforms for existing toolchain, unless the default is specified.
     if not hasattr(parsed, "command") or parsed.command is None:
         raise ArgValidationException("'fprime-util' not supplied sub-command argument")
     if parsed.command == "generate":
         d_args = {
@@ -210,64 +310,9 @@
     except ArgValidationException as exc:
         print(f"[ERROR] {exc}", end="\n\n")
         parsers.get(parsed.command, (parser,))[0].print_usage()
         sys.exit(1)
     return parsed, cmake_args, make_args, parser, runners
 
 
-def utility_entry(args):
-    """Main interface to F prime utility"""
-    parsed, cmake_args, make_args, parser, runners = parse_args(args)
-
-    try:
-        try:
-            target = get_target(parsed)
-            build_type = target.build_type
-        except NoSuchTargetException:
-            build_type = (
-                BuildType.BUILD_TESTING if parsed.ut else BuildType.BUILD_NORMAL
-            )
-
-        deployment = (
-            Path(parsed.deploy)
-            if parsed.deploy is not None
-            else Build.find_nearest_deployment(Path.cwd())  # Deployments look in CWD
-        )
-        build = Build(build_type, deployment, verbose=parsed.verbose)
-
-        # All commands need to load the build cache to setup the basic information for the build with the exception of
-        # generate, which is run before the creation of the build cache and thus must invent the cache instead. This
-        # call will ensure the build is in a ready state before attempting to check tool versions and run the command.
-        #
-        # Some commands, like purge and info, run on sets of directories and will attempt to load those sets later.
-        # However, the base directory must be setup here. Errors in this load are ignored to allow the command to find
-        # build caches related to that set.
-        if parsed.command == "generate":
-            build.invent(parsed.platform, build_dir=parsed.build_cache)
-        else:
-            does_not_need_cache_directory = parsed.command in [
-                "purge",
-                "info",
-                "format",
-            ]
-            build.load(
-                parsed.platform,
-                parsed.build_cache,
-                skip_validation=does_not_need_cache_directory,
-            )
-        validate_tools_from_requirements(build)
-        status = runners[parsed.command](
-            build, parsed, cmake_args, make_args, getattr(parsed, "pass_through", [])
-        )
-    except GenerateException as genex:
-        print(
-            f"[ERROR] {genex}. Partial build cache remains. Run purge to clean-up.",
-            file=sys.stderr,
-        )
-        return genex.exit_code
-    except UnableToDetectDeploymentException:
-        print(f"[ERROR] Could not detect deployment directory for: {parsed.path}")
-        return 1
-    except Exception as exc:
-        print(f"[ERROR] {exc}", file=sys.stderr)
-        return 1
-    return 0 if status is None else status
+class ArgValidationException(Exception):
+    """An exception used for argument validation"""
```

### Comparing `fprime-tools-3.1.2a3/src/fprime/util/code_formatter.py` & `fprime-tools-3.1.2a4/src/fprime/util/code_formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 class ClangFormatter(ExecutableAction):
     """Class encapsulating the clang-format logic for fprime-util"""
 
     def __init__(self, executable: str, style_file: "Path", options: Dict):
         super().__init__(TargetScope.LOCAL)
         self.executable = executable
         self.style_file = style_file
-        self.backup = options["backup"]
-        self.verbose = options["verbose"]
-        self.validate_extensions = options["validate_extensions"]
+        self.backup = options.get("backup", True)
+        self.verbose = options.get("verbose", False)
+        self.validate_extensions = options.get("validate_extensions", True)
         self.allowed_extensions = ALLOWED_EXTENSIONS.copy()
         self._files_to_format: List[Path] = []
 
     def is_supported(self) -> bool:
         return bool(shutil.which(self.executable))
 
     def allow_extension(self, file_ext: str) -> None:
@@ -93,17 +93,17 @@
         """
         for filepath in self._files_to_format:
             # It is unsafe to write to file while reading from it
             # Better to read in memory, close the file, then re-open to write out from memory
             with open(filepath, "r") as file:
                 content = file.read()
             # Replace the strings in the file content
-            content = re.sub("PROTECTED:", PROTECTED_PRE_PATTERN, content)
-            content = re.sub("PRIVATE:", PRIVATE_PRE_PATTERN, content)
-            content = re.sub("STATIC:", STATIC_PRE_PATTERN, content)
+            content = re.sub("PROTECTED[\s]*:", PROTECTED_PRE_PATTERN, content)
+            content = re.sub("PRIVATE[\s]*:", PRIVATE_PRE_PATTERN, content)
+            content = re.sub("STATIC[\s]*:", STATIC_PRE_PATTERN, content)
             # Write the file out to the same location, seemingly in-place
             with open(filepath, "w") as file:
                 file.write(content)
 
     def _postprocess_files(self) -> None:
         """Postprocess a file to restore the access specifier macros."""
         for filepath in self._files_to_format:
```

### Comparing `fprime-tools-3.1.2a3/src/fprime/util/help_text.py` & `fprime-tools-3.1.2a4/src/fprime/util/help_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -273,18 +273,33 @@
   cd Ref
   {EXECUTABLE} hash-to-file 0xABCD1234
 
   -- Map Ref Hash to File for RaspberryPI Platform --
   cd Ref
   {EXECUTABLE} hash-to-file raspberrypi 0xABCD1234
 """,
-    "new": f"""{EXECUTABLE} new ({VERSION}):       -- WARNING: prototype code -- Creates a new fprime object
+    "new": f"""{EXECUTABLE} new ({VERSION}):       -- Creates a new fprime object
 
-WARNING: prototype code. Not recommended for inexperienced users. '{EXECUTABLE} new' runs a wizard to create new ports
-and components in fprime. The code has not been updated to use FPP models. Please check back later.
+'{EXECUTABLE} new' runs a wizard to create new objects in fprime (component, deployment, project).
+
+Usage:
+  -- New Project --
+  Generate a new F' project. This will create a Git repository and add F' as a submodule, optionally creating a new
+  virtual environment. Defaults to current directory, but --path can be used to point to a different location. 
+  Using --overwrite will overwrite only the files that are generated by the new project.
+  -- New Deployment --
+  Generate a new F' deployment within a F' project. The new deployment command is expected to be ran at the root of
+  the project and will create a new deployment in the current directory. Using --overwrite will overwrite only the
+  files that are generated by the new deployment.
+  -- New Component --
+  Generate a new F' component within a F' project. This command prompts for what type of component and what it should
+  include. At the end of the generation, the user can chose to automatically add the component to the build system and
+  run the implementation generator.
+  -- New Port --
+  WARNING: prototype code generating XML only. Not recommended for inexperienced users. Please check back later.
 """,
     "format": f"""{EXECUTABLE} format ({VERSION}): Formats C/C++ files using clang-format
 
 '{EXECUTABLE} format' uses 'clang-format' to format C/C++ files. It uses the style specified in the .clang-format file
 found at the root of the F' framework used by the project (i.e. the 'framework_path' specified in settings.ini).
 Files are specified through stdin or by using the '--files [<path/to/file>]*' flag. When reading from stdin, file paths
 should be separated by whitespace characters.
```

### Comparing `fprime-tools-3.1.2a3/src/fprime/util/string_util.py` & `fprime-tools-3.1.2a4/src/fprime/util/string_util.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime/util/versioning.py` & `fprime-tools-3.1.2a4/src/fprime/util/versioning.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/src/fprime_tools.egg-info/PKG-INFO` & `fprime-tools-3.1.2a4/src/fprime_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime-tools
-Version: 3.1.2a3
+Version: 3.1.2a4
 Summary: F Prime Flight Software core data types
 Home-page: https://github.com/nasa/fprime
 Author: Michael Starch
 Author-email: Michael.D.Starch@jpl.nasa.gov
 License: Apache 2.0 License
 Project-URL: Issue Tracker, https://github.com/nasa/fprime/issues
 Keywords: fprime,embedded,nasa
```

### Comparing `fprime-tools-3.1.2a3/test/fprime/common/models/serialize/test_types.py` & `fprime-tools-3.1.2a4/test/fprime/common/models/serialize/test_types.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/test/fprime/common/models/serialize/time_type_unit_test.py` & `fprime-tools-3.1.2a4/test/fprime/common/models/serialize/time_type_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/test/fprime/fbuild/test_build.py` & `fprime-tools-3.1.2a4/test/fprime/fbuild/test_build.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.1.2a3/test/fprime/fbuild/test_settings.py` & `fprime-tools-3.1.2a4/test/fprime/fbuild/test_settings.py`

 * *Files identical despite different names*

