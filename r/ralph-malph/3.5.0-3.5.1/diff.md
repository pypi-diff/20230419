# Comparing `tmp/ralph-malph-3.5.0.tar.gz` & `tmp/ralph-malph-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralph-malph-3.5.0.tar", last modified: Thu Mar  9 11:13:11 2023, max compression
+gzip compressed data, was "ralph-malph-3.5.1.tar", last modified: Wed Apr 19 07:45:08 2023, max compression
```

## Comparing `ralph-malph-3.5.0.tar` & `ralph-malph-3.5.1.tar`

### file list

```diff
@@ -1,135 +1,145 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.409255 ralph-malph-3.5.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6303 2023-03-09 11:13:11.409255 ralph-malph-3.5.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5151 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2722 2023-03-09 11:13:11.409255 ralph-malph-3.5.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.389256 ralph-malph-3.5.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.393256 ralph-malph-3.5.0/src/ralph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/__main__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.393256 ralph-malph-3.5.0/src/ralph/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      840 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5321 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/api/auth.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/api/forwarding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1573 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/api/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.393256 ralph-malph-3.5.0/src/ralph/api/routers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/api/routers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/api/routers/health.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13641 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/api/routers/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.393256 ralph-malph-3.5.0/src/ralph/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.397256 ralph-malph-3.5.0/src/ralph/backends/database/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/database/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3688 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/database/base.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    12281 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/database/clickhouse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8536 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/database/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/database/mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/mixins.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.397256 ralph-malph-3.5.0/src/ralph/backends/storage/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/storage/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/storage/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/storage/fs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4987 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/storage/ldp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5171 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/storage/s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/storage/swift.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.397256 ralph-malph-3.5.0/src/ralph/backends/stream/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/stream/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/stream/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/backends/stream/ws.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19679 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10266 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.397256 ralph-malph-3.5.0/src/ralph/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/converter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.397256 ralph-malph-3.5.0/src/ralph/models/edx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1603 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/browser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.397256 ralph-malph-3.5.0/src/ralph/models/edx/converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/converters/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2860 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/navigational.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7162 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/enrollment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/enrollment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/enrollment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/enrollment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/enrollment/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/enrollment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/enrollment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/navigational/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/navigational/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/navigational/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/navigational/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/navigational/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/navigational/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/problem_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/problem_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/problem_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/problem_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/problem_interaction/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/textbook_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/textbook_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/textbook_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/textbook_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/textbook_interaction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.401255 ralph-malph-3.5.0/src/ralph/models/edx/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/video/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.405255 ralph-malph-3.5.0/src/ralph/models/edx/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/video/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/edx/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/selector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.405255 ralph-malph-3.5.0/src/ralph/models/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      356 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3007 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1820 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.405255 ralph-malph-3.5.0/src/ralph/models/xapi/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3802 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/fields/actors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/fields/attachments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/fields/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2380 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1941 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/fields/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2326 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/fields/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3941 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/fields/unnested_objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1554 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/fields/verbs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.405255 ralph-malph-3.5.0/src/ralph/models/xapi/navigation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/navigation/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.405255 ralph-malph-3.5.0/src/ralph/models/xapi/navigation/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/navigation/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1201 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/navigation/fields/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1304 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/navigation/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.405255 ralph-malph-3.5.0/src/ralph/models/xapi/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/video/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/video/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.409255 ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8241 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5335 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/verbs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7490 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/models/xapi/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2920 2023-03-09 11:13:10.000000 ralph-malph-3.5.0/src/ralph/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 11:13:11.409255 ralph-malph-3.5.0/src/ralph_malph.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6303 2023-03-09 11:13:11.000000 ralph-malph-3.5.0/src/ralph_malph.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3912 2023-03-09 11:13:11.000000 ralph-malph-3.5.0/src/ralph_malph.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-09 11:13:11.000000 ralph-malph-3.5.0/src/ralph_malph.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-03-09 11:13:11.000000 ralph-malph-3.5.0/src/ralph_malph.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2023-03-09 11:13:11.000000 ralph-malph-3.5.0/src/ralph_malph.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-03-09 11:13:11.000000 ralph-malph-3.5.0/src/ralph_malph.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-09 11:13:11.000000 ralph-malph-3.5.0/src/ralph_malph.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.131809 ralph-malph-3.5.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6299 2023-04-19 07:45:08.131809 ralph-malph-3.5.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5147 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2726 2023-04-19 07:45:08.131809 ralph-malph-3.5.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.099809 ralph-malph-3.5.1/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.099809 ralph-malph-3.5.1/src/ralph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.099809 ralph-malph-3.5.1/src/ralph/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      840 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5321 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/auth.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/forwarding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1573 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/api/routers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/routers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/routers/health.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13641 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/routers/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/backends/database/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3688 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/base.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    12909 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/clickhouse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8536 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/mixins.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/backends/storage/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/fs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4995 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/ldp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5171 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/swift.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/backends/stream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/stream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/stream/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/stream/ws.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19679 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10266 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/converter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/edx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1603 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/browser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/edx/converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2860 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/navigational.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7162 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/navigational/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/navigational/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/navigational/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/navigational/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/navigational/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/navigational/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/video/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/video/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/video/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/video/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/video/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/selector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.123809 ralph-malph-3.5.1/src/ralph/models/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      356 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3007 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1820 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.123809 ralph-malph-3.5.1/src/ralph/models/xapi/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3802 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/actors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/attachments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2380 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1941 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2326 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3941 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/unnested_objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1554 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/verbs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.123809 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.123809 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1201 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/fields/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1304 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.127809 ralph-malph-3.5.1/src/ralph/models/xapi/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.127809 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8241 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5335 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/verbs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7490 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.127809 ralph-malph-3.5.1/src/ralph_malph.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6299 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4104 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.131809 ralph-malph-3.5.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3521 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_auth.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9427 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_cli_usage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6621 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_dependencies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4904 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_utils.py
```

### Comparing `ralph-malph-3.5.0/LICENSE.md` & `ralph-malph-3.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/PKG-INFO` & `ralph-malph-3.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.5.0
+Version: 3.5.1
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
@@ -83,15 +83,15 @@
 # This is an alias for:
 $ docker compose ps
 ```
 
 You may now start the LRS server using:
 
 ```
-$ make run-lrs
+$ make run
 ```
 
 The server should be up and running at
 [http://localhost:8100](http://localhost:8100). You can check its status using
 the hearbeat probe:
 
 ```
```

### Comparing `ralph-malph-3.5.0/README.md` & `ralph-malph-3.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 # This is an alias for:
 $ docker compose ps
 ```
 
 You may now start the LRS server using:
 
 ```
-$ make run-lrs
+$ make run
 ```
 
 The server should be up and running at
 [http://localhost:8100](http://localhost:8100). You can check its status using
 the hearbeat probe:
 
 ```
```

### Comparing `ralph-malph-3.5.0/setup.cfg` & `ralph-malph-3.5.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ralph-malph
-version = 3.5.0
+version = 3.5.1
 description = The ultimate toolbox for your learning analytics
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://openfun.github.io/ralph/
 license = MIT
@@ -55,52 +55,52 @@
 	websockets>=10.3
 cli = 
 	bcrypt>=4.0.0
 	click>=8.1.0
 	click-option-group>=0.5.0
 	sentry-sdk[fastapi]>=1.9.0
 dev = 
-	bandit==1.7.4
-	black==23.1.0
+	bandit==1.7.5
+	black==23.3.0
 	factory-boy==3.2.1
-	Faker==17.6.0
+	Faker==18.4.0
 	flake8==6.0.0
-	hypothesis==6.68.2
-	ipdb==0.13.11
-	ipython==8.11.0
+	hypothesis==6.72.0
+	ipdb==0.13.13
+	ipython==8.12.0
 	isort==5.12.0
 	logging-gelf==0.0.26
 	memory-profiler==0.61.0
 	mkdocs==1.4.2
 	mkdocs-click==0.8.0
-	mkdocs-material==9.1.1
-	mkdocstrings[python-legacy]==0.20.0
-	moto==4.1.4
+	mkdocs-material==9.1.6
+	mkdocstrings[python-legacy]==0.21.2
+	moto==4.1.7
 	pydocstyle==6.3.0
-	pyfakefs==5.1.0
-	pylint==2.16.3
-	pytest==7.2.2
-	pytest-asyncio==0.20.3
+	pyfakefs==5.2.2
+	pylint==2.17.2
+	pytest==7.3.1
+	pytest-asyncio==0.21.0
 	pytest-cov==4.0.0
 ci = 
 	twine==4.0.2
 lrs = 
 	bcrypt==4.0.1
-	fastapi==0.92.0
+	fastapi==0.95.1
 	h11>=0.11.0
-	httpx==0.23.3
-	sentry_sdk==1.16.0
-	uvicorn[standard]==0.20.0
+	httpx==0.24.0
+	sentry_sdk==1.19.1
+	uvicorn[standard]==0.21.1
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
-	ralph = ralph.__main__:cli
+	ralph = ralph.__main__:cli.cli
 
 [wheel]
 universal = 1
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
```

### Comparing `ralph-malph-3.5.0/src/ralph/__main__.py` & `ralph-malph-3.5.1/src/ralph/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,8 +16,9 @@
         dsn=settings.SENTRY_DSN,
         traces_sample_rate=settings.SENTRY_CLI_TRACES_SAMPLE_RATE,
         release=__version__,
         environment=settings.EXECUTION_ENVIRONMENT,
         max_breadcrumbs=50,
     )
 
-cli.cli()
+if __name__ == "__main__":
+    cli.cli()
```

### Comparing `ralph-malph-3.5.0/src/ralph/api/__init__.py` & `ralph-malph-3.5.1/src/ralph/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/api/auth.py` & `ralph-malph-3.5.1/src/ralph/api/auth.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/api/forwarding.py` & `ralph-malph-3.5.1/src/ralph/api/forwarding.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/api/models.py` & `ralph-malph-3.5.1/src/ralph/api/models.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/api/routers/health.py` & `ralph-malph-3.5.1/src/ralph/api/routers/health.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/api/routers/statements.py` & `ralph-malph-3.5.1/src/ralph/api/routers/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/backends/database/base.py` & `ralph-malph-3.5.1/src/ralph/backends/database/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/backends/database/clickhouse.py` & `ralph-malph-3.5.1/src/ralph/backends/database/clickhouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 class ClickHouseQuery(BaseQuery):
     """ClickHouse query model."""
 
     where_clause: Optional[str]
     return_fields: Optional[List[str]]
 
 
-class ClickHouseDatabase(BaseDatabase):
+class ClickHouseDatabase(BaseDatabase):  # pylint: disable=too-many-instance-attributes
     """ClickHouse database backend."""
 
     name = "clickhouse"
     query_model = ClickHouseQuery
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
@@ -52,15 +52,15 @@
         port: int = clickhouse_settings.PORT,
         database: str = clickhouse_settings.DATABASE,
         event_table_name: str = clickhouse_settings.EVENT_TABLE_NAME,
         username: str = clickhouse_settings.USERNAME,
         password: str = clickhouse_settings.PASSWORD,
         client_options: dict = clickhouse_settings.CLIENT_OPTIONS,
     ):
-        """Instantiates the ClickHouse client.
+        """Instantiates the ClickHouse configuration.
 
         Args:
             host (str): ClickHouse server host to connect to.
             port (int): ClickHouse server port to connect to.
             database (str): ClickHouse database to connect to.
             event_table_name (str): Table where events live.
             username (str): ClickHouse username to connect as (optional).
@@ -79,23 +79,37 @@
 
         self.host = host
         self.port = port
         self.database = database
         self.event_table_name = event_table_name
         self.username = username
         self.password = password
+        self.client_options = client_options
+        self._client = None
 
-        self.client = clickhouse_connect.get_client(
-            host=self.host,
-            port=self.port,
-            database=self.database,
-            username=self.username,
-            password=self.password,
-            settings=client_options,
-        )
+    @property
+    def client(self):
+        """Creates a ClickHouse client if it doesn't exist.
+
+        We do this here so that we don't interrupt initialization in the case
+        where ClickHouse is not running when Ralph starts up, which will cause
+        Ralph to hang. This client is HTTP, so not actually stateful. Ralph
+        should be able to gracefully deal with ClickHouse outages at all other
+        times.
+        """
+        if not self._client:
+            self._client = clickhouse_connect.get_client(
+                host=self.host,
+                port=self.port,
+                database=self.database,
+                username=self.username,
+                password=self.password,
+                settings=self.client_options,
+            )
+        return self._client
 
     def status(self) -> DatabaseStatus:
         """Checks ClickHouse connection status."""
         try:
             self.client.query("SELECT 1")
         except ClickHouseError:
             return DatabaseStatus.AWAY
@@ -103,15 +117,15 @@
         return DatabaseStatus.OK
 
     @enforce_query_checks
     def get(self, query: ClickHouseQuery = None, chunk_size: int = 500):
         """Gets table rows and yields them."""
         fields = ",".join(query.return_fields) if query.return_fields else "event"
 
-        sql = f"SELECT {fields} FROM {self.event_table_name}"
+        sql = f"SELECT {fields} FROM {self.event_table_name}"  # nosec
 
         if query.where_clause:
             sql += f"  WHERE {query.where_clause}"
 
         result = self.client.query(sql).named_results()
 
         for statement in result:
@@ -220,15 +234,14 @@
 
         logger.debug("Inserted a total of %s documents with success", rows_inserted)
 
         return rows_inserted
 
     def query_statements_by_ids(self, ids: List[str]) -> List:
         """Returns the list of matching statement IDs from the database."""
-        ids = [f"'{id}'" for id in ids]
 
         def chunk_id_list(chunk_size=10000):
             for i in range(0, len(ids), chunk_size):
                 yield ids[i : i + chunk_size]
 
         sql = """
                 SELECT event_id
```

### Comparing `ralph-malph-3.5.0/src/ralph/backends/database/es.py` & `ralph-malph-3.5.1/src/ralph/backends/database/es.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/backends/database/mongo.py` & `ralph-malph-3.5.1/src/ralph/backends/database/mongo.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/backends/mixins.py` & `ralph-malph-3.5.1/src/ralph/backends/mixins.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/backends/storage/base.py` & `ralph-malph-3.5.1/src/ralph/backends/storage/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/backends/storage/fs.py` & `ralph-malph-3.5.1/src/ralph/backends/storage/fs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/backends/storage/ldp.py` & `ralph-malph-3.5.1/src/ralph/backends/storage/ldp.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         """Reads the `name` archive file and yields its content."""
         logger.debug("Getting archive: %s", name)
 
         # Get detailed information about the archive to fetch
         details = self._details(name)
 
         # Stream response (archive content)
-        with requests.get(  # pylint: disable=missing-timeout
+        with requests.get(  # pylint: disable=missing-timeout # nosec
             self.url(name), stream=True
         ) as result:
             result.raise_for_status()
             for chunk in result.iter_content(chunk_size=chunk_size):
                 yield chunk
 
         # Archive is supposed to have been fully fetched, add a new entry to
```

### Comparing `ralph-malph-3.5.0/src/ralph/backends/storage/s3.py` & `ralph-malph-3.5.1/src/ralph/backends/storage/s3.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/backends/storage/swift.py` & `ralph-malph-3.5.1/src/ralph/backends/storage/swift.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/backends/stream/ws.py` & `ralph-malph-3.5.1/src/ralph/backends/stream/ws.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/cli.py` & `ralph-malph-3.5.1/src/ralph/cli.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/conf.py` & `ralph-malph-3.5.1/src/ralph/conf.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/exceptions.py` & `ralph-malph-3.5.1/src/ralph/exceptions.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/filters.py` & `ralph-malph-3.5.1/src/ralph/filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/converter.py` & `ralph-malph-3.5.1/src/ralph/models/converter.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/__init__.py` & `ralph-malph-3.5.1/src/ralph/models/edx/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/base.py` & `ralph-malph-3.5.1/src/ralph/models/edx/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/browser.py` & `ralph-malph-3.5.1/src/ralph/models/edx/browser.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/base.py` & `ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/navigational.py` & `ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/navigational.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/server.py` & `ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/converters/xapi/video.py` & `ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/enrollment/fields/contexts.py` & `ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/enrollment/fields/events.py` & `ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/enrollment/statements.py` & `ralph-malph-3.5.1/src/ralph/models/edx/enrollment/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/navigational/fields/events.py` & `ralph-malph-3.5.1/src/ralph/models/edx/navigational/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/navigational/statements.py` & `ralph-malph-3.5.1/src/ralph/models/edx/navigational/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/problem_interaction/fields/events.py` & `ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/problem_interaction/statements.py` & `ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/server.py` & `ralph-malph-3.5.1/src/ralph/models/edx/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/textbook_interaction/fields/events.py` & `ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/textbook_interaction/statements.py` & `ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/video/fields/events.py` & `ralph-malph-3.5.1/src/ralph/models/edx/video/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/edx/video/statements.py` & `ralph-malph-3.5.1/src/ralph/models/edx/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/selector.py` & `ralph-malph-3.5.1/src/ralph/models/selector.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/validator.py` & `ralph-malph-3.5.1/src/ralph/models/validator.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/base.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/config.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/config.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/constants.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/constants.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/fields/actors.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/fields/actors.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/fields/attachments.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/fields/attachments.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/fields/common.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/fields/common.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/fields/contexts.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/fields/objects.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/fields/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/fields/results.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/fields/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/fields/unnested_objects.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/fields/unnested_objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/fields/verbs.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/fields/verbs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/navigation/fields/objects.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/navigation/fields/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/navigation/statements.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/navigation/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/video/constants.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/video/constants.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/contexts.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/objects.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/results.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/video/fields/verbs.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/verbs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/models/xapi/video/statements.py` & `ralph-malph-3.5.1/src/ralph/models/xapi/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/parsers.py` & `ralph-malph-3.5.1/src/ralph/parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.0/src/ralph/utils.py` & `ralph-malph-3.5.1/src/ralph/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,29 +65,30 @@
     return datetime.datetime.now(tz=datetime.timezone.utc).isoformat()
 
 
 def get_dict_value_from_path(dict_: dict, path: List[str]):
     """Gets a nested dictionary value.
 
     Args:
-        dict_ (dict): #FIXME I miss the info for this argument.
+        dict_ (dict): dictionnary of values to which the reduction is
+            applied
         path (List): array of keys representing the path to the value
     """
     if path is None:
         return None
     try:
         return reduce(operator.getitem, path, dict_)
     except (KeyError, TypeError):
         return None
 
 
 def set_dict_value_from_path(dict_: dict, path: List[str], value: any):
     """Sets a nested dictionary value.
 
     Args:
-        dict_ (dict): #FIXME I miss the info for this argument.
+        dict_ (dict): dictionnary where the given value is set
         path (List): array of keys representing the path to the value
-        value: #FIXME I miss the info for this argument.
+        value: value to be set
     """
     for key in path[:-1]:
         dict_ = dict_.setdefault(key, {})
     dict_[path[-1]] = value
```

### Comparing `ralph-malph-3.5.0/src/ralph_malph.egg-info/PKG-INFO` & `ralph-malph-3.5.1/src/ralph_malph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.5.0
+Version: 3.5.1
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
@@ -83,15 +83,15 @@
 # This is an alias for:
 $ docker compose ps
 ```
 
 You may now start the LRS server using:
 
 ```
-$ make run-lrs
+$ make run
 ```
 
 The server should be up and running at
 [http://localhost:8100](http://localhost:8100). You can check its status using
 the hearbeat probe:
 
 ```
```

### Comparing `ralph-malph-3.5.0/src/ralph_malph.egg-info/SOURCES.txt` & `ralph-malph-3.5.1/src/ralph_malph.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -97,8 +97,17 @@
 src/ralph/models/xapi/video/fields/verbs.py
 src/ralph_malph.egg-info/PKG-INFO
 src/ralph_malph.egg-info/SOURCES.txt
 src/ralph_malph.egg-info/dependency_links.txt
 src/ralph_malph.egg-info/entry_points.txt
 src/ralph_malph.egg-info/requires.txt
 src/ralph_malph.egg-info/top_level.txt
-src/ralph_malph.egg-info/zip-safe
+src/ralph_malph.egg-info/zip-safe
+tests/test_auth.py
+tests/test_cli.py
+tests/test_cli_usage.py
+tests/test_conf.py
+tests/test_dependencies.py
+tests/test_filters.py
+tests/test_logger.py
+tests/test_parsers.py
+tests/test_utils.py
```

### Comparing `ralph-malph-3.5.0/src/ralph_malph.egg-info/requires.txt` & `ralph-malph-3.5.1/src/ralph_malph.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -34,37 +34,37 @@
 [cli]
 bcrypt>=4.0.0
 click>=8.1.0
 click-option-group>=0.5.0
 sentry-sdk[fastapi]>=1.9.0
 
 [dev]
-bandit==1.7.4
-black==23.1.0
+bandit==1.7.5
+black==23.3.0
 factory-boy==3.2.1
-Faker==17.6.0
+Faker==18.4.0
 flake8==6.0.0
-hypothesis==6.68.2
-ipdb==0.13.11
-ipython==8.11.0
+hypothesis==6.72.0
+ipdb==0.13.13
+ipython==8.12.0
 isort==5.12.0
 logging-gelf==0.0.26
 memory-profiler==0.61.0
 mkdocs==1.4.2
 mkdocs-click==0.8.0
-mkdocs-material==9.1.1
-mkdocstrings[python-legacy]==0.20.0
-moto==4.1.4
+mkdocs-material==9.1.6
+mkdocstrings[python-legacy]==0.21.2
+moto==4.1.7
 pydocstyle==6.3.0
-pyfakefs==5.1.0
-pylint==2.16.3
-pytest==7.2.2
-pytest-asyncio==0.20.3
+pyfakefs==5.2.2
+pylint==2.17.2
+pytest==7.3.1
+pytest-asyncio==0.21.0
 pytest-cov==4.0.0
 
 [lrs]
 bcrypt==4.0.1
-fastapi==0.92.0
+fastapi==0.95.1
 h11>=0.11.0
-httpx==0.23.3
-sentry_sdk==1.16.0
-uvicorn[standard]==0.20.0
+httpx==0.24.0
+sentry_sdk==1.19.1
+uvicorn[standard]==0.21.1
```

