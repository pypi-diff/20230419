# Comparing `tmp/spdlog-2.0.2.tar.gz` & `tmp/spdlog-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spdlog-2.0.2.tar", last modified: Tue Oct 27 19:51:55 2020, max compression
+gzip compressed data, was "dist/spdlog-2.0.4.tar", last modified: Fri Feb 12 18:08:31 2021, max compression
```

## Comparing `spdlog-2.0.2.tar` & `spdlog-2.0.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.149722 spdlog-2.0.2/
--rw-rw-r--   0 geri      (1000) geri      (1000)     1067 2020-10-15 16:09:55.000000 spdlog-2.0.2/LICENSE
--rw-rw-r--   0 geri      (1000) geri      (1000)       83 2020-10-27 19:50:21.000000 spdlog-2.0.2/MANIFEST.in
--rw-rw-r--   0 geri      (1000) geri      (1000)      408 2020-10-27 19:51:55.149722 spdlog-2.0.2/PKG-INFO
--rw-rw-r--   0 geri      (1000) geri      (1000)     2550 2020-10-15 16:09:55.000000 spdlog-2.0.2/README.md
--rw-rw-r--   0 geri      (1000) geri      (1000)       63 2020-10-27 19:51:55.149722 spdlog-2.0.2/setup.cfg
--rw-rw-r--   0 geri      (1000) geri      (1000)     2244 2020-10-27 19:51:32.000000 spdlog-2.0.2/setup.py
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.117723 spdlog-2.0.2/spdlog/
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.117723 spdlog-2.0.2/spdlog/include/
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.125723 spdlog-2.0.2/spdlog/include/spdlog/
--rw-rw-r--   0 geri      (1000) geri      (1000)     3082 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/async.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2323 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/async_logger.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     5923 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/common.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.137722 spdlog-2.0.2/spdlog/include/spdlog/details/
--rw-rw-r--   0 geri      (1000) geri      (1000)     2989 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/async_logger_impl.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1531 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/circular_q.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1195 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/console_globals.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     3892 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/file_helper.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     3444 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/fmt_helper.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1269 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/log_msg.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    11805 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/logger_impl.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     3437 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/mpmc_blocking_q.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      683 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/null_mutex.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    10605 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/os.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    39208 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/pattern_formatter.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1844 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/periodic_worker.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     8086 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/registry.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     6420 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/details/thread_pool.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.137722 spdlog-2.0.2/spdlog/include/spdlog/fmt/
--rw-rw-r--   0 geri      (1000) geri      (1000)     4360 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bin_to_hex.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.141722 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/
--rw-rw-r--   0 geri      (1000) geri      (1000)     1310 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/LICENSE.rst
--rw-rw-r--   0 geri      (1000) geri      (1000)    13284 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/chrono.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    21968 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/color.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    47459 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/core.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    32309 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/format-inl.h
--rw-rw-r--   0 geri      (1000) geri      (1000)   109393 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/format.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2782 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/locale.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4771 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/ostream.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     8820 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/posix.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    25813 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/printf.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     9069 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/ranges.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4311 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/time.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      534 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/fmt.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      371 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/fmt/ostr.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      436 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/formatter.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     6150 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/logger.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.149722 spdlog-2.0.2/spdlog/include/spdlog/sinks/
--rw-rw-r--   0 geri      (1000) geri      (1000)     3292 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/android_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     5177 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/ansicolor_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1738 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/base_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1735 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/basic_file_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4189 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/daily_file_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2233 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/dist_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1034 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/msvc_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1175 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/null_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1276 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/ostream_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4961 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/rotating_file_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1416 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1659 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/stdout_color_sinks.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2867 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/stdout_sinks.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2963 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/syslog_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4844 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/sinks/wincolor_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    10861 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/spdlog.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     6442 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/tweakme.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      305 2020-10-15 16:14:23.000000 spdlog-2.0.2/spdlog/include/spdlog/version.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.121723 spdlog-2.0.2/spdlog.egg-info/
--rw-rw-r--   0 geri      (1000) geri      (1000)      408 2020-10-27 19:51:55.000000 spdlog-2.0.2/spdlog.egg-info/PKG-INFO
--rw-rw-r--   0 geri      (1000) geri      (1000)     2389 2020-10-27 19:51:55.000000 spdlog-2.0.2/spdlog.egg-info/SOURCES.txt
--rw-rw-r--   0 geri      (1000) geri      (1000)        1 2020-10-27 19:51:55.000000 spdlog-2.0.2/spdlog.egg-info/dependency_links.txt
--rw-rw-r--   0 geri      (1000) geri      (1000)        1 2020-10-15 16:12:47.000000 spdlog-2.0.2/spdlog.egg-info/not-zip-safe
--rw-rw-r--   0 geri      (1000) geri      (1000)       14 2020-10-27 19:51:55.000000 spdlog-2.0.2/spdlog.egg-info/requires.txt
--rw-rw-r--   0 geri      (1000) geri      (1000)        7 2020-10-27 19:51:55.000000 spdlog-2.0.2/spdlog.egg-info/top_level.txt
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2020-10-27 19:51:55.149722 spdlog-2.0.2/src/
--rw-rw-r--   0 geri      (1000) geri      (1000)    30811 2020-10-15 16:09:55.000000 spdlog-2.0.2/src/pyspdlog.cpp
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.441282 spdlog-2.0.4/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1067 2020-10-15 16:09:55.000000 spdlog-2.0.4/LICENSE
+-rw-rw-r--   0 geri      (1000) geri      (1000)       83 2020-10-27 19:50:21.000000 spdlog-2.0.4/MANIFEST.in
+-rw-rw-r--   0 geri      (1000) geri      (1000)      408 2021-02-12 18:08:31.441282 spdlog-2.0.4/PKG-INFO
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2478 2021-02-12 17:14:51.000000 spdlog-2.0.4/README.md
+-rw-rw-r--   0 geri      (1000) geri      (1000)       63 2021-02-12 18:08:31.441282 spdlog-2.0.4/setup.cfg
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2397 2021-02-12 18:07:10.000000 spdlog-2.0.4/setup.py
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.429282 spdlog-2.0.4/spdlog/
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.429282 spdlog-2.0.4/spdlog/include/
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.433282 spdlog-2.0.4/spdlog/include/spdlog/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3082 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/async.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2323 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/async_logger.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     5923 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/common.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.433282 spdlog-2.0.4/spdlog/include/spdlog/details/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2989 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/async_logger_impl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1531 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/circular_q.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1195 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/console_globals.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3892 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/file_helper.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3444 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/fmt_helper.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1269 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/log_msg.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    11805 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/logger_impl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3437 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/mpmc_blocking_q.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      683 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/null_mutex.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    10605 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/os.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    39208 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/pattern_formatter.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1844 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/periodic_worker.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     8086 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/registry.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     6420 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/thread_pool.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.433282 spdlog-2.0.4/spdlog/include/spdlog/fmt/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4360 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bin_to_hex.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.437282 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1310 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/LICENSE.rst
+-rw-rw-r--   0 geri      (1000) geri      (1000)    13284 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/chrono.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    21968 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/color.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    47459 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/core.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    32309 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/format-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)   109393 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/format.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2782 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/locale.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4771 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/ostream.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     8820 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/posix.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    25813 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/printf.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     9069 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/ranges.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4311 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/time.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      534 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/fmt.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      371 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/ostr.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      436 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/formatter.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     6150 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/logger.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.441282 spdlog-2.0.4/spdlog/include/spdlog/sinks/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3292 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/android_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     5177 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/ansicolor_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1738 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/base_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1735 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/basic_file_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4189 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/daily_file_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2233 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/dist_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1034 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/msvc_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1175 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/null_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1276 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/ostream_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4961 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/rotating_file_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1416 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1659 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/stdout_color_sinks.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2867 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/stdout_sinks.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2963 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/syslog_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4844 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/wincolor_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    10861 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/spdlog.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     6442 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/tweakme.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      305 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/version.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.429282 spdlog-2.0.4/spdlog.egg-info/
+-rw-rw-r--   0 geri      (1000) geri      (1000)      408 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/PKG-INFO
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2389 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 geri      (1000) geri      (1000)        1 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 geri      (1000) geri      (1000)        1 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/not-zip-safe
+-rw-rw-r--   0 geri      (1000) geri      (1000)       14 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/requires.txt
+-rw-rw-r--   0 geri      (1000) geri      (1000)        7 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/top_level.txt
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.441282 spdlog-2.0.4/src/
+-rw-rw-r--   0 geri      (1000) geri      (1000)    30845 2021-02-12 17:14:51.000000 spdlog-2.0.4/src/pyspdlog.cpp
```

### Comparing `spdlog-2.0.2/LICENSE` & `spdlog-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/README.md` & `spdlog-2.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [![Build Status](https://travis-ci.org/bodgergely/spdlog-python.svg?branch=master)](https://travis-ci.org/bodgergely/spdlog-python)
 
 spdlog-python
 =============
 
 python wrapper around the fast C++ logger called [spdlog](https://github.com/gabime/spdlog)
 
-**Current version: tag - v2.0.0**
 
 Introduction
 ============
 
 Python wrapper (pybind11) around the C++ spdlog logging library. 
 
 Why choose [spdlog](https://github.com/gabime/spdlog)?
@@ -34,21 +33,19 @@
 |  1000             |  2.4            |  1.16           |   26.8                                    |
 |  5000             |  6.2            |  2.31           |   31.7                                    |
 |  20000            |  15.3           |  7.51           |   48.0                                    |
 
 Installation
 ============
 
-1) `pip install pybind11` - required
-
-2) `pip install spdlog` will get a distribution from pypi.org
+1) `pip install spdlog` will get a distribution from pypi.org
 
 or
 
-1) from github: 
+2) from github: 
 
 `pip install pybind11` - if missing
 
 ```bash
 git clone https://github.com/bodgergely/spdlog-python.git
 cd spdlog-python
 git submodule update --init --recursive
```

### Comparing `spdlog-2.0.2/setup.py` & `spdlog-2.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import os
 import platform
 import sys
 
 import sysconfig
-from distutils.command.install_headers import install_headers
 from setuptools import setup
 from setuptools.extension import Extension
+from distutils.command.install_headers import install_headers
+
+def is_posix():
+    return platform.os.name == "posix"
 
+def link_libs():
+    libs = []
+    if is_posix():
+        libs.append("stdc++")
+    return libs
 
 class get_pybind_include(object):
     def __init__(self, user=False):
         self.user = user
 
     def __str__(self):
         import pybind11
@@ -36,15 +44,15 @@
             install_dir = os.path.join(self.install_dir, submod_dir)
             self.mkpath(install_dir)
             (out, _) = self.copy_file(header, install_dir)
             self.outfiles.append(out)
 
 setup(
     name='spdlog',
-    version='2.0.2',
+    version='2.0.4',
     author='Gergely Bod',
     author_email='bodgergely@hotmail.com',
     description='python wrapper around C++ spdlog logging library (https://github.com/bodgergely/spdlog-python)',
     license='MIT',
     long_description='python wrapper (https://github.com/bodgergely/spdlog-python) around C++ spdlog (http://github.com/gabime/spdlog.git) logging library.',
     setup_requires=['pytest-runner'],
     install_requires=['pybind11>=2.2'],
@@ -54,15 +62,15 @@
             'spdlog',
             ['src/pyspdlog.cpp'],
             include_dirs=[
                 'spdlog/include/',
                 get_pybind_include(),
                 get_pybind_include(user=True)
             ],
-            libraries=['stdc++'],
+            libraries=link_libs(),
             extra_compile_args=["-std=c++11", "-v"],
             language='c++11'
         )
     ],
     headers=include_dir_files('spdlog/include/spdlog'),
     cmdclass={'install_headers': install_headers_subdir},
     zip_safe=False,
```

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/async.h` & `spdlog-2.0.4/spdlog/include/spdlog/async.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/async_logger.h` & `spdlog-2.0.4/spdlog/include/spdlog/async_logger.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/common.h` & `spdlog-2.0.4/spdlog/include/spdlog/common.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/async_logger_impl.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/async_logger_impl.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/circular_q.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/circular_q.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/console_globals.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/console_globals.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/file_helper.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/file_helper.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/fmt_helper.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/fmt_helper.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/log_msg.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/log_msg.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/logger_impl.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/logger_impl.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/mpmc_blocking_q.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/mpmc_blocking_q.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/null_mutex.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/null_mutex.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/os.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/os.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/pattern_formatter.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/pattern_formatter.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/periodic_worker.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/periodic_worker.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/registry.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/registry.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/details/thread_pool.h` & `spdlog-2.0.4/spdlog/include/spdlog/details/thread_pool.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bin_to_hex.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bin_to_hex.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/LICENSE.rst` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/chrono.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/chrono.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/color.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/color.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/core.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/core.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/format-inl.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/format-inl.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/format.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/format.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/locale.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/locale.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/ostream.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/ostream.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/posix.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/posix.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/printf.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/printf.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/ranges.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/ranges.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/bundled/time.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/time.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/fmt/fmt.h` & `spdlog-2.0.4/spdlog/include/spdlog/fmt/fmt.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/logger.h` & `spdlog-2.0.4/spdlog/include/spdlog/logger.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/android_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/android_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/ansicolor_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/ansicolor_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/base_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/base_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/basic_file_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/basic_file_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/daily_file_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/daily_file_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/dist_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/dist_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/msvc_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/msvc_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/null_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/null_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/ostream_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/ostream_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/rotating_file_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/rotating_file_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/stdout_color_sinks.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/stdout_color_sinks.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/stdout_sinks.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/stdout_sinks.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/syslog_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/syslog_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/sinks/wincolor_sink.h` & `spdlog-2.0.4/spdlog/include/spdlog/sinks/wincolor_sink.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/spdlog.h` & `spdlog-2.0.4/spdlog/include/spdlog/spdlog.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog/include/spdlog/tweakme.h` & `spdlog-2.0.4/spdlog/include/spdlog/tweakme.h`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/spdlog.egg-info/SOURCES.txt` & `spdlog-2.0.4/spdlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.2/src/pyspdlog.cpp` & `spdlog-2.0.4/src/pyspdlog.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 #include <spdlog/async_logger.h>
 #include <spdlog/sinks/basic_file_sink.h>
 #include <spdlog/sinks/daily_file_sink.h>
 #include <spdlog/sinks/null_sink.h>
 #include <spdlog/sinks/rotating_file_sink.h>
 #include <spdlog/sinks/stdout_color_sinks.h>
 #include <spdlog/sinks/stdout_sinks.h>
+#ifndef _WIN32
 #include <spdlog/sinks/syslog_sink.h>
+#endif
 
 #include <iostream>
 #include <memory>
 #include <mutex>
 #include <stdexcept>
 #include <string>
 #include <unordered_map>
@@ -363,18 +365,18 @@
     const std::string _name;
     bool _async;
     std::shared_ptr<spdlog::logger> _logger{ nullptr };
 };
 
 class ConsoleLogger : public Logger {
 public:
-    ConsoleLogger(const std::string& logger_name, bool multithreaded, bool stdout, bool colored, bool async_mode = g_async_mode_on)
+    ConsoleLogger(const std::string& logger_name, bool multithreaded, bool standard_out, bool colored, bool async_mode = g_async_mode_on)
         : Logger(logger_name, async_mode)
     {
-        if (stdout) {
+        if (standard_out) {
             if (multithreaded) {
                 if (colored) {
                     if (async_mode) {
                         if (g_async_overflow_policy == spdlog::async_overflow_policy::overrun_oldest) {
                             _logger = spd::stdout_color_mt<async_factory_nb>(logger_name);
                         } else {
                             _logger = spd::stdout_color_mt<spdlog::async_factory>(logger_name);
```

