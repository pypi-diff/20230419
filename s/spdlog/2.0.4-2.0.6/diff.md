# Comparing `tmp/spdlog-2.0.4.tar.gz` & `tmp/spdlog-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spdlog-2.0.4.tar", last modified: Fri Feb 12 18:08:31 2021, max compression
+gzip compressed data, was "spdlog-2.0.6.tar", last modified: Wed Apr 19 16:17:23 2023, max compression
```

## Comparing `spdlog-2.0.4.tar` & `spdlog-2.0.6.tar`

### file list

```diff
@@ -1,75 +1,124 @@
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.441282 spdlog-2.0.4/
--rw-rw-r--   0 geri      (1000) geri      (1000)     1067 2020-10-15 16:09:55.000000 spdlog-2.0.4/LICENSE
--rw-rw-r--   0 geri      (1000) geri      (1000)       83 2020-10-27 19:50:21.000000 spdlog-2.0.4/MANIFEST.in
--rw-rw-r--   0 geri      (1000) geri      (1000)      408 2021-02-12 18:08:31.441282 spdlog-2.0.4/PKG-INFO
--rw-rw-r--   0 geri      (1000) geri      (1000)     2478 2021-02-12 17:14:51.000000 spdlog-2.0.4/README.md
--rw-rw-r--   0 geri      (1000) geri      (1000)       63 2021-02-12 18:08:31.441282 spdlog-2.0.4/setup.cfg
--rw-rw-r--   0 geri      (1000) geri      (1000)     2397 2021-02-12 18:07:10.000000 spdlog-2.0.4/setup.py
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.429282 spdlog-2.0.4/spdlog/
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.429282 spdlog-2.0.4/spdlog/include/
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.433282 spdlog-2.0.4/spdlog/include/spdlog/
--rw-rw-r--   0 geri      (1000) geri      (1000)     3082 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/async.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2323 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/async_logger.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     5923 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/common.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.433282 spdlog-2.0.4/spdlog/include/spdlog/details/
--rw-rw-r--   0 geri      (1000) geri      (1000)     2989 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/async_logger_impl.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1531 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/circular_q.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1195 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/console_globals.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     3892 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/file_helper.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     3444 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/fmt_helper.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1269 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/log_msg.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    11805 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/logger_impl.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     3437 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/mpmc_blocking_q.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      683 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/null_mutex.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    10605 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/os.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    39208 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/pattern_formatter.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1844 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/periodic_worker.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     8086 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/registry.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     6420 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/details/thread_pool.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.433282 spdlog-2.0.4/spdlog/include/spdlog/fmt/
--rw-rw-r--   0 geri      (1000) geri      (1000)     4360 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bin_to_hex.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.437282 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/
--rw-rw-r--   0 geri      (1000) geri      (1000)     1310 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/LICENSE.rst
--rw-rw-r--   0 geri      (1000) geri      (1000)    13284 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/chrono.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    21968 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/color.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    47459 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/core.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    32309 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/format-inl.h
--rw-rw-r--   0 geri      (1000) geri      (1000)   109393 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/format.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2782 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/locale.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4771 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/ostream.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     8820 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/posix.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    25813 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/printf.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     9069 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/ranges.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4311 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/time.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      534 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/fmt.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      371 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/fmt/ostr.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      436 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/formatter.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     6150 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/logger.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.441282 spdlog-2.0.4/spdlog/include/spdlog/sinks/
--rw-rw-r--   0 geri      (1000) geri      (1000)     3292 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/android_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     5177 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/ansicolor_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1738 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/base_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1735 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/basic_file_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4189 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/daily_file_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2233 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/dist_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1034 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/msvc_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1175 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/null_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1276 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/ostream_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4961 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/rotating_file_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1416 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     1659 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/stdout_color_sinks.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2867 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/stdout_sinks.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     2963 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/syslog_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     4844 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/sinks/wincolor_sink.h
--rw-rw-r--   0 geri      (1000) geri      (1000)    10861 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/spdlog.h
--rw-rw-r--   0 geri      (1000) geri      (1000)     6442 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/tweakme.h
--rw-rw-r--   0 geri      (1000) geri      (1000)      305 2020-10-15 16:14:23.000000 spdlog-2.0.4/spdlog/include/spdlog/version.h
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.429282 spdlog-2.0.4/spdlog.egg-info/
--rw-rw-r--   0 geri      (1000) geri      (1000)      408 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/PKG-INFO
--rw-rw-r--   0 geri      (1000) geri      (1000)     2389 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/SOURCES.txt
--rw-rw-r--   0 geri      (1000) geri      (1000)        1 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/dependency_links.txt
--rw-rw-r--   0 geri      (1000) geri      (1000)        1 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/not-zip-safe
--rw-rw-r--   0 geri      (1000) geri      (1000)       14 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/requires.txt
--rw-rw-r--   0 geri      (1000) geri      (1000)        7 2021-02-12 18:08:31.000000 spdlog-2.0.4/spdlog.egg-info/top_level.txt
-drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2021-02-12 18:08:31.441282 spdlog-2.0.4/src/
--rw-rw-r--   0 geri      (1000) geri      (1000)    30845 2021-02-12 17:14:51.000000 spdlog-2.0.4/src/pyspdlog.cpp
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.239024 spdlog-2.0.6/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1067 2023-04-19 15:44:54.000000 spdlog-2.0.6/LICENSE
+-rw-rw-r--   0 geri      (1000) geri      (1000)       83 2023-04-19 15:44:54.000000 spdlog-2.0.6/MANIFEST.in
+-rw-rw-r--   0 geri      (1000) geri      (1000)      419 2023-04-19 16:17:23.239024 spdlog-2.0.6/PKG-INFO
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2516 2023-04-19 16:02:39.000000 spdlog-2.0.6/README.md
+-rw-rw-r--   0 geri      (1000) geri      (1000)       63 2023-04-19 16:17:23.239024 spdlog-2.0.6/setup.cfg
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2633 2023-04-19 16:15:02.000000 spdlog-2.0.6/setup.py
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.219020 spdlog-2.0.6/spdlog/
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.219020 spdlog-2.0.6/spdlog/include/
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.223020 spdlog-2.0.6/spdlog/include/spdlog/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3587 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/async.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2494 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/async_logger-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2276 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/async_logger.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.227021 spdlog-2.0.6/spdlog/include/spdlog/cfg/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1229 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/cfg/argv.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      988 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/cfg/env.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3174 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/cfg/helpers-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      714 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/cfg/helpers.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2050 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/common-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    11823 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/common.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.231022 spdlog-2.0.6/spdlog/include/spdlog/details/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1884 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/backtracer-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1139 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/backtracer.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3436 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/circular_q.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      609 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/console_globals.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4582 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/file_helper-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1739 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/file_helper.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4567 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/fmt_helper.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1104 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/log_msg-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1154 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/log_msg.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1656 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/log_msg_buffer-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      933 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/log_msg_buffer.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3645 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/mpmc_blocking_q.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1026 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/null_mutex.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    16728 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/os-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3818 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/os.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1234 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/periodic_worker-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1133 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/periodic_worker.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     8670 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/registry-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3652 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/registry.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      754 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/synchronous_factory.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4329 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/tcp_client-windows.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3911 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/tcp_client.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3535 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/thread_pool-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3360 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/thread_pool.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3108 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/udp_client-windows.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2264 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/udp_client.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      187 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/details/windows_include.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.231022 spdlog-2.0.6/spdlog/include/spdlog/fmt/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     7245 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bin_to_hex.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.235023 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     7518 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/args.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    67575 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/chrono.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    24610 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/color.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    21753 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/compile.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)   107187 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/core.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1408 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/fmt.license.rst
+-rw-rw-r--   0 geri      (1000) geri      (1000)   104940 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/format-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)   113399 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/format.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      100 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/locale.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    15566 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/os.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4378 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/ostream.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    20707 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/printf.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    29679 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/ranges.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     9241 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/xchar.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      523 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/chrono.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      531 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/compile.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      898 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/fmt.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      526 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/ostr.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      523 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/ranges.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      520 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fmt/xchar.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      462 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/formatter.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      304 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/fwd.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     7036 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/logger-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    15311 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/logger.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    43341 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/pattern_formatter-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3560 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/pattern_formatter.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.239024 spdlog-2.0.6/spdlog/include/spdlog/sinks/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3436 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/android_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4594 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/ansicolor_sink-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3954 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/ansicolor_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1778 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/base_sink-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1565 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/base_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1102 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/basic_file_sink-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1834 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/basic_file_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    10231 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/daily_file_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2410 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/dist_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3014 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/dup_filter_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     6343 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/hourly_file_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3289 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/mongo_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1240 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/msvc_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1229 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/null_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1250 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/ostream_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3382 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/qt_sinks.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2195 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/ringbuffer_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4733 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/rotating_file_sink-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2648 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/rotating_file_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      725 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/sink-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      891 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1214 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/stdout_color_sinks-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1626 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/stdout_color_sinks.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4364 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/stdout_sinks-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2419 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/stdout_sinks.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3727 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/syslog_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4146 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/systemd_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2147 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/tcp_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1820 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/udp_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     8832 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/win_eventlog_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     6315 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/wincolor_sink-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2711 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/sinks/wincolor_sink.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     3098 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/spdlog-inl.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)    10918 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/spdlog.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1708 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/stopwatch.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)     6124 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/tweakme.h
+-rw-rw-r--   0 geri      (1000) geri      (1000)      331 2023-04-19 16:02:49.000000 spdlog-2.0.6/spdlog/include/spdlog/version.h
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.223020 spdlog-2.0.6/spdlog.egg-info/
+-rw-rw-r--   0 geri      (1000) geri      (1000)      419 2023-04-19 16:17:23.000000 spdlog-2.0.6/spdlog.egg-info/PKG-INFO
+-rw-rw-r--   0 geri      (1000) geri      (1000)     4432 2023-04-19 16:17:23.000000 spdlog-2.0.6/spdlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 geri      (1000) geri      (1000)        1 2023-04-19 16:17:23.000000 spdlog-2.0.6/spdlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 geri      (1000) geri      (1000)        1 2023-04-19 16:15:24.000000 spdlog-2.0.6/spdlog.egg-info/not-zip-safe
+-rw-rw-r--   0 geri      (1000) geri      (1000)       14 2023-04-19 16:17:23.000000 spdlog-2.0.6/spdlog.egg-info/requires.txt
+-rw-rw-r--   0 geri      (1000) geri      (1000)        7 2023-04-19 16:17:23.000000 spdlog-2.0.6/spdlog.egg-info/top_level.txt
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 16:17:23.239024 spdlog-2.0.6/src/
+-rw-rw-r--   0 geri      (1000) geri      (1000)    32096 2023-04-19 16:02:39.000000 spdlog-2.0.6/src/pyspdlog.cpp
```

### Comparing `spdlog-2.0.4/LICENSE` & `spdlog-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.4/README.md` & `spdlog-2.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-[![Build Status](https://travis-ci.org/bodgergely/spdlog-python.svg?branch=master)](https://travis-ci.org/bodgergely/spdlog-python)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/bodgergely/spdlog-python/ci.yaml?branch=master)](https://github.com/bodgergely/spdlog-python/actions)
 
 spdlog-python
 =============
 
 python wrapper around the fast C++ logger called [spdlog](https://github.com/gabime/spdlog)
 
 
 Introduction
 ============
 
-Python wrapper (pybind11) around the C++ spdlog logging library. 
+Python wrapper (pybind11) around the C++ spdlog logging library.
 
 Why choose [spdlog](https://github.com/gabime/spdlog)?
 
 https://kjellkod.wordpress.com/2015/06/30/the-worlds-fastest-logger-vs-g3log/
 
 Try running [tests/spdlog_vs_logging.py](https://github.com/bodgergely/spdlog-python/blob/master/tests/test_spdlog.py) and see what results you get on your system.
 
@@ -37,15 +37,15 @@
 Installation
 ============
 
 1) `pip install spdlog` will get a distribution from pypi.org
 
 or
 
-2) from github: 
+2) from github:
 
 `pip install pybind11` - if missing
 
 ```bash
 git clone https://github.com/bodgergely/spdlog-python.git
 cd spdlog-python
 git submodule update --init --recursive
@@ -65,8 +65,7 @@
 ```
 
 To run the speed test:
 
 ```bash
 python ./tests/spdlog_vs_logging.py
 ```
-
```

### Comparing `spdlog-2.0.4/setup.py` & `spdlog-2.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,14 +20,27 @@
     def __init__(self, user=False):
         self.user = user
 
     def __str__(self):
         import pybind11
         return pybind11.get_include(self.user)
 
+def get_include_dirs():
+    include_dirs=[
+        'spdlog/include/',
+        get_pybind_include(),
+        get_pybind_include(user=True),
+    ]
+
+    conda_prefix = os.environ.get('CONDA_PREFIX')
+    if conda_prefix is not None:
+        include_dirs.append(os.path.join(conda_prefix, "include"))
+    
+    return include_dirs
+
 
 def include_dir_files(folder):
     """Find all C++ header files in folder"""
     from os import walk
     files = []
     for (dirpath, _, filenames) in walk(folder):
         for fn in filenames:
@@ -44,32 +57,28 @@
             install_dir = os.path.join(self.install_dir, submod_dir)
             self.mkpath(install_dir)
             (out, _) = self.copy_file(header, install_dir)
             self.outfiles.append(out)
 
 setup(
     name='spdlog',
-    version='2.0.4',
+    version='2.0.6',
     author='Gergely Bod',
     author_email='bodgergely@hotmail.com',
     description='python wrapper around C++ spdlog logging library (https://github.com/bodgergely/spdlog-python)',
     license='MIT',
     long_description='python wrapper (https://github.com/bodgergely/spdlog-python) around C++ spdlog (http://github.com/gabime/spdlog.git) logging library.',
-    setup_requires=['pytest-runner'],
+    setup_requires=['pybind11>=2.2', 'wheel', 'pytest-runner'],
     install_requires=['pybind11>=2.2'],
     tests_require=['pytest'],
     ext_modules=[
         Extension(
             'spdlog',
             ['src/pyspdlog.cpp'],
-            include_dirs=[
-                'spdlog/include/',
-                get_pybind_include(),
-                get_pybind_include(user=True)
-            ],
+            include_dirs=get_include_dirs(),
             libraries=link_libs(),
             extra_compile_args=["-std=c++11", "-v"],
             language='c++11'
         )
     ],
     headers=include_dir_files('spdlog/include/spdlog'),
     cmdclass={'install_headers': install_headers_subdir},
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/async.h` & `spdlog-2.0.6/spdlog/include/spdlog/async.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-
-//
-// Copyright(c) 2018 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
 //
 // Async logging using global thread pool
 // All loggers created here share same global thread pool.
-// Each log message is pushed to a queue along withe a shared pointer to the
+// Each log message is pushed to a queue along with a shared pointer to the
 // logger.
 // If a logger deleted while having pending messages in the queue, it's actual
 // destruction will defer
 // until all its messages are processed by the thread pool.
 // This is because each message in the queue holds a shared_ptr to the
 // originating logger.
 
-#include "spdlog/async_logger.h"
-#include "spdlog/details/registry.h"
-#include "spdlog/details/thread_pool.h"
+#include <spdlog/async_logger.h>
+#include <spdlog/details/registry.h>
+#include <spdlog/details/thread_pool.h>
 
 #include <memory>
 #include <mutex>
+#include <functional>
 
 namespace spdlog {
 
 namespace details {
 static const size_t default_async_q_size = 8192;
 }
 
@@ -38,19 +36,21 @@
 {
     template<typename Sink, typename... SinkArgs>
     static std::shared_ptr<async_logger> create(std::string logger_name, SinkArgs &&... args)
     {
         auto &registry_inst = details::registry::instance();
 
         // create global thread pool if not already exists..
-        std::lock_guard<std::recursive_mutex> tp_lock(registry_inst.tp_mutex());
+
+        auto &mutex = registry_inst.tp_mutex();
+        std::lock_guard<std::recursive_mutex> tp_lock(mutex);
         auto tp = registry_inst.get_tp();
         if (tp == nullptr)
         {
-            tp = std::make_shared<details::thread_pool>(details::default_async_q_size, 1);
+            tp = std::make_shared<details::thread_pool>(details::default_async_q_size, 1U);
             registry_inst.set_tp(tp);
         }
 
         auto sink = std::make_shared<Sink>(std::forward<SinkArgs>(args)...);
         auto new_logger = std::make_shared<async_logger>(std::move(logger_name), std::move(sink), std::move(tp), OverflowPolicy);
         registry_inst.initialize_logger(new_logger);
         return new_logger;
@@ -69,19 +69,31 @@
 template<typename Sink, typename... SinkArgs>
 inline std::shared_ptr<spdlog::logger> create_async_nb(std::string logger_name, SinkArgs &&... sink_args)
 {
     return async_factory_nonblock::create<Sink>(std::move(logger_name), std::forward<SinkArgs>(sink_args)...);
 }
 
 // set global thread pool.
-inline void init_thread_pool(size_t q_size, size_t thread_count)
+inline void init_thread_pool(
+    size_t q_size, size_t thread_count, std::function<void()> on_thread_start, std::function<void()> on_thread_stop)
 {
-    auto tp = std::make_shared<details::thread_pool>(q_size, thread_count);
+    auto tp = std::make_shared<details::thread_pool>(q_size, thread_count, on_thread_start, on_thread_stop);
     details::registry::instance().set_tp(std::move(tp));
 }
 
+inline void init_thread_pool(size_t q_size, size_t thread_count, std::function<void()> on_thread_start)
+{
+    init_thread_pool(q_size, thread_count, on_thread_start, [] {});
+}
+
+inline void init_thread_pool(size_t q_size, size_t thread_count)
+{
+    init_thread_pool(
+        q_size, thread_count, [] {}, [] {});
+}
+
 // get the global thread pool.
 inline std::shared_ptr<spdlog::details::thread_pool> thread_pool()
 {
     return details::registry::instance().get_tp();
 }
 } // namespace spdlog
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/async_logger.h` & `spdlog-2.0.6/spdlog/include/spdlog/async_logger.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,24 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-// Very fast asynchronous logger (millions of logs per second on an average
-// desktop)
-// Uses pre allocated lockfree queue for maximum throughput even under large
-// number of threads.
+// Fast asynchronous logger.
+// Uses pre allocated queue.
 // Creates a single back thread to pop messages from the queue and log them.
 //
 // Upon each log write the logger:
 //    1. Checks if its log level is enough to log the message
 //    2. Push a new copy of the message to a queue (or block the caller until
 //    space is available in the queue)
-//    3. will throw spdlog_ex upon log exceptions
 // Upon destruction, logs all remaining messages in the queue before
 // destructing..
 
-#include "spdlog/common.h"
-#include "spdlog/logger.h"
-
-#include <chrono>
-#include <memory>
-#include <string>
+#include <spdlog/logger.h>
 
 namespace spdlog {
 
 // Async overflow policy - block by default.
 enum class async_overflow_policy
 {
     block,         // Block until message can be enqueued
@@ -36,38 +26,43 @@
                    // add new item.
 };
 
 namespace details {
 class thread_pool;
 }
 
-class async_logger final : public std::enable_shared_from_this<async_logger>, public logger
+class SPDLOG_API async_logger final : public std::enable_shared_from_this<async_logger>, public logger
 {
     friend class details::thread_pool;
 
 public:
     template<typename It>
     async_logger(std::string logger_name, It begin, It end, std::weak_ptr<details::thread_pool> tp,
-        async_overflow_policy overflow_policy = async_overflow_policy::block);
+        async_overflow_policy overflow_policy = async_overflow_policy::block)
+        : logger(std::move(logger_name), begin, end)
+        , thread_pool_(std::move(tp))
+        , overflow_policy_(overflow_policy)
+    {}
 
     async_logger(std::string logger_name, sinks_init_list sinks_list, std::weak_ptr<details::thread_pool> tp,
         async_overflow_policy overflow_policy = async_overflow_policy::block);
 
     async_logger(std::string logger_name, sink_ptr single_sink, std::weak_ptr<details::thread_pool> tp,
         async_overflow_policy overflow_policy = async_overflow_policy::block);
 
     std::shared_ptr<logger> clone(std::string new_name) override;
 
 protected:
-    void sink_it_(details::log_msg &msg) override;
+    void sink_it_(const details::log_msg &msg) override;
     void flush_() override;
-
-    void backend_log_(const details::log_msg &incoming_log_msg);
+    void backend_sink_it_(const details::log_msg &incoming_log_msg);
     void backend_flush_();
 
 private:
     std::weak_ptr<details::thread_pool> thread_pool_;
     async_overflow_policy overflow_policy_;
 };
 } // namespace spdlog
 
-#include "details/async_logger_impl.h"
+#ifdef SPDLOG_HEADER_ONLY
+#    include "async_logger-inl.h"
+#endif
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/details/async_logger_impl.h` & `spdlog-2.0.6/spdlog/include/spdlog/async_logger-inl.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,110 +1,92 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-// async logger implementation
-// uses a thread pool to perform the actual logging
+#ifndef SPDLOG_HEADER_ONLY
+#    include <spdlog/async_logger.h>
+#endif
 
-#include "spdlog/details/thread_pool.h"
+#include <spdlog/sinks/sink.h>
+#include <spdlog/details/thread_pool.h>
 
-#include <chrono>
 #include <memory>
 #include <string>
 
-template<typename It>
-inline spdlog::async_logger::async_logger(
-    std::string logger_name, It begin, It end, std::weak_ptr<details::thread_pool> tp, async_overflow_policy overflow_policy)
-    : logger(std::move(logger_name), begin, end)
-    , thread_pool_(std::move(tp))
-    , overflow_policy_(overflow_policy)
-{
-}
-
-inline spdlog::async_logger::async_logger(
+SPDLOG_INLINE spdlog::async_logger::async_logger(
     std::string logger_name, sinks_init_list sinks_list, std::weak_ptr<details::thread_pool> tp, async_overflow_policy overflow_policy)
     : async_logger(std::move(logger_name), sinks_list.begin(), sinks_list.end(), std::move(tp), overflow_policy)
-{
-}
+{}
 
-inline spdlog::async_logger::async_logger(
+SPDLOG_INLINE spdlog::async_logger::async_logger(
     std::string logger_name, sink_ptr single_sink, std::weak_ptr<details::thread_pool> tp, async_overflow_policy overflow_policy)
     : async_logger(std::move(logger_name), {std::move(single_sink)}, std::move(tp), overflow_policy)
-{
-}
+{}
 
 // send the log message to the thread pool
-inline void spdlog::async_logger::sink_it_(details::log_msg &msg)
+SPDLOG_INLINE void spdlog::async_logger::sink_it_(const details::log_msg &msg)
 {
-#if defined(SPDLOG_ENABLE_MESSAGE_COUNTER)
-    incr_msg_counter_(msg);
-#endif
     if (auto pool_ptr = thread_pool_.lock())
     {
         pool_ptr->post_log(shared_from_this(), msg, overflow_policy_);
     }
     else
     {
-        throw spdlog_ex("async log: thread pool doesn't exist anymore");
+        throw_spdlog_ex("async log: thread pool doesn't exist anymore");
     }
 }
 
 // send flush request to the thread pool
-inline void spdlog::async_logger::flush_()
+SPDLOG_INLINE void spdlog::async_logger::flush_()
 {
     if (auto pool_ptr = thread_pool_.lock())
     {
         pool_ptr->post_flush(shared_from_this(), overflow_policy_);
     }
     else
     {
-        throw spdlog_ex("async flush: thread pool doesn't exist anymore");
+        throw_spdlog_ex("async flush: thread pool doesn't exist anymore");
     }
 }
 
 //
 // backend functions - called from the thread pool to do the actual job
 //
-inline void spdlog::async_logger::backend_log_(const details::log_msg &incoming_log_msg)
+SPDLOG_INLINE void spdlog::async_logger::backend_sink_it_(const details::log_msg &msg)
 {
-    try
+    for (auto &sink : sinks_)
     {
-        for (auto &s : sinks_)
+        if (sink->should_log(msg.level))
         {
-            if (s->should_log(incoming_log_msg.level))
+            SPDLOG_TRY
             {
-                s->log(incoming_log_msg);
+                sink->log(msg);
             }
+            SPDLOG_LOGGER_CATCH(msg.source)
         }
     }
-    SPDLOG_CATCH_AND_HANDLE
 
-    if (should_flush_(incoming_log_msg))
+    if (should_flush_(msg))
     {
         backend_flush_();
     }
 }
 
-inline void spdlog::async_logger::backend_flush_()
+SPDLOG_INLINE void spdlog::async_logger::backend_flush_()
 {
-    try
+    for (auto &sink : sinks_)
     {
-        for (auto &sink : sinks_)
+        SPDLOG_TRY
         {
             sink->flush();
         }
+        SPDLOG_LOGGER_CATCH(source_loc())
     }
-    SPDLOG_CATCH_AND_HANDLE
 }
 
-inline std::shared_ptr<spdlog::logger> spdlog::async_logger::clone(std::string new_name)
+SPDLOG_INLINE std::shared_ptr<spdlog::logger> spdlog::async_logger::clone(std::string new_name)
 {
-    auto cloned = std::make_shared<spdlog::async_logger>(std::move(new_name), sinks_.begin(), sinks_.end(), thread_pool_, overflow_policy_);
-
-    cloned->set_level(this->level());
-    cloned->flush_on(this->flush_level());
-    cloned->set_error_handler(this->error_handler());
-    return std::move(cloned);
+    auto cloned = std::make_shared<spdlog::async_logger>(*this);
+    cloned->name_ = std::move(new_name);
+    return cloned;
 }
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/details/circular_q.h` & `spdlog-2.0.6/spdlog/include/spdlog/details/circular_q.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,141 @@
-//
-// Copyright(c) 2018 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
-// cirucal q view of std::vector.
+// circular q view of std::vector.
 #pragma once
 
 #include <vector>
+#include <cassert>
 
 namespace spdlog {
 namespace details {
 template<typename T>
 class circular_q
 {
+    size_t max_items_ = 0;
+    typename std::vector<T>::size_type head_ = 0;
+    typename std::vector<T>::size_type tail_ = 0;
+    size_t overrun_counter_ = 0;
+    std::vector<T> v_;
+
 public:
-    using item_type = T;
+    using value_type = T;
+
+    // empty ctor - create a disabled queue with no elements allocated at all
+    circular_q() = default;
 
     explicit circular_q(size_t max_items)
         : max_items_(max_items + 1) // one item is reserved as marker for full q
         , v_(max_items_)
+    {}
+
+    circular_q(const circular_q &) = default;
+    circular_q &operator=(const circular_q &) = default;
+
+    // move cannot be default,
+    // since we need to reset head_, tail_, etc to zero in the moved object
+    circular_q(circular_q &&other) SPDLOG_NOEXCEPT
     {
+        copy_moveable(std::move(other));
+    }
+
+    circular_q &operator=(circular_q &&other) SPDLOG_NOEXCEPT
+    {
+        copy_moveable(std::move(other));
+        return *this;
     }
 
     // push back, overrun (oldest) item if no room left
     void push_back(T &&item)
     {
-        v_[tail_] = std::move(item);
-        tail_ = (tail_ + 1) % max_items_;
+        if (max_items_ > 0)
+        {
+            v_[tail_] = std::move(item);
+            tail_ = (tail_ + 1) % max_items_;
+
+            if (tail_ == head_) // overrun last item if full
+            {
+                head_ = (head_ + 1) % max_items_;
+                ++overrun_counter_;
+            }
+        }
+    }
+
+    // Return reference to the front item.
+    // If there are no elements in the container, the behavior is undefined.
+    const T &front() const
+    {
+        return v_[head_];
+    }
+
+    T &front()
+    {
+        return v_[head_];
+    }
 
-        if (tail_ == head_) // overrun last item if full
+    // Return number of elements actually stored
+    size_t size() const
+    {
+        if (tail_ >= head_)
+        {
+            return tail_ - head_;
+        }
+        else
         {
-            head_ = (head_ + 1) % max_items_;
-            ++overrun_counter_;
+            return max_items_ - (head_ - tail_);
         }
     }
 
+    // Return const reference to item by index.
+    // If index is out of range 0…size()-1, the behavior is undefined.
+    const T &at(size_t i) const
+    {
+        assert(i < size());
+        return v_[(head_ + i) % max_items_];
+    }
+
     // Pop item from front.
     // If there are no elements in the container, the behavior is undefined.
-    void pop_front(T &popped_item)
+    void pop_front()
     {
-        popped_item = std::move(v_[head_]);
         head_ = (head_ + 1) % max_items_;
     }
 
-    bool empty()
+    bool empty() const
     {
         return tail_ == head_;
     }
 
-    bool full()
+    bool full() const
     {
         // head is ahead of the tail by 1
-        return ((tail_ + 1) % max_items_) == head_;
+        if (max_items_ > 0)
+        {
+            return ((tail_ + 1) % max_items_) == head_;
+        }
+        return false;
     }
 
     size_t overrun_counter() const
     {
         return overrun_counter_;
     }
 
 private:
-    size_t max_items_;
-    typename std::vector<T>::size_type head_ = 0;
-    typename std::vector<T>::size_type tail_ = 0;
-
-    std::vector<T> v_;
-
-    size_t overrun_counter_ = 0;
+    // copy from other&& and reset it to disabled state
+    void copy_moveable(circular_q &&other) SPDLOG_NOEXCEPT
+    {
+        max_items_ = other.max_items_;
+        head_ = other.head_;
+        tail_ = other.tail_;
+        overrun_counter_ = other.overrun_counter_;
+        v_ = std::move(other.v_);
+
+        // put &&other in disabled, but valid state
+        other.max_items_ = 0;
+        other.head_ = other.tail_ = 0;
+        other.overrun_counter_ = 0;
+    }
 };
 } // namespace details
 } // namespace spdlog
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/details/log_msg.h` & `spdlog-2.0.6/spdlog/include/spdlog/details/log_msg.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,37 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#include "spdlog/common.h"
-#include "spdlog/details/os.h"
-
+#include <spdlog/common.h>
 #include <string>
-#include <utility>
 
 namespace spdlog {
 namespace details {
-struct log_msg
+struct SPDLOG_API log_msg
 {
-
-    log_msg(source_loc loc, const std::string *loggers_name, level::level_enum lvl, string_view_t view)
-        : logger_name(loggers_name)
-        , level(lvl)
-#ifndef SPDLOG_NO_DATETIME
-        , time(os::now())
-#endif
-
-#ifndef SPDLOG_NO_THREAD_ID
-        , thread_id(os::thread_id())
-#endif
-        , source(loc)
-        , payload(view)
-    {
-    }
-
-    log_msg(const std::string *loggers_name, level::level_enum lvl, string_view_t view)
-        : log_msg(source_loc{}, loggers_name, lvl, view)
-    {
-    }
-
+    log_msg() = default;
+    log_msg(log_clock::time_point log_time, source_loc loc, string_view_t logger_name, level::level_enum lvl, string_view_t msg);
+    log_msg(source_loc loc, string_view_t logger_name, level::level_enum lvl, string_view_t msg);
+    log_msg(string_view_t logger_name, level::level_enum lvl, string_view_t msg);
     log_msg(const log_msg &other) = default;
+    log_msg &operator=(const log_msg &other) = default;
 
-    const std::string *logger_name{nullptr};
+    string_view_t logger_name;
     level::level_enum level{level::off};
     log_clock::time_point time;
     size_t thread_id{0};
-    size_t msg_id{0};
 
     // wrapping the formatted text with color (updated by pattern_formatter).
     mutable size_t color_range_start{0};
     mutable size_t color_range_end{0};
 
     source_loc source;
-    const string_view_t payload;
+    string_view_t payload;
 };
 } // namespace details
 } // namespace spdlog
+
+#ifdef SPDLOG_HEADER_ONLY
+#    include "log_msg-inl.h"
+#endif
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/details/mpmc_blocking_q.h` & `spdlog-2.0.6/spdlog/include/spdlog/details/mpmc_blocking_q.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-#pragma once
-
-//
-// Copyright(c) 2018 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
+
+#pragma once
 
 // multi producer-multi consumer blocking queue.
 // enqueue(..) - will block until room found to put the new message.
 // enqueue_nowait(..) - will return immediately with false if no room left in
 // the queue.
 // dequeue_for(..) - will block until the queue is not empty or timeout have
 // passed.
 
-#include "spdlog/details/circular_q.h"
+#include <spdlog/details/circular_q.h>
 
 #include <condition_variable>
 #include <mutex>
 
 namespace spdlog {
 namespace details {
 
 template<typename T>
 class mpmc_blocking_queue
 {
 public:
     using item_type = T;
     explicit mpmc_blocking_queue(size_t max_items)
         : q_(max_items)
-    {
-    }
+    {}
 
 #ifndef __MINGW32__
     // try to enqueue and block if no room left
     void enqueue(T &&item)
     {
         {
             std::unique_lock<std::mutex> lock(queue_mutex_);
@@ -48,25 +45,26 @@
         {
             std::unique_lock<std::mutex> lock(queue_mutex_);
             q_.push_back(std::move(item));
         }
         push_cv_.notify_one();
     }
 
-    // try to dequeue item. if no item found. wait upto timeout and try again
+    // try to dequeue item. if no item found. wait up to timeout and try again
     // Return true, if succeeded dequeue item, false otherwise
     bool dequeue_for(T &popped_item, std::chrono::milliseconds wait_duration)
     {
         {
             std::unique_lock<std::mutex> lock(queue_mutex_);
             if (!push_cv_.wait_for(lock, wait_duration, [this] { return !this->q_.empty(); }))
             {
                 return false;
             }
-            q_.pop_front(popped_item);
+            popped_item = std::move(q_.front());
+            q_.pop_front();
         }
         pop_cv_.notify_one();
         return true;
     }
 
 #else
     // apparently mingw deadlocks if the mutex is released before cv.notify_one(),
@@ -85,36 +83,43 @@
     void enqueue_nowait(T &&item)
     {
         std::unique_lock<std::mutex> lock(queue_mutex_);
         q_.push_back(std::move(item));
         push_cv_.notify_one();
     }
 
-    // try to dequeue item. if no item found. wait upto timeout and try again
+    // try to dequeue item. if no item found. wait up to timeout and try again
     // Return true, if succeeded dequeue item, false otherwise
     bool dequeue_for(T &popped_item, std::chrono::milliseconds wait_duration)
     {
         std::unique_lock<std::mutex> lock(queue_mutex_);
         if (!push_cv_.wait_for(lock, wait_duration, [this] { return !this->q_.empty(); }))
         {
             return false;
         }
-        q_.pop_front(popped_item);
+        popped_item = std::move(q_.front());
+        q_.pop_front();
         pop_cv_.notify_one();
         return true;
     }
 
 #endif
 
     size_t overrun_counter()
     {
         std::unique_lock<std::mutex> lock(queue_mutex_);
         return q_.overrun_counter();
     }
 
+    size_t size()
+    {
+        std::unique_lock<std::mutex> lock(queue_mutex_);
+        return q_.size();
+    }
+
 private:
     std::mutex queue_mutex_;
     std::condition_variable push_cv_;
     std::condition_variable pop_cv_;
     spdlog::details::circular_q<T> q_;
 };
 } // namespace details
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/details/os.h` & `spdlog-2.0.6/spdlog/include/spdlog/details/os-inl.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,282 +1,296 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
+
 #pragma once
 
-#include "../common.h"
+#ifndef SPDLOG_HEADER_ONLY
+#    include <spdlog/details/os.h>
+#endif
+
+#include <spdlog/common.h>
 
 #include <algorithm>
 #include <chrono>
 #include <cstdio>
 #include <cstdlib>
 #include <cstring>
 #include <ctime>
-#include <functional>
 #include <string>
+#include <thread>
+#include <array>
 #include <sys/stat.h>
 #include <sys/types.h>
-#include <thread>
 
 #ifdef _WIN32
 
-#ifndef NOMINMAX
-#define NOMINMAX // prevent windows redefining min/max
-#endif
-
-#ifndef WIN32_LEAN_AND_MEAN
-#define WIN32_LEAN_AND_MEAN
-#endif
-#include <io.h>      // _get_osfhandle and _isatty support
-#include <process.h> //  _get_pid support
-#include <windows.h>
+#    include <io.h>      // _get_osfhandle and _isatty support
+#    include <process.h> //  _get_pid support
+#    include <spdlog/details/windows_include.h>
+
+#    ifdef __MINGW32__
+#        include <share.h>
+#    endif
+
+#    if defined(SPDLOG_WCHAR_TO_UTF8_SUPPORT) || defined(SPDLOG_WCHAR_FILENAMES)
+#        include <limits>
+#    endif
 
-#ifdef __MINGW32__
-#include <share.h>
-#endif
+#    include <direct.h> // for _mkdir/_wmkdir
 
 #else // unix
 
-#include <fcntl.h>
-#include <unistd.h>
+#    include <fcntl.h>
+#    include <unistd.h>
 
-#ifdef __linux__
-#include <sys/syscall.h> //Use gettid() syscall under linux to get thread id
+#    ifdef __linux__
+#        include <sys/syscall.h> //Use gettid() syscall under linux to get thread id
 
-#elif __FreeBSD__
-#include <sys/thr.h> //Use thr_self() syscall under FreeBSD to get thread id
-#endif
+#    elif defined(_AIX)
+#        include <pthread.h> // for pthread_getthrds_np
+
+#    elif defined(__DragonFly__) || defined(__FreeBSD__)
+#        include <pthread_np.h> // for pthread_getthreadid_np
+
+#    elif defined(__NetBSD__)
+#        include <lwp.h> // for _lwp_self
+
+#    elif defined(__sun)
+#        include <thread.h> // for thr_self
+#    endif
 
 #endif // unix
 
-#ifndef __has_feature      // Clang - feature checking macros.
-#define __has_feature(x) 0 // Compatibility with non-clang compilers.
+#ifndef __has_feature          // Clang - feature checking macros.
+#    define __has_feature(x) 0 // Compatibility with non-clang compilers.
 #endif
 
 namespace spdlog {
 namespace details {
 namespace os {
 
-inline spdlog::log_clock::time_point now() SPDLOG_NOEXCEPT
+SPDLOG_INLINE spdlog::log_clock::time_point now() SPDLOG_NOEXCEPT
 {
 
 #if defined __linux__ && defined SPDLOG_CLOCK_COARSE
     timespec ts;
     ::clock_gettime(CLOCK_REALTIME_COARSE, &ts);
     return std::chrono::time_point<log_clock, typename log_clock::duration>(
         std::chrono::duration_cast<typename log_clock::duration>(std::chrono::seconds(ts.tv_sec) + std::chrono::nanoseconds(ts.tv_nsec)));
 
 #else
     return log_clock::now();
 #endif
 }
-inline std::tm localtime(const std::time_t &time_tt) SPDLOG_NOEXCEPT
+SPDLOG_INLINE std::tm localtime(const std::time_t &time_tt) SPDLOG_NOEXCEPT
 {
 
 #ifdef _WIN32
     std::tm tm;
-    localtime_s(&tm, &time_tt);
+    ::localtime_s(&tm, &time_tt);
 #else
     std::tm tm;
-    localtime_r(&time_tt, &tm);
+    ::localtime_r(&time_tt, &tm);
 #endif
     return tm;
 }
 
-inline std::tm localtime() SPDLOG_NOEXCEPT
+SPDLOG_INLINE std::tm localtime() SPDLOG_NOEXCEPT
 {
-    std::time_t now_t = time(nullptr);
+    std::time_t now_t = ::time(nullptr);
     return localtime(now_t);
 }
 
-inline std::tm gmtime(const std::time_t &time_tt) SPDLOG_NOEXCEPT
+SPDLOG_INLINE std::tm gmtime(const std::time_t &time_tt) SPDLOG_NOEXCEPT
 {
 
 #ifdef _WIN32
     std::tm tm;
-    gmtime_s(&tm, &time_tt);
+    ::gmtime_s(&tm, &time_tt);
 #else
     std::tm tm;
-    gmtime_r(&time_tt, &tm);
+    ::gmtime_r(&time_tt, &tm);
 #endif
     return tm;
 }
 
-inline std::tm gmtime() SPDLOG_NOEXCEPT
+SPDLOG_INLINE std::tm gmtime() SPDLOG_NOEXCEPT
 {
-    std::time_t now_t = time(nullptr);
+    std::time_t now_t = ::time(nullptr);
     return gmtime(now_t);
 }
 
-// eol definition
-#if !defined(SPDLOG_EOL)
-#ifdef _WIN32
-#define SPDLOG_EOL "\r\n"
-#else
-#define SPDLOG_EOL "\n"
-#endif
-#endif
-
-SPDLOG_CONSTEXPR static const char *default_eol = SPDLOG_EOL;
-
-// folder separator
-#ifdef _WIN32
-SPDLOG_CONSTEXPR static const char folder_sep = '\\';
-#else
-SPDLOG_CONSTEXPR static const char folder_sep = '/';
-#endif
-
-inline void prevent_child_fd(FILE *f)
+// fopen_s on non windows for writing
+SPDLOG_INLINE bool fopen_s(FILE **fp, const filename_t &filename, const filename_t &mode)
 {
-
 #ifdef _WIN32
-#if !defined(__cplusplus_winrt)
-    auto file_handle = (HANDLE)_get_osfhandle(_fileno(f));
-    if (!::SetHandleInformation(file_handle, HANDLE_FLAG_INHERIT, 0))
-        throw spdlog_ex("SetHandleInformation failed", errno);
-#endif
-#else
-    auto fd = fileno(f);
-    if (fcntl(fd, F_SETFD, FD_CLOEXEC) == -1)
+#    ifdef SPDLOG_WCHAR_FILENAMES
+    *fp = ::_wfsopen((filename.c_str()), mode.c_str(), _SH_DENYNO);
+#    else
+    *fp = ::_fsopen((filename.c_str()), mode.c_str(), _SH_DENYNO);
+#    endif
+#    if defined(SPDLOG_PREVENT_CHILD_FD)
+    if (*fp != nullptr)
     {
-        throw spdlog_ex("fcntl with FD_CLOEXEC failed", errno);
+        auto file_handle = reinterpret_cast<HANDLE>(_get_osfhandle(::_fileno(*fp)));
+        if (!::SetHandleInformation(file_handle, HANDLE_FLAG_INHERIT, 0))
+        {
+            ::fclose(*fp);
+            *fp = nullptr;
+        }
     }
-#endif
-}
-
-// fopen_s on non windows for writing
-inline bool fopen_s(FILE **fp, const filename_t &filename, const filename_t &mode)
-{
-#ifdef _WIN32
-#ifdef SPDLOG_WCHAR_FILENAMES
-    *fp = _wfsopen((filename.c_str()), mode.c_str(), _SH_DENYNO);
-#else
-    *fp = _fsopen((filename.c_str()), mode.c_str(), _SH_DENYNO);
-#endif
+#    endif
 #else // unix
-    *fp = fopen((filename.c_str()), mode.c_str());
-#endif
-
-#ifdef SPDLOG_PREVENT_CHILD_FD
-    if (*fp != nullptr)
+#    if defined(SPDLOG_PREVENT_CHILD_FD)
+    const int mode_flag = mode == SPDLOG_FILENAME_T("ab") ? O_APPEND : O_TRUNC;
+    const int fd = ::open((filename.c_str()), O_CREAT | O_WRONLY | O_CLOEXEC | mode_flag, mode_t(0644));
+    if (fd == -1)
+    {
+        return true;
+    }
+    *fp = ::fdopen(fd, mode.c_str());
+    if (*fp == nullptr)
     {
-        prevent_child_fd(*fp);
+        ::close(fd);
     }
+#    else
+    *fp = ::fopen((filename.c_str()), mode.c_str());
+#    endif
 #endif
+
     return *fp == nullptr;
 }
 
-inline int remove(const filename_t &filename) SPDLOG_NOEXCEPT
+SPDLOG_INLINE int remove(const filename_t &filename) SPDLOG_NOEXCEPT
 {
 #if defined(_WIN32) && defined(SPDLOG_WCHAR_FILENAMES)
-    return _wremove(filename.c_str());
+    return ::_wremove(filename.c_str());
 #else
     return std::remove(filename.c_str());
 #endif
 }
 
-inline int rename(const filename_t &filename1, const filename_t &filename2) SPDLOG_NOEXCEPT
+SPDLOG_INLINE int remove_if_exists(const filename_t &filename) SPDLOG_NOEXCEPT
+{
+    return path_exists(filename) ? remove(filename) : 0;
+}
+
+SPDLOG_INLINE int rename(const filename_t &filename1, const filename_t &filename2) SPDLOG_NOEXCEPT
 {
 #if defined(_WIN32) && defined(SPDLOG_WCHAR_FILENAMES)
-    return _wrename(filename1.c_str(), filename2.c_str());
+    return ::_wrename(filename1.c_str(), filename2.c_str());
 #else
     return std::rename(filename1.c_str(), filename2.c_str());
 #endif
 }
 
-// Return if file exists
-inline bool file_exists(const filename_t &filename) SPDLOG_NOEXCEPT
+// Return true if path exists (file or directory)
+SPDLOG_INLINE bool path_exists(const filename_t &filename) SPDLOG_NOEXCEPT
 {
 #ifdef _WIN32
-#ifdef SPDLOG_WCHAR_FILENAMES
-    auto attribs = GetFileAttributesW(filename.c_str());
-#else
-    auto attribs = GetFileAttributesA(filename.c_str());
-#endif
-    return (attribs != INVALID_FILE_ATTRIBUTES && !(attribs & FILE_ATTRIBUTE_DIRECTORY));
+#    ifdef SPDLOG_WCHAR_FILENAMES
+    auto attribs = ::GetFileAttributesW(filename.c_str());
+#    else
+    auto attribs = ::GetFileAttributesA(filename.c_str());
+#    endif
+    return attribs != INVALID_FILE_ATTRIBUTES;
 #else // common linux/unix all have the stat system call
     struct stat buffer;
-    return (stat(filename.c_str(), &buffer) == 0);
+    return (::stat(filename.c_str(), &buffer) == 0);
 #endif
 }
 
+#ifdef _MSC_VER
+// avoid warning about unreachable statement at the end of filesize()
+#    pragma warning(push)
+#    pragma warning(disable : 4702)
+#endif
+
 // Return file size according to open FILE* object
-inline size_t filesize(FILE *f)
+SPDLOG_INLINE size_t filesize(FILE *f)
 {
     if (f == nullptr)
     {
-        throw spdlog_ex("Failed getting file size. fd is null");
+        throw_spdlog_ex("Failed getting file size. fd is null");
     }
 #if defined(_WIN32) && !defined(__CYGWIN__)
-    int fd = _fileno(f);
-#if _WIN64 // 64 bits
-    __int64 ret = _filelengthi64(fd);
+    int fd = ::_fileno(f);
+#    if defined(_WIN64) // 64 bits
+    __int64 ret = ::_filelengthi64(fd);
     if (ret >= 0)
     {
         return static_cast<size_t>(ret);
     }
 
-#else // windows 32 bits
-    long ret = _filelength(fd);
+#    else // windows 32 bits
+    long ret = ::_filelength(fd);
     if (ret >= 0)
     {
         return static_cast<size_t>(ret);
     }
-#endif
+#    endif
 
 #else // unix
+// OpenBSD and AIX doesn't compile with :: before the fileno(..)
+#    if defined(__OpenBSD__) || defined(_AIX)
     int fd = fileno(f);
+#    else
+    int fd = ::fileno(f);
+#    endif
 // 64 bits(but not in osx or cygwin, where fstat64 is deprecated)
-#if !defined(__FreeBSD__) && !defined(__APPLE__) && (defined(__x86_64__) || defined(__ppc64__)) && !defined(__CYGWIN__)
+#    if (defined(__linux__) || defined(__sun) || defined(_AIX)) && (defined(__LP64__) || defined(_LP64))
     struct stat64 st;
-    if (fstat64(fd, &st) == 0)
+    if (::fstat64(fd, &st) == 0)
     {
         return static_cast<size_t>(st.st_size);
     }
-#else // unix 32 bits or cygwin
+#    else // other unix or linux 32 bits or cygwin
     struct stat st;
-
-    if (fstat(fd, &st) == 0)
+    if (::fstat(fd, &st) == 0)
     {
         return static_cast<size_t>(st.st_size);
     }
+#    endif
 #endif
-#endif
-    throw spdlog_ex("Failed getting file size from fd", errno);
+    throw_spdlog_ex("Failed getting file size from fd", errno);
+    return 0; // will not be reached.
 }
 
+#ifdef _MSC_VER
+#    pragma warning(pop)
+#endif
+
 // Return utc offset in minutes or throw spdlog_ex on failure
-inline int utc_minutes_offset(const std::tm &tm = details::os::localtime())
+SPDLOG_INLINE int utc_minutes_offset(const std::tm &tm)
 {
 
 #ifdef _WIN32
-#if _WIN32_WINNT < _WIN32_WINNT_WS08
+#    if _WIN32_WINNT < _WIN32_WINNT_WS08
     TIME_ZONE_INFORMATION tzinfo;
-    auto rv = GetTimeZoneInformation(&tzinfo);
-#else
+    auto rv = ::GetTimeZoneInformation(&tzinfo);
+#    else
     DYNAMIC_TIME_ZONE_INFORMATION tzinfo;
-    auto rv = GetDynamicTimeZoneInformation(&tzinfo);
-#endif
+    auto rv = ::GetDynamicTimeZoneInformation(&tzinfo);
+#    endif
     if (rv == TIME_ZONE_ID_INVALID)
-        throw spdlog::spdlog_ex("Failed getting timezone info. ", errno);
+        throw_spdlog_ex("Failed getting timezone info. ", errno);
 
     int offset = -tzinfo.Bias;
     if (tm.tm_isdst)
     {
         offset -= tzinfo.DaylightBias;
     }
     else
     {
         offset -= tzinfo.StandardBias;
     }
     return offset;
 #else
 
-#if defined(sun) || defined(__sun) || defined(_AIX)
+#    if defined(sun) || defined(__sun) || defined(_AIX) || (!defined(_BSD_SOURCE) && !defined(_GNU_SOURCE))
     // 'tm_gmtoff' field is BSD extension and it's missing on SunOS/Solaris
     struct helper
     {
         static long int calculate_gmt_offset(const std::tm &localtm = details::os::localtime(), const std::tm &gmtm = details::os::gmtime())
         {
             int local_year = localtm.tm_year + (1900 - 1);
             int gmt_year = gmtm.tm_year + (1900 - 1);
@@ -287,135 +301,310 @@
                 gmtm.tm_yday
 
                 // + intervening leap days
                 + ((local_year >> 2) - (gmt_year >> 2)) - (local_year / 100 - gmt_year / 100) +
                 ((local_year / 100 >> 2) - (gmt_year / 100 >> 2))
 
                 // + difference in years * 365 */
-                + (long int)(local_year - gmt_year) * 365);
+                + static_cast<long int>(local_year - gmt_year) * 365);
 
             long int hours = (24 * days) + (localtm.tm_hour - gmtm.tm_hour);
             long int mins = (60 * hours) + (localtm.tm_min - gmtm.tm_min);
             long int secs = (60 * mins) + (localtm.tm_sec - gmtm.tm_sec);
 
             return secs;
         }
     };
 
     auto offset_seconds = helper::calculate_gmt_offset(tm);
-#else
+#    else
     auto offset_seconds = tm.tm_gmtoff;
-#endif
+#    endif
 
     return static_cast<int>(offset_seconds / 60);
 #endif
 }
 
 // Return current thread id as size_t
 // It exists because the std::this_thread::get_id() is much slower(especially
 // under VS 2013)
-inline size_t _thread_id() SPDLOG_NOEXCEPT
+SPDLOG_INLINE size_t _thread_id() SPDLOG_NOEXCEPT
 {
 #ifdef _WIN32
     return static_cast<size_t>(::GetCurrentThreadId());
-#elif __linux__
-#if defined(__ANDROID__) && defined(__ANDROID_API__) && (__ANDROID_API__ < 21)
-#define SYS_gettid __NR_gettid
-#endif
-    return static_cast<size_t>(syscall(SYS_gettid));
-#elif __FreeBSD__
-    long tid;
-    thr_self(&tid);
+#elif defined(__linux__)
+#    if defined(__ANDROID__) && defined(__ANDROID_API__) && (__ANDROID_API__ < 21)
+#        define SYS_gettid __NR_gettid
+#    endif
+    return static_cast<size_t>(::syscall(SYS_gettid));
+#elif defined(_AIX)
+    struct __pthrdsinfo buf;
+    int reg_size = 0;
+    pthread_t pt = pthread_self();
+    int retval = pthread_getthrds_np(&pt, PTHRDSINFO_QUERY_TID, &buf, sizeof(buf), NULL, &reg_size);
+    int tid = (!retval) ? buf.__pi_tid : 0;
     return static_cast<size_t>(tid);
+#elif defined(__DragonFly__) || defined(__FreeBSD__)
+    return static_cast<size_t>(::pthread_getthreadid_np());
+#elif defined(__NetBSD__)
+    return static_cast<size_t>(::_lwp_self());
+#elif defined(__OpenBSD__)
+    return static_cast<size_t>(::getthrid());
+#elif defined(__sun)
+    return static_cast<size_t>(::thr_self());
 #elif __APPLE__
     uint64_t tid;
     pthread_threadid_np(nullptr, &tid);
     return static_cast<size_t>(tid);
 #else // Default to standard C++11 (other Unix)
     return static_cast<size_t>(std::hash<std::thread::id>()(std::this_thread::get_id()));
 #endif
 }
 
 // Return current thread id as size_t (from thread local storage)
-inline size_t thread_id() SPDLOG_NOEXCEPT
+SPDLOG_INLINE size_t thread_id() SPDLOG_NOEXCEPT
 {
 #if defined(SPDLOG_NO_TLS)
     return _thread_id();
 #else // cache thread id in tls
     static thread_local const size_t tid = _thread_id();
     return tid;
 #endif
 }
 
 // This is avoid msvc issue in sleep_for that happens if the clock changes.
 // See https://github.com/gabime/spdlog/issues/609
-inline void sleep_for_millis(int milliseconds) SPDLOG_NOEXCEPT
+SPDLOG_INLINE void sleep_for_millis(unsigned int milliseconds) SPDLOG_NOEXCEPT
 {
 #if defined(_WIN32)
     ::Sleep(milliseconds);
 #else
     std::this_thread::sleep_for(std::chrono::milliseconds(milliseconds));
 #endif
 }
 
 // wchar support for windows file names (SPDLOG_WCHAR_FILENAMES must be defined)
 #if defined(_WIN32) && defined(SPDLOG_WCHAR_FILENAMES)
-#define SPDLOG_FILENAME_T(s) L##s
-inline std::string filename_to_str(const filename_t &filename)
+SPDLOG_INLINE std::string filename_to_str(const filename_t &filename)
 {
-    std::wstring_convert<std::codecvt_utf8<wchar_t>, wchar_t> c;
-    return c.to_bytes(filename);
+    memory_buf_t buf;
+    wstr_to_utf8buf(filename, buf);
+#    ifdef SPDLOG_USE_STD_FORMAT
+    return buf;
+#    else
+    return fmt::to_string(buf);
+#    endif
 }
 #else
-#define SPDLOG_FILENAME_T(s) s
-inline std::string filename_to_str(const filename_t &filename)
+SPDLOG_INLINE std::string filename_to_str(const filename_t &filename)
 {
     return filename;
 }
 #endif
 
-inline int pid()
+SPDLOG_INLINE int pid() SPDLOG_NOEXCEPT
 {
 
 #ifdef _WIN32
-    return static_cast<int>(::GetCurrentProcessId());
+    return conditional_static_cast<int>(::GetCurrentProcessId());
 #else
-    return static_cast<int>(::getpid());
+    return conditional_static_cast<int>(::getpid());
 #endif
 }
 
 // Determine if the terminal supports colors
-// Source: https://github.com/agauniyal/rang/
-inline bool is_color_terminal() SPDLOG_NOEXCEPT
+// Based on: https://github.com/agauniyal/rang/
+SPDLOG_INLINE bool is_color_terminal() SPDLOG_NOEXCEPT
 {
 #ifdef _WIN32
     return true;
 #else
-    static constexpr const char *Terms[] = {
-        "ansi", "color", "console", "cygwin", "gnome", "konsole", "kterm", "linux", "msys", "putty", "rxvt", "screen", "vt100", "xterm"};
 
-    const char *env_p = std::getenv("TERM");
-    if (env_p == nullptr)
-    {
-        return false;
-    }
+    static const bool result = []() {
+        const char *env_colorterm_p = std::getenv("COLORTERM");
+        if (env_colorterm_p != nullptr)
+        {
+            return true;
+        }
+
+        static constexpr std::array<const char *, 16> terms = {{"ansi", "color", "console", "cygwin", "gnome", "konsole", "kterm", "linux",
+            "msys", "putty", "rxvt", "screen", "vt100", "xterm", "alacritty", "vt102"}};
+
+        const char *env_term_p = std::getenv("TERM");
+        if (env_term_p == nullptr)
+        {
+            return false;
+        }
+
+        return std::any_of(terms.begin(), terms.end(), [&](const char *term) { return std::strstr(env_term_p, term) != nullptr; });
+    }();
 
-    static const bool result =
-        std::any_of(std::begin(Terms), std::end(Terms), [&](const char *term) { return std::strstr(env_p, term) != nullptr; });
     return result;
 #endif
 }
 
-// Detrmine if the terminal attached
+// Determine if the terminal attached
 // Source: https://github.com/agauniyal/rang/
-inline bool in_terminal(FILE *file) SPDLOG_NOEXCEPT
+SPDLOG_INLINE bool in_terminal(FILE *file) SPDLOG_NOEXCEPT
+{
+
+#ifdef _WIN32
+    return ::_isatty(_fileno(file)) != 0;
+#else
+    return ::isatty(fileno(file)) != 0;
+#endif
+}
+
+#if (defined(SPDLOG_WCHAR_TO_UTF8_SUPPORT) || defined(SPDLOG_WCHAR_FILENAMES)) && defined(_WIN32)
+SPDLOG_INLINE void wstr_to_utf8buf(wstring_view_t wstr, memory_buf_t &target)
+{
+    if (wstr.size() > static_cast<size_t>((std::numeric_limits<int>::max)()) / 2 - 1)
+    {
+        throw_spdlog_ex("UTF-16 string is too big to be converted to UTF-8");
+    }
+
+    int wstr_size = static_cast<int>(wstr.size());
+    if (wstr_size == 0)
+    {
+        target.resize(0);
+        return;
+    }
+
+    int result_size = static_cast<int>(target.capacity());
+    if ((wstr_size + 1) * 2 > result_size)
+    {
+        result_size = ::WideCharToMultiByte(CP_UTF8, 0, wstr.data(), wstr_size, NULL, 0, NULL, NULL);
+    }
+
+    if (result_size > 0)
+    {
+        target.resize(result_size);
+        result_size = ::WideCharToMultiByte(CP_UTF8, 0, wstr.data(), wstr_size, target.data(), result_size, NULL, NULL);
+
+        if (result_size > 0)
+        {
+            target.resize(result_size);
+            return;
+        }
+    }
+
+    throw_spdlog_ex(fmt_lib::format("WideCharToMultiByte failed. Last error: {}", ::GetLastError()));
+}
+
+SPDLOG_INLINE void utf8_to_wstrbuf(string_view_t str, wmemory_buf_t &target)
 {
+    if (str.size() > static_cast<size_t>((std::numeric_limits<int>::max)()) - 1)
+    {
+        throw_spdlog_ex("UTF-8 string is too big to be converted to UTF-16");
+    }
+
+    int str_size = static_cast<int>(str.size());
+    if (str_size == 0)
+    {
+        target.resize(0);
+        return;
+    }
+
+    int result_size = static_cast<int>(target.capacity());
+    if (str_size + 1 > result_size)
+    {
+        result_size = ::MultiByteToWideChar(CP_UTF8, MB_ERR_INVALID_CHARS, str.data(), str_size, NULL, 0);
+    }
 
+    if (result_size > 0)
+    {
+        target.resize(result_size);
+        result_size = ::MultiByteToWideChar(CP_UTF8, MB_ERR_INVALID_CHARS, str.data(), str_size, target.data(), result_size);
+
+        if (result_size > 0)
+        {
+            target.resize(result_size);
+            return;
+        }
+    }
+
+    throw_spdlog_ex(fmt_lib::format("MultiByteToWideChar failed. Last error: {}", ::GetLastError()));
+}
+#endif // (defined(SPDLOG_WCHAR_TO_UTF8_SUPPORT) || defined(SPDLOG_WCHAR_FILENAMES)) && defined(_WIN32)
+
+// return true on success
+static SPDLOG_INLINE bool mkdir_(const filename_t &path)
+{
 #ifdef _WIN32
-    return _isatty(_fileno(file)) != 0;
+#    ifdef SPDLOG_WCHAR_FILENAMES
+    return ::_wmkdir(path.c_str()) == 0;
+#    else
+    return ::_mkdir(path.c_str()) == 0;
+#    endif
 #else
-    return isatty(fileno(file)) != 0;
+    return ::mkdir(path.c_str(), mode_t(0755)) == 0;
+#endif
+}
+
+// create the given directory - and all directories leading to it
+// return true on success or if the directory already exists
+SPDLOG_INLINE bool create_dir(const filename_t &path)
+{
+    if (path_exists(path))
+    {
+        return true;
+    }
+
+    if (path.empty())
+    {
+        return false;
+    }
+
+    size_t search_offset = 0;
+    do
+    {
+        auto token_pos = path.find_first_of(folder_seps_filename, search_offset);
+        // treat the entire path as a folder if no folder separator not found
+        if (token_pos == filename_t::npos)
+        {
+            token_pos = path.size();
+        }
+
+        auto subdir = path.substr(0, token_pos);
+
+        if (!subdir.empty() && !path_exists(subdir) && !mkdir_(subdir))
+        {
+            return false; // return error if failed creating dir
+        }
+        search_offset = token_pos + 1;
+    } while (search_offset < path.size());
+
+    return true;
+}
+
+// Return directory name from given path or empty string
+// "abc/file" => "abc"
+// "abc/" => "abc"
+// "abc" => ""
+// "abc///" => "abc//"
+SPDLOG_INLINE filename_t dir_name(const filename_t &path)
+{
+    auto pos = path.find_last_of(folder_seps_filename);
+    return pos != filename_t::npos ? path.substr(0, pos) : filename_t{};
+}
+
+std::string SPDLOG_INLINE getenv(const char *field)
+{
+
+#if defined(_MSC_VER)
+#    if defined(__cplusplus_winrt)
+    return std::string{}; // not supported under uwp
+#    else
+    size_t len = 0;
+    char buf[128];
+    bool ok = ::getenv_s(&len, buf, sizeof(buf), field) == 0;
+    return ok ? buf : std::string{};
+#    endif
+#else // revert to getenv
+    char *buf = ::getenv(field);
+    return buf ? buf : std::string{};
 #endif
 }
+
 } // namespace os
 } // namespace details
 } // namespace spdlog
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/details/pattern_formatter.h` & `spdlog-2.0.6/spdlog/include/spdlog/pattern_formatter-inl.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,194 +1,157 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#include "spdlog/details/fmt_helper.h"
-#include "spdlog/details/log_msg.h"
-#include "spdlog/details/os.h"
-#include "spdlog/fmt/fmt.h"
-#include "spdlog/formatter.h"
+#ifndef SPDLOG_HEADER_ONLY
+#    include <spdlog/pattern_formatter.h>
+#endif
+
+#include <spdlog/details/fmt_helper.h>
+#include <spdlog/details/log_msg.h>
+#include <spdlog/details/os.h>
+#include <spdlog/fmt/fmt.h>
+#include <spdlog/formatter.h>
 
+#include <algorithm>
 #include <array>
 #include <chrono>
 #include <ctime>
 #include <cctype>
+#include <cstring>
+#include <iterator>
 #include <memory>
 #include <mutex>
 #include <string>
 #include <thread>
 #include <utility>
 #include <vector>
 
 namespace spdlog {
 namespace details {
 
-// padding information.
-struct padding_info
-{
-    enum pad_side
-    {
-        left,
-        right,
-        center
-    };
-
-    padding_info() = default;
-    padding_info(size_t width, padding_info::pad_side side)
-        : width_(width)
-        , side_(side)
-    {
-    }
-
-    bool enabled() const
-    {
-        return width_ != 0;
-    }
-    const size_t width_ = 0;
-    const pad_side side_ = left;
-};
+///////////////////////////////////////////////////////////////////////
+// name & level pattern appender
+///////////////////////////////////////////////////////////////////////
 
-class scoped_pad
+class scoped_padder
 {
 public:
-    scoped_pad(size_t wrapped_size, padding_info &padinfo, fmt::memory_buffer &dest)
+    scoped_padder(size_t wrapped_size, const padding_info &padinfo, memory_buf_t &dest)
         : padinfo_(padinfo)
         , dest_(dest)
     {
-
-        if (padinfo_.width_ <= wrapped_size)
+        remaining_pad_ = static_cast<long>(padinfo.width_) - static_cast<long>(wrapped_size);
+        if (remaining_pad_ <= 0)
         {
-            total_pad_ = 0;
             return;
         }
 
-        total_pad_ = padinfo.width_ - wrapped_size;
-        if (padinfo_.side_ == padding_info::left)
+        if (padinfo_.side_ == padding_info::pad_side::left)
         {
-            pad_it(total_pad_);
-            total_pad_ = 0;
+            pad_it(remaining_pad_);
+            remaining_pad_ = 0;
         }
-        else if (padinfo_.side_ == padding_info::center)
+        else if (padinfo_.side_ == padding_info::pad_side::center)
         {
-            auto half_pad = total_pad_ / 2;
-            auto reminder = total_pad_ & 1;
+            auto half_pad = remaining_pad_ / 2;
+            auto reminder = remaining_pad_ & 1;
             pad_it(half_pad);
-            total_pad_ = half_pad + reminder; // for the right side
+            remaining_pad_ = half_pad + reminder; // for the right side
         }
     }
 
-    scoped_pad(spdlog::string_view_t txt, padding_info &padinfo, fmt::memory_buffer &dest)
-        : scoped_pad(txt.size(), padinfo, dest)
+    template<typename T>
+    static unsigned int count_digits(T n)
     {
+        return fmt_helper::count_digits(n);
     }
 
-    ~scoped_pad()
+    ~scoped_padder()
     {
-        if (total_pad_)
+        if (remaining_pad_ >= 0)
         {
-            pad_it(total_pad_);
+            pad_it(remaining_pad_);
+        }
+        else if (padinfo_.truncate_)
+        {
+            long new_size = static_cast<long>(dest_.size()) + remaining_pad_;
+            dest_.resize(static_cast<size_t>(new_size));
         }
     }
 
 private:
-    void pad_it(size_t count)
+    void pad_it(long count)
     {
-        // count = std::min(count, spaces_.size());
-        assert(count <= spaces_.size());
-        fmt_helper::append_string_view(string_view_t(spaces_.data(), count), dest_);
+        fmt_helper::append_string_view(string_view_t(spaces_.data(), static_cast<size_t>(count)), dest_);
     }
 
     const padding_info &padinfo_;
-    fmt::memory_buffer &dest_;
-    size_t total_pad_;
-    string_view_t spaces_{"                                                                "
-                          "                                                                ",
-        128};
+    memory_buf_t &dest_;
+    long remaining_pad_;
+    string_view_t spaces_{"                                                                ", 64};
 };
 
-class flag_formatter
+struct null_scoped_padder
 {
-public:
-    explicit flag_formatter(padding_info padinfo)
-        : padinfo_(padinfo)
+    null_scoped_padder(size_t /*wrapped_size*/, const padding_info & /*padinfo*/, memory_buf_t & /*dest*/) {}
+
+    template<typename T>
+    static unsigned int count_digits(T /* number */)
     {
+        return 0;
     }
-    flag_formatter() = default;
-    virtual ~flag_formatter() = default;
-    virtual void format(const details::log_msg &msg, const std::tm &tm_time, fmt::memory_buffer &dest) = 0;
-
-protected:
-    padding_info padinfo_;
 };
 
-///////////////////////////////////////////////////////////////////////
-// name & level pattern appender
-///////////////////////////////////////////////////////////////////////
-class name_formatter : public flag_formatter
+template<typename ScopedPadder>
+class name_formatter final : public flag_formatter
 {
 public:
     explicit name_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
-        if (padinfo_.enabled())
-        {
-            scoped_pad p(*msg.logger_name, padinfo_, dest);
-            fmt_helper::append_string_view(*msg.logger_name, dest);
-        }
-        else
-        {
-            fmt_helper::append_string_view(*msg.logger_name, dest);
-        }
+        ScopedPadder p(msg.logger_name.size(), padinfo_, dest);
+        fmt_helper::append_string_view(msg.logger_name, dest);
     }
 };
 
 // log level appender
-class level_formatter : public flag_formatter
+template<typename ScopedPadder>
+class level_formatter final : public flag_formatter
 {
 public:
     explicit level_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
-        string_view_t &level_name = level::to_string_view(msg.level);
-        if (padinfo_.enabled())
-        {
-            scoped_pad p(level_name, padinfo_, dest);
-            fmt_helper::append_string_view(level_name, dest);
-        }
-        else
-        {
-            fmt_helper::append_string_view(level_name, dest);
-        }
+        const string_view_t &level_name = level::to_string_view(msg.level);
+        ScopedPadder p(level_name.size(), padinfo_, dest);
+        fmt_helper::append_string_view(level_name, dest);
     }
 };
 
 // short log level appender
-class short_level_formatter : public flag_formatter
+template<typename ScopedPadder>
+class short_level_formatter final : public flag_formatter
 {
 public:
     explicit short_level_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         string_view_t level_name{level::to_short_c_str(msg.level)};
-        scoped_pad p(level_name, padinfo_, dest);
+        ScopedPadder p(level_name.size(), padinfo_, dest);
         fmt_helper::append_string_view(level_name, dest);
     }
 };
 
 ///////////////////////////////////////////////////////////////////////
 // Date time pattern appenders
 ///////////////////////////////////////////////////////////////////////
@@ -200,103 +163,107 @@
 
 static int to12h(const tm &t)
 {
     return t.tm_hour > 12 ? t.tm_hour - 12 : t.tm_hour;
 }
 
 // Abbreviated weekday name
-static const char *days[]{"Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"};
-class a_formatter : public flag_formatter
+static std::array<const char *, 7> days{{"Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"}};
+
+template<typename ScopedPadder>
+class a_formatter final : public flag_formatter
 {
 public:
     explicit a_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
-        string_view_t field_value{days[tm_time.tm_wday]};
-        scoped_pad p(field_value, padinfo_, dest);
+        string_view_t field_value{days[static_cast<size_t>(tm_time.tm_wday)]};
+        ScopedPadder p(field_value.size(), padinfo_, dest);
         fmt_helper::append_string_view(field_value, dest);
     }
 };
 
 // Full weekday name
-static const char *full_days[]{"Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"};
+static std::array<const char *, 7> full_days{{"Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"}};
+
+template<typename ScopedPadder>
 class A_formatter : public flag_formatter
 {
 public:
     explicit A_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
-        string_view_t field_value{full_days[tm_time.tm_wday]};
-        scoped_pad p(field_value, padinfo_, dest);
+        string_view_t field_value{full_days[static_cast<size_t>(tm_time.tm_wday)]};
+        ScopedPadder p(field_value.size(), padinfo_, dest);
         fmt_helper::append_string_view(field_value, dest);
     }
 };
 
 // Abbreviated month
-static const char *months[]{"Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sept", "Oct", "Nov", "Dec"};
-class b_formatter : public flag_formatter
+static const std::array<const char *, 12> months{{"Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sept", "Oct", "Nov", "Dec"}};
+
+template<typename ScopedPadder>
+class b_formatter final : public flag_formatter
 {
 public:
     explicit b_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
-        string_view_t field_value{months[tm_time.tm_mon]};
-        scoped_pad p(field_value, padinfo_, dest);
+        string_view_t field_value{months[static_cast<size_t>(tm_time.tm_mon)]};
+        ScopedPadder p(field_value.size(), padinfo_, dest);
         fmt_helper::append_string_view(field_value, dest);
     }
 };
 
 // Full month name
-static const char *full_months[]{
-    "January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"};
-class B_formatter : public flag_formatter
+static const std::array<const char *, 12> full_months{
+    {"January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"}};
+
+template<typename ScopedPadder>
+class B_formatter final : public flag_formatter
 {
 public:
     explicit B_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
-        string_view_t field_value{full_months[tm_time.tm_mon]};
-        scoped_pad p(field_value, padinfo_, dest);
+        string_view_t field_value{full_months[static_cast<size_t>(tm_time.tm_mon)]};
+        ScopedPadder p(field_value.size(), padinfo_, dest);
         fmt_helper::append_string_view(field_value, dest);
     }
 };
 
 // Date and time representation (Thu Aug 23 15:35:46 2014)
+template<typename ScopedPadder>
 class c_formatter final : public flag_formatter
 {
 public:
     explicit c_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 24;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
 
-        fmt_helper::append_string_view(days[tm_time.tm_wday], dest);
+        fmt_helper::append_string_view(days[static_cast<size_t>(tm_time.tm_wday)], dest);
         dest.push_back(' ');
-        fmt_helper::append_string_view(months[tm_time.tm_mon], dest);
+        fmt_helper::append_string_view(months[static_cast<size_t>(tm_time.tm_mon)], dest);
         dest.push_back(' ');
         fmt_helper::append_int(tm_time.tm_mday, dest);
         dest.push_back(' ');
         // time
 
         fmt_helper::pad2(tm_time.tm_hour, dest);
         dest.push_back(':');
@@ -305,350 +272,347 @@
         fmt_helper::pad2(tm_time.tm_sec, dest);
         dest.push_back(' ');
         fmt_helper::append_int(tm_time.tm_year + 1900, dest);
     }
 };
 
 // year - 2 digit
+template<typename ScopedPadder>
 class C_formatter final : public flag_formatter
 {
 public:
     explicit C_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 2;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         fmt_helper::pad2(tm_time.tm_year % 100, dest);
     }
 };
 
 // Short MM/DD/YY date, equivalent to %m/%d/%y 08/23/01
+template<typename ScopedPadder>
 class D_formatter final : public flag_formatter
 {
 public:
     explicit D_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 10;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
 
         fmt_helper::pad2(tm_time.tm_mon + 1, dest);
         dest.push_back('/');
         fmt_helper::pad2(tm_time.tm_mday, dest);
         dest.push_back('/');
         fmt_helper::pad2(tm_time.tm_year % 100, dest);
     }
 };
 
 // year - 4 digit
+template<typename ScopedPadder>
 class Y_formatter final : public flag_formatter
 {
 public:
     explicit Y_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 4;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         fmt_helper::append_int(tm_time.tm_year + 1900, dest);
     }
 };
 
 // month 1-12
+template<typename ScopedPadder>
 class m_formatter final : public flag_formatter
 {
 public:
     explicit m_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 2;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         fmt_helper::pad2(tm_time.tm_mon + 1, dest);
     }
 };
 
 // day of month 1-31
+template<typename ScopedPadder>
 class d_formatter final : public flag_formatter
 {
 public:
     explicit d_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 2;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         fmt_helper::pad2(tm_time.tm_mday, dest);
     }
 };
 
 // hours in 24 format 0-23
+template<typename ScopedPadder>
 class H_formatter final : public flag_formatter
 {
 public:
     explicit H_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 2;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         fmt_helper::pad2(tm_time.tm_hour, dest);
     }
 };
 
 // hours in 12 format 1-12
+template<typename ScopedPadder>
 class I_formatter final : public flag_formatter
 {
 public:
     explicit I_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 2;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         fmt_helper::pad2(to12h(tm_time), dest);
     }
 };
 
 // minutes 0-59
+template<typename ScopedPadder>
 class M_formatter final : public flag_formatter
 {
 public:
     explicit M_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 2;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         fmt_helper::pad2(tm_time.tm_min, dest);
     }
 };
 
 // seconds 0-59
+template<typename ScopedPadder>
 class S_formatter final : public flag_formatter
 {
 public:
     explicit S_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 2;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         fmt_helper::pad2(tm_time.tm_sec, dest);
     }
 };
 
 // milliseconds
+template<typename ScopedPadder>
 class e_formatter final : public flag_formatter
 {
 public:
     explicit e_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         auto millis = fmt_helper::time_fraction<std::chrono::milliseconds>(msg.time);
-        if (padinfo_.enabled())
-        {
-            const size_t field_size = 3;
-            scoped_pad p(field_size, padinfo_, dest);
-            fmt_helper::pad3(static_cast<uint32_t>(millis.count()), dest);
-        }
-        else
-        {
-            fmt_helper::pad3(static_cast<uint32_t>(millis.count()), dest);
-        }
+        const size_t field_size = 3;
+        ScopedPadder p(field_size, padinfo_, dest);
+        fmt_helper::pad3(static_cast<uint32_t>(millis.count()), dest);
     }
 };
 
 // microseconds
+template<typename ScopedPadder>
 class f_formatter final : public flag_formatter
 {
 public:
     explicit f_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         auto micros = fmt_helper::time_fraction<std::chrono::microseconds>(msg.time);
-        if (padinfo_.enabled())
-        {
-            const size_t field_size = 6;
-            scoped_pad p(field_size, padinfo_, dest);
-            fmt_helper::pad6(static_cast<size_t>(micros.count()), dest);
-        }
-        else
-        {
-            fmt_helper::pad6(static_cast<size_t>(micros.count()), dest);
-        }
+
+        const size_t field_size = 6;
+        ScopedPadder p(field_size, padinfo_, dest);
+        fmt_helper::pad6(static_cast<size_t>(micros.count()), dest);
     }
 };
 
 // nanoseconds
+template<typename ScopedPadder>
 class F_formatter final : public flag_formatter
 {
 public:
     explicit F_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         auto ns = fmt_helper::time_fraction<std::chrono::nanoseconds>(msg.time);
-        if (padinfo_.enabled())
-        {
-            const size_t field_size = 9;
-            scoped_pad p(field_size, padinfo_, dest);
-            fmt_helper::pad9(static_cast<size_t>(ns.count()), dest);
-        }
-        else
-        {
-            fmt_helper::pad9(static_cast<size_t>(ns.count()), dest);
-        }
+        const size_t field_size = 9;
+        ScopedPadder p(field_size, padinfo_, dest);
+        fmt_helper::pad9(static_cast<size_t>(ns.count()), dest);
     }
 };
 
 // seconds since epoch
+template<typename ScopedPadder>
 class E_formatter final : public flag_formatter
 {
 public:
     explicit E_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         const size_t field_size = 10;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         auto duration = msg.time.time_since_epoch();
         auto seconds = std::chrono::duration_cast<std::chrono::seconds>(duration).count();
         fmt_helper::append_int(seconds, dest);
     }
 };
 
 // AM/PM
+template<typename ScopedPadder>
 class p_formatter final : public flag_formatter
 {
 public:
     explicit p_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 2;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
         fmt_helper::append_string_view(ampm(tm_time), dest);
     }
 };
 
 // 12 hour clock 02:55:02 pm
+template<typename ScopedPadder>
 class r_formatter final : public flag_formatter
 {
 public:
     explicit r_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 11;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
 
         fmt_helper::pad2(to12h(tm_time), dest);
         dest.push_back(':');
         fmt_helper::pad2(tm_time.tm_min, dest);
         dest.push_back(':');
         fmt_helper::pad2(tm_time.tm_sec, dest);
         dest.push_back(' ');
         fmt_helper::append_string_view(ampm(tm_time), dest);
     }
 };
 
 // 24-hour HH:MM time, equivalent to %H:%M
+template<typename ScopedPadder>
 class R_formatter final : public flag_formatter
 {
 public:
     explicit R_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 5;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
 
         fmt_helper::pad2(tm_time.tm_hour, dest);
         dest.push_back(':');
         fmt_helper::pad2(tm_time.tm_min, dest);
     }
 };
 
 // ISO 8601 time format (HH:MM:SS), equivalent to %H:%M:%S
+template<typename ScopedPadder>
 class T_formatter final : public flag_formatter
 {
 public:
     explicit T_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 8;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
 
         fmt_helper::pad2(tm_time.tm_hour, dest);
         dest.push_back(':');
         fmt_helper::pad2(tm_time.tm_min, dest);
         dest.push_back(':');
         fmt_helper::pad2(tm_time.tm_sec, dest);
     }
 };
 
 // ISO 8601 offset from UTC in timezone (+-HH:MM)
+template<typename ScopedPadder>
 class z_formatter final : public flag_formatter
 {
 public:
     explicit z_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
-
-    const std::chrono::seconds cache_refresh = std::chrono::seconds(5);
+        : flag_formatter(padinfo)
+    {}
 
     z_formatter() = default;
     z_formatter(const z_formatter &) = delete;
     z_formatter &operator=(const z_formatter &) = delete;
 
-    void format(const details::log_msg &msg, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &tm_time, memory_buf_t &dest) override
     {
         const size_t field_size = 6;
-        scoped_pad p(field_size, padinfo_, dest);
+        ScopedPadder p(field_size, padinfo_, dest);
 
-#ifdef _WIN32
-        int total_minutes = get_cached_offset(msg, tm_time);
-#else
-        // No need to chache under gcc,
-        // it is very fast (already stored in tm.tm_gmtoff)
-        (void)(msg);
-        int total_minutes = os::utc_minutes_offset(tm_time);
-#endif
+        auto total_minutes = get_cached_offset(msg, tm_time);
         bool is_negative = total_minutes < 0;
         if (is_negative)
         {
             total_minutes = -total_minutes;
             dest.push_back('-');
         }
         else
@@ -659,121 +623,87 @@
         fmt_helper::pad2(total_minutes / 60, dest); // hours
         dest.push_back(':');
         fmt_helper::pad2(total_minutes % 60, dest); // minutes
     }
 
 private:
     log_clock::time_point last_update_{std::chrono::seconds(0)};
-#ifdef _WIN32
     int offset_minutes_{0};
 
     int get_cached_offset(const log_msg &msg, const std::tm &tm_time)
     {
-        if (msg.time - last_update_ >= cache_refresh)
+        // refresh every 10 seconds
+        if (msg.time - last_update_ >= std::chrono::seconds(10))
         {
             offset_minutes_ = os::utc_minutes_offset(tm_time);
             last_update_ = msg.time;
         }
         return offset_minutes_;
     }
-#endif
 };
 
 // Thread id
+template<typename ScopedPadder>
 class t_formatter final : public flag_formatter
 {
 public:
     explicit t_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
-        if (padinfo_.enabled())
-        {
-            const auto field_size = fmt_helper::count_digits(msg.thread_id);
-            scoped_pad p(field_size, padinfo_, dest);
-            fmt_helper::append_int(msg.thread_id, dest);
-        }
-        else
-        {
-            fmt_helper::append_int(msg.thread_id, dest);
-        }
+        const auto field_size = ScopedPadder::count_digits(msg.thread_id);
+        ScopedPadder p(field_size, padinfo_, dest);
+        fmt_helper::append_int(msg.thread_id, dest);
     }
 };
 
 // Current pid
+template<typename ScopedPadder>
 class pid_formatter final : public flag_formatter
 {
 public:
     explicit pid_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &, memory_buf_t &dest) override
     {
         const auto pid = static_cast<uint32_t>(details::os::pid());
-        if (padinfo_.enabled())
-        {
-            auto field_size = fmt_helper::count_digits(pid);
-            scoped_pad p(field_size, padinfo_, dest);
-            fmt_helper::append_int(pid, dest);
-        }
-        else
-        {
-            fmt_helper::append_int(pid, dest);
-        }
-    }
-};
-
-// message counter formatter
-class i_formatter final : public flag_formatter
-{
-public:
-    explicit i_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
-
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
-    {
-        const size_t field_size = 6;
-        scoped_pad p(field_size, padinfo_, dest);
-        fmt_helper::pad6(msg.msg_id, dest);
+        auto field_size = ScopedPadder::count_digits(pid);
+        ScopedPadder p(field_size, padinfo_, dest);
+        fmt_helper::append_int(pid, dest);
     }
 };
 
+template<typename ScopedPadder>
 class v_formatter final : public flag_formatter
 {
 public:
     explicit v_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
-        if (padinfo_.enabled())
-        {
-            scoped_pad p(msg.payload, padinfo_, dest);
-            fmt_helper::append_string_view(msg.payload, dest);
-        }
-        else
-        {
-            fmt_helper::append_string_view(msg.payload, dest);
-        }
+        ScopedPadder p(msg.payload.size(), padinfo_, dest);
+        fmt_helper::append_string_view(msg.payload, dest);
     }
 };
 
 class ch_formatter final : public flag_formatter
 {
 public:
     explicit ch_formatter(char ch)
         : ch_(ch)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &, memory_buf_t &dest) override
     {
-        const size_t field_size = 1;
-        scoped_pad p(field_size, padinfo_, dest);
         dest.push_back(ch_);
     }
 
 private:
     char ch_;
 };
 
@@ -783,158 +713,241 @@
 public:
     aggregate_formatter() = default;
 
     void add_ch(char ch)
     {
         str_ += ch;
     }
-    void format(const details::log_msg &, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &, const std::tm &, memory_buf_t &dest) override
     {
         fmt_helper::append_string_view(str_, dest);
     }
 
 private:
     std::string str_;
 };
 
 // mark the color range. expect it to be in the form of "%^colored text%$"
 class color_start_formatter final : public flag_formatter
 {
 public:
     explicit color_start_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         msg.color_range_start = dest.size();
     }
 };
+
 class color_stop_formatter final : public flag_formatter
 {
 public:
     explicit color_stop_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         msg.color_range_end = dest.size();
     }
 };
 
 // print source location
+template<typename ScopedPadder>
 class source_location_formatter final : public flag_formatter
 {
 public:
     explicit source_location_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         if (msg.source.empty())
         {
+            ScopedPadder p(0, padinfo_, dest);
             return;
         }
+
+        size_t text_size;
         if (padinfo_.enabled())
         {
-            const auto text_size = std::char_traits<char>::length(msg.source.filename) + fmt_helper::count_digits(msg.source.line) + 1;
-            scoped_pad p(text_size, padinfo_, dest);
-            fmt_helper::append_string_view(msg.source.filename, dest);
-            dest.push_back(':');
-            fmt_helper::append_int(msg.source.line, dest);
+            // calc text size for padding based on "filename:line"
+            text_size = std::char_traits<char>::length(msg.source.filename) + ScopedPadder::count_digits(msg.source.line) + 1;
         }
         else
         {
-            fmt_helper::append_string_view(msg.source.filename, dest);
-            dest.push_back(':');
-            fmt_helper::append_int(msg.source.line, dest);
+            text_size = 0;
         }
+
+        ScopedPadder p(text_size, padinfo_, dest);
+        fmt_helper::append_string_view(msg.source.filename, dest);
+        dest.push_back(':');
+        fmt_helper::append_int(msg.source.line, dest);
     }
 };
+
 // print source filename
+template<typename ScopedPadder>
 class source_filename_formatter final : public flag_formatter
 {
 public:
     explicit source_filename_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         if (msg.source.empty())
         {
+            ScopedPadder p(0, padinfo_, dest);
             return;
         }
-        scoped_pad p(msg.source.filename, padinfo_, dest);
+        size_t text_size = padinfo_.enabled() ? std::char_traits<char>::length(msg.source.filename) : 0;
+        ScopedPadder p(text_size, padinfo_, dest);
         fmt_helper::append_string_view(msg.source.filename, dest);
     }
 };
 
-class source_linenum_formatter final : public flag_formatter
+template<typename ScopedPadder>
+class short_filename_formatter final : public flag_formatter
 {
 public:
-    explicit source_linenum_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+    explicit short_filename_formatter(padding_info padinfo)
+        : flag_formatter(padinfo)
+    {}
+
+#ifdef _MSC_VER
+#    pragma warning(push)
+#    pragma warning(disable : 4127) // consider using 'if constexpr' instead
+#endif                              // _MSC_VER
+    static const char *basename(const char *filename)
+    {
+        // if the size is 2 (1 character + null terminator) we can use the more efficient strrchr
+        // the branch will be elided by optimizations
+        if (sizeof(os::folder_seps) == 2)
+        {
+            const char *rv = std::strrchr(filename, os::folder_seps[0]);
+            return rv != nullptr ? rv + 1 : filename;
+        }
+        else
+        {
+            const std::reverse_iterator<const char *> begin(filename + std::strlen(filename));
+            const std::reverse_iterator<const char *> end(filename);
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+            const auto it = std::find_first_of(begin, end, std::begin(os::folder_seps), std::end(os::folder_seps) - 1);
+            return it != end ? it.base() : filename;
+        }
+    }
+#ifdef _MSC_VER
+#    pragma warning(pop)
+#endif // _MSC_VER
+
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         if (msg.source.empty())
         {
+            ScopedPadder p(0, padinfo_, dest);
             return;
         }
-        if (padinfo_.enabled())
-        {
-            auto field_size = fmt_helper::count_digits(msg.source.line);
-            scoped_pad p(field_size, padinfo_, dest);
-            fmt_helper::append_int(msg.source.line, dest);
-        }
-        else
+        auto filename = basename(msg.source.filename);
+        size_t text_size = padinfo_.enabled() ? std::char_traits<char>::length(filename) : 0;
+        ScopedPadder p(text_size, padinfo_, dest);
+        fmt_helper::append_string_view(filename, dest);
+    }
+};
+
+template<typename ScopedPadder>
+class source_linenum_formatter final : public flag_formatter
+{
+public:
+    explicit source_linenum_formatter(padding_info padinfo)
+        : flag_formatter(padinfo)
+    {}
+
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
+    {
+        if (msg.source.empty())
         {
-            fmt_helper::append_int(msg.source.line, dest);
+            ScopedPadder p(0, padinfo_, dest);
+            return;
         }
+
+        auto field_size = ScopedPadder::count_digits(msg.source.line);
+        ScopedPadder p(field_size, padinfo_, dest);
+        fmt_helper::append_int(msg.source.line, dest);
     }
 };
+
 // print source funcname
+template<typename ScopedPadder>
 class source_funcname_formatter final : public flag_formatter
 {
 public:
     explicit source_funcname_formatter(padding_info padinfo)
-        : flag_formatter(padinfo){};
+        : flag_formatter(padinfo)
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
     {
         if (msg.source.empty())
         {
+            ScopedPadder p(0, padinfo_, dest);
             return;
         }
-        scoped_pad p(msg.source.funcname, padinfo_, dest);
+        size_t text_size = padinfo_.enabled() ? std::char_traits<char>::length(msg.source.funcname) : 0;
+        ScopedPadder p(text_size, padinfo_, dest);
         fmt_helper::append_string_view(msg.source.funcname, dest);
     }
 };
 
+// print elapsed time since last message
+template<typename ScopedPadder, typename Units>
+class elapsed_formatter final : public flag_formatter
+{
+public:
+    using DurationUnits = Units;
+
+    explicit elapsed_formatter(padding_info padinfo)
+        : flag_formatter(padinfo)
+        , last_message_time_(log_clock::now())
+    {}
+
+    void format(const details::log_msg &msg, const std::tm &, memory_buf_t &dest) override
+    {
+        auto delta = (std::max)(msg.time - last_message_time_, log_clock::duration::zero());
+        auto delta_units = std::chrono::duration_cast<DurationUnits>(delta);
+        last_message_time_ = msg.time;
+        auto delta_count = static_cast<size_t>(delta_units.count());
+        auto n_digits = static_cast<size_t>(ScopedPadder::count_digits(delta_count));
+        ScopedPadder p(n_digits, padinfo_, dest);
+        fmt_helper::append_int(delta_count, dest);
+    }
+
+private:
+    log_clock::time_point last_message_time_;
+};
+
 // Full info formatter
-// pattern: [%Y-%m-%d %H:%M:%S.%e] [%n] [%l] %v
+// pattern: [%Y-%m-%d %H:%M:%S.%e] [%n] [%l] [%s:%#] %v
 class full_formatter final : public flag_formatter
 {
 public:
     explicit full_formatter(padding_info padinfo)
         : flag_formatter(padinfo)
-    {
-    }
+    {}
 
-    void format(const details::log_msg &msg, const std::tm &tm_time, fmt::memory_buffer &dest) override
+    void format(const details::log_msg &msg, const std::tm &tm_time, memory_buf_t &dest) override
     {
         using std::chrono::duration_cast;
         using std::chrono::milliseconds;
         using std::chrono::seconds;
 
-#ifndef SPDLOG_NO_DATETIME
-
         // cache the date/time part for the next second.
         auto duration = msg.time.time_since_epoch();
         auto secs = duration_cast<seconds>(duration);
 
         if (cache_timestamp_ != secs || cached_datetime_.size() == 0)
         {
             cached_datetime_.clear();
@@ -955,382 +968,458 @@
             cached_datetime_.push_back(':');
 
             fmt_helper::pad2(tm_time.tm_sec, cached_datetime_);
             cached_datetime_.push_back('.');
 
             cache_timestamp_ = secs;
         }
-        fmt_helper::append_buf(cached_datetime_, dest);
+        dest.append(cached_datetime_.begin(), cached_datetime_.end());
 
         auto millis = fmt_helper::time_fraction<milliseconds>(msg.time);
         fmt_helper::pad3(static_cast<uint32_t>(millis.count()), dest);
         dest.push_back(']');
         dest.push_back(' ');
 
-#else // no datetime needed
-        (void)tm_time;
-#endif
-
-#ifndef SPDLOG_NO_NAME
-        if (!msg.logger_name->empty())
+        // append logger name if exists
+        if (msg.logger_name.size() > 0)
         {
             dest.push_back('[');
-            // fmt_helper::append_str(*msg.logger_name, dest);
-            fmt_helper::append_string_view(*msg.logger_name, dest);
+            fmt_helper::append_string_view(msg.logger_name, dest);
             dest.push_back(']');
             dest.push_back(' ');
         }
-#endif
 
         dest.push_back('[');
         // wrap the level name with color
         msg.color_range_start = dest.size();
         // fmt_helper::append_string_view(level::to_c_str(msg.level), dest);
         fmt_helper::append_string_view(level::to_string_view(msg.level), dest);
         msg.color_range_end = dest.size();
         dest.push_back(']');
         dest.push_back(' ');
 
         // add source location if present
         if (!msg.source.empty())
         {
             dest.push_back('[');
-            fmt_helper::append_string_view(msg.source.filename, dest);
+            const char *filename = details::short_filename_formatter<details::null_scoped_padder>::basename(msg.source.filename);
+            fmt_helper::append_string_view(filename, dest);
             dest.push_back(':');
             fmt_helper::append_int(msg.source.line, dest);
             dest.push_back(']');
             dest.push_back(' ');
         }
         // fmt_helper::append_string_view(msg.msg(), dest);
         fmt_helper::append_string_view(msg.payload, dest);
     }
 
 private:
     std::chrono::seconds cache_timestamp_{0};
-    fmt::basic_memory_buffer<char, 128> cached_datetime_;
+    memory_buf_t cached_datetime_;
 };
 
 } // namespace details
 
-class pattern_formatter final : public formatter
+SPDLOG_INLINE pattern_formatter::pattern_formatter(
+    std::string pattern, pattern_time_type time_type, std::string eol, custom_flags custom_user_flags)
+    : pattern_(std::move(pattern))
+    , eol_(std::move(eol))
+    , pattern_time_type_(time_type)
+    , need_localtime_(false)
+    , last_log_secs_(0)
+    , custom_handlers_(std::move(custom_user_flags))
 {
-public:
-    explicit pattern_formatter(
-        std::string pattern, pattern_time_type time_type = pattern_time_type::local, std::string eol = spdlog::details::os::default_eol)
-        : pattern_(std::move(pattern))
-        , eol_(std::move(eol))
-        , pattern_time_type_(time_type)
-        , last_log_secs_(0)
-    {
-        std::memset(&cached_tm_, 0, sizeof(cached_tm_));
-        compile_pattern_(pattern_);
-    }
-
-    // use by default full formatter for if pattern is not given
-    explicit pattern_formatter(pattern_time_type time_type = pattern_time_type::local, std::string eol = spdlog::details::os::default_eol)
-        : pattern_("%+")
-        , eol_(std::move(eol))
-        , pattern_time_type_(time_type)
-        , last_log_secs_(0)
-    {
-        std::memset(&cached_tm_, 0, sizeof(cached_tm_));
-        formatters_.push_back(details::make_unique<details::full_formatter>(details::padding_info{}));
-    }
+    std::memset(&cached_tm_, 0, sizeof(cached_tm_));
+    compile_pattern_(pattern_);
+}
 
-    pattern_formatter(const pattern_formatter &other) = delete;
-    pattern_formatter &operator=(const pattern_formatter &other) = delete;
+// use by default full formatter for if pattern is not given
+SPDLOG_INLINE pattern_formatter::pattern_formatter(pattern_time_type time_type, std::string eol)
+    : pattern_("%+")
+    , eol_(std::move(eol))
+    , pattern_time_type_(time_type)
+    , need_localtime_(true)
+    , last_log_secs_(0)
+{
+    std::memset(&cached_tm_, 0, sizeof(cached_tm_));
+    formatters_.push_back(details::make_unique<details::full_formatter>(details::padding_info{}));
+}
 
-    std::unique_ptr<formatter> clone() const override
+SPDLOG_INLINE std::unique_ptr<formatter> pattern_formatter::clone() const
+{
+    custom_flags cloned_custom_formatters;
+    for (auto &it : custom_handlers_)
     {
-        return details::make_unique<pattern_formatter>(pattern_, pattern_time_type_, eol_);
+        cloned_custom_formatters[it.first] = it.second->clone();
     }
+    return details::make_unique<pattern_formatter>(pattern_, pattern_time_type_, eol_, std::move(cloned_custom_formatters));
+}
 
-    void format(const details::log_msg &msg, fmt::memory_buffer &dest) override
+SPDLOG_INLINE void pattern_formatter::format(const details::log_msg &msg, memory_buf_t &dest)
+{
+    if (need_localtime_)
     {
-#ifndef SPDLOG_NO_DATETIME
-        auto secs = std::chrono::duration_cast<std::chrono::seconds>(msg.time.time_since_epoch());
+        const auto secs = std::chrono::duration_cast<std::chrono::seconds>(msg.time.time_since_epoch());
         if (secs != last_log_secs_)
         {
             cached_tm_ = get_time_(msg);
             last_log_secs_ = secs;
         }
-#endif
-        for (auto &f : formatters_)
-        {
-            f->format(msg, cached_tm_, dest);
-        }
-        // write eol
-        details::fmt_helper::append_string_view(eol_, dest);
     }
 
-private:
-    std::string pattern_;
-    std::string eol_;
-    pattern_time_type pattern_time_type_;
-    std::tm cached_tm_;
-    std::chrono::seconds last_log_secs_;
-
-    std::vector<std::unique_ptr<details::flag_formatter>> formatters_;
-
-    std::tm get_time_(const details::log_msg &msg)
+    for (auto &f : formatters_)
     {
-        if (pattern_time_type_ == pattern_time_type::local)
-        {
-            return details::os::localtime(log_clock::to_time_t(msg.time));
-        }
-        return details::os::gmtime(log_clock::to_time_t(msg.time));
+        f->format(msg, cached_tm_, dest);
     }
+    // write eol
+    details::fmt_helper::append_string_view(eol_, dest);
+}
 
-    void handle_flag_(char flag, details::padding_info padding)
-    {
-        switch (flag)
-        {
-
-        case ('+'): // default formatter
-            formatters_.push_back(details::make_unique<details::full_formatter>(padding));
-            break;
-
-        case 'n': // logger name
-            formatters_.push_back(details::make_unique<details::name_formatter>(padding));
-            break;
-
-        case 'l': // level
-            formatters_.push_back(details::make_unique<details::level_formatter>(padding));
-            break;
-
-        case 'L': // short level
-            formatters_.push_back(details::make_unique<details::short_level_formatter>(padding));
-            break;
-
-        case ('t'): // thread id
-            formatters_.push_back(details::make_unique<details::t_formatter>(padding));
-            break;
-
-        case ('v'): // the message text
-            formatters_.push_back(details::make_unique<details::v_formatter>(padding));
-            break;
-
-        case ('a'): // weekday
-            formatters_.push_back(details::make_unique<details::a_formatter>(padding));
-            break;
-
-        case ('A'): // short weekday
-            formatters_.push_back(details::make_unique<details::A_formatter>(padding));
-            break;
-
-        case ('b'):
-        case ('h'): // month
-            formatters_.push_back(details::make_unique<details::b_formatter>(padding));
-            break;
-
-        case ('B'): // short month
-            formatters_.push_back(details::make_unique<details::B_formatter>(padding));
-            break;
-
-        case ('c'): // datetime
-            formatters_.push_back(details::make_unique<details::c_formatter>(padding));
-            break;
-
-        case ('C'): // year 2 digits
-            formatters_.push_back(details::make_unique<details::C_formatter>(padding));
-            break;
-
-        case ('Y'): // year 4 digits
-            formatters_.push_back(details::make_unique<details::Y_formatter>(padding));
-            break;
-
-        case ('D'):
-        case ('x'): // datetime MM/DD/YY
-            formatters_.push_back(details::make_unique<details::D_formatter>(padding));
-            break;
-
-        case ('m'): // month 1-12
-            formatters_.push_back(details::make_unique<details::m_formatter>(padding));
-            break;
-
-        case ('d'): // day of month 1-31
-            formatters_.push_back(details::make_unique<details::d_formatter>(padding));
-            break;
-
-        case ('H'): // hours 24
-            formatters_.push_back(details::make_unique<details::H_formatter>(padding));
-            break;
-
-        case ('I'): // hours 12
-            formatters_.push_back(details::make_unique<details::I_formatter>(padding));
-            break;
-
-        case ('M'): // minutes
-            formatters_.push_back(details::make_unique<details::M_formatter>(padding));
-            break;
-
-        case ('S'): // seconds
-            formatters_.push_back(details::make_unique<details::S_formatter>(padding));
-            break;
-
-        case ('e'): // milliseconds
-            formatters_.push_back(details::make_unique<details::e_formatter>(padding));
-            break;
-
-        case ('f'): // microseconds
-            formatters_.push_back(details::make_unique<details::f_formatter>(padding));
-            break;
-
-        case ('F'): // nanoseconds
-            formatters_.push_back(details::make_unique<details::F_formatter>(padding));
-            break;
-
-        case ('E'): // seconds since epoch
-            formatters_.push_back(details::make_unique<details::E_formatter>(padding));
-            break;
-
-        case ('p'): // am/pm
-            formatters_.push_back(details::make_unique<details::p_formatter>(padding));
-            break;
-
-        case ('r'): // 12 hour clock 02:55:02 pm
-            formatters_.push_back(details::make_unique<details::r_formatter>(padding));
-            break;
-
-        case ('R'): // 24-hour HH:MM time
-            formatters_.push_back(details::make_unique<details::R_formatter>(padding));
-            break;
-
-        case ('T'):
-        case ('X'): // ISO 8601 time format (HH:MM:SS)
-            formatters_.push_back(details::make_unique<details::T_formatter>(padding));
-            break;
+SPDLOG_INLINE void pattern_formatter::set_pattern(std::string pattern)
+{
+    pattern_ = std::move(pattern);
+    need_localtime_ = false;
+    compile_pattern_(pattern_);
+}
 
-        case ('z'): // timezone
-            formatters_.push_back(details::make_unique<details::z_formatter>(padding));
-            break;
+SPDLOG_INLINE std::tm pattern_formatter::get_time_(const details::log_msg &msg)
+{
+    if (pattern_time_type_ == pattern_time_type::local)
+    {
+        return details::os::localtime(log_clock::to_time_t(msg.time));
+    }
+    return details::os::gmtime(log_clock::to_time_t(msg.time));
+}
 
-        case ('P'): // pid
-            formatters_.push_back(details::make_unique<details::pid_formatter>(padding));
-            break;
+template<typename Padder>
+SPDLOG_INLINE void pattern_formatter::handle_flag_(char flag, details::padding_info padding)
+{
+    // process custom flags
+    auto it = custom_handlers_.find(flag);
+    if (it != custom_handlers_.end())
+    {
+        auto custom_handler = it->second->clone();
+        custom_handler->set_padding_info(padding);
+        formatters_.push_back(std::move(custom_handler));
+        return;
+    }
+
+    // process built-in flags
+    switch (flag)
+    {
+    case ('+'): // default formatter
+        formatters_.push_back(details::make_unique<details::full_formatter>(padding));
+        need_localtime_ = true;
+        break;
+
+    case 'n': // logger name
+        formatters_.push_back(details::make_unique<details::name_formatter<Padder>>(padding));
+        break;
+
+    case 'l': // level
+        formatters_.push_back(details::make_unique<details::level_formatter<Padder>>(padding));
+        break;
+
+    case 'L': // short level
+        formatters_.push_back(details::make_unique<details::short_level_formatter<Padder>>(padding));
+        break;
+
+    case ('t'): // thread id
+        formatters_.push_back(details::make_unique<details::t_formatter<Padder>>(padding));
+        break;
+
+    case ('v'): // the message text
+        formatters_.push_back(details::make_unique<details::v_formatter<Padder>>(padding));
+        break;
+
+    case ('a'): // weekday
+        formatters_.push_back(details::make_unique<details::a_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('A'): // short weekday
+        formatters_.push_back(details::make_unique<details::A_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('b'):
+    case ('h'): // month
+        formatters_.push_back(details::make_unique<details::b_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('B'): // short month
+        formatters_.push_back(details::make_unique<details::B_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('c'): // datetime
+        formatters_.push_back(details::make_unique<details::c_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('C'): // year 2 digits
+        formatters_.push_back(details::make_unique<details::C_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('Y'): // year 4 digits
+        formatters_.push_back(details::make_unique<details::Y_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('D'):
+    case ('x'): // datetime MM/DD/YY
+        formatters_.push_back(details::make_unique<details::D_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('m'): // month 1-12
+        formatters_.push_back(details::make_unique<details::m_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('d'): // day of month 1-31
+        formatters_.push_back(details::make_unique<details::d_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('H'): // hours 24
+        formatters_.push_back(details::make_unique<details::H_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('I'): // hours 12
+        formatters_.push_back(details::make_unique<details::I_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('M'): // minutes
+        formatters_.push_back(details::make_unique<details::M_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('S'): // seconds
+        formatters_.push_back(details::make_unique<details::S_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('e'): // milliseconds
+        formatters_.push_back(details::make_unique<details::e_formatter<Padder>>(padding));
+        break;
+
+    case ('f'): // microseconds
+        formatters_.push_back(details::make_unique<details::f_formatter<Padder>>(padding));
+        break;
+
+    case ('F'): // nanoseconds
+        formatters_.push_back(details::make_unique<details::F_formatter<Padder>>(padding));
+        break;
+
+    case ('E'): // seconds since epoch
+        formatters_.push_back(details::make_unique<details::E_formatter<Padder>>(padding));
+        break;
+
+    case ('p'): // am/pm
+        formatters_.push_back(details::make_unique<details::p_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('r'): // 12 hour clock 02:55:02 pm
+        formatters_.push_back(details::make_unique<details::r_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('R'): // 24-hour HH:MM time
+        formatters_.push_back(details::make_unique<details::R_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('T'):
+    case ('X'): // ISO 8601 time format (HH:MM:SS)
+        formatters_.push_back(details::make_unique<details::T_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('z'): // timezone
+        formatters_.push_back(details::make_unique<details::z_formatter<Padder>>(padding));
+        need_localtime_ = true;
+        break;
+
+    case ('P'): // pid
+        formatters_.push_back(details::make_unique<details::pid_formatter<Padder>>(padding));
+        break;
+
+    case ('^'): // color range start
+        formatters_.push_back(details::make_unique<details::color_start_formatter>(padding));
+        break;
+
+    case ('$'): // color range end
+        formatters_.push_back(details::make_unique<details::color_stop_formatter>(padding));
+        break;
+
+    case ('@'): // source location (filename:filenumber)
+        formatters_.push_back(details::make_unique<details::source_location_formatter<Padder>>(padding));
+        break;
+
+    case ('s'): // short source filename - without directory name
+        formatters_.push_back(details::make_unique<details::short_filename_formatter<Padder>>(padding));
+        break;
+
+    case ('g'): // full source filename
+        formatters_.push_back(details::make_unique<details::source_filename_formatter<Padder>>(padding));
+        break;
+
+    case ('#'): // source line number
+        formatters_.push_back(details::make_unique<details::source_linenum_formatter<Padder>>(padding));
+        break;
+
+    case ('!'): // source funcname
+        formatters_.push_back(details::make_unique<details::source_funcname_formatter<Padder>>(padding));
+        break;
+
+    case ('%'): // % char
+        formatters_.push_back(details::make_unique<details::ch_formatter>('%'));
+        break;
+
+    case ('u'): // elapsed time since last log message in nanos
+        formatters_.push_back(details::make_unique<details::elapsed_formatter<Padder, std::chrono::nanoseconds>>(padding));
+        break;
+
+    case ('i'): // elapsed time since last log message in micros
+        formatters_.push_back(details::make_unique<details::elapsed_formatter<Padder, std::chrono::microseconds>>(padding));
+        break;
+
+    case ('o'): // elapsed time since last log message in millis
+        formatters_.push_back(details::make_unique<details::elapsed_formatter<Padder, std::chrono::milliseconds>>(padding));
+        break;
+
+    case ('O'): // elapsed time since last log message in seconds
+        formatters_.push_back(details::make_unique<details::elapsed_formatter<Padder, std::chrono::seconds>>(padding));
+        break;
 
-#ifdef SPDLOG_ENABLE_MESSAGE_COUNTER
-        case ('i'):
-            formatters_.push_back(details::make_unique<details::i_formatter>(padding));
-            break;
-#endif
-        case ('^'): // color range start
-            formatters_.push_back(details::make_unique<details::color_start_formatter>(padding));
-            break;
-
-        case ('$'): // color range end
-            formatters_.push_back(details::make_unique<details::color_stop_formatter>(padding));
-            break;
-
-        case ('@'): // source location (filename:filenumber)
-            formatters_.push_back(details::make_unique<details::source_location_formatter>(padding));
-            break;
-
-        case ('s'): // source filename
-            formatters_.push_back(details::make_unique<details::source_filename_formatter>(padding));
-            break;
-
-        case ('#'): // source line number
-            formatters_.push_back(details::make_unique<details::source_linenum_formatter>(padding));
-            break;
-
-        case ('!'): // source funcname
-            formatters_.push_back(details::make_unique<details::source_funcname_formatter>(padding));
-            break;
-
-        case ('%'): // % char
-            formatters_.push_back(details::make_unique<details::ch_formatter>('%'));
-            break;
+    default: // Unknown flag appears as is
+        auto unknown_flag = details::make_unique<details::aggregate_formatter>();
 
-        default: // Unknown flag appears as is
-            auto unknown_flag = details::make_unique<details::aggregate_formatter>();
+        if (!padding.truncate_)
+        {
             unknown_flag->add_ch('%');
             unknown_flag->add_ch(flag);
             formatters_.push_back((std::move(unknown_flag)));
-            break;
         }
+        // fix issue #1617 (prev char was '!' and should have been treated as funcname flag instead of truncating flag)
+        // spdlog::set_pattern("[%10!] %v") => "[      main] some message"
+        // spdlog::set_pattern("[%3!!] %v") => "[mai] some message"
+        else
+        {
+            padding.truncate_ = false;
+            formatters_.push_back(details::make_unique<details::source_funcname_formatter<Padder>>(padding));
+            unknown_flag->add_ch(flag);
+            formatters_.push_back((std::move(unknown_flag)));
+        }
+
+        break;
     }
+}
 
-    // Extract given pad spec (e.g. %8X)
-    // Advance the given it pass the end of the padding spec found (if any)
-    // Return padding.
-    details::padding_info handle_padspec_(std::string::const_iterator &it, std::string::const_iterator end)
+// Extract given pad spec (e.g. %8X, %=8X, %-8!X, %8!X, %=8!X, %-8!X, %+8!X)
+// Advance the given it pass the end of the padding spec found (if any)
+// Return padding.
+SPDLOG_INLINE details::padding_info pattern_formatter::handle_padspec_(std::string::const_iterator &it, std::string::const_iterator end)
+{
+    using details::padding_info;
+    using details::scoped_padder;
+    const size_t max_width = 64;
+    if (it == end)
     {
-        using details::padding_info;
-        using details::scoped_pad;
-        const size_t max_width = 128;
-        if (it == end)
-        {
-            return padding_info{};
-        }
+        return padding_info{};
+    }
 
-        padding_info::pad_side side;
-        switch (*it)
-        {
-        case '-':
-            side = padding_info::right;
-            ++it;
-            break;
-        case '=':
-            side = padding_info::center;
-            ++it;
-            break;
-        default:
-            side = details::padding_info::left;
-            break;
-        }
+    padding_info::pad_side side;
+    switch (*it)
+    {
+    case '-':
+        side = padding_info::pad_side::right;
+        ++it;
+        break;
+    case '=':
+        side = padding_info::pad_side::center;
+        ++it;
+        break;
+    default:
+        side = details::padding_info::pad_side::left;
+        break;
+    }
 
-        if (it == end || !std::isdigit(static_cast<unsigned char>(*it)))
-        {
-            return padding_info{0, side};
-        }
+    if (it == end || !std::isdigit(static_cast<unsigned char>(*it)))
+    {
+        return padding_info{}; // no padding if no digit found here
+    }
 
-        auto width = static_cast<size_t>(*it - '0');
-        for (++it; it != end && std::isdigit(static_cast<unsigned char>(*it)); ++it)
-        {
-            auto digit = static_cast<size_t>(*it - '0');
-            width = width * 10 + digit;
-        }
-        return details::padding_info{std::min<size_t>(width, max_width), side};
+    auto width = static_cast<size_t>(*it) - '0';
+    for (++it; it != end && std::isdigit(static_cast<unsigned char>(*it)); ++it)
+    {
+        auto digit = static_cast<size_t>(*it) - '0';
+        width = width * 10 + digit;
     }
 
-    void compile_pattern_(const std::string &pattern)
+    // search for the optional truncate marker '!'
+    bool truncate;
+    if (it != end && *it == '!')
     {
-        auto end = pattern.end();
-        std::unique_ptr<details::aggregate_formatter> user_chars;
-        formatters_.clear();
-        for (auto it = pattern.begin(); it != end; ++it)
+        truncate = true;
+        ++it;
+    }
+    else
+    {
+        truncate = false;
+    }
+    return details::padding_info{std::min<size_t>(width, max_width), side, truncate};
+}
+
+SPDLOG_INLINE void pattern_formatter::compile_pattern_(const std::string &pattern)
+{
+    auto end = pattern.end();
+    std::unique_ptr<details::aggregate_formatter> user_chars;
+    formatters_.clear();
+    for (auto it = pattern.begin(); it != end; ++it)
+    {
+        if (*it == '%')
         {
-            if (*it == '%')
+            if (user_chars) // append user chars found so far
             {
-                if (user_chars) // append user chars found so far
-                {
-                    formatters_.push_back(std::move(user_chars));
-                }
+                formatters_.push_back(std::move(user_chars));
+            }
 
-                auto padding = handle_padspec_(++it, end);
+            auto padding = handle_padspec_(++it, end);
 
-                if (it != end)
+            if (it != end)
+            {
+                if (padding.enabled())
                 {
-                    handle_flag_(*it, padding);
+                    handle_flag_<details::scoped_padder>(*it, padding);
                 }
                 else
                 {
-                    break;
+                    handle_flag_<details::null_scoped_padder>(*it, padding);
                 }
             }
-            else // chars not following the % sign should be displayed as is
+            else
             {
-                if (!user_chars)
-                {
-                    user_chars = details::make_unique<details::aggregate_formatter>();
-                }
-                user_chars->add_ch(*it);
+                break;
             }
         }
-        if (user_chars) // append raw chars found so far
+        else // chars not following the % sign should be displayed as is
         {
-            formatters_.push_back(std::move(user_chars));
+            if (!user_chars)
+            {
+                user_chars = details::make_unique<details::aggregate_formatter>();
+            }
+            user_chars->add_ch(*it);
         }
     }
-};
+    if (user_chars) // append raw chars found so far
+    {
+        formatters_.push_back(std::move(user_chars));
+    }
+}
 } // namespace spdlog
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/details/periodic_worker.h` & `spdlog-2.0.6/spdlog/include/spdlog/details/periodic_worker-inl.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,49 @@
-
-//
-// Copyright(c) 2018 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-// periodic worker thread - periodically executes the given callback function.
-//
-// RAII over the owned thread:
-//    creates the thread on construction.
-//    stops and joins the thread on destruction (if the thread is executing a callback, wait for it to finish first).
-
-#include <chrono>
-#include <condition_variable>
-#include <functional>
-#include <mutex>
-#include <thread>
+#ifndef SPDLOG_HEADER_ONLY
+#    include <spdlog/details/periodic_worker.h>
+#endif
+
 namespace spdlog {
 namespace details {
 
-class periodic_worker
+SPDLOG_INLINE periodic_worker::periodic_worker(const std::function<void()> &callback_fun, std::chrono::seconds interval)
 {
-public:
-    periodic_worker(const std::function<void()> &callback_fun, std::chrono::seconds interval)
+    active_ = (interval > std::chrono::seconds::zero());
+    if (!active_)
     {
-        active_ = (interval > std::chrono::seconds::zero());
-        if (!active_)
-        {
-            return;
-        }
+        return;
+    }
 
-        worker_thread_ = std::thread([this, callback_fun, interval]() {
-            for (;;)
+    worker_thread_ = std::thread([this, callback_fun, interval]() {
+        for (;;)
+        {
+            std::unique_lock<std::mutex> lock(this->mutex_);
+            if (this->cv_.wait_for(lock, interval, [this] { return !this->active_; }))
             {
-                std::unique_lock<std::mutex> lock(this->mutex_);
-                if (this->cv_.wait_for(lock, interval, [this] { return !this->active_; }))
-                {
-                    return; // active_ == false, so exit this thread
-                }
-                callback_fun();
+                return; // active_ == false, so exit this thread
             }
-        });
-    }
-
-    periodic_worker(const periodic_worker &) = delete;
-    periodic_worker &operator=(const periodic_worker &) = delete;
+            callback_fun();
+        }
+    });
+}
 
-    // stop the worker thread and join it
-    ~periodic_worker()
+// stop the worker thread and join it
+SPDLOG_INLINE periodic_worker::~periodic_worker()
+{
+    if (worker_thread_.joinable())
     {
-        if (worker_thread_.joinable())
         {
-            {
-                std::lock_guard<std::mutex> lock(mutex_);
-                active_ = false;
-            }
-            cv_.notify_one();
-            worker_thread_.join();
+            std::lock_guard<std::mutex> lock(mutex_);
+            active_ = false;
         }
+        cv_.notify_one();
+        worker_thread_.join();
     }
+}
 
-private:
-    bool active_;
-    std::thread worker_thread_;
-    std::mutex mutex_;
-    std::condition_variable cv_;
-};
 } // namespace details
 } // namespace spdlog
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/details/registry.h` & `spdlog-2.0.6/spdlog/include/spdlog/details/registry-inl.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,285 +1,313 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-// Loggers registy of unique name->logger pointer
-// An attempt to create a logger with an already existing name will be ignored
-// If user requests a non existing logger, nullptr will be returned
-// This class is thread safe
-
-#include "spdlog/common.h"
-#include "spdlog/details/periodic_worker.h"
-#include "spdlog/logger.h"
+#ifndef SPDLOG_HEADER_ONLY
+#    include <spdlog/details/registry.h>
+#endif
+
+#include <spdlog/common.h>
+#include <spdlog/details/periodic_worker.h>
+#include <spdlog/logger.h>
+#include <spdlog/pattern_formatter.h>
 
 #ifndef SPDLOG_DISABLE_DEFAULT_LOGGER
 // support for the default stdout color logger
-#ifdef _WIN32
-#include "spdlog/sinks/wincolor_sink.h"
-#else
-#include "spdlog/sinks/ansicolor_sink.h"
-#endif
+#    ifdef _WIN32
+#        include <spdlog/sinks/wincolor_sink.h>
+#    else
+#        include <spdlog/sinks/ansicolor_sink.h>
+#    endif
 #endif // SPDLOG_DISABLE_DEFAULT_LOGGER
 
 #include <chrono>
 #include <functional>
 #include <memory>
 #include <string>
 #include <unordered_map>
 
 namespace spdlog {
 namespace details {
-class thread_pool;
 
-class registry
+SPDLOG_INLINE registry::registry()
+    : formatter_(new pattern_formatter())
 {
-public:
-    registry(const registry &) = delete;
-    registry &operator=(const registry &) = delete;
 
-    void register_logger(std::shared_ptr<logger> new_logger)
-    {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        register_logger_(std::move(new_logger));
-    }
+#ifndef SPDLOG_DISABLE_DEFAULT_LOGGER
+    // create default logger (ansicolor_stdout_sink_mt or wincolor_stdout_sink_mt in windows).
+#    ifdef _WIN32
+    auto color_sink = std::make_shared<sinks::wincolor_stdout_sink_mt>();
+#    else
+    auto color_sink = std::make_shared<sinks::ansicolor_stdout_sink_mt>();
+#    endif
+
+    const char *default_logger_name = "";
+    default_logger_ = std::make_shared<spdlog::logger>(default_logger_name, std::move(color_sink));
+    loggers_[default_logger_name] = default_logger_;
 
-    void initialize_logger(std::shared_ptr<logger> new_logger)
-    {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        new_logger->set_formatter(formatter_->clone());
+#endif // SPDLOG_DISABLE_DEFAULT_LOGGER
+}
 
-        if (err_handler_)
-        {
-            new_logger->set_error_handler(err_handler_);
-        }
+SPDLOG_INLINE registry::~registry() = default;
 
-        new_logger->set_level(level_);
-        new_logger->flush_on(flush_level_);
+SPDLOG_INLINE void registry::register_logger(std::shared_ptr<logger> new_logger)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    register_logger_(std::move(new_logger));
+}
 
-        if (automatic_registration_)
-        {
-            register_logger_(std::move(new_logger));
-        }
-    }
+SPDLOG_INLINE void registry::initialize_logger(std::shared_ptr<logger> new_logger)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    new_logger->set_formatter(formatter_->clone());
 
-    std::shared_ptr<logger> get(const std::string &logger_name)
+    if (err_handler_)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        auto found = loggers_.find(logger_name);
-        return found == loggers_.end() ? nullptr : found->second;
+        new_logger->set_error_handler(err_handler_);
     }
 
-    std::shared_ptr<logger> default_logger()
-    {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        return default_logger_;
-    }
+    // set new level according to previously configured level or default level
+    auto it = log_levels_.find(new_logger->name());
+    auto new_level = it != log_levels_.end() ? it->second : global_log_level_;
+    new_logger->set_level(new_level);
 
-    // Return raw ptr to the default logger.
-    // To be used directly by the spdlog default api (e.g. spdlog::info)
-    // This make the default API faster, but cannot be used concurrently with set_default_logger().
-    // e.g do not call set_default_logger() from one thread while calling spdlog::info() from another.
-    logger *get_default_raw()
+    new_logger->flush_on(flush_level_);
+
+    if (backtrace_n_messages_ > 0)
     {
-        return default_logger_.get();
+        new_logger->enable_backtrace(backtrace_n_messages_);
     }
 
-    // set default logger.
-    // default logger is stored in default_logger_ (for faster retrieval) and in the loggers_ map.
-    void set_default_logger(std::shared_ptr<logger> new_default_logger)
+    if (automatic_registration_)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        // remove previous default logger from the map
-        if (default_logger_ != nullptr)
-        {
-            loggers_.erase(default_logger_->name());
-        }
-        if (new_default_logger != nullptr)
-        {
-            loggers_[new_default_logger->name()] = new_default_logger;
-        }
-        default_logger_ = std::move(new_default_logger);
+        register_logger_(std::move(new_logger));
     }
+}
 
-    void set_tp(std::shared_ptr<thread_pool> tp)
+SPDLOG_INLINE std::shared_ptr<logger> registry::get(const std::string &logger_name)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    auto found = loggers_.find(logger_name);
+    return found == loggers_.end() ? nullptr : found->second;
+}
+
+SPDLOG_INLINE std::shared_ptr<logger> registry::default_logger()
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    return default_logger_;
+}
+
+// Return raw ptr to the default logger.
+// To be used directly by the spdlog default api (e.g. spdlog::info)
+// This make the default API faster, but cannot be used concurrently with set_default_logger().
+// e.g do not call set_default_logger() from one thread while calling spdlog::info() from another.
+SPDLOG_INLINE logger *registry::get_default_raw()
+{
+    return default_logger_.get();
+}
+
+// set default logger.
+// default logger is stored in default_logger_ (for faster retrieval) and in the loggers_ map.
+SPDLOG_INLINE void registry::set_default_logger(std::shared_ptr<logger> new_default_logger)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    // remove previous default logger from the map
+    if (default_logger_ != nullptr)
     {
-        std::lock_guard<std::recursive_mutex> lock(tp_mutex_);
-        tp_ = std::move(tp);
+        loggers_.erase(default_logger_->name());
     }
-
-    std::shared_ptr<thread_pool> get_tp()
+    if (new_default_logger != nullptr)
     {
-        std::lock_guard<std::recursive_mutex> lock(tp_mutex_);
-        return tp_;
+        loggers_[new_default_logger->name()] = new_default_logger;
     }
+    default_logger_ = std::move(new_default_logger);
+}
+
+SPDLOG_INLINE void registry::set_tp(std::shared_ptr<thread_pool> tp)
+{
+    std::lock_guard<std::recursive_mutex> lock(tp_mutex_);
+    tp_ = std::move(tp);
+}
+
+SPDLOG_INLINE std::shared_ptr<thread_pool> registry::get_tp()
+{
+    std::lock_guard<std::recursive_mutex> lock(tp_mutex_);
+    return tp_;
+}
 
-    // Set global formatter. Each sink in each logger will get a clone of this object
-    void set_formatter(std::unique_ptr<formatter> formatter)
+// Set global formatter. Each sink in each logger will get a clone of this object
+SPDLOG_INLINE void registry::set_formatter(std::unique_ptr<formatter> formatter)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    formatter_ = std::move(formatter);
+    for (auto &l : loggers_)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        formatter_ = std::move(formatter);
-        for (auto &l : loggers_)
-        {
-            l.second->set_formatter(formatter_->clone());
-        }
+        l.second->set_formatter(formatter_->clone());
     }
+}
+
+SPDLOG_INLINE void registry::enable_backtrace(size_t n_messages)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    backtrace_n_messages_ = n_messages;
 
-    void set_level(level::level_enum log_level)
+    for (auto &l : loggers_)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        for (auto &l : loggers_)
-        {
-            l.second->set_level(log_level);
-        }
-        level_ = log_level;
+        l.second->enable_backtrace(n_messages);
     }
+}
 
-    void flush_on(level::level_enum log_level)
+SPDLOG_INLINE void registry::disable_backtrace()
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    backtrace_n_messages_ = 0;
+    for (auto &l : loggers_)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        for (auto &l : loggers_)
-        {
-            l.second->flush_on(log_level);
-        }
-        flush_level_ = log_level;
+        l.second->disable_backtrace();
     }
+}
 
-    void flush_every(std::chrono::seconds interval)
+SPDLOG_INLINE void registry::set_level(level::level_enum log_level)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    for (auto &l : loggers_)
     {
-        std::lock_guard<std::mutex> lock(flusher_mutex_);
-        std::function<void()> clbk = std::bind(&registry::flush_all, this);
-        periodic_flusher_ = details::make_unique<periodic_worker>(clbk, interval);
+        l.second->set_level(log_level);
     }
+    global_log_level_ = log_level;
+}
 
-    void set_error_handler(log_err_handler handler)
+SPDLOG_INLINE void registry::flush_on(level::level_enum log_level)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    for (auto &l : loggers_)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        for (auto &l : loggers_)
-        {
-            l.second->set_error_handler(handler);
-        }
-        err_handler_ = handler;
+        l.second->flush_on(log_level);
     }
+    flush_level_ = log_level;
+}
+
+SPDLOG_INLINE void registry::flush_every(std::chrono::seconds interval)
+{
+    std::lock_guard<std::mutex> lock(flusher_mutex_);
+    auto clbk = [this]() { this->flush_all(); };
+    periodic_flusher_ = details::make_unique<periodic_worker>(clbk, interval);
+}
 
-    void apply_all(const std::function<void(const std::shared_ptr<logger>)> &fun)
+SPDLOG_INLINE void registry::set_error_handler(err_handler handler)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    for (auto &l : loggers_)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        for (auto &l : loggers_)
-        {
-            fun(l.second);
-        }
+        l.second->set_error_handler(handler);
     }
+    err_handler_ = std::move(handler);
+}
 
-    void flush_all()
+SPDLOG_INLINE void registry::apply_all(const std::function<void(const std::shared_ptr<logger>)> &fun)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    for (auto &l : loggers_)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        for (auto &l : loggers_)
-        {
-            l.second->flush();
-        }
+        fun(l.second);
     }
+}
 
-    void drop(const std::string &logger_name)
+SPDLOG_INLINE void registry::flush_all()
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    for (auto &l : loggers_)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        loggers_.erase(logger_name);
-        if (default_logger_ && default_logger_->name() == logger_name)
-        {
-            default_logger_.reset();
-        }
+        l.second->flush();
     }
+}
 
-    void drop_all()
+SPDLOG_INLINE void registry::drop(const std::string &logger_name)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    loggers_.erase(logger_name);
+    if (default_logger_ && default_logger_->name() == logger_name)
     {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        loggers_.clear();
         default_logger_.reset();
     }
+}
 
-    // clean all resources and threads started by the registry
-    void shutdown()
-    {
-        {
-            std::lock_guard<std::mutex> lock(flusher_mutex_);
-            periodic_flusher_.reset();
-        }
-
-        drop_all();
-
-        {
-            std::lock_guard<std::recursive_mutex> lock(tp_mutex_);
-            tp_.reset();
-        }
-    }
+SPDLOG_INLINE void registry::drop_all()
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    loggers_.clear();
+    default_logger_.reset();
+}
 
-    std::recursive_mutex &tp_mutex()
+// clean all resources and threads started by the registry
+SPDLOG_INLINE void registry::shutdown()
+{
     {
-        return tp_mutex_;
+        std::lock_guard<std::mutex> lock(flusher_mutex_);
+        periodic_flusher_.reset();
     }
 
-    void set_automatic_registration(bool automatic_regsistration)
-    {
-        std::lock_guard<std::mutex> lock(logger_map_mutex_);
-        automatic_registration_ = automatic_regsistration;
-    }
+    drop_all();
 
-    static registry &instance()
     {
-        static registry s_instance;
-        return s_instance;
+        std::lock_guard<std::recursive_mutex> lock(tp_mutex_);
+        tp_.reset();
     }
+}
 
-private:
-    registry()
-        : formatter_(new pattern_formatter())
-    {
-
-#ifndef SPDLOG_DISABLE_DEFAULT_LOGGER
-        // create default logger (ansicolor_stdout_sink_mt or wincolor_stdout_sink_mt in windows).
-#ifdef _WIN32
-        auto color_sink = std::make_shared<sinks::wincolor_stdout_sink_mt>();
-#else
-        auto color_sink = std::make_shared<sinks::ansicolor_stdout_sink_mt>();
-#endif
-
-        const char *default_logger_name = "";
-        default_logger_ = std::make_shared<spdlog::logger>(default_logger_name, std::move(color_sink));
-        loggers_[default_logger_name] = default_logger_;
+SPDLOG_INLINE std::recursive_mutex &registry::tp_mutex()
+{
+    return tp_mutex_;
+}
 
-#endif // SPDLOG_DISABLE_DEFAULT_LOGGER
-    }
+SPDLOG_INLINE void registry::set_automatic_registration(bool automatic_registration)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    automatic_registration_ = automatic_registration;
+}
 
-    ~registry() = default;
+SPDLOG_INLINE void registry::set_levels(log_levels levels, level::level_enum *global_level)
+{
+    std::lock_guard<std::mutex> lock(logger_map_mutex_);
+    log_levels_ = std::move(levels);
+    auto global_level_requested = global_level != nullptr;
+    global_log_level_ = global_level_requested ? *global_level : global_log_level_;
 
-    void throw_if_exists_(const std::string &logger_name)
+    for (auto &logger : loggers_)
     {
-        if (loggers_.find(logger_name) != loggers_.end())
+        auto logger_entry = log_levels_.find(logger.first);
+        if (logger_entry != log_levels_.end())
+        {
+            logger.second->set_level(logger_entry->second);
+        }
+        else if (global_level_requested)
         {
-            throw spdlog_ex("logger with name '" + logger_name + "' already exists");
+            logger.second->set_level(*global_level);
         }
     }
+}
 
-    void register_logger_(std::shared_ptr<logger> new_logger)
+SPDLOG_INLINE registry &registry::instance()
+{
+    static registry s_instance;
+    return s_instance;
+}
+
+SPDLOG_INLINE void registry::throw_if_exists_(const std::string &logger_name)
+{
+    if (loggers_.find(logger_name) != loggers_.end())
     {
-        auto logger_name = new_logger->name();
-        throw_if_exists_(logger_name);
-        loggers_[logger_name] = std::move(new_logger);
-    }
-
-    std::mutex logger_map_mutex_, flusher_mutex_;
-    std::recursive_mutex tp_mutex_;
-    std::unordered_map<std::string, std::shared_ptr<logger>> loggers_;
-    std::unique_ptr<formatter> formatter_;
-    level::level_enum level_ = spdlog::logger::default_level();
-    level::level_enum flush_level_ = level::off;
-    log_err_handler err_handler_;
-    std::shared_ptr<thread_pool> tp_;
-    std::unique_ptr<periodic_worker> periodic_flusher_;
-    std::shared_ptr<logger> default_logger_;
-    bool automatic_registration_ = true;
-};
+        throw_spdlog_ex("logger with name '" + logger_name + "' already exists");
+    }
+}
+
+SPDLOG_INLINE void registry::register_logger_(std::shared_ptr<logger> new_logger)
+{
+    auto logger_name = new_logger->name();
+    throw_if_exists_(logger_name);
+    loggers_[logger_name] = std::move(new_logger);
+}
 
 } // namespace details
 } // namespace spdlog
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/format.h` & `spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/format.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,504 +1,728 @@
 /*
  Formatting library for C++
 
  Copyright (c) 2012 - present, Victor Zverovich
- All rights reserved.
 
- Redistribution and use in source and binary forms, with or without
- modification, are permitted provided that the following conditions are met:
-
- 1. Redistributions of source code must retain the above copyright notice, this
-    list of conditions and the following disclaimer.
- 2. Redistributions in binary form must reproduce the above copyright notice,
-    this list of conditions and the following disclaimer in the documentation
-    and/or other materials provided with the distribution.
-
- THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
- ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
- WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
- DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
- ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
- (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
- LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
- ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
- (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
- SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ Permission is hereby granted, free of charge, to any person obtaining
+ a copy of this software and associated documentation files (the
+ "Software"), to deal in the Software without restriction, including
+ without limitation the rights to use, copy, modify, merge, publish,
+ distribute, sublicense, and/or sell copies of the Software, and to
+ permit persons to whom the Software is furnished to do so, subject to
+ the following conditions:
+
+ The above copyright notice and this permission notice shall be
+ included in all copies or substantial portions of the Software.
+
+ THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+ EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+ MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+ NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+ LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+ OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+ WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+ --- Optional exception to the license ---
+
+ As an exception, if, as a result of your compiling your source code, portions
+ of this Software are embedded into a machine-executable object form of such
+ source code, you may redistribute such embedded portions in such object form
+ without including the above copyright and permission notices.
  */
 
 #ifndef FMT_FORMAT_H_
 #define FMT_FORMAT_H_
 
-#include <algorithm>
-#include <cassert>
-#include <cmath>
-#include <cstring>
-#include <limits>
-#include <memory>
-#include <stdexcept>
-#include <stdint.h>
+#include <cmath>         // std::signbit
+#include <cstdint>       // uint32_t
+#include <limits>        // std::numeric_limits
+#include <memory>        // std::uninitialized_copy
+#include <stdexcept>     // std::runtime_error
+#include <system_error>  // std::system_error
+#include <utility>       // std::swap
 
-#ifdef __clang__
-# define FMT_CLANG_VERSION (__clang_major__ * 100 + __clang_minor__)
-#else
-# define FMT_CLANG_VERSION 0
+#ifdef __cpp_lib_bit_cast
+#  include <bit>  // std::bitcast
 #endif
 
-#ifdef __INTEL_COMPILER
-# define FMT_ICC_VERSION __INTEL_COMPILER
-#elif defined(__ICL)
-# define FMT_ICC_VERSION __ICL
+#include "core.h"
+
+#if FMT_GCC_VERSION
+#  define FMT_GCC_VISIBILITY_HIDDEN __attribute__((visibility("hidden")))
 #else
-# define FMT_ICC_VERSION 0
+#  define FMT_GCC_VISIBILITY_HIDDEN
 #endif
 
 #ifdef __NVCC__
-# define FMT_CUDA_VERSION (__CUDACC_VER_MAJOR__ * 100 + __CUDACC_VER_MINOR__)
+#  define FMT_CUDA_VERSION (__CUDACC_VER_MAJOR__ * 100 + __CUDACC_VER_MINOR__)
 #else
-# define FMT_CUDA_VERSION 0
-#endif
-
-#include "core.h"
-
-#if FMT_GCC_VERSION >= 406 || FMT_CLANG_VERSION
-# pragma GCC diagnostic push
-
-// Disable the warning about declaration shadowing because it affects too
-// many valid cases.
-# pragma GCC diagnostic ignored "-Wshadow"
-
-// Disable the warning about nonliteral format strings because we construct
-// them dynamically when falling back to snprintf for FP formatting.
-# pragma GCC diagnostic ignored "-Wformat-nonliteral"
+#  define FMT_CUDA_VERSION 0
 #endif
 
-# if FMT_CLANG_VERSION
-#  pragma GCC diagnostic ignored "-Wgnu-string-literal-operator-template"
-# endif
-
-#ifdef _SECURE_SCL
-# define FMT_SECURE_SCL _SECURE_SCL
+#ifdef __has_builtin
+#  define FMT_HAS_BUILTIN(x) __has_builtin(x)
 #else
-# define FMT_SECURE_SCL 0
+#  define FMT_HAS_BUILTIN(x) 0
 #endif
 
-#if FMT_SECURE_SCL
-# include <iterator>
-#endif
-
-#ifdef __has_builtin
-# define FMT_HAS_BUILTIN(x) __has_builtin(x)
+#if FMT_GCC_VERSION || FMT_CLANG_VERSION
+#  define FMT_NOINLINE __attribute__((noinline))
 #else
-# define FMT_HAS_BUILTIN(x) 0
+#  define FMT_NOINLINE
 #endif
 
-#ifdef __GNUC_LIBSTD__
-# define FMT_GNUC_LIBSTD_VERSION (__GNUC_LIBSTD__ * 100 + __GNUC_LIBSTD_MINOR__)
+#if FMT_MSC_VER
+#  define FMT_MSC_DEFAULT = default
+#else
+#  define FMT_MSC_DEFAULT
 #endif
 
 #ifndef FMT_THROW
-# if FMT_EXCEPTIONS
-#  if FMT_MSC_VER
+#  if FMT_EXCEPTIONS
+#    if FMT_MSC_VER || FMT_NVCC
 FMT_BEGIN_NAMESPACE
-namespace internal {
-template <typename Exception>
-inline void do_throw(const Exception &x) {
-  // Silence unreachable code warnings in MSVC because these are nearly
-  // impossible to fix in a generic code.
+namespace detail {
+template <typename Exception> inline void do_throw(const Exception& x) {
+  // Silence unreachable code warnings in MSVC and NVCC because these
+  // are nearly impossible to fix in a generic code.
   volatile bool b = true;
-  if (b)
-    throw x;
-}
+  if (b) throw x;
 }
+}  // namespace detail
 FMT_END_NAMESPACE
-#   define FMT_THROW(x) fmt::internal::do_throw(x)
+#      define FMT_THROW(x) detail::do_throw(x)
+#    else
+#      define FMT_THROW(x) throw x
+#    endif
 #  else
-#   define FMT_THROW(x) throw x
+#    define FMT_THROW(x)               \
+      do {                             \
+        FMT_ASSERT(false, (x).what()); \
+      } while (false)
 #  endif
-# else
-#  define FMT_THROW(x) do { static_cast<void>(sizeof(x)); assert(false); } while(false);
-# endif
 #endif
 
-#ifndef FMT_USE_USER_DEFINED_LITERALS
-// For Intel's compiler and NVIDIA's compiler both it and the system gcc/msc
-// must support UDLs.
-# if (FMT_HAS_FEATURE(cxx_user_literals) || \
-      FMT_GCC_VERSION >= 407 || FMT_MSC_VER >= 1900) && \
-      (!(FMT_ICC_VERSION || FMT_CUDA_VERSION) || \
-       FMT_ICC_VERSION >= 1500 || FMT_CUDA_VERSION >= 700)
-#  define FMT_USE_USER_DEFINED_LITERALS 1
-# else
-#  define FMT_USE_USER_DEFINED_LITERALS 0
-# endif
-#endif
-
-// EDG C++ Front End based compilers (icc, nvcc) do not currently support UDL
-// templates.
-#if FMT_USE_USER_DEFINED_LITERALS && \
-    FMT_ICC_VERSION == 0 && \
-    FMT_CUDA_VERSION == 0 && \
-    ((FMT_GCC_VERSION >= 600 && __cplusplus >= 201402L) || \
-    (defined(FMT_CLANG_VERSION) && FMT_CLANG_VERSION >= 304))
-# define FMT_UDL_TEMPLATE 1
+#if FMT_EXCEPTIONS
+#  define FMT_TRY try
+#  define FMT_CATCH(x) catch (x)
 #else
-# define FMT_UDL_TEMPLATE 0
+#  define FMT_TRY if (true)
+#  define FMT_CATCH(x) if (false)
+#endif
+
+#ifndef FMT_MAYBE_UNUSED
+#  if FMT_HAS_CPP17_ATTRIBUTE(maybe_unused)
+#    define FMT_MAYBE_UNUSED [[maybe_unused]]
+#  else
+#    define FMT_MAYBE_UNUSED
+#  endif
 #endif
 
-#ifndef FMT_USE_EXTERN_TEMPLATES
-# ifndef FMT_HEADER_ONLY
-#  define FMT_USE_EXTERN_TEMPLATES \
-     ((FMT_CLANG_VERSION >= 209 && __cplusplus >= 201103L) || \
-      (FMT_GCC_VERSION >= 303 && FMT_HAS_GXX_CXX11))
-# else
-#  define FMT_USE_EXTERN_TEMPLATES 0
-# endif
-#endif
-
-#if FMT_HAS_GXX_CXX11 || FMT_HAS_FEATURE(cxx_trailing_return) || \
-    FMT_MSC_VER >= 1600
-# define FMT_USE_TRAILING_RETURN 1
+// Workaround broken [[deprecated]] in the Intel, PGI and NVCC compilers.
+#if FMT_ICC_VERSION || defined(__PGI) || FMT_NVCC
+#  define FMT_DEPRECATED_ALIAS
 #else
-# define FMT_USE_TRAILING_RETURN 0
+#  define FMT_DEPRECATED_ALIAS FMT_DEPRECATED
+#endif
+
+#ifndef FMT_USE_USER_DEFINED_LITERALS
+// EDG based compilers (Intel, NVIDIA, Elbrus, etc), GCC and MSVC support UDLs.
+#  if (FMT_HAS_FEATURE(cxx_user_literals) || FMT_GCC_VERSION >= 407 || \
+       FMT_MSC_VER >= 1900) &&                                         \
+      (!defined(__EDG_VERSION__) || __EDG_VERSION__ >= /* UDL feature */ 480)
+#    define FMT_USE_USER_DEFINED_LITERALS 1
+#  else
+#    define FMT_USE_USER_DEFINED_LITERALS 0
+#  endif
 #endif
 
-#ifndef FMT_USE_GRISU
-# define FMT_USE_GRISU 0
-//# define FMT_USE_GRISU std::numeric_limits<double>::is_iec559
+// Defining FMT_REDUCE_INT_INSTANTIATIONS to 1, will reduce the number of
+// integer formatter template instantiations to just one by only using the
+// largest integer type. This results in a reduction in binary size but will
+// cause a decrease in integer formatting performance.
+#if !defined(FMT_REDUCE_INT_INSTANTIATIONS)
+#  define FMT_REDUCE_INT_INSTANTIATIONS 0
 #endif
 
 // __builtin_clz is broken in clang with Microsoft CodeGen:
-// https://github.com/fmtlib/fmt/issues/519
-#ifndef _MSC_VER
-# if FMT_GCC_VERSION >= 400 || FMT_HAS_BUILTIN(__builtin_clz)
-#  define FMT_BUILTIN_CLZ(n) __builtin_clz(n)
-# endif
-
-# if FMT_GCC_VERSION >= 400 || FMT_HAS_BUILTIN(__builtin_clzll)
-#  define FMT_BUILTIN_CLZLL(n) __builtin_clzll(n)
-# endif
+// https://github.com/fmtlib/fmt/issues/519.
+#if !FMT_MSC_VER
+#  if FMT_HAS_BUILTIN(__builtin_clz) || FMT_GCC_VERSION || FMT_ICC_VERSION
+#    define FMT_BUILTIN_CLZ(n) __builtin_clz(n)
+#  endif
+#  if FMT_HAS_BUILTIN(__builtin_clzll) || FMT_GCC_VERSION || FMT_ICC_VERSION
+#    define FMT_BUILTIN_CLZLL(n) __builtin_clzll(n)
+#  endif
+#endif
+
+// __builtin_ctz is broken in Intel Compiler Classic on Windows:
+// https://github.com/fmtlib/fmt/issues/2510.
+#ifndef __ICL
+#  if FMT_HAS_BUILTIN(__builtin_ctz) || FMT_GCC_VERSION || FMT_ICC_VERSION
+#    define FMT_BUILTIN_CTZ(n) __builtin_ctz(n)
+#  endif
+#  if FMT_HAS_BUILTIN(__builtin_ctzll) || FMT_GCC_VERSION || FMT_ICC_VERSION
+#    define FMT_BUILTIN_CTZLL(n) __builtin_ctzll(n)
+#  endif
+#endif
+
+#if FMT_MSC_VER
+#  include <intrin.h>  // _BitScanReverse[64], _BitScanForward[64], _umul128
 #endif
 
 // Some compilers masquerade as both MSVC and GCC-likes or otherwise support
 // __builtin_clz and __builtin_clzll, so only define FMT_BUILTIN_CLZ using the
 // MSVC intrinsics if the clz and clzll builtins are not available.
-#if FMT_MSC_VER && !defined(FMT_BUILTIN_CLZLL) && !defined(_MANAGED)
-# include <intrin.h>  // _BitScanReverse, _BitScanReverse64
-
+#if FMT_MSC_VER && !defined(FMT_BUILTIN_CLZLL) && !defined(FMT_BUILTIN_CTZLL)
 FMT_BEGIN_NAMESPACE
-namespace internal {
+namespace detail {
 // Avoid Clang with Microsoft CodeGen's -Wunknown-pragmas warning.
-# ifndef __clang__
-#  pragma intrinsic(_BitScanReverse)
-# endif
-inline uint32_t clz(uint32_t x) {
+#  if !defined(__clang__)
+#    pragma intrinsic(_BitScanForward)
+#    pragma intrinsic(_BitScanReverse)
+#    if defined(_WIN64)
+#      pragma intrinsic(_BitScanForward64)
+#      pragma intrinsic(_BitScanReverse64)
+#    endif
+#  endif
+
+inline auto clz(uint32_t x) -> int {
   unsigned long r = 0;
   _BitScanReverse(&r, x);
-
-  assert(x != 0);
+  FMT_ASSERT(x != 0, "");
   // Static analysis complains about using uninitialized data
   // "r", but the only way that can happen is if "x" is 0,
   // which the callers guarantee to not happen.
-# pragma warning(suppress: 6102)
-  return 31 - r;
+  FMT_MSC_WARNING(suppress : 6102)
+  return 31 ^ static_cast<int>(r);
 }
-# define FMT_BUILTIN_CLZ(n) fmt::internal::clz(n)
-
-# if defined(_WIN64) && !defined(__clang__)
-#  pragma intrinsic(_BitScanReverse64)
-# endif
+#  define FMT_BUILTIN_CLZ(n) detail::clz(n)
 
-inline uint32_t clzll(uint64_t x) {
+inline auto clzll(uint64_t x) -> int {
   unsigned long r = 0;
-# ifdef _WIN64
+#  ifdef _WIN64
   _BitScanReverse64(&r, x);
-# else
+#  else
   // Scan the high 32 bits.
-  if (_BitScanReverse(&r, static_cast<uint32_t>(x >> 32)))
-    return 63 - (r + 32);
-
+  if (_BitScanReverse(&r, static_cast<uint32_t>(x >> 32))) return 63 ^ (r + 32);
   // Scan the low 32 bits.
   _BitScanReverse(&r, static_cast<uint32_t>(x));
-# endif
+#  endif
+  FMT_ASSERT(x != 0, "");
+  FMT_MSC_WARNING(suppress : 6102)  // Suppress a bogus static analysis warning.
+  return 63 ^ static_cast<int>(r);
+}
+#  define FMT_BUILTIN_CLZLL(n) detail::clzll(n)
 
-  assert(x != 0);
-  // Static analysis complains about using uninitialized data
-  // "r", but the only way that can happen is if "x" is 0,
-  // which the callers guarantee to not happen.
-# pragma warning(suppress: 6102)
-  return 63 - r;
+inline auto ctz(uint32_t x) -> int {
+  unsigned long r = 0;
+  _BitScanForward(&r, x);
+  FMT_ASSERT(x != 0, "");
+  FMT_MSC_WARNING(suppress : 6102)  // Suppress a bogus static analysis warning.
+  return static_cast<int>(r);
 }
-# define FMT_BUILTIN_CLZLL(n) fmt::internal::clzll(n)
+#  define FMT_BUILTIN_CTZ(n) detail::ctz(n)
+
+inline auto ctzll(uint64_t x) -> int {
+  unsigned long r = 0;
+  FMT_ASSERT(x != 0, "");
+  FMT_MSC_WARNING(suppress : 6102)  // Suppress a bogus static analysis warning.
+#  ifdef _WIN64
+  _BitScanForward64(&r, x);
+#  else
+  // Scan the low 32 bits.
+  if (_BitScanForward(&r, static_cast<uint32_t>(x))) return static_cast<int>(r);
+  // Scan the high 32 bits.
+  _BitScanForward(&r, static_cast<uint32_t>(x >> 32));
+  r += 32;
+#  endif
+  return static_cast<int>(r);
 }
+#  define FMT_BUILTIN_CTZLL(n) detail::ctzll(n)
+}  // namespace detail
 FMT_END_NAMESPACE
 #endif
 
-FMT_BEGIN_NAMESPACE
-namespace internal {
-
-// An equivalent of `*reinterpret_cast<Dest*>(&source)` that doesn't produce
-// undefined behavior (e.g. due to type aliasing).
-// Example: uint64_t d = bit_cast<uint64_t>(2.718);
-template <typename Dest, typename Source>
-inline Dest bit_cast(const Source& source) {
-  static_assert(sizeof(Dest) == sizeof(Source), "size mismatch");
-  Dest dest;
-  std::memcpy(&dest, &source, sizeof(dest));
-  return dest;
-}
-
-// An implementation of begin and end for pre-C++11 compilers such as gcc 4.
-template <typename C>
-FMT_CONSTEXPR auto begin(const C &c) -> decltype(c.begin()) {
-  return c.begin();
-}
-template <typename T, std::size_t N>
-FMT_CONSTEXPR T *begin(T (&array)[N]) FMT_NOEXCEPT { return array; }
-template <typename C>
-FMT_CONSTEXPR auto end(const C &c) -> decltype(c.end()) { return c.end(); }
-template <typename T, std::size_t N>
-FMT_CONSTEXPR T *end(T (&array)[N]) FMT_NOEXCEPT { return array + N; }
-
-// For std::result_of in gcc 4.4.
-template <typename Result>
-struct function {
-  template <typename T>
-  struct result { typedef Result type; };
-};
-
-struct dummy_int {
-  int data[2];
-  operator int() const { return 0; }
-};
-typedef std::numeric_limits<internal::dummy_int> fputil;
-
-// Dummy implementations of system functions called if the latter are not
-// available.
-inline dummy_int isinf(...) { return dummy_int(); }
-inline dummy_int _finite(...) { return dummy_int(); }
-inline dummy_int isnan(...) { return dummy_int(); }
-inline dummy_int _isnan(...) { return dummy_int(); }
-
-template <typename Allocator>
-typename Allocator::value_type *allocate(Allocator& alloc, std::size_t n) {
-#if __cplusplus >= 201103L || FMT_MSC_VER >= 1700
-  return std::allocator_traits<Allocator>::allocate(alloc, n);
+#ifdef FMT_HEADER_ONLY
+#  define FMT_HEADER_ONLY_CONSTEXPR20 FMT_CONSTEXPR20
 #else
-  return alloc.allocate(n);
+#  define FMT_HEADER_ONLY_CONSTEXPR20
 #endif
-}
-
-// A helper function to suppress bogus "conditional expression is constant"
-// warnings.
-template <typename T>
-inline T const_check(T value) { return value; }
-}  // namespace internal
-FMT_END_NAMESPACE
-
-namespace std {
-// Standard permits specialization of std::numeric_limits. This specialization
-// is used to resolve ambiguity between isinf and std::isinf in glibc:
-// https://gcc.gnu.org/bugzilla/show_bug.cgi?id=48891
-// and the same for isnan.
-template <>
-class numeric_limits<fmt::internal::dummy_int> :
-    public std::numeric_limits<int> {
- public:
-  // Portable version of isinf.
-  template <typename T>
-  static bool isinfinity(T x) {
-    using namespace fmt::internal;
-    // The resolution "priority" is:
-    // isinf macro > std::isinf > ::isinf > fmt::internal::isinf
-    if (const_check(sizeof(isinf(x)) != sizeof(fmt::internal::dummy_int)))
-      return isinf(x) != 0;
-    return !_finite(static_cast<double>(x));
-  }
-
-  // Portable version of isnan.
-  template <typename T>
-  static bool isnotanumber(T x) {
-    using namespace fmt::internal;
-    if (const_check(sizeof(isnan(x)) != sizeof(fmt::internal::dummy_int)))
-      return isnan(x) != 0;
-    return _isnan(static_cast<double>(x)) != 0;
-  }
-};
-}  // namespace std
 
 FMT_BEGIN_NAMESPACE
-template <typename Range>
-class basic_writer;
+namespace detail {
 
-template <typename OutputIt, typename T = typename OutputIt::value_type>
-class output_range {
+template <typename Streambuf> class formatbuf : public Streambuf {
  private:
-  OutputIt it_;
+  using char_type = typename Streambuf::char_type;
+  using streamsize = decltype(std::declval<Streambuf>().sputn(nullptr, 0));
+  using int_type = typename Streambuf::int_type;
+  using traits_type = typename Streambuf::traits_type;
 
-  // Unused yet.
-  typedef void sentinel;
-  sentinel end() const;
+  buffer<char_type>& buffer_;
 
  public:
-  typedef OutputIt iterator;
-  typedef T value_type;
+  explicit formatbuf(buffer<char_type>& buf) : buffer_(buf) {}
 
-  explicit output_range(OutputIt it): it_(it) {}
-  OutputIt begin() const { return it_; }
-};
+ protected:
+  // The put area is always empty. This makes the implementation simpler and has
+  // the advantage that the streambuf and the buffer are always in sync and
+  // sputc never writes into uninitialized memory. A disadvantage is that each
+  // call to sputc always results in a (virtual) call to overflow. There is no
+  // disadvantage here for sputn since this always results in a call to xsputn.
 
-// A range where begin() returns back_insert_iterator.
-template <typename Container>
-class back_insert_range:
-    public output_range<std::back_insert_iterator<Container>> {
-  typedef output_range<std::back_insert_iterator<Container>> base;
- public:
-  typedef typename Container::value_type value_type;
+  auto overflow(int_type ch) -> int_type override {
+    if (!traits_type::eq_int_type(ch, traits_type::eof()))
+      buffer_.push_back(static_cast<char_type>(ch));
+    return ch;
+  }
 
-  back_insert_range(Container &c): base(std::back_inserter(c)) {}
-  back_insert_range(typename base::iterator it): base(it) {}
+  auto xsputn(const char_type* s, streamsize count) -> streamsize override {
+    buffer_.append(s, s + count);
+    return count;
+  }
 };
 
-typedef basic_writer<back_insert_range<internal::buffer>> writer;
-typedef basic_writer<back_insert_range<internal::wbuffer>> wwriter;
+// Implementation of std::bit_cast for pre-C++20.
+template <typename To, typename From>
+FMT_CONSTEXPR20 auto bit_cast(const From& from) -> To {
+  static_assert(sizeof(To) == sizeof(From), "size mismatch");
+#ifdef __cpp_lib_bit_cast
+  if (is_constant_evaluated()) return std::bit_cast<To>(from);
+#endif
+  auto to = To();
+  std::memcpy(&to, &from, sizeof(to));
+  return to;
+}
 
-/** A formatting error such as invalid format string. */
-class format_error : public std::runtime_error {
- public:
-  explicit format_error(const char *message)
-  : std::runtime_error(message) {}
+inline auto is_big_endian() -> bool {
+#ifdef _WIN32
+  return false;
+#elif defined(__BIG_ENDIAN__)
+  return true;
+#elif defined(__BYTE_ORDER__) && defined(__ORDER_BIG_ENDIAN__)
+  return __BYTE_ORDER__ == __ORDER_BIG_ENDIAN__;
+#else
+  struct bytes {
+    char data[sizeof(int)];
+  };
+  return bit_cast<bytes>(1).data[0] == 0;
+#endif
+}
+
+// A fallback implementation of uintptr_t for systems that lack it.
+struct fallback_uintptr {
+  unsigned char value[sizeof(void*)];
 
-  explicit format_error(const std::string &message)
-  : std::runtime_error(message) {}
+  fallback_uintptr() = default;
+  explicit fallback_uintptr(const void* p) {
+    *this = bit_cast<fallback_uintptr>(p);
+    if (const_check(is_big_endian())) {
+      for (size_t i = 0, j = sizeof(void*) - 1; i < j; ++i, --j)
+        std::swap(value[i], value[j]);
+    }
+  }
 };
+#ifdef UINTPTR_MAX
+using uintptr_t = ::uintptr_t;
+inline auto to_uintptr(const void* p) -> uintptr_t {
+  return bit_cast<uintptr_t>(p);
+}
+#else
+using uintptr_t = fallback_uintptr;
+inline auto to_uintptr(const void* p) -> fallback_uintptr {
+  return fallback_uintptr(p);
+}
+#endif
+
+// Returns the largest possible value for type T. Same as
+// std::numeric_limits<T>::max() but shorter and not affected by the max macro.
+template <typename T> constexpr auto max_value() -> T {
+  return (std::numeric_limits<T>::max)();
+}
+template <typename T> constexpr auto num_bits() -> int {
+  return std::numeric_limits<T>::digits;
+}
+// std::numeric_limits<T>::digits may return 0 for 128-bit ints.
+template <> constexpr auto num_bits<int128_t>() -> int { return 128; }
+template <> constexpr auto num_bits<uint128_t>() -> int { return 128; }
+template <> constexpr auto num_bits<fallback_uintptr>() -> int {
+  return static_cast<int>(sizeof(void*) *
+                          std::numeric_limits<unsigned char>::digits);
+}
 
-namespace internal {
+FMT_INLINE void assume(bool condition) {
+  (void)condition;
+#if FMT_HAS_BUILTIN(__builtin_assume)
+  __builtin_assume(condition);
+#endif
+}
 
-#if FMT_SECURE_SCL
+// An approximation of iterator_t for pre-C++20 systems.
 template <typename T>
-struct checked { typedef stdext::checked_array_iterator<T*> type; };
+using iterator_t = decltype(std::begin(std::declval<T&>()));
+template <typename T> using sentinel_t = decltype(std::end(std::declval<T&>()));
+
+// A workaround for std::string not having mutable data() until C++17.
+template <typename Char>
+inline auto get_data(std::basic_string<Char>& s) -> Char* {
+  return &s[0];
+}
+template <typename Container>
+inline auto get_data(Container& c) -> typename Container::value_type* {
+  return c.data();
+}
 
-// Make a checked iterator to avoid warnings on MSVC.
+#if defined(_SECURE_SCL) && _SECURE_SCL
+// Make a checked iterator to avoid MSVC warnings.
+template <typename T> using checked_ptr = stdext::checked_array_iterator<T*>;
 template <typename T>
-inline stdext::checked_array_iterator<T*> make_checked(T *p, std::size_t size) {
+constexpr auto make_checked(T* p, size_t size) -> checked_ptr<T> {
   return {p, size};
 }
 #else
-template <typename T>
-struct checked { typedef T *type; };
-template <typename T>
-inline T *make_checked(T *p, std::size_t) { return p; }
+template <typename T> using checked_ptr = T*;
+template <typename T> constexpr auto make_checked(T* p, size_t) -> T* {
+  return p;
+}
 #endif
 
+// Attempts to reserve space for n extra characters in the output range.
+// Returns a pointer to the reserved range or a reference to it.
+template <typename Container, FMT_ENABLE_IF(is_contiguous<Container>::value)>
+#if FMT_CLANG_VERSION >= 307 && !FMT_ICC_VERSION
+__attribute__((no_sanitize("undefined")))
+#endif
+inline auto
+reserve(std::back_insert_iterator<Container> it, size_t n)
+    -> checked_ptr<typename Container::value_type> {
+  Container& c = get_container(it);
+  size_t size = c.size();
+  c.resize(size + n);
+  return make_checked(get_data(c) + size, n);
+}
+
 template <typename T>
-template <typename U>
-void basic_buffer<T>::append(const U *begin, const U *end) {
-  std::size_t new_size = size_ + internal::to_unsigned(end - begin);
-  reserve(new_size);
-  std::uninitialized_copy(begin, end,
-                          internal::make_checked(ptr_, capacity_) + size_);
-  size_ = new_size;
-}
-}  // namespace internal
-
-// C++20 feature test, since r346892 Clang considers char8_t a fundamental
-// type in this mode. If this is the case __cpp_char8_t will be defined.
-#if !defined(__cpp_char8_t)
-// A UTF-8 code unit type.
-enum char8_t: unsigned char {};
+inline auto reserve(buffer_appender<T> it, size_t n) -> buffer_appender<T> {
+  buffer<T>& buf = get_container(it);
+  buf.try_reserve(buf.size() + n);
+  return it;
+}
+
+template <typename Iterator>
+constexpr auto reserve(Iterator& it, size_t) -> Iterator& {
+  return it;
+}
+
+template <typename OutputIt>
+using reserve_iterator =
+    remove_reference_t<decltype(reserve(std::declval<OutputIt&>(), 0))>;
+
+template <typename T, typename OutputIt>
+constexpr auto to_pointer(OutputIt, size_t) -> T* {
+  return nullptr;
+}
+template <typename T> auto to_pointer(buffer_appender<T> it, size_t n) -> T* {
+  buffer<T>& buf = get_container(it);
+  auto size = buf.size();
+  if (buf.capacity() < size + n) return nullptr;
+  buf.try_resize(size + n);
+  return buf.data() + size;
+}
+
+template <typename Container, FMT_ENABLE_IF(is_contiguous<Container>::value)>
+inline auto base_iterator(std::back_insert_iterator<Container>& it,
+                          checked_ptr<typename Container::value_type>)
+    -> std::back_insert_iterator<Container> {
+  return it;
+}
+
+template <typename Iterator>
+constexpr auto base_iterator(Iterator, Iterator it) -> Iterator {
+  return it;
+}
+
+// <algorithm> is spectacularly slow to compile in C++20 so use a simple fill_n
+// instead (#1998).
+template <typename OutputIt, typename Size, typename T>
+FMT_CONSTEXPR auto fill_n(OutputIt out, Size count, const T& value)
+    -> OutputIt {
+  for (Size i = 0; i < count; ++i) *out++ = value;
+  return out;
+}
+template <typename T, typename Size>
+FMT_CONSTEXPR20 auto fill_n(T* out, Size count, char value) -> T* {
+  if (is_constant_evaluated()) {
+    return fill_n<T*, Size, T>(out, count, value);
+  }
+  std::memset(out, value, to_unsigned(count));
+  return out + count;
+}
+
+#ifdef __cpp_char8_t
+using char8_type = char8_t;
+#else
+enum char8_type : unsigned char {};
 #endif
 
-// A UTF-8 string view.
-class u8string_view : public basic_string_view<char8_t> {
- public:
-  typedef char8_t char_type;
+template <typename OutChar, typename InputIt, typename OutputIt>
+FMT_CONSTEXPR FMT_NOINLINE auto copy_str_noinline(InputIt begin, InputIt end,
+                                                  OutputIt out) -> OutputIt {
+  return copy_str<OutChar>(begin, end, out);
+}
+
+// A public domain branchless UTF-8 decoder by Christopher Wellons:
+// https://github.com/skeeto/branchless-utf8
+/* Decode the next character, c, from s, reporting errors in e.
+ *
+ * Since this is a branchless decoder, four bytes will be read from the
+ * buffer regardless of the actual length of the next character. This
+ * means the buffer _must_ have at least three bytes of zero padding
+ * following the end of the data stream.
+ *
+ * Errors are reported in e, which will be non-zero if the parsed
+ * character was somehow invalid: invalid byte sequence, non-canonical
+ * encoding, or a surrogate half.
+ *
+ * The function returns a pointer to the next character. When an error
+ * occurs, this pointer will be a guess that depends on the particular
+ * error, but it will always advance at least one byte.
+ */
+FMT_CONSTEXPR inline auto utf8_decode(const char* s, uint32_t* c, int* e)
+    -> const char* {
+  constexpr const int masks[] = {0x00, 0x7f, 0x1f, 0x0f, 0x07};
+  constexpr const uint32_t mins[] = {4194304, 0, 128, 2048, 65536};
+  constexpr const int shiftc[] = {0, 18, 12, 6, 0};
+  constexpr const int shifte[] = {0, 6, 4, 2, 0};
+
+  int len = code_point_length(s);
+  const char* next = s + len;
+
+  // Assume a four-byte character and load four bytes. Unused bits are
+  // shifted out.
+  *c = uint32_t(s[0] & masks[len]) << 18;
+  *c |= uint32_t(s[1] & 0x3f) << 12;
+  *c |= uint32_t(s[2] & 0x3f) << 6;
+  *c |= uint32_t(s[3] & 0x3f) << 0;
+  *c >>= shiftc[len];
+
+  // Accumulate the various error conditions.
+  using uchar = unsigned char;
+  *e = (*c < mins[len]) << 6;       // non-canonical encoding
+  *e |= ((*c >> 11) == 0x1b) << 7;  // surrogate half?
+  *e |= (*c > 0x10FFFF) << 8;       // out of range?
+  *e |= (uchar(s[1]) & 0xc0) >> 2;
+  *e |= (uchar(s[2]) & 0xc0) >> 4;
+  *e |= uchar(s[3]) >> 6;
+  *e ^= 0x2a;  // top two bits of each tail byte correct?
+  *e >>= shifte[len];
+
+  return next;
+}
+
+constexpr uint32_t invalid_code_point = ~uint32_t();
+
+// Invokes f(cp, sv) for every code point cp in s with sv being the string view
+// corresponding to the code point. cp is invalid_code_point on error.
+template <typename F>
+FMT_CONSTEXPR void for_each_codepoint(string_view s, F f) {
+  auto decode = [f](const char* buf_ptr, const char* ptr) {
+    auto cp = uint32_t();
+    auto error = 0;
+    auto end = utf8_decode(buf_ptr, &cp, &error);
+    bool result = f(error ? invalid_code_point : cp,
+                    string_view(ptr, to_unsigned(end - buf_ptr)));
+    return result ? end : nullptr;
+  };
+  auto p = s.data();
+  const size_t block_size = 4;  // utf8_decode always reads blocks of 4 chars.
+  if (s.size() >= block_size) {
+    for (auto end = p + s.size() - block_size + 1; p < end;) {
+      p = decode(p, p);
+      if (!p) return;
+    }
+  }
+  if (auto num_chars_left = s.data() + s.size() - p) {
+    char buf[2 * block_size - 1] = {};
+    copy_str<char>(p, p + num_chars_left, buf);
+    const char* buf_ptr = buf;
+    do {
+      auto end = decode(buf_ptr, p);
+      if (!end) return;
+      p += end - buf_ptr;
+      buf_ptr = end;
+    } while (buf_ptr - buf < num_chars_left);
+  }
+}
 
-  u8string_view(const char *s):
-    basic_string_view<char8_t>(reinterpret_cast<const char8_t*>(s)) {}
-  u8string_view(const char *s, size_t count) FMT_NOEXCEPT:
-    basic_string_view<char8_t>(reinterpret_cast<const char8_t*>(s), count) {}
-};
+template <typename Char>
+inline auto compute_width(basic_string_view<Char> s) -> size_t {
+  return s.size();
+}
 
-#if FMT_USE_USER_DEFINED_LITERALS
-inline namespace literals {
-inline u8string_view operator"" _u(const char *s, std::size_t n) {
-  return {s, n};
+// Computes approximate display width of a UTF-8 string.
+FMT_CONSTEXPR inline size_t compute_width(string_view s) {
+  size_t num_code_points = 0;
+  // It is not a lambda for compatibility with C++14.
+  struct count_code_points {
+    size_t* count;
+    FMT_CONSTEXPR auto operator()(uint32_t cp, string_view) const -> bool {
+      *count += detail::to_unsigned(
+          1 +
+          (cp >= 0x1100 &&
+           (cp <= 0x115f ||  // Hangul Jamo init. consonants
+            cp == 0x2329 ||  // LEFT-POINTING ANGLE BRACKET
+            cp == 0x232a ||  // RIGHT-POINTING ANGLE BRACKET
+            // CJK ... Yi except IDEOGRAPHIC HALF FILL SPACE:
+            (cp >= 0x2e80 && cp <= 0xa4cf && cp != 0x303f) ||
+            (cp >= 0xac00 && cp <= 0xd7a3) ||    // Hangul Syllables
+            (cp >= 0xf900 && cp <= 0xfaff) ||    // CJK Compatibility Ideographs
+            (cp >= 0xfe10 && cp <= 0xfe19) ||    // Vertical Forms
+            (cp >= 0xfe30 && cp <= 0xfe6f) ||    // CJK Compatibility Forms
+            (cp >= 0xff00 && cp <= 0xff60) ||    // Fullwidth Forms
+            (cp >= 0xffe0 && cp <= 0xffe6) ||    // Fullwidth Forms
+            (cp >= 0x20000 && cp <= 0x2fffd) ||  // CJK
+            (cp >= 0x30000 && cp <= 0x3fffd) ||
+            // Miscellaneous Symbols and Pictographs + Emoticons:
+            (cp >= 0x1f300 && cp <= 0x1f64f) ||
+            // Supplemental Symbols and Pictographs:
+            (cp >= 0x1f900 && cp <= 0x1f9ff))));
+      return true;
+    }
+  };
+  for_each_codepoint(s, count_code_points{&num_code_points});
+  return num_code_points;
+}
+
+inline auto compute_width(basic_string_view<char8_type> s) -> size_t {
+  return compute_width(basic_string_view<char>(
+      reinterpret_cast<const char*>(s.data()), s.size()));
 }
+
+template <typename Char>
+inline auto code_point_index(basic_string_view<Char> s, size_t n) -> size_t {
+  size_t size = s.size();
+  return n < size ? n : size;
 }
+
+// Calculates the index of the nth code point in a UTF-8 string.
+inline auto code_point_index(basic_string_view<char8_type> s, size_t n)
+    -> size_t {
+  const char8_type* data = s.data();
+  size_t num_code_points = 0;
+  for (size_t i = 0, size = s.size(); i != size; ++i) {
+    if ((data[i] & 0xc0) != 0x80 && ++num_code_points > n) return i;
+  }
+  return s.size();
+}
+
+template <typename T, bool = std::is_floating_point<T>::value>
+struct is_fast_float : bool_constant<std::numeric_limits<T>::is_iec559 &&
+                                     sizeof(T) <= sizeof(double)> {};
+template <typename T> struct is_fast_float<T, false> : std::false_type {};
+
+#ifndef FMT_USE_FULL_CACHE_DRAGONBOX
+#  define FMT_USE_FULL_CACHE_DRAGONBOX 0
 #endif
 
+template <typename T>
+template <typename U>
+void buffer<T>::append(const U* begin, const U* end) {
+  while (begin != end) {
+    auto count = to_unsigned(end - begin);
+    try_reserve(size_ + count);
+    auto free_cap = capacity_ - size_;
+    if (free_cap < count) count = free_cap;
+    std::uninitialized_copy_n(begin, count, make_checked(ptr_ + size_, count));
+    size_ += count;
+    begin += count;
+  }
+}
+
+template <typename T, typename Enable = void>
+struct is_locale : std::false_type {};
+template <typename T>
+struct is_locale<T, void_t<decltype(T::classic())>> : std::true_type {};
+}  // namespace detail
+
+FMT_MODULE_EXPORT_BEGIN
+
 // The number of characters to store in the basic_memory_buffer object itself
 // to avoid dynamic memory allocation.
 enum { inline_buffer_size = 500 };
 
 /**
   \rst
   A dynamically growing memory buffer for trivially copyable/constructible types
   with the first ``SIZE`` elements stored in the object itself.
 
-  You can use one of the following typedefs for common character types:
-
-  +----------------+------------------------------+
-  | Type           | Definition                   |
-  +================+==============================+
-  | memory_buffer  | basic_memory_buffer<char>    |
-  +----------------+------------------------------+
-  | wmemory_buffer | basic_memory_buffer<wchar_t> |
-  +----------------+------------------------------+
+  You can use the ``memory_buffer`` type alias for ``char`` instead.
 
   **Example**::
 
-     fmt::memory_buffer out;
-     format_to(out, "The answer is {}.", 42);
+     auto out = fmt::memory_buffer();
+     format_to(std::back_inserter(out), "The answer is {}.", 42);
 
   This will append the following output to the ``out`` object:
 
   .. code-block:: none
 
      The answer is 42.
 
   The output can be converted to an ``std::string`` with ``to_string(out)``.
   \endrst
  */
-template <typename T, std::size_t SIZE = inline_buffer_size,
-          typename Allocator = std::allocator<T> >
-class basic_memory_buffer: private Allocator, public internal::basic_buffer<T> {
+template <typename T, size_t SIZE = inline_buffer_size,
+          typename Allocator = std::allocator<T>>
+class basic_memory_buffer final : public detail::buffer<T> {
  private:
   T store_[SIZE];
 
+  // Don't inherit from Allocator avoid generating type_info for it.
+  Allocator alloc_;
+
   // Deallocate memory allocated by the buffer.
-  void deallocate() {
+  FMT_CONSTEXPR20 void deallocate() {
     T* data = this->data();
-    if (data != store_) Allocator::deallocate(data, this->capacity());
+    if (data != store_) alloc_.deallocate(data, this->capacity());
   }
 
  protected:
-  void grow(std::size_t size) FMT_OVERRIDE;
+  FMT_CONSTEXPR20 void grow(size_t size) override;
 
  public:
-  typedef T value_type;
-  typedef const T &const_reference;
+  using value_type = T;
+  using const_reference = const T&;
 
-  explicit basic_memory_buffer(const Allocator &alloc = Allocator())
-      : Allocator(alloc) {
+  FMT_CONSTEXPR20 explicit basic_memory_buffer(
+      const Allocator& alloc = Allocator())
+      : alloc_(alloc) {
     this->set(store_, SIZE);
+    if (detail::is_constant_evaluated()) {
+      detail::fill_n(store_, SIZE, T{});
+    }
   }
-  ~basic_memory_buffer() { deallocate(); }
+  FMT_CONSTEXPR20 ~basic_memory_buffer() { deallocate(); }
 
  private:
   // Move data from other to this buffer.
-  void move(basic_memory_buffer &other) {
-    Allocator &this_alloc = *this, &other_alloc = other;
-    this_alloc = std::move(other_alloc);
+  FMT_CONSTEXPR20 void move(basic_memory_buffer& other) {
+    alloc_ = std::move(other.alloc_);
     T* data = other.data();
-    std::size_t size = other.size(), capacity = other.capacity();
+    size_t size = other.size(), capacity = other.capacity();
     if (data == other.store_) {
       this->set(store_, capacity);
-      std::uninitialized_copy(other.store_, other.store_ + size,
-                              internal::make_checked(store_, capacity));
+      if (detail::is_constant_evaluated()) {
+        detail::copy_str<T>(other.store_, other.store_ + size,
+                            detail::make_checked(store_, capacity));
+      } else {
+        std::uninitialized_copy(other.store_, other.store_ + size,
+                                detail::make_checked(store_, capacity));
+      }
     } else {
       this->set(data, capacity);
       // Set pointer to the inline array so that delete is not called
       // when deallocating.
       other.set(other.store_, 0);
     }
     this->resize(size);
@@ -507,3049 +731,2374 @@
  public:
   /**
     \rst
     Constructs a :class:`fmt::basic_memory_buffer` object moving the content
     of the other object to it.
     \endrst
    */
-  basic_memory_buffer(basic_memory_buffer &&other) {
+  FMT_CONSTEXPR20 basic_memory_buffer(basic_memory_buffer&& other)
+      FMT_NOEXCEPT {
     move(other);
   }
 
   /**
     \rst
     Moves the content of the other ``basic_memory_buffer`` object to this one.
     \endrst
    */
-  basic_memory_buffer &operator=(basic_memory_buffer &&other) {
-    assert(this != &other);
+  auto operator=(basic_memory_buffer&& other) FMT_NOEXCEPT
+      -> basic_memory_buffer& {
+    FMT_ASSERT(this != &other, "");
     deallocate();
     move(other);
     return *this;
   }
 
   // Returns a copy of the allocator associated with this buffer.
-  Allocator get_allocator() const { return *this; }
+  auto get_allocator() const -> Allocator { return alloc_; }
+
+  /**
+    Resizes the buffer to contain *count* elements. If T is a POD type new
+    elements may not be initialized.
+   */
+  FMT_CONSTEXPR20 void resize(size_t count) { this->try_resize(count); }
+
+  /** Increases the buffer capacity to *new_capacity*. */
+  void reserve(size_t new_capacity) { this->try_reserve(new_capacity); }
+
+  // Directly append data into the buffer
+  using detail::buffer<T>::append;
+  template <typename ContiguousRange>
+  void append(const ContiguousRange& range) {
+    append(range.data(), range.data() + range.size());
+  }
 };
 
-template <typename T, std::size_t SIZE, typename Allocator>
-void basic_memory_buffer<T, SIZE, Allocator>::grow(std::size_t size) {
-  std::size_t old_capacity = this->capacity();
-  std::size_t new_capacity = old_capacity + old_capacity / 2;
+template <typename T, size_t SIZE, typename Allocator>
+FMT_CONSTEXPR20 void basic_memory_buffer<T, SIZE, Allocator>::grow(
+    size_t size) {
+#ifdef FMT_FUZZ
+  if (size > 5000) throw std::runtime_error("fuzz mode - won't grow that much");
+#endif
+  const size_t max_size = std::allocator_traits<Allocator>::max_size(alloc_);
+  size_t old_capacity = this->capacity();
+  size_t new_capacity = old_capacity + old_capacity / 2;
   if (size > new_capacity)
-      new_capacity = size;
-  T *old_data = this->data();
-  T *new_data = internal::allocate<Allocator>(*this, new_capacity);
+    new_capacity = size;
+  else if (new_capacity > max_size)
+    new_capacity = size > max_size ? size : max_size;
+  T* old_data = this->data();
+  T* new_data =
+      std::allocator_traits<Allocator>::allocate(alloc_, new_capacity);
   // The following code doesn't throw, so the raw pointer above doesn't leak.
   std::uninitialized_copy(old_data, old_data + this->size(),
-                          internal::make_checked(new_data, new_capacity));
+                          detail::make_checked(new_data, new_capacity));
   this->set(new_data, new_capacity);
   // deallocate must not throw according to the standard, but even if it does,
   // the buffer already uses the new storage and will deallocate it in
   // destructor.
-  if (old_data != store_)
-    Allocator::deallocate(old_data, old_capacity);
+  if (old_data != store_) alloc_.deallocate(old_data, old_capacity);
 }
 
-typedef basic_memory_buffer<char> memory_buffer;
-typedef basic_memory_buffer<wchar_t> wmemory_buffer;
-
-namespace internal {
-
-template <typename Char>
-struct char_traits;
+using memory_buffer = basic_memory_buffer<char>;
 
-template <>
-struct char_traits<char> {
-  // Formats a floating-point number.
-  template <typename T>
-  FMT_API static int format_float(char *buffer, std::size_t size,
-      const char *format, int precision, T value);
+template <typename T, size_t SIZE, typename Allocator>
+struct is_contiguous<basic_memory_buffer<T, SIZE, Allocator>> : std::true_type {
 };
 
-template <>
-struct char_traits<wchar_t> {
-  template <typename T>
-  FMT_API static int format_float(wchar_t *buffer, std::size_t size,
-      const wchar_t *format, int precision, T value);
-};
-
-#if FMT_USE_EXTERN_TEMPLATES
-extern template int char_traits<char>::format_float<double>(
-    char *buffer, std::size_t size, const char* format, int precision,
-    double value);
-extern template int char_traits<char>::format_float<long double>(
-    char *buffer, std::size_t size, const char* format, int precision,
-    long double value);
-
-extern template int char_traits<wchar_t>::format_float<double>(
-    wchar_t *buffer, std::size_t size, const wchar_t* format, int precision,
-    double value);
-extern template int char_traits<wchar_t>::format_float<long double>(
-    wchar_t *buffer, std::size_t size, const wchar_t* format, int precision,
-    long double value);
-#endif
-
-template <typename Container>
-inline typename std::enable_if<
-  is_contiguous<Container>::value,
-  typename checked<typename Container::value_type>::type>::type
-    reserve(std::back_insert_iterator<Container> &it, std::size_t n) {
-  Container &c = internal::get_container(it);
-  std::size_t size = c.size();
-  c.resize(size + n);
-  return make_checked(&c[size], n);
+namespace detail {
+FMT_API void print(std::FILE*, string_view);
 }
 
-template <typename Iterator>
-inline Iterator &reserve(Iterator &it, std::size_t) { return it; }
-
-template <typename Char>
-class null_terminating_iterator;
-
-template <typename Char>
-FMT_CONSTEXPR_DECL const Char *pointer_from(null_terminating_iterator<Char> it);
-
-// An output iterator that counts the number of objects written to it and
-// discards them.
-template <typename T>
-class counting_iterator {
- private:
-  std::size_t count_;
-  mutable T blackhole_;
-
- public:
-  typedef std::output_iterator_tag iterator_category;
-  typedef T value_type;
-  typedef std::ptrdiff_t difference_type;
-  typedef T* pointer;
-  typedef T& reference;
-  typedef counting_iterator _Unchecked_type;  // Mark iterator as checked.
-
-  counting_iterator(): count_(0) {}
-
-  std::size_t count() const { return count_; }
-
-  counting_iterator& operator++() {
-    ++count_;
-    return *this;
-  }
-
-  counting_iterator operator++(int) {
-    auto it = *this;
-    ++*this;
-    return it;
-  }
-
-  T &operator*() const { return blackhole_; }
-};
-
-template <typename OutputIt>
-class truncating_iterator_base {
- protected:
-  OutputIt out_;
-  std::size_t limit_;
-  std::size_t count_;
-
-  truncating_iterator_base(OutputIt out, std::size_t limit)
-    : out_(out), limit_(limit), count_(0) {}
-
+/** A formatting error such as invalid format string. */
+FMT_CLASS_API
+class FMT_API format_error : public std::runtime_error {
  public:
-  typedef std::output_iterator_tag iterator_category;
-  typedef void difference_type;
-  typedef void pointer;
-  typedef void reference;
-  typedef truncating_iterator_base _Unchecked_type; // Mark iterator as checked.
-
-  OutputIt base() const { return out_; }
-  std::size_t count() const { return count_; }
+  explicit format_error(const char* message) : std::runtime_error(message) {}
+  explicit format_error(const std::string& message)
+      : std::runtime_error(message) {}
+  format_error(const format_error&) = default;
+  format_error& operator=(const format_error&) = default;
+  format_error(format_error&&) = default;
+  format_error& operator=(format_error&&) = default;
+  ~format_error() FMT_NOEXCEPT override FMT_MSC_DEFAULT;
 };
 
-// An output iterator that truncates the output and counts the number of objects
-// written to it.
-template <typename OutputIt, typename Enable = typename std::is_void<
-    typename std::iterator_traits<OutputIt>::value_type>::type>
-class truncating_iterator;
-
-template <typename OutputIt>
-class truncating_iterator<OutputIt, std::false_type>:
-  public truncating_iterator_base<OutputIt> {
-  typedef std::iterator_traits<OutputIt> traits;
-
-  mutable typename traits::value_type blackhole_;
-
- public:
-  typedef typename traits::value_type value_type;
-
-  truncating_iterator(OutputIt out, std::size_t limit)
-    : truncating_iterator_base<OutputIt>(out, limit) {}
-
-  truncating_iterator& operator++() {
-    if (this->count_++ < this->limit_)
-      ++this->out_;
-    return *this;
-  }
-
-  truncating_iterator operator++(int) {
-    auto it = *this;
-    ++*this;
-    return it;
-  }
-
-  value_type& operator*() const {
-    return this->count_ < this->limit_ ? *this->out_ : blackhole_;
-  }
+/**
+  \rst
+  Constructs a `~fmt::format_arg_store` object that contains references
+  to arguments and can be implicitly converted to `~fmt::format_args`.
+  If ``fmt`` is a compile-time string then `make_args_checked` checks
+  its validity at compile time.
+  \endrst
+ */
+template <typename... Args, typename S, typename Char = char_t<S>>
+FMT_INLINE auto make_args_checked(const S& fmt,
+                                  const remove_reference_t<Args>&... args)
+    -> format_arg_store<buffer_context<Char>, remove_reference_t<Args>...> {
+  static_assert(
+      detail::count<(
+              std::is_base_of<detail::view, remove_reference_t<Args>>::value &&
+              std::is_reference<Args>::value)...>() == 0,
+      "passing views as lvalues is disallowed");
+  detail::check_format_string<Args...>(fmt);
+  return {args...};
+}
+
+// compile-time support
+namespace detail_exported {
+#if FMT_USE_NONTYPE_TEMPLATE_PARAMETERS
+template <typename Char, size_t N> struct fixed_string {
+  constexpr fixed_string(const Char (&str)[N]) {
+    detail::copy_str<Char, const Char*, Char*>(static_cast<const Char*>(str),
+                                               str + N, data);
+  }
+  Char data[N]{};
 };
+#endif
 
-template <typename OutputIt>
-class truncating_iterator<OutputIt, std::true_type>:
-  public truncating_iterator_base<OutputIt> {
- public:
-  typedef typename OutputIt::container_type::value_type value_type;
+// Converts a compile-time string to basic_string_view.
+template <typename Char, size_t N>
+constexpr auto compile_string_to_view(const Char (&s)[N])
+    -> basic_string_view<Char> {
+  // Remove trailing NUL character if needed. Won't be present if this is used
+  // with a raw character array (i.e. not defined as a string).
+  return {s, N - (std::char_traits<Char>::to_int_type(s[N - 1]) == 0 ? 1 : 0)};
+}
+template <typename Char>
+constexpr auto compile_string_to_view(detail::std_string_view<Char> s)
+    -> basic_string_view<Char> {
+  return {s.data(), s.size()};
+}
+}  // namespace detail_exported
 
-  truncating_iterator(OutputIt out, std::size_t limit)
-    : truncating_iterator_base<OutputIt>(out, limit) {}
+FMT_BEGIN_DETAIL_NAMESPACE
 
-  truncating_iterator& operator=(value_type val) {
-    if (this->count_++ < this->limit_)
-      this->out_ = val;
-    return *this;
-  }
+template <typename T> struct is_integral : std::is_integral<T> {};
+template <> struct is_integral<int128_t> : std::true_type {};
+template <> struct is_integral<uint128_t> : std::true_type {};
 
-  truncating_iterator& operator++() { return *this; }
-  truncating_iterator& operator++(int) { return *this; }
-  truncating_iterator& operator*() { return *this; }
-};
+template <typename T>
+using is_signed =
+    std::integral_constant<bool, std::numeric_limits<T>::is_signed ||
+                                     std::is_same<T, int128_t>::value>;
 
 // Returns true if value is negative, false otherwise.
-// Same as (value < 0) but doesn't produce warnings if T is an unsigned type.
-template <typename T>
-FMT_CONSTEXPR typename std::enable_if<
-    std::numeric_limits<T>::is_signed, bool>::type is_negative(T value) {
+// Same as `value < 0` but doesn't produce warnings if T is an unsigned type.
+template <typename T, FMT_ENABLE_IF(is_signed<T>::value)>
+FMT_CONSTEXPR auto is_negative(T value) -> bool {
   return value < 0;
 }
-template <typename T>
-FMT_CONSTEXPR typename std::enable_if<
-    !std::numeric_limits<T>::is_signed, bool>::type is_negative(T) {
+template <typename T, FMT_ENABLE_IF(!is_signed<T>::value)>
+FMT_CONSTEXPR auto is_negative(T) -> bool {
   return false;
 }
 
+template <typename T, FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+FMT_CONSTEXPR auto is_supported_floating_point(T) -> uint16_t {
+  return (std::is_same<T, float>::value && FMT_USE_FLOAT) ||
+         (std::is_same<T, double>::value && FMT_USE_DOUBLE) ||
+         (std::is_same<T, long double>::value && FMT_USE_LONG_DOUBLE);
+}
+
+// Smallest of uint32_t, uint64_t, uint128_t that is large enough to
+// represent all values of an integral type T.
 template <typename T>
-struct int_traits {
-  // Smallest of uint32_t and uint64_t that is large enough to represent
-  // all values of T.
-  typedef typename std::conditional<
-    std::numeric_limits<T>::digits <= 32, uint32_t, uint64_t>::type main_type;
-};
-
-// Static data is placed in this class template to allow header-only
-// configuration.
-template <typename T = void>
-struct FMT_API basic_data {
-  static const uint32_t POWERS_OF_10_32[];
-  static const uint32_t ZERO_OR_POWERS_OF_10_32[];
-  static const uint64_t ZERO_OR_POWERS_OF_10_64[];
-  static const uint64_t POW10_SIGNIFICANDS[];
-  static const int16_t POW10_EXPONENTS[];
-  static const char DIGITS[];
-  static const char FOREGROUND_COLOR[];
-  static const char BACKGROUND_COLOR[];
-  static const char RESET_COLOR[];
-  static const wchar_t WRESET_COLOR[];
-};
+using uint32_or_64_or_128_t =
+    conditional_t<num_bits<T>() <= 32 && !FMT_REDUCE_INT_INSTANTIATIONS,
+                  uint32_t,
+                  conditional_t<num_bits<T>() <= 64, uint64_t, uint128_t>>;
+template <typename T>
+using uint64_or_128_t = conditional_t<num_bits<T>() <= 64, uint64_t, uint128_t>;
 
-#if FMT_USE_EXTERN_TEMPLATES
-extern template struct basic_data<void>;
-#endif
+#define FMT_POWERS_OF_10(factor)                                             \
+  factor * 10, (factor)*100, (factor)*1000, (factor)*10000, (factor)*100000, \
+      (factor)*1000000, (factor)*10000000, (factor)*100000000,               \
+      (factor)*1000000000
 
-typedef basic_data<> data;
+// Converts value in the range [0, 100) to a string.
+constexpr const char* digits2(size_t value) {
+  // GCC generates slightly better code when value is pointer-size.
+  return &"0001020304050607080910111213141516171819"
+         "2021222324252627282930313233343536373839"
+         "4041424344454647484950515253545556575859"
+         "6061626364656667686970717273747576777879"
+         "8081828384858687888990919293949596979899"[value * 2];
+}
 
-#ifdef FMT_BUILTIN_CLZLL
-// Returns the number of decimal digits in n. Leading zeros are not counted
-// except for n == 0 in which case count_digits returns 1.
-inline int count_digits(uint64_t n) {
-  // Based on http://graphics.stanford.edu/~seander/bithacks.html#IntegerLog10
-  // and the benchmark https://github.com/localvoid/cxx-benchmark-count-digits.
-  int t = (64 - FMT_BUILTIN_CLZLL(n | 1)) * 1233 >> 12;
-  return t - (n < data::ZERO_OR_POWERS_OF_10_64[t]) + 1;
+// Sign is a template parameter to workaround a bug in gcc 4.8.
+template <typename Char, typename Sign> constexpr Char sign(Sign s) {
+#if !FMT_GCC_VERSION || FMT_GCC_VERSION >= 604
+  static_assert(std::is_same<Sign, sign_t>::value, "");
+#endif
+  return static_cast<Char>("\0-+ "[s]);
 }
-#else
-// Fallback version of count_digits used when __builtin_clz is not available.
-inline int count_digits(uint64_t n) {
+
+template <typename T> FMT_CONSTEXPR auto count_digits_fallback(T n) -> int {
   int count = 1;
   for (;;) {
     // Integer division is slow so do it for a group of four digits instead
     // of for every digit. The idea comes from the talk by Alexandrescu
     // "Three Optimization Tips for C++". See speed-test for a comparison.
     if (n < 10) return count;
     if (n < 100) return count + 1;
     if (n < 1000) return count + 2;
     if (n < 10000) return count + 3;
     n /= 10000u;
     count += 4;
   }
 }
-#endif
-
-template <typename Char>
-inline size_t count_code_points(basic_string_view<Char> s) { return s.size(); }
-
-// Counts the number of code points in a UTF-8 string.
-FMT_API size_t count_code_points(basic_string_view<char8_t> s);
-
-inline char8_t to_char8_t(char c) { return static_cast<char8_t>(c); }
-
-template <typename InputIt, typename OutChar>
-struct needs_conversion: std::integral_constant<bool,
-  std::is_same<
-    typename std::iterator_traits<InputIt>::value_type, char>::value &&
-  std::is_same<OutChar, char8_t>::value> {};
-
-template <typename OutChar, typename InputIt, typename OutputIt>
-typename std::enable_if<
-  !needs_conversion<InputIt, OutChar>::value, OutputIt>::type
-    copy_str(InputIt begin, InputIt end, OutputIt it) {
-  return std::copy(begin, end, it);
+#if FMT_USE_INT128
+FMT_CONSTEXPR inline auto count_digits(uint128_t n) -> int {
+  return count_digits_fallback(n);
 }
+#endif
 
-template <typename OutChar, typename InputIt, typename OutputIt>
-typename std::enable_if<
-  needs_conversion<InputIt, OutChar>::value, OutputIt>::type
-    copy_str(InputIt begin, InputIt end, OutputIt it) {
-  return std::transform(begin, end, it, to_char8_t);
+#ifdef FMT_BUILTIN_CLZLL
+// It is a separate function rather than a part of count_digits to workaround
+// the lack of static constexpr in constexpr functions.
+inline auto do_count_digits(uint64_t n) -> int {
+  // This has comparable performance to the version by Kendall Willets
+  // (https://github.com/fmtlib/format-benchmark/blob/master/digits10)
+  // but uses smaller tables.
+  // Maps bsr(n) to ceil(log10(pow(2, bsr(n) + 1) - 1)).
+  static constexpr uint8_t bsr2log10[] = {
+      1,  1,  1,  2,  2,  2,  3,  3,  3,  4,  4,  4,  4,  5,  5,  5,
+      6,  6,  6,  7,  7,  7,  7,  8,  8,  8,  9,  9,  9,  10, 10, 10,
+      10, 11, 11, 11, 12, 12, 12, 13, 13, 13, 13, 14, 14, 14, 15, 15,
+      15, 16, 16, 16, 16, 17, 17, 17, 18, 18, 18, 19, 19, 19, 19, 20};
+  auto t = bsr2log10[FMT_BUILTIN_CLZLL(n | 1) ^ 63];
+  static constexpr const uint64_t zero_or_powers_of_10[] = {
+      0, 0, FMT_POWERS_OF_10(1U), FMT_POWERS_OF_10(1000000000ULL),
+      10000000000000000000ULL};
+  return t - (n < zero_or_powers_of_10[t]);
 }
-
-#if FMT_HAS_CPP_ATTRIBUTE(always_inline)
-# define FMT_ALWAYS_INLINE __attribute__((always_inline))
-#else
-# define FMT_ALWAYS_INLINE
 #endif
 
-template <typename Handler>
-inline char *lg(uint32_t n, Handler h) FMT_ALWAYS_INLINE;
-
-// Computes g = floor(log10(n)) and calls h.on<g>(n);
-template <typename Handler>
-inline char *lg(uint32_t n, Handler h) {
-  return n < 100 ? n < 10 ? h.template on<0>(n) : h.template on<1>(n)
-                 : n < 1000000
-                       ? n < 10000 ? n < 1000 ? h.template on<2>(n)
-                                              : h.template on<3>(n)
-                                   : n < 100000 ? h.template on<4>(n)
-                                                : h.template on<5>(n)
-                       : n < 100000000 ? n < 10000000 ? h.template on<6>(n)
-                                                      : h.template on<7>(n)
-                                       : n < 1000000000 ? h.template on<8>(n)
-                                                        : h.template on<9>(n);
-}
-
-// An lg handler that formats a decimal number.
-// Usage: lg(n, decimal_formatter(buffer));
-class decimal_formatter {
- private:
-  char *buffer_;
-
-  void write_pair(unsigned N, uint32_t index) {
-    std::memcpy(buffer_ + N, data::DIGITS + index * 2, 2);
-  }
-
- public:
-  explicit decimal_formatter(char *buf) : buffer_(buf) {}
-
-  template <unsigned N> char *on(uint32_t u) {
-    if (N == 0) {
-      *buffer_ = static_cast<char>(u) + '0';
-    } else if (N == 1) {
-      write_pair(0, u);
-    } else {
-      // The idea of using 4.32 fixed-point numbers is based on
-      // https://github.com/jeaiii/itoa
-      unsigned n = N - 1;
-      unsigned a = n / 5 * n * 53 / 16;
-      uint64_t t = ((1ULL << (32 + a)) /
-                   data::ZERO_OR_POWERS_OF_10_32[n] + 1 - n / 9);
-      t = ((t * u) >> a) + n / 5 * 4;
-      write_pair(0, t >> 32);
-      for (unsigned i = 2; i < N; i += 2) {
-        t = 100ULL * static_cast<uint32_t>(t);
-        write_pair(i, t >> 32);
-      }
-      if (N % 2 == 0) {
-        buffer_[N] = static_cast<char>(
-          (10ULL * static_cast<uint32_t>(t)) >> 32) + '0';
-      }
-    }
-    return buffer_ += N + 1;
+// Returns the number of decimal digits in n. Leading zeros are not counted
+// except for n == 0 in which case count_digits returns 1.
+FMT_CONSTEXPR20 inline auto count_digits(uint64_t n) -> int {
+#ifdef FMT_BUILTIN_CLZLL
+  if (!is_constant_evaluated()) {
+    return do_count_digits(n);
   }
-};
+#endif
+  return count_digits_fallback(n);
+}
 
-// An lg handler that formats a decimal number with a terminating null.
-class decimal_formatter_null : public decimal_formatter {
- public:
-  explicit decimal_formatter_null(char *buf) : decimal_formatter(buf) {}
+// Counts the number of digits in n. BITS = log2(radix).
+template <int BITS, typename UInt>
+FMT_CONSTEXPR auto count_digits(UInt n) -> int {
+#ifdef FMT_BUILTIN_CLZ
+  if (num_bits<UInt>() == 32)
+    return (FMT_BUILTIN_CLZ(static_cast<uint32_t>(n) | 1) ^ 31) / BITS + 1;
+#endif
+  // Lambda avoids unreachable code warnings from NVHPC.
+  return [](UInt m) {
+    int num_digits = 0;
+    do {
+      ++num_digits;
+    } while ((m >>= BITS) != 0);
+    return num_digits;
+  }(n);
+}
 
-  template <unsigned N> char *on(uint32_t u) {
-    char *buf = decimal_formatter::on<N>(u);
-    *buf = '\0';
-    return buf;
-  }
-};
+template <> auto count_digits<4>(detail::fallback_uintptr n) -> int;
 
 #ifdef FMT_BUILTIN_CLZ
-// Optional version of count_digits for better performance on 32-bit platforms.
-inline int count_digits(uint32_t n) {
-  int t = (32 - FMT_BUILTIN_CLZ(n | 1)) * 1233 >> 12;
-  return t - (n < data::ZERO_OR_POWERS_OF_10_32[t]) + 1;
+// It is a separate function rather than a part of count_digits to workaround
+// the lack of static constexpr in constexpr functions.
+FMT_INLINE auto do_count_digits(uint32_t n) -> int {
+// An optimization by Kendall Willets from https://bit.ly/3uOIQrB.
+// This increments the upper 32 bits (log10(T) - 1) when >= T is added.
+#  define FMT_INC(T) (((sizeof(#  T) - 1ull) << 32) - T)
+  static constexpr uint64_t table[] = {
+      FMT_INC(0),          FMT_INC(0),          FMT_INC(0),           // 8
+      FMT_INC(10),         FMT_INC(10),         FMT_INC(10),          // 64
+      FMT_INC(100),        FMT_INC(100),        FMT_INC(100),         // 512
+      FMT_INC(1000),       FMT_INC(1000),       FMT_INC(1000),        // 4096
+      FMT_INC(10000),      FMT_INC(10000),      FMT_INC(10000),       // 32k
+      FMT_INC(100000),     FMT_INC(100000),     FMT_INC(100000),      // 256k
+      FMT_INC(1000000),    FMT_INC(1000000),    FMT_INC(1000000),     // 2048k
+      FMT_INC(10000000),   FMT_INC(10000000),   FMT_INC(10000000),    // 16M
+      FMT_INC(100000000),  FMT_INC(100000000),  FMT_INC(100000000),   // 128M
+      FMT_INC(1000000000), FMT_INC(1000000000), FMT_INC(1000000000),  // 1024M
+      FMT_INC(1000000000), FMT_INC(1000000000)                        // 4B
+  };
+  auto inc = table[FMT_BUILTIN_CLZ(n | 1) ^ 31];
+  return static_cast<int>((n + inc) >> 32);
 }
 #endif
 
-// A functor that doesn't add a thousands separator.
-struct no_thousands_sep {
-  typedef char char_type;
+// Optional version of count_digits for better performance on 32-bit platforms.
+FMT_CONSTEXPR20 inline auto count_digits(uint32_t n) -> int {
+#ifdef FMT_BUILTIN_CLZ
+  if (!is_constant_evaluated()) {
+    return do_count_digits(n);
+  }
+#endif
+  return count_digits_fallback(n);
+}
 
-  template <typename Char>
-  void operator()(Char *) {}
+template <typename Int> constexpr auto digits10() FMT_NOEXCEPT -> int {
+  return std::numeric_limits<Int>::digits10;
+}
+template <> constexpr auto digits10<int128_t>() FMT_NOEXCEPT -> int {
+  return 38;
+}
+template <> constexpr auto digits10<uint128_t>() FMT_NOEXCEPT -> int {
+  return 38;
+}
 
-  enum { size = 0 };
+template <typename Char> struct thousands_sep_result {
+  std::string grouping;
+  Char thousands_sep;
 };
 
-// A functor that adds a thousands separator.
 template <typename Char>
-class add_thousands_sep {
- private:
-  basic_string_view<Char> sep_;
-
-  // Index of a decimal digit with the least significant digit having index 0.
-  unsigned digit_index_;
-
- public:
-  typedef Char char_type;
-
-  explicit add_thousands_sep(basic_string_view<Char> sep)
-    : sep_(sep), digit_index_(0) {}
-
-  void operator()(Char *&buffer) {
-    if (++digit_index_ % 3 != 0)
-      return;
-    buffer -= sep_.size();
-    std::uninitialized_copy(sep_.data(), sep_.data() + sep_.size(),
-                            internal::make_checked(buffer, sep_.size()));
-  }
-
-  enum { size = 1 };
-};
-
+FMT_API auto thousands_sep_impl(locale_ref loc) -> thousands_sep_result<Char>;
 template <typename Char>
-FMT_API Char thousands_sep_impl(locale_ref loc);
+inline auto thousands_sep(locale_ref loc) -> thousands_sep_result<Char> {
+  auto result = thousands_sep_impl<char>(loc);
+  return {result.grouping, Char(result.thousands_sep)};
+}
+template <>
+inline auto thousands_sep(locale_ref loc) -> thousands_sep_result<wchar_t> {
+  return thousands_sep_impl<wchar_t>(loc);
+}
 
 template <typename Char>
-inline Char thousands_sep(locale_ref loc) {
-  return Char(thousands_sep_impl<char>(loc));
+FMT_API auto decimal_point_impl(locale_ref loc) -> Char;
+template <typename Char> inline auto decimal_point(locale_ref loc) -> Char {
+  return Char(decimal_point_impl<char>(loc));
+}
+template <> inline auto decimal_point(locale_ref loc) -> wchar_t {
+  return decimal_point_impl<wchar_t>(loc);
 }
 
-template <>
-inline wchar_t thousands_sep(locale_ref loc) {
-  return thousands_sep_impl<wchar_t>(loc);
+// Compares two characters for equality.
+template <typename Char> auto equal2(const Char* lhs, const char* rhs) -> bool {
+  return lhs[0] == Char(rhs[0]) && lhs[1] == Char(rhs[1]);
+}
+inline auto equal2(const char* lhs, const char* rhs) -> bool {
+  return memcmp(lhs, rhs, 2) == 0;
 }
 
-// Formats a decimal unsigned integer value writing into buffer.
-// thousands_sep is a functor that is called after writing each char to
-// add a thousands separator if necessary.
-template <typename UInt, typename Char, typename ThousandsSep>
-inline Char *format_decimal(Char *buffer, UInt value, int num_digits,
-                            ThousandsSep thousands_sep) {
-  FMT_ASSERT(num_digits >= 0, "invalid digit count");
-  buffer += num_digits;
-  Char *end = buffer;
+// Copies two characters from src to dst.
+template <typename Char>
+FMT_CONSTEXPR20 FMT_INLINE void copy2(Char* dst, const char* src) {
+  if (!is_constant_evaluated() && sizeof(Char) == sizeof(char)) {
+    memcpy(dst, src, 2);
+    return;
+  }
+  *dst++ = static_cast<Char>(*src++);
+  *dst = static_cast<Char>(*src);
+}
+
+template <typename Iterator> struct format_decimal_result {
+  Iterator begin;
+  Iterator end;
+};
+
+// Formats a decimal unsigned integer value writing into out pointing to a
+// buffer of specified size. The caller must ensure that the buffer is large
+// enough.
+template <typename Char, typename UInt>
+FMT_CONSTEXPR20 auto format_decimal(Char* out, UInt value, int size)
+    -> format_decimal_result<Char*> {
+  FMT_ASSERT(size >= count_digits(value), "invalid digit count");
+  out += size;
+  Char* end = out;
   while (value >= 100) {
     // Integer division is slow so do it for a group of two digits instead
     // of for every digit. The idea comes from the talk by Alexandrescu
     // "Three Optimization Tips for C++". See speed-test for a comparison.
-    unsigned index = static_cast<unsigned>((value % 100) * 2);
+    out -= 2;
+    copy2(out, digits2(static_cast<size_t>(value % 100)));
     value /= 100;
-    *--buffer = static_cast<Char>(data::DIGITS[index + 1]);
-    thousands_sep(buffer);
-    *--buffer = static_cast<Char>(data::DIGITS[index]);
-    thousands_sep(buffer);
   }
   if (value < 10) {
-    *--buffer = static_cast<Char>('0' + value);
-    return end;
+    *--out = static_cast<Char>('0' + value);
+    return {out, end};
   }
-  unsigned index = static_cast<unsigned>(value * 2);
-  *--buffer = static_cast<Char>(data::DIGITS[index + 1]);
-  thousands_sep(buffer);
-  *--buffer = static_cast<Char>(data::DIGITS[index]);
-  return end;
-}
-
-template <typename OutChar, typename UInt, typename Iterator,
-          typename ThousandsSep>
-inline Iterator format_decimal(
-    Iterator out, UInt value, int num_digits, ThousandsSep sep) {
-  FMT_ASSERT(num_digits >= 0, "invalid digit count");
-  typedef typename ThousandsSep::char_type char_type;
-  // Buffer should be large enough to hold all digits (<= digits10 + 1).
-  enum { max_size = std::numeric_limits<UInt>::digits10 + 1 };
-  FMT_ASSERT(ThousandsSep::size <= 1, "invalid separator");
-  char_type buffer[max_size + max_size / 3];
-  auto end = format_decimal(buffer, value, num_digits, sep);
-  return internal::copy_str<OutChar>(buffer, end, out);
-}
-
-template <typename OutChar, typename It, typename UInt>
-inline It format_decimal(It out, UInt value, int num_digits) {
-  return format_decimal<OutChar>(out, value, num_digits, no_thousands_sep());
+  out -= 2;
+  copy2(out, digits2(static_cast<size_t>(value)));
+  return {out, end};
+}
+
+template <typename Char, typename UInt, typename Iterator,
+          FMT_ENABLE_IF(!std::is_pointer<remove_cvref_t<Iterator>>::value)>
+inline auto format_decimal(Iterator out, UInt value, int size)
+    -> format_decimal_result<Iterator> {
+  // Buffer is large enough to hold all digits (digits10 + 1).
+  Char buffer[digits10<UInt>() + 1];
+  auto end = format_decimal(buffer, value, size).end;
+  return {out, detail::copy_str_noinline<Char>(buffer, end, out)};
 }
 
 template <unsigned BASE_BITS, typename Char, typename UInt>
-inline Char *format_uint(Char *buffer, UInt value, int num_digits,
-                         bool upper = false) {
+FMT_CONSTEXPR auto format_uint(Char* buffer, UInt value, int num_digits,
+                               bool upper = false) -> Char* {
   buffer += num_digits;
-  Char *end = buffer;
+  Char* end = buffer;
   do {
-    const char *digits = upper ? "0123456789ABCDEF" : "0123456789abcdef";
+    const char* digits = upper ? "0123456789ABCDEF" : "0123456789abcdef";
     unsigned digit = (value & ((1 << BASE_BITS) - 1));
     *--buffer = static_cast<Char>(BASE_BITS < 4 ? static_cast<char>('0' + digit)
                                                 : digits[digit]);
   } while ((value >>= BASE_BITS) != 0);
   return end;
 }
 
+template <unsigned BASE_BITS, typename Char>
+auto format_uint(Char* buffer, detail::fallback_uintptr n, int num_digits,
+                 bool = false) -> Char* {
+  auto char_digits = std::numeric_limits<unsigned char>::digits / 4;
+  int start = (num_digits + char_digits - 1) / char_digits - 1;
+  if (int start_digits = num_digits % char_digits) {
+    unsigned value = n.value[start--];
+    buffer = format_uint<BASE_BITS>(buffer, value, start_digits);
+  }
+  for (; start >= 0; --start) {
+    unsigned value = n.value[start];
+    buffer += char_digits;
+    auto p = buffer;
+    for (int i = 0; i < char_digits; ++i) {
+      unsigned digit = (value & ((1 << BASE_BITS) - 1));
+      *--p = static_cast<Char>("0123456789abcdef"[digit]);
+      value >>= BASE_BITS;
+    }
+  }
+  return buffer;
+}
+
 template <unsigned BASE_BITS, typename Char, typename It, typename UInt>
-inline It format_uint(It out, UInt value, int num_digits,
-                      bool upper = false) {
-  // Buffer should be large enough to hold all digits (digits / BASE_BITS + 1)
-  // and null.
-  char buffer[std::numeric_limits<UInt>::digits / BASE_BITS + 2];
+inline auto format_uint(It out, UInt value, int num_digits, bool upper = false)
+    -> It {
+  if (auto ptr = to_pointer<Char>(out, to_unsigned(num_digits))) {
+    format_uint<BASE_BITS>(ptr, value, num_digits, upper);
+    return out;
+  }
+  // Buffer should be large enough to hold all digits (digits / BASE_BITS + 1).
+  char buffer[num_bits<UInt>() / BASE_BITS + 1];
   format_uint<BASE_BITS>(buffer, value, num_digits, upper);
-  return internal::copy_str<Char>(buffer, buffer + num_digits, out);
+  return detail::copy_str_noinline<Char>(buffer, buffer + num_digits, out);
 }
 
-#ifndef _WIN32
-# define FMT_USE_WINDOWS_H 0
-#elif !defined(FMT_USE_WINDOWS_H)
-# define FMT_USE_WINDOWS_H 1
-#endif
-
-// Define FMT_USE_WINDOWS_H to 0 to disable use of windows.h.
-// All the functionality that relies on it will be disabled too.
-#if FMT_USE_WINDOWS_H
 // A converter from UTF-8 to UTF-16.
-// It is only provided for Windows since other systems support UTF-8 natively.
 class utf8_to_utf16 {
  private:
-  wmemory_buffer buffer_;
+  basic_memory_buffer<wchar_t> buffer_;
 
  public:
   FMT_API explicit utf8_to_utf16(string_view s);
-  operator wstring_view() const { return wstring_view(&buffer_[0], size()); }
-  size_t size() const { return buffer_.size() - 1; }
-  const wchar_t *c_str() const { return &buffer_[0]; }
-  std::wstring str() const { return std::wstring(&buffer_[0], size()); }
+  operator basic_string_view<wchar_t>() const { return {&buffer_[0], size()}; }
+  auto size() const -> size_t { return buffer_.size() - 1; }
+  auto c_str() const -> const wchar_t* { return &buffer_[0]; }
+  auto str() const -> std::wstring { return {&buffer_[0], size()}; }
+};
+
+namespace dragonbox {
+
+// Type-specific information that Dragonbox uses.
+template <class T> struct float_info;
+
+template <> struct float_info<float> {
+  using carrier_uint = uint32_t;
+  static const int significand_bits = 23;
+  static const int exponent_bits = 8;
+  static const int min_exponent = -126;
+  static const int max_exponent = 127;
+  static const int exponent_bias = -127;
+  static const int decimal_digits = 9;
+  static const int kappa = 1;
+  static const int big_divisor = 100;
+  static const int small_divisor = 10;
+  static const int min_k = -31;
+  static const int max_k = 46;
+  static const int cache_bits = 64;
+  static const int divisibility_check_by_5_threshold = 39;
+  static const int case_fc_pm_half_lower_threshold = -1;
+  static const int case_fc_pm_half_upper_threshold = 6;
+  static const int case_fc_lower_threshold = -2;
+  static const int case_fc_upper_threshold = 6;
+  static const int case_shorter_interval_left_endpoint_lower_threshold = 2;
+  static const int case_shorter_interval_left_endpoint_upper_threshold = 3;
+  static const int shorter_interval_tie_lower_threshold = -35;
+  static const int shorter_interval_tie_upper_threshold = -35;
+  static const int max_trailing_zeros = 7;
+};
+
+template <> struct float_info<double> {
+  using carrier_uint = uint64_t;
+  static const int significand_bits = 52;
+  static const int exponent_bits = 11;
+  static const int min_exponent = -1022;
+  static const int max_exponent = 1023;
+  static const int exponent_bias = -1023;
+  static const int decimal_digits = 17;
+  static const int kappa = 2;
+  static const int big_divisor = 1000;
+  static const int small_divisor = 100;
+  static const int min_k = -292;
+  static const int max_k = 326;
+  static const int cache_bits = 128;
+  static const int divisibility_check_by_5_threshold = 86;
+  static const int case_fc_pm_half_lower_threshold = -2;
+  static const int case_fc_pm_half_upper_threshold = 9;
+  static const int case_fc_lower_threshold = -4;
+  static const int case_fc_upper_threshold = 9;
+  static const int case_shorter_interval_left_endpoint_lower_threshold = 2;
+  static const int case_shorter_interval_left_endpoint_upper_threshold = 3;
+  static const int shorter_interval_tie_lower_threshold = -77;
+  static const int shorter_interval_tie_upper_threshold = -77;
+  static const int max_trailing_zeros = 16;
+};
+
+template <typename T> struct decimal_fp {
+  using significand_type = typename float_info<T>::carrier_uint;
+  significand_type significand;
+  int exponent;
 };
 
-// A converter from UTF-16 to UTF-8.
-// It is only provided for Windows since other systems support UTF-8 natively.
-class utf16_to_utf8 {
- private:
-  memory_buffer buffer_;
-
- public:
-  utf16_to_utf8() {}
-  FMT_API explicit utf16_to_utf8(wstring_view s);
-  operator string_view() const { return string_view(&buffer_[0], size()); }
-  size_t size() const { return buffer_.size() - 1; }
-  const char *c_str() const { return &buffer_[0]; }
-  std::string str() const { return std::string(&buffer_[0], size()); }
-
-  // Performs conversion returning a system error code instead of
-  // throwing exception on conversion error. This method may still throw
-  // in case of memory allocation error.
-  FMT_API int convert(wstring_view s);
-};
-
-FMT_API void format_windows_error(fmt::internal::buffer &out, int error_code,
-                                  fmt::string_view message) FMT_NOEXCEPT;
-#endif
-
-template <typename T = void>
-struct null {};
-}  // namespace internal
-
-enum alignment {
-  ALIGN_DEFAULT, ALIGN_LEFT, ALIGN_RIGHT, ALIGN_CENTER, ALIGN_NUMERIC
-};
-
-// Flags.
-enum { SIGN_FLAG = 1, PLUS_FLAG = 2, MINUS_FLAG = 4, HASH_FLAG = 8 };
-
-// An alignment specifier.
-struct align_spec {
-  unsigned width_;
-  // Fill is always wchar_t and cast to char if necessary to avoid having
-  // two specialization of AlignSpec and its subclasses.
-  wchar_t fill_;
-  alignment align_;
-
-  FMT_CONSTEXPR align_spec() : width_(0), fill_(' '), align_(ALIGN_DEFAULT) {}
-  FMT_CONSTEXPR unsigned width() const { return width_; }
-  FMT_CONSTEXPR wchar_t fill() const { return fill_; }
-  FMT_CONSTEXPR alignment align() const { return align_; }
-};
-
-struct core_format_specs {
-  int precision;
-  uint_least8_t flags;
-  char type;
-
-  FMT_CONSTEXPR core_format_specs() : precision(-1), flags(0), type(0) {}
-  FMT_CONSTEXPR bool has(unsigned f) const { return (flags & f) != 0; }
-};
-
-// Format specifiers.
-template <typename Char>
-struct basic_format_specs : align_spec, core_format_specs {
-  FMT_CONSTEXPR basic_format_specs() {}
-};
-
-typedef basic_format_specs<char> format_specs;
+template <typename T>
+FMT_API auto to_decimal(T x) FMT_NOEXCEPT -> decimal_fp<T>;
+}  // namespace dragonbox
 
-template <typename Char, typename ErrorHandler>
-FMT_CONSTEXPR unsigned basic_parse_context<Char, ErrorHandler>::next_arg_id() {
-  if (next_arg_id_ >= 0)
-    return internal::to_unsigned(next_arg_id_++);
-  on_error("cannot switch from manual to automatic argument indexing");
-  return 0;
-}
-
-namespace internal {
-
-// Formats value using Grisu2 algorithm:
-// https://www.cs.tufts.edu/~nr/cs257/archive/florian-loitsch/printf.pdf
-template <typename Double>
-FMT_API typename std::enable_if<sizeof(Double) == sizeof(uint64_t), bool>::type
-  grisu2_format(Double value, buffer &buf, core_format_specs);
-template <typename Double>
-inline typename std::enable_if<sizeof(Double) != sizeof(uint64_t), bool>::type
-  grisu2_format(Double, buffer &, core_format_specs) { return false; }
-
-template <typename Double>
-void sprintf_format(Double, internal::buffer &, core_format_specs);
-
-template <typename Handler>
-FMT_CONSTEXPR void handle_int_type_spec(char spec, Handler &&handler) {
-  switch (spec) {
-  case 0: case 'd':
-    handler.on_dec();
-    break;
-  case 'x': case 'X':
-    handler.on_hex();
-    break;
-  case 'b': case 'B':
-    handler.on_bin();
-    break;
-  case 'o':
-    handler.on_oct();
-    break;
-  case 'n':
-    handler.on_num();
-    break;
-  default:
-    handler.on_error();
-  }
+template <typename T>
+constexpr auto exponent_mask() ->
+    typename dragonbox::float_info<T>::carrier_uint {
+  using uint = typename dragonbox::float_info<T>::carrier_uint;
+  return ((uint(1) << dragonbox::float_info<T>::exponent_bits) - 1)
+         << dragonbox::float_info<T>::significand_bits;
 }
 
-template <typename Handler>
-FMT_CONSTEXPR void handle_float_type_spec(char spec, Handler &&handler) {
-  switch (spec) {
-  case 0: case 'g': case 'G':
-    handler.on_general();
-    break;
-  case 'e': case 'E':
-    handler.on_exp();
-    break;
-  case 'f': case 'F':
-    handler.on_fixed();
-    break;
-   case 'a': case 'A':
-    handler.on_hex();
-    break;
-  default:
-    handler.on_error();
-    break;
+// Writes the exponent exp in the form "[+-]d{2,3}" to buffer.
+template <typename Char, typename It>
+FMT_CONSTEXPR auto write_exponent(int exp, It it) -> It {
+  FMT_ASSERT(-10000 < exp && exp < 10000, "exponent out of range");
+  if (exp < 0) {
+    *it++ = static_cast<Char>('-');
+    exp = -exp;
+  } else {
+    *it++ = static_cast<Char>('+');
   }
+  if (exp >= 100) {
+    const char* top = digits2(to_unsigned(exp / 100));
+    if (exp >= 1000) *it++ = static_cast<Char>(top[0]);
+    *it++ = static_cast<Char>(top[1]);
+    exp %= 100;
+  }
+  const char* d = digits2(to_unsigned(exp));
+  *it++ = static_cast<Char>(d[0]);
+  *it++ = static_cast<Char>(d[1]);
+  return it;
 }
 
-template <typename Char, typename Handler>
-FMT_CONSTEXPR void handle_char_specs(
-    const basic_format_specs<Char> *specs, Handler &&handler) {
-  if (!specs) return handler.on_char();
-  if (specs->type && specs->type != 'c') return handler.on_int();
-  if (specs->align() == ALIGN_NUMERIC || specs->flags != 0)
-    handler.on_error("invalid format specifier for char");
-  handler.on_char();
-}
-
-template <typename Char, typename Handler>
-FMT_CONSTEXPR void handle_cstring_type_spec(Char spec, Handler &&handler) {
-  if (spec == 0 || spec == 's')
-    handler.on_string();
-  else if (spec == 'p')
-    handler.on_pointer();
-  else
-    handler.on_error("invalid type specifier");
-}
-
-template <typename Char, typename ErrorHandler>
-FMT_CONSTEXPR void check_string_type_spec(Char spec, ErrorHandler &&eh) {
-  if (spec != 0 && spec != 's')
-    eh.on_error("invalid type specifier");
-}
-
-template <typename Char, typename ErrorHandler>
-FMT_CONSTEXPR void check_pointer_type_spec(Char spec, ErrorHandler &&eh) {
-  if (spec != 0 && spec != 'p')
-    eh.on_error("invalid type specifier");
-}
-
-template <typename ErrorHandler>
-class int_type_checker : private ErrorHandler {
- public:
-  FMT_CONSTEXPR explicit int_type_checker(ErrorHandler eh) : ErrorHandler(eh) {}
-
-  FMT_CONSTEXPR void on_dec() {}
-  FMT_CONSTEXPR void on_hex() {}
-  FMT_CONSTEXPR void on_bin() {}
-  FMT_CONSTEXPR void on_oct() {}
-  FMT_CONSTEXPR void on_num() {}
-
-  FMT_CONSTEXPR void on_error() {
-    ErrorHandler::on_error("invalid type specifier");
-  }
-};
-
-template <typename ErrorHandler>
-class float_type_checker : private ErrorHandler {
- public:
-  FMT_CONSTEXPR explicit float_type_checker(ErrorHandler eh)
-    : ErrorHandler(eh) {}
-
-  FMT_CONSTEXPR void on_general() {}
-  FMT_CONSTEXPR void on_exp() {}
-  FMT_CONSTEXPR void on_fixed() {}
-  FMT_CONSTEXPR void on_hex() {}
-
-  FMT_CONSTEXPR void on_error() {
-    ErrorHandler::on_error("invalid type specifier");
-  }
-};
-
-template <typename ErrorHandler>
-class char_specs_checker : public ErrorHandler {
- private:
-  char type_;
+template <typename T>
+FMT_HEADER_ONLY_CONSTEXPR20 auto format_float(T value, int precision,
+                                              float_specs specs,
+                                              buffer<char>& buf) -> int;
 
- public:
-  FMT_CONSTEXPR char_specs_checker(char type, ErrorHandler eh)
-    : ErrorHandler(eh), type_(type) {}
+// Formats a floating-point number with snprintf.
+template <typename T>
+auto snprintf_float(T value, int precision, float_specs specs,
+                    buffer<char>& buf) -> int;
 
-  FMT_CONSTEXPR void on_int() {
-    handle_int_type_spec(type_, int_type_checker<ErrorHandler>(*this));
-  }
-  FMT_CONSTEXPR void on_char() {}
-};
+template <typename T> constexpr auto promote_float(T value) -> T {
+  return value;
+}
+constexpr auto promote_float(float value) -> double {
+  return static_cast<double>(value);
+}
 
-template <typename ErrorHandler>
-class cstring_type_checker : public ErrorHandler {
- public:
-  FMT_CONSTEXPR explicit cstring_type_checker(ErrorHandler eh)
-    : ErrorHandler(eh) {}
+template <typename OutputIt, typename Char>
+FMT_NOINLINE FMT_CONSTEXPR auto fill(OutputIt it, size_t n,
+                                     const fill_t<Char>& fill) -> OutputIt {
+  auto fill_size = fill.size();
+  if (fill_size == 1) return detail::fill_n(it, n, fill[0]);
+  auto data = fill.data();
+  for (size_t i = 0; i < n; ++i)
+    it = copy_str<Char>(data, data + fill_size, it);
+  return it;
+}
 
-  FMT_CONSTEXPR void on_string() {}
-  FMT_CONSTEXPR void on_pointer() {}
-};
+// Writes the output of f, padded according to format specifications in specs.
+// size: output size in code units.
+// width: output display width in (terminal) column positions.
+template <align::type align = align::left, typename OutputIt, typename Char,
+          typename F>
+FMT_CONSTEXPR auto write_padded(OutputIt out,
+                                const basic_format_specs<Char>& specs,
+                                size_t size, size_t width, F&& f) -> OutputIt {
+  static_assert(align == align::left || align == align::right, "");
+  unsigned spec_width = to_unsigned(specs.width);
+  size_t padding = spec_width > width ? spec_width - width : 0;
+  // Shifts are encoded as string literals because static constexpr is not
+  // supported in constexpr functions.
+  auto* shifts = align == align::left ? "\x1f\x1f\x00\x01" : "\x00\x1f\x00\x01";
+  size_t left_padding = padding >> shifts[specs.align];
+  size_t right_padding = padding - left_padding;
+  auto it = reserve(out, size + padding * specs.fill.size());
+  if (left_padding != 0) it = fill(it, left_padding, specs.fill);
+  it = f(it);
+  if (right_padding != 0) it = fill(it, right_padding, specs.fill);
+  return base_iterator(out, it);
+}
+
+template <align::type align = align::left, typename OutputIt, typename Char,
+          typename F>
+constexpr auto write_padded(OutputIt out, const basic_format_specs<Char>& specs,
+                            size_t size, F&& f) -> OutputIt {
+  return write_padded<align>(out, specs, size, size, f);
+}
+
+template <align::type align = align::left, typename Char, typename OutputIt>
+FMT_CONSTEXPR auto write_bytes(OutputIt out, string_view bytes,
+                               const basic_format_specs<Char>& specs)
+    -> OutputIt {
+  return write_padded<align>(
+      out, specs, bytes.size(), [bytes](reserve_iterator<OutputIt> it) {
+        const char* data = bytes.data();
+        return copy_str<Char>(data, data + bytes.size(), it);
+      });
+}
+
+template <typename Char, typename OutputIt, typename UIntPtr>
+auto write_ptr(OutputIt out, UIntPtr value,
+               const basic_format_specs<Char>* specs) -> OutputIt {
+  int num_digits = count_digits<4>(value);
+  auto size = to_unsigned(num_digits) + size_t(2);
+  auto write = [=](reserve_iterator<OutputIt> it) {
+    *it++ = static_cast<Char>('0');
+    *it++ = static_cast<Char>('x');
+    return format_uint<4, Char>(it, value, num_digits);
+  };
+  return specs ? write_padded<align::right>(out, *specs, size, write)
+               : base_iterator(out, write(reserve(out, size)));
+}
 
-template <typename Context>
-void arg_map<Context>::init(const basic_format_args<Context> &args) {
-  if (map_)
-    return;
-  map_ = new entry[args.max_size()];
-  if (args.is_packed()) {
-    for (unsigned i = 0;/*nothing*/; ++i) {
-      internal::type arg_type = args.type(i);
-      switch (arg_type) {
-        case internal::none_type:
-          return;
-        case internal::named_arg_type:
-          push_back(args.values_[i]);
-          break;
-        default:
-          break; // Do nothing.
+template <typename Char, typename OutputIt>
+FMT_CONSTEXPR auto write_char(OutputIt out, Char value,
+                              const basic_format_specs<Char>& specs)
+    -> OutputIt {
+  return write_padded(out, specs, 1, [=](reserve_iterator<OutputIt> it) {
+    *it++ = value;
+    return it;
+  });
+}
+template <typename Char, typename OutputIt>
+FMT_CONSTEXPR auto write(OutputIt out, Char value,
+                         const basic_format_specs<Char>& specs,
+                         locale_ref loc = {}) -> OutputIt {
+  return check_char_specs(specs)
+             ? write_char(out, value, specs)
+             : write(out, static_cast<int>(value), specs, loc);
+}
+
+// Data for write_int that doesn't depend on output iterator type. It is used to
+// avoid template code bloat.
+template <typename Char> struct write_int_data {
+  size_t size;
+  size_t padding;
+
+  FMT_CONSTEXPR write_int_data(int num_digits, unsigned prefix,
+                               const basic_format_specs<Char>& specs)
+      : size((prefix >> 24) + to_unsigned(num_digits)), padding(0) {
+    if (specs.align == align::numeric) {
+      auto width = to_unsigned(specs.width);
+      if (width > size) {
+        padding = width - size;
+        size = width;
       }
+    } else if (specs.precision > num_digits) {
+      size = (prefix >> 24) + to_unsigned(specs.precision);
+      padding = to_unsigned(specs.precision - num_digits);
     }
   }
-  for (unsigned i = 0; ; ++i) {
-    switch (args.args_[i].type_) {
-      case internal::none_type:
-        return;
-      case internal::named_arg_type:
-        push_back(args.args_[i].value_);
-        break;
-      default:
-        break; // Do nothing.
-    }
-  }
-}
-
-template <typename Range>
-class arg_formatter_base {
- public:
-  typedef typename Range::value_type char_type;
-  typedef decltype(internal::declval<Range>().begin()) iterator;
-  typedef basic_format_specs<char_type> format_specs;
-
- private:
-  typedef basic_writer<Range> writer_type;
-  writer_type writer_;
-  format_specs *specs_;
-
-  struct char_writer {
-    char_type value;
-
-    size_t size() const { return 1; }
-    size_t width() const { return 1; }
+};
 
-    template <typename It>
-    void operator()(It &&it) const { *it++ = value; }
+// Writes an integer in the format
+//   <left-padding><prefix><numeric-padding><digits><right-padding>
+// where <digits> are written by write_digits(it).
+// prefix contains chars in three lower bytes and the size in the fourth byte.
+template <typename OutputIt, typename Char, typename W>
+FMT_CONSTEXPR FMT_INLINE auto write_int(OutputIt out, int num_digits,
+                                        unsigned prefix,
+                                        const basic_format_specs<Char>& specs,
+                                        W write_digits) -> OutputIt {
+  // Slightly faster check for specs.width == 0 && specs.precision == -1.
+  if ((specs.width | (specs.precision + 1)) == 0) {
+    auto it = reserve(out, to_unsigned(num_digits) + (prefix >> 24));
+    if (prefix != 0) {
+      for (unsigned p = prefix & 0xffffff; p != 0; p >>= 8)
+        *it++ = static_cast<Char>(p & 0xff);
+    }
+    return base_iterator(out, write_digits(it));
+  }
+  auto data = write_int_data<Char>(num_digits, prefix, specs);
+  return write_padded<align::right>(
+      out, specs, data.size, [=](reserve_iterator<OutputIt> it) {
+        for (unsigned p = prefix & 0xffffff; p != 0; p >>= 8)
+          *it++ = static_cast<Char>(p & 0xff);
+        it = detail::fill_n(it, data.padding, static_cast<Char>('0'));
+        return write_digits(it);
+      });
+}
+
+template <typename Char> class digit_grouping {
+ private:
+  thousands_sep_result<Char> sep_;
+
+  struct next_state {
+    std::string::const_iterator group;
+    int pos;
   };
+  next_state initial_state() const { return {sep_.grouping.begin(), 0}; }
 
-  void write_char(char_type value) {
-    if (specs_)
-      writer_.write_padded(*specs_, char_writer{value});
-    else
-      writer_.write(value);
-  }
-
-  void write_pointer(const void *p) {
-    format_specs specs = specs_ ? *specs_ : format_specs();
-    specs.flags = HASH_FLAG;
-    specs.type = 'x';
-    writer_.write_int(reinterpret_cast<uintptr_t>(p), specs);
-  }
-
- protected:
-  writer_type &writer() { return writer_; }
-  format_specs *spec() { return specs_; }
-  iterator out() { return writer_.out(); }
-
-  void write(bool value) {
-    string_view sv(value ? "true" : "false");
-    specs_ ? writer_.write(sv, *specs_) : writer_.write(sv);
-  }
-
-  void write(const char_type *value) {
-    if (!value)
-      FMT_THROW(format_error("string pointer is null"));
-    auto length = std::char_traits<char_type>::length(value);
-    basic_string_view<char_type> sv(value, length);
-    specs_ ? writer_.write(sv, *specs_) : writer_.write(sv);
+  // Returns the next digit group separator position.
+  int next(next_state& state) const {
+    if (!sep_.thousands_sep) return max_value<int>();
+    if (state.group == sep_.grouping.end())
+      return state.pos += sep_.grouping.back();
+    if (*state.group <= 0 || *state.group == max_value<char>())
+      return max_value<int>();
+    state.pos += *state.group++;
+    return state.pos;
   }
 
  public:
-  arg_formatter_base(Range r, format_specs *s, locale_ref loc)
-    : writer_(r, loc), specs_(s) {}
-
-  iterator operator()(monostate) {
-    FMT_ASSERT(false, "invalid argument type");
-    return out();
-  }
-
-  template <typename T>
-  typename std::enable_if<
-    std::is_integral<T>::value || std::is_same<T, char_type>::value,
-    iterator>::type operator()(T value) {
-    // MSVC2013 fails to compile separate overloads for bool and char_type so
-    // use std::is_same instead.
-    if (std::is_same<T, bool>::value) {
-      if (specs_ && specs_->type)
-        return (*this)(value ? 1 : 0);
-      write(value != 0);
-    } else if (std::is_same<T, char_type>::value) {
-      internal::handle_char_specs(
-        specs_, char_spec_handler(*this, static_cast<char_type>(value)));
-    } else {
-      specs_ ? writer_.write_int(value, *specs_) : writer_.write(value);
-    }
-    return out();
+  explicit digit_grouping(locale_ref loc, bool localized = true) {
+    if (localized)
+      sep_ = thousands_sep<Char>(loc);
+    else
+      sep_.thousands_sep = Char();
   }
+  explicit digit_grouping(thousands_sep_result<Char> sep) : sep_(sep) {}
 
-  template <typename T>
-  typename std::enable_if<std::is_floating_point<T>::value, iterator>::type
-      operator()(T value) {
-    writer_.write_double(value, specs_ ? *specs_ : format_specs());
-    return out();
-  }
-
-  struct char_spec_handler : internal::error_handler {
-    arg_formatter_base &formatter;
-    char_type value;
-
-    char_spec_handler(arg_formatter_base& f, char_type val)
-      : formatter(f), value(val) {}
-
-    void on_int() {
-      if (formatter.specs_)
-        formatter.writer_.write_int(value, *formatter.specs_);
-      else
-        formatter.writer_.write(value);
-    }
-    void on_char() { formatter.write_char(value); }
-  };
-
-  struct cstring_spec_handler : internal::error_handler {
-    arg_formatter_base &formatter;
-    const char_type *value;
-
-    cstring_spec_handler(arg_formatter_base &f, const char_type *val)
-      : formatter(f), value(val) {}
+  Char separator() const { return sep_.thousands_sep; }
 
-    void on_string() { formatter.write(value); }
-    void on_pointer() { formatter.write_pointer(value); }
-  };
-
-  iterator operator()(const char_type *value) {
-    if (!specs_) return write(value), out();
-    internal::handle_cstring_type_spec(
-          specs_->type, cstring_spec_handler(*this, value));
-    return out();
-  }
-
-  iterator operator()(basic_string_view<char_type> value) {
-    if (specs_) {
-      internal::check_string_type_spec(
-            specs_->type, internal::error_handler());
-      writer_.write(value, *specs_);
-    } else {
-      writer_.write(value);
+  int count_separators(int num_digits) const {
+    int count = 0;
+    auto state = initial_state();
+    while (num_digits > next(state)) ++count;
+    return count;
+  }
+
+  // Applies grouping to digits and write the output to out.
+  template <typename Out, typename C>
+  Out apply(Out out, basic_string_view<C> digits) const {
+    auto num_digits = static_cast<int>(digits.size());
+    auto separators = basic_memory_buffer<int>();
+    separators.push_back(0);
+    auto state = initial_state();
+    while (int i = next(state)) {
+      if (i >= num_digits) break;
+      separators.push_back(i);
+    }
+    for (int i = 0, sep_index = static_cast<int>(separators.size() - 1);
+         i < num_digits; ++i) {
+      if (num_digits - i == separators[sep_index]) {
+        *out++ = separator();
+        --sep_index;
+      }
+      *out++ = static_cast<Char>(digits[to_unsigned(i)]);
     }
-    return out();
-  }
-
-  iterator operator()(const void *value) {
-    if (specs_)
-      check_pointer_type_spec(specs_->type, internal::error_handler());
-    write_pointer(value);
-    return out();
+    return out;
   }
 };
 
-template <typename Char>
-FMT_CONSTEXPR bool is_name_start(Char c) {
-  return ('a' <= c && c <= 'z') || ('A' <= c && c <= 'Z') || '_' == c;
+template <typename OutputIt, typename UInt, typename Char>
+auto write_int_localized(OutputIt out, UInt value, unsigned prefix,
+                         const basic_format_specs<Char>& specs,
+                         const digit_grouping<Char>& grouping) -> OutputIt {
+  static_assert(std::is_same<uint64_or_128_t<UInt>, UInt>::value, "");
+  int num_digits = count_digits(value);
+  char digits[40];
+  format_decimal(digits, value, num_digits);
+  unsigned size = to_unsigned((prefix != 0 ? 1 : 0) + num_digits +
+                              grouping.count_separators(num_digits));
+  return write_padded<align::right>(
+      out, specs, size, size, [&](reserve_iterator<OutputIt> it) {
+        if (prefix != 0) *it++ = static_cast<Char>(prefix);
+        return grouping.apply(it, string_view(digits, to_unsigned(num_digits)));
+      });
+}
+
+template <typename OutputIt, typename UInt, typename Char>
+auto write_int_localized(OutputIt& out, UInt value, unsigned prefix,
+                         const basic_format_specs<Char>& specs, locale_ref loc)
+    -> bool {
+  auto grouping = digit_grouping<Char>(loc);
+  out = write_int_localized(out, value, prefix, specs, grouping);
+  return true;
 }
 
-// Parses the range [begin, end) as an unsigned integer. This function assumes
-// that the range is non-empty and the first character is a digit.
-template <typename Char, typename ErrorHandler>
-FMT_CONSTEXPR unsigned parse_nonnegative_int(
-    const Char *&begin, const Char *end, ErrorHandler &&eh) {
-  assert(begin != end && '0' <= *begin && *begin <= '9');
-  if (*begin == '0') {
-    ++begin;
-    return 0;
-  }
-  unsigned value = 0;
-  // Convert to unsigned to prevent a warning.
-  unsigned max_int = (std::numeric_limits<int>::max)();
-  unsigned big = max_int / 10;
-  do {
-    // Check for overflow.
-    if (value > big) {
-      value = max_int + 1;
-      break;
-    }
-    value = value * 10 + unsigned(*begin - '0');
-    ++begin;
-  } while (begin != end && '0' <= *begin && *begin <= '9');
-  if (value > max_int)
-    eh.on_error("number is too big");
-  return value;
+FMT_CONSTEXPR inline void prefix_append(unsigned& prefix, unsigned value) {
+  prefix |= prefix != 0 ? value << 8 : value;
+  prefix += (1u + (value > 0xff ? 1 : 0)) << 24;
 }
 
-template <typename Char, typename Context>
-class custom_formatter: public function<bool> {
- private:
-  Context &ctx_;
-
- public:
-  explicit custom_formatter(Context &ctx): ctx_(ctx) {}
-
-  bool operator()(typename basic_format_arg<Context>::handle h) const {
-    h.format(ctx_);
-    return true;
-  }
-
-  template <typename T>
-  bool operator()(T) const { return false; }
+template <typename UInt> struct write_int_arg {
+  UInt abs_value;
+  unsigned prefix;
 };
 
 template <typename T>
-struct is_integer {
-  enum {
-    value = std::is_integral<T>::value && !std::is_same<T, bool>::value &&
-            !std::is_same<T, char>::value && !std::is_same<T, wchar_t>::value
-  };
-};
-
-template <typename ErrorHandler>
-class width_checker: public function<unsigned long long> {
- public:
-  explicit FMT_CONSTEXPR width_checker(ErrorHandler &eh) : handler_(eh) {}
-
-  template <typename T>
-  FMT_CONSTEXPR
-  typename std::enable_if<
-      is_integer<T>::value, unsigned long long>::type operator()(T value) {
-    if (is_negative(value))
-      handler_.on_error("negative width");
-    return static_cast<unsigned long long>(value);
+FMT_CONSTEXPR auto make_write_int_arg(T value, sign_t sign)
+    -> write_int_arg<uint32_or_64_or_128_t<T>> {
+  auto prefix = 0u;
+  auto abs_value = static_cast<uint32_or_64_or_128_t<T>>(value);
+  if (is_negative(value)) {
+    prefix = 0x01000000 | '-';
+    abs_value = 0 - abs_value;
+  } else {
+    constexpr const unsigned prefixes[4] = {0, 0, 0x1000000u | '+',
+                                            0x1000000u | ' '};
+    prefix = prefixes[sign];
+  }
+  return {abs_value, prefix};
+}
+
+template <typename Char, typename OutputIt, typename T>
+FMT_CONSTEXPR FMT_INLINE auto write_int(OutputIt out, write_int_arg<T> arg,
+                                        const basic_format_specs<Char>& specs,
+                                        locale_ref loc) -> OutputIt {
+  static_assert(std::is_same<T, uint32_or_64_or_128_t<T>>::value, "");
+  auto abs_value = arg.abs_value;
+  auto prefix = arg.prefix;
+  switch (specs.type) {
+  case presentation_type::none:
+  case presentation_type::dec: {
+    if (specs.localized &&
+        write_int_localized(out, static_cast<uint64_or_128_t<T>>(abs_value),
+                            prefix, specs, loc)) {
+      return out;
+    }
+    auto num_digits = count_digits(abs_value);
+    return write_int(
+        out, num_digits, prefix, specs, [=](reserve_iterator<OutputIt> it) {
+          return format_decimal<Char>(it, abs_value, num_digits).end;
+        });
+  }
+  case presentation_type::hex_lower:
+  case presentation_type::hex_upper: {
+    bool upper = specs.type == presentation_type::hex_upper;
+    if (specs.alt)
+      prefix_append(prefix, unsigned(upper ? 'X' : 'x') << 8 | '0');
+    int num_digits = count_digits<4>(abs_value);
+    return write_int(
+        out, num_digits, prefix, specs, [=](reserve_iterator<OutputIt> it) {
+          return format_uint<4, Char>(it, abs_value, num_digits, upper);
+        });
+  }
+  case presentation_type::bin_lower:
+  case presentation_type::bin_upper: {
+    bool upper = specs.type == presentation_type::bin_upper;
+    if (specs.alt)
+      prefix_append(prefix, unsigned(upper ? 'B' : 'b') << 8 | '0');
+    int num_digits = count_digits<1>(abs_value);
+    return write_int(out, num_digits, prefix, specs,
+                     [=](reserve_iterator<OutputIt> it) {
+                       return format_uint<1, Char>(it, abs_value, num_digits);
+                     });
+  }
+  case presentation_type::oct: {
+    int num_digits = count_digits<3>(abs_value);
+    // Octal prefix '0' is counted as a digit, so only add it if precision
+    // is not greater than the number of digits.
+    if (specs.alt && specs.precision <= num_digits && abs_value != 0)
+      prefix_append(prefix, '0');
+    return write_int(out, num_digits, prefix, specs,
+                     [=](reserve_iterator<OutputIt> it) {
+                       return format_uint<3, Char>(it, abs_value, num_digits);
+                     });
   }
-
-  template <typename T>
-  FMT_CONSTEXPR typename std::enable_if<
-      !is_integer<T>::value, unsigned long long>::type operator()(T) {
-    handler_.on_error("width is not integer");
-    return 0;
+  case presentation_type::chr:
+    return write_char(out, static_cast<Char>(abs_value), specs);
+  default:
+    throw_format_error("invalid type specifier");
   }
-
- private:
-  ErrorHandler &handler_;
+  return out;
+}
+template <typename Char, typename OutputIt, typename T>
+FMT_CONSTEXPR FMT_NOINLINE auto write_int_noinline(
+    OutputIt out, write_int_arg<T> arg, const basic_format_specs<Char>& specs,
+    locale_ref loc) -> OutputIt {
+  return write_int(out, arg, specs, loc);
+}
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(is_integral<T>::value &&
+                        !std::is_same<T, bool>::value &&
+                        std::is_same<OutputIt, buffer_appender<Char>>::value)>
+FMT_CONSTEXPR FMT_INLINE auto write(OutputIt out, T value,
+                                    const basic_format_specs<Char>& specs,
+                                    locale_ref loc) -> OutputIt {
+  return write_int_noinline(out, make_write_int_arg(value, specs.sign), specs,
+                            loc);
+}
+// An inlined version of write used in format string compilation.
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(is_integral<T>::value &&
+                        !std::is_same<T, bool>::value &&
+                        !std::is_same<OutputIt, buffer_appender<Char>>::value)>
+FMT_CONSTEXPR FMT_INLINE auto write(OutputIt out, T value,
+                                    const basic_format_specs<Char>& specs,
+                                    locale_ref loc) -> OutputIt {
+  return write_int(out, make_write_int_arg(value, specs.sign), specs, loc);
+}
+
+template <typename Char, typename OutputIt>
+FMT_CONSTEXPR auto write(OutputIt out, basic_string_view<Char> s,
+                         const basic_format_specs<Char>& specs) -> OutputIt {
+  auto data = s.data();
+  auto size = s.size();
+  if (specs.precision >= 0 && to_unsigned(specs.precision) < size)
+    size = code_point_index(s, to_unsigned(specs.precision));
+  auto width =
+      specs.width != 0 ? compute_width(basic_string_view<Char>(data, size)) : 0;
+  return write_padded(out, specs, size, width,
+                      [=](reserve_iterator<OutputIt> it) {
+                        return copy_str<Char>(data, data + size, it);
+                      });
+}
+template <typename Char, typename OutputIt>
+FMT_CONSTEXPR auto write(OutputIt out,
+                         basic_string_view<type_identity_t<Char>> s,
+                         const basic_format_specs<Char>& specs, locale_ref)
+    -> OutputIt {
+  check_string_type_spec(specs.type);
+  return write(out, s, specs);
+}
+template <typename Char, typename OutputIt>
+FMT_CONSTEXPR auto write(OutputIt out, const Char* s,
+                         const basic_format_specs<Char>& specs, locale_ref)
+    -> OutputIt {
+  return check_cstring_type_spec(specs.type)
+             ? write(out, basic_string_view<Char>(s), specs, {})
+             : write_ptr<Char>(out, to_uintptr(s), &specs);
+}
+
+template <typename Char, typename OutputIt>
+FMT_CONSTEXPR20 auto write_nonfinite(OutputIt out, bool isinf,
+                                     basic_format_specs<Char> specs,
+                                     const float_specs& fspecs) -> OutputIt {
+  auto str =
+      isinf ? (fspecs.upper ? "INF" : "inf") : (fspecs.upper ? "NAN" : "nan");
+  constexpr size_t str_size = 3;
+  auto sign = fspecs.sign;
+  auto size = str_size + (sign ? 1 : 0);
+  // Replace '0'-padding with space for non-finite values.
+  const bool is_zero_fill =
+      specs.fill.size() == 1 && *specs.fill.data() == static_cast<Char>('0');
+  if (is_zero_fill) specs.fill[0] = static_cast<Char>(' ');
+  return write_padded(out, specs, size, [=](reserve_iterator<OutputIt> it) {
+    if (sign) *it++ = detail::sign<Char>(sign);
+    return copy_str<Char>(str, str + str_size, it);
+  });
+}
+
+// A decimal floating-point number significand * pow(10, exp).
+struct big_decimal_fp {
+  const char* significand;
+  int significand_size;
+  int exponent;
 };
 
-template <typename ErrorHandler>
-class precision_checker: public function<unsigned long long> {
- public:
-  explicit FMT_CONSTEXPR precision_checker(ErrorHandler &eh) : handler_(eh) {}
+constexpr auto get_significand_size(const big_decimal_fp& fp) -> int {
+  return fp.significand_size;
+}
+template <typename T>
+inline auto get_significand_size(const dragonbox::decimal_fp<T>& fp) -> int {
+  return count_digits(fp.significand);
+}
 
-  template <typename T>
-  FMT_CONSTEXPR typename std::enable_if<
-      is_integer<T>::value, unsigned long long>::type operator()(T value) {
-    if (is_negative(value))
-      handler_.on_error("negative precision");
-    return static_cast<unsigned long long>(value);
+template <typename Char, typename OutputIt>
+constexpr auto write_significand(OutputIt out, const char* significand,
+                                 int significand_size) -> OutputIt {
+  return copy_str<Char>(significand, significand + significand_size, out);
+}
+template <typename Char, typename OutputIt, typename UInt>
+inline auto write_significand(OutputIt out, UInt significand,
+                              int significand_size) -> OutputIt {
+  return format_decimal<Char>(out, significand, significand_size).end;
+}
+template <typename Char, typename OutputIt, typename T, typename Grouping>
+FMT_CONSTEXPR20 auto write_significand(OutputIt out, T significand,
+                                       int significand_size, int exponent,
+                                       const Grouping& grouping) -> OutputIt {
+  if (!grouping.separator()) {
+    out = write_significand<Char>(out, significand, significand_size);
+    return detail::fill_n(out, exponent, static_cast<Char>('0'));
+  }
+  auto buffer = memory_buffer();
+  write_significand<char>(appender(buffer), significand, significand_size);
+  detail::fill_n(appender(buffer), exponent, '0');
+  return grouping.apply(out, string_view(buffer.data(), buffer.size()));
+}
+
+template <typename Char, typename UInt,
+          FMT_ENABLE_IF(std::is_integral<UInt>::value)>
+inline auto write_significand(Char* out, UInt significand, int significand_size,
+                              int integral_size, Char decimal_point) -> Char* {
+  if (!decimal_point)
+    return format_decimal(out, significand, significand_size).end;
+  out += significand_size + 1;
+  Char* end = out;
+  int floating_size = significand_size - integral_size;
+  for (int i = floating_size / 2; i > 0; --i) {
+    out -= 2;
+    copy2(out, digits2(significand % 100));
+    significand /= 100;
+  }
+  if (floating_size % 2 != 0) {
+    *--out = static_cast<Char>('0' + significand % 10);
+    significand /= 10;
   }
+  *--out = decimal_point;
+  format_decimal(out - integral_size, significand, integral_size);
+  return end;
+}
 
-  template <typename T>
-  FMT_CONSTEXPR typename std::enable_if<
-      !is_integer<T>::value, unsigned long long>::type operator()(T) {
-    handler_.on_error("precision is not integer");
-    return 0;
+template <typename OutputIt, typename UInt, typename Char,
+          FMT_ENABLE_IF(!std::is_pointer<remove_cvref_t<OutputIt>>::value)>
+inline auto write_significand(OutputIt out, UInt significand,
+                              int significand_size, int integral_size,
+                              Char decimal_point) -> OutputIt {
+  // Buffer is large enough to hold digits (digits10 + 1) and a decimal point.
+  Char buffer[digits10<UInt>() + 2];
+  auto end = write_significand(buffer, significand, significand_size,
+                               integral_size, decimal_point);
+  return detail::copy_str_noinline<Char>(buffer, end, out);
+}
+
+template <typename OutputIt, typename Char>
+FMT_CONSTEXPR auto write_significand(OutputIt out, const char* significand,
+                                     int significand_size, int integral_size,
+                                     Char decimal_point) -> OutputIt {
+  out = detail::copy_str_noinline<Char>(significand,
+                                        significand + integral_size, out);
+  if (!decimal_point) return out;
+  *out++ = decimal_point;
+  return detail::copy_str_noinline<Char>(significand + integral_size,
+                                         significand + significand_size, out);
+}
+
+template <typename OutputIt, typename Char, typename T, typename Grouping>
+FMT_CONSTEXPR20 auto write_significand(OutputIt out, T significand,
+                                       int significand_size, int integral_size,
+                                       Char decimal_point,
+                                       const Grouping& grouping) -> OutputIt {
+  if (!grouping.separator()) {
+    return write_significand(out, significand, significand_size, integral_size,
+                             decimal_point);
+  }
+  auto buffer = basic_memory_buffer<Char>();
+  write_significand(buffer_appender<Char>(buffer), significand,
+                    significand_size, integral_size, decimal_point);
+  grouping.apply(
+      out, basic_string_view<Char>(buffer.data(), to_unsigned(integral_size)));
+  return detail::copy_str_noinline<Char>(buffer.data() + integral_size,
+                                         buffer.end(), out);
+}
+
+template <typename OutputIt, typename DecimalFP, typename Char,
+          typename Grouping = digit_grouping<Char>>
+FMT_CONSTEXPR20 auto do_write_float(OutputIt out, const DecimalFP& fp,
+                                    const basic_format_specs<Char>& specs,
+                                    float_specs fspecs, locale_ref loc)
+    -> OutputIt {
+  auto significand = fp.significand;
+  int significand_size = get_significand_size(fp);
+  constexpr Char zero = static_cast<Char>('0');
+  auto sign = fspecs.sign;
+  size_t size = to_unsigned(significand_size) + (sign ? 1 : 0);
+  using iterator = reserve_iterator<OutputIt>;
+
+  Char decimal_point =
+      fspecs.locale ? detail::decimal_point<Char>(loc) : static_cast<Char>('.');
+
+  int output_exp = fp.exponent + significand_size - 1;
+  auto use_exp_format = [=]() {
+    if (fspecs.format == float_format::exp) return true;
+    if (fspecs.format != float_format::general) return false;
+    // Use the fixed notation if the exponent is in [exp_lower, exp_upper),
+    // e.g. 0.0001 instead of 1e-04. Otherwise use the exponent notation.
+    const int exp_lower = -4, exp_upper = 16;
+    return output_exp < exp_lower ||
+           output_exp >= (fspecs.precision > 0 ? fspecs.precision : exp_upper);
+  };
+  if (use_exp_format()) {
+    int num_zeros = 0;
+    if (fspecs.showpoint) {
+      num_zeros = fspecs.precision - significand_size;
+      if (num_zeros < 0) num_zeros = 0;
+      size += to_unsigned(num_zeros);
+    } else if (significand_size == 1) {
+      decimal_point = Char();
+    }
+    auto abs_output_exp = output_exp >= 0 ? output_exp : -output_exp;
+    int exp_digits = 2;
+    if (abs_output_exp >= 100) exp_digits = abs_output_exp >= 1000 ? 4 : 3;
+
+    size += to_unsigned((decimal_point ? 1 : 0) + 2 + exp_digits);
+    char exp_char = fspecs.upper ? 'E' : 'e';
+    auto write = [=](iterator it) {
+      if (sign) *it++ = detail::sign<Char>(sign);
+      // Insert a decimal point after the first digit and add an exponent.
+      it = write_significand(it, significand, significand_size, 1,
+                             decimal_point);
+      if (num_zeros > 0) it = detail::fill_n(it, num_zeros, zero);
+      *it++ = static_cast<Char>(exp_char);
+      return write_exponent<Char>(output_exp, it);
+    };
+    return specs.width > 0 ? write_padded<align::right>(out, specs, size, write)
+                           : base_iterator(out, write(reserve(out, size)));
   }
 
- private:
-  ErrorHandler &handler_;
-};
-
-// A format specifier handler that sets fields in basic_format_specs.
-template <typename Char>
-class specs_setter {
+  int exp = fp.exponent + significand_size;
+  if (fp.exponent >= 0) {
+    // 1234e5 -> 123400000[.0+]
+    size += to_unsigned(fp.exponent);
+    int num_zeros = fspecs.precision - exp;
+#ifdef FMT_FUZZ
+    if (num_zeros > 5000)
+      throw std::runtime_error("fuzz mode - avoiding excessive cpu use");
+#endif
+    if (fspecs.showpoint) {
+      if (num_zeros <= 0 && fspecs.format != float_format::fixed) num_zeros = 1;
+      if (num_zeros > 0) size += to_unsigned(num_zeros) + 1;
+    }
+    auto grouping = Grouping(loc, fspecs.locale);
+    size += to_unsigned(grouping.count_separators(significand_size));
+    return write_padded<align::right>(out, specs, size, [&](iterator it) {
+      if (sign) *it++ = detail::sign<Char>(sign);
+      it = write_significand<Char>(it, significand, significand_size,
+                                   fp.exponent, grouping);
+      if (!fspecs.showpoint) return it;
+      *it++ = decimal_point;
+      return num_zeros > 0 ? detail::fill_n(it, num_zeros, zero) : it;
+    });
+  } else if (exp > 0) {
+    // 1234e-2 -> 12.34[0+]
+    int num_zeros = fspecs.showpoint ? fspecs.precision - significand_size : 0;
+    size += 1 + to_unsigned(num_zeros > 0 ? num_zeros : 0);
+    auto grouping = Grouping(loc, fspecs.locale);
+    size += to_unsigned(grouping.count_separators(significand_size));
+    return write_padded<align::right>(out, specs, size, [&](iterator it) {
+      if (sign) *it++ = detail::sign<Char>(sign);
+      it = write_significand(it, significand, significand_size, exp,
+                             decimal_point, grouping);
+      return num_zeros > 0 ? detail::fill_n(it, num_zeros, zero) : it;
+    });
+  }
+  // 1234e-6 -> 0.001234
+  int num_zeros = -exp;
+  if (significand_size == 0 && fspecs.precision >= 0 &&
+      fspecs.precision < num_zeros) {
+    num_zeros = fspecs.precision;
+  }
+  bool pointy = num_zeros != 0 || significand_size != 0 || fspecs.showpoint;
+  size += 1 + (pointy ? 1 : 0) + to_unsigned(num_zeros);
+  return write_padded<align::right>(out, specs, size, [&](iterator it) {
+    if (sign) *it++ = detail::sign<Char>(sign);
+    *it++ = zero;
+    if (!pointy) return it;
+    *it++ = decimal_point;
+    it = detail::fill_n(it, num_zeros, zero);
+    return write_significand<Char>(it, significand, significand_size);
+  });
+}
+
+template <typename Char> class fallback_digit_grouping {
  public:
-  explicit FMT_CONSTEXPR specs_setter(basic_format_specs<Char> &specs):
-    specs_(specs) {}
-
-  FMT_CONSTEXPR specs_setter(const specs_setter &other): specs_(other.specs_) {}
-
-  FMT_CONSTEXPR void on_align(alignment align) { specs_.align_ = align; }
-  FMT_CONSTEXPR void on_fill(Char fill) { specs_.fill_ = fill; }
-  FMT_CONSTEXPR void on_plus() { specs_.flags |= SIGN_FLAG | PLUS_FLAG; }
-  FMT_CONSTEXPR void on_minus() { specs_.flags |= MINUS_FLAG; }
-  FMT_CONSTEXPR void on_space() { specs_.flags |= SIGN_FLAG; }
-  FMT_CONSTEXPR void on_hash() { specs_.flags |= HASH_FLAG; }
+  constexpr fallback_digit_grouping(locale_ref, bool) {}
 
-  FMT_CONSTEXPR void on_zero() {
-    specs_.align_ = ALIGN_NUMERIC;
-    specs_.fill_ = '0';
-  }
+  constexpr Char separator() const { return Char(); }
 
-  FMT_CONSTEXPR void on_width(unsigned width) { specs_.width_ = width; }
-  FMT_CONSTEXPR void on_precision(unsigned precision) {
-    specs_.precision = static_cast<int>(precision);
-  }
-  FMT_CONSTEXPR void end_precision() {}
+  constexpr int count_separators(int) const { return 0; }
 
-  FMT_CONSTEXPR void on_type(Char type) {
-    specs_.type = static_cast<char>(type);
+  template <typename Out, typename C>
+  constexpr Out apply(Out out, basic_string_view<C>) const {
+    return out;
   }
-
- protected:
-  basic_format_specs<Char> &specs_;
 };
 
-// A format specifier handler that checks if specifiers are consistent with the
-// argument type.
-template <typename Handler>
-class specs_checker : public Handler {
- public:
-  FMT_CONSTEXPR specs_checker(const Handler& handler, internal::type arg_type)
-    : Handler(handler), arg_type_(arg_type) {}
-
-  FMT_CONSTEXPR specs_checker(const specs_checker &other)
-    : Handler(other), arg_type_(other.arg_type_) {}
-
-  FMT_CONSTEXPR void on_align(alignment align) {
-    if (align == ALIGN_NUMERIC)
-      require_numeric_argument();
-    Handler::on_align(align);
-  }
-
-  FMT_CONSTEXPR void on_plus() {
-    check_sign();
-    Handler::on_plus();
+template <typename OutputIt, typename DecimalFP, typename Char>
+FMT_CONSTEXPR20 auto write_float(OutputIt out, const DecimalFP& fp,
+                                 const basic_format_specs<Char>& specs,
+                                 float_specs fspecs, locale_ref loc)
+    -> OutputIt {
+  if (is_constant_evaluated()) {
+    return do_write_float<OutputIt, DecimalFP, Char,
+                          fallback_digit_grouping<Char>>(out, fp, specs, fspecs,
+                                                         loc);
+  } else {
+    return do_write_float(out, fp, specs, fspecs, loc);
   }
+}
 
-  FMT_CONSTEXPR void on_minus() {
-    check_sign();
-    Handler::on_minus();
+template <typename T, FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+FMT_CONSTEXPR20 bool isinf(T value) {
+  if (is_constant_evaluated()) {
+#if defined(__cpp_if_constexpr)
+    if constexpr (std::numeric_limits<double>::is_iec559) {
+      auto bits = detail::bit_cast<uint64_t>(static_cast<double>(value));
+      constexpr auto significand_bits =
+          dragonbox::float_info<double>::significand_bits;
+      return (bits & exponent_mask<double>()) &&
+             !(bits & ((uint64_t(1) << significand_bits) - 1));
+    }
+#endif
   }
+  return std::isinf(value);
+}
 
-  FMT_CONSTEXPR void on_space() {
-    check_sign();
-    Handler::on_space();
+template <typename T, FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+FMT_CONSTEXPR20 bool isfinite(T value) {
+  if (is_constant_evaluated()) {
+#if defined(__cpp_if_constexpr)
+    if constexpr (std::numeric_limits<double>::is_iec559) {
+      auto bits = detail::bit_cast<uint64_t>(static_cast<double>(value));
+      return (bits & exponent_mask<double>()) != exponent_mask<double>();
+    }
+#endif
   }
+  return std::isfinite(value);
+}
 
-  FMT_CONSTEXPR void on_hash() {
-    require_numeric_argument();
-    Handler::on_hash();
+template <typename T, FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+FMT_INLINE FMT_CONSTEXPR bool signbit(T value) {
+  if (is_constant_evaluated()) {
+#ifdef __cpp_if_constexpr
+    if constexpr (std::numeric_limits<double>::is_iec559) {
+      auto bits = detail::bit_cast<uint64_t>(static_cast<double>(value));
+      return (bits & (uint64_t(1) << (num_bits<uint64_t>() - 1))) != 0;
+    }
+#endif
   }
+  return std::signbit(value);
+}
 
-  FMT_CONSTEXPR void on_zero() {
-    require_numeric_argument();
-    Handler::on_zero();
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+FMT_CONSTEXPR20 auto write(OutputIt out, T value,
+                           basic_format_specs<Char> specs, locale_ref loc = {})
+    -> OutputIt {
+  if (const_check(!is_supported_floating_point(value))) return out;
+  float_specs fspecs = parse_float_type_spec(specs);
+  fspecs.sign = specs.sign;
+  if (detail::signbit(value)) {  // value < 0 is false for NaN so use signbit.
+    fspecs.sign = sign::minus;
+    value = -value;
+  } else if (fspecs.sign == sign::minus) {
+    fspecs.sign = sign::none;
   }
 
-  FMT_CONSTEXPR void end_precision() {
-    if (is_integral(arg_type_) || arg_type_ == pointer_type)
-      this->on_error("precision not allowed for this argument type");
-  }
+  if (!detail::isfinite(value))
+    return write_nonfinite(out, detail::isinf(value), specs, fspecs);
 
- private:
-  FMT_CONSTEXPR void require_numeric_argument() {
-    if (!is_arithmetic(arg_type_))
-      this->on_error("format specifier requires numeric argument");
+  if (specs.align == align::numeric && fspecs.sign) {
+    auto it = reserve(out, 1);
+    *it++ = detail::sign<Char>(fspecs.sign);
+    out = base_iterator(out, it);
+    fspecs.sign = sign::none;
+    if (specs.width != 0) --specs.width;
   }
 
-  FMT_CONSTEXPR void check_sign() {
-    require_numeric_argument();
-    if (is_integral(arg_type_) && arg_type_ != int_type &&
-        arg_type_ != long_long_type && arg_type_ != internal::char_type) {
-      this->on_error("format specifier requires signed argument");
-    }
+  memory_buffer buffer;
+  if (fspecs.format == float_format::hex) {
+    if (fspecs.sign) buffer.push_back(detail::sign<char>(fspecs.sign));
+    snprintf_float(promote_float(value), specs.precision, fspecs, buffer);
+    return write_bytes<align::right>(out, {buffer.data(), buffer.size()},
+                                     specs);
+  }
+  int precision = specs.precision >= 0 || specs.type == presentation_type::none
+                      ? specs.precision
+                      : 6;
+  if (fspecs.format == float_format::exp) {
+    if (precision == max_value<int>())
+      throw_format_error("number is too big");
+    else
+      ++precision;
   }
-
-  internal::type arg_type_;
-};
-
-template <template <typename> class Handler, typename T,
-          typename Context, typename ErrorHandler>
-FMT_CONSTEXPR void set_dynamic_spec(
-    T &value, basic_format_arg<Context> arg, ErrorHandler eh) {
-  unsigned long long big_value =
-      visit_format_arg(Handler<ErrorHandler>(eh), arg);
-  if (big_value > to_unsigned((std::numeric_limits<int>::max)()))
-    eh.on_error("number is too big");
-  value = static_cast<T>(big_value);
+  if (const_check(std::is_same<T, float>())) fspecs.binary32 = true;
+  if (!is_fast_float<T>()) fspecs.fallback = true;
+  int exp = format_float(promote_float(value), precision, fspecs, buffer);
+  fspecs.precision = precision;
+  auto fp = big_decimal_fp{buffer.data(), static_cast<int>(buffer.size()), exp};
+  return write_float(out, fp, specs, fspecs, loc);
 }
 
-struct auto_id {};
-
-// The standard format specifier handler with checking.
-template <typename Context>
-class specs_handler: public specs_setter<typename Context::char_type> {
- public:
-  typedef typename Context::char_type char_type;
-
-  FMT_CONSTEXPR specs_handler(
-      basic_format_specs<char_type> &specs, Context &ctx)
-    : specs_setter<char_type>(specs), context_(ctx) {}
-
-  template <typename Id>
-  FMT_CONSTEXPR void on_dynamic_width(Id arg_id) {
-    set_dynamic_spec<width_checker>(
-          this->specs_.width_, get_arg(arg_id), context_.error_handler());
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(is_fast_float<T>::value)>
+FMT_CONSTEXPR20 auto write(OutputIt out, T value) -> OutputIt {
+  if (is_constant_evaluated()) {
+    return write(out, value, basic_format_specs<Char>());
   }
 
-  template <typename Id>
-  FMT_CONSTEXPR void on_dynamic_precision(Id arg_id) {
-    set_dynamic_spec<precision_checker>(
-          this->specs_.precision, get_arg(arg_id), context_.error_handler());
-  }
+  if (const_check(!is_supported_floating_point(value))) return out;
 
-  void on_error(const char *message) {
-    context_.on_error(message);
-  }
+  using floaty = conditional_t<std::is_same<T, long double>::value, double, T>;
+  using uint = typename dragonbox::float_info<floaty>::carrier_uint;
+  auto bits = bit_cast<uint>(value);
 
- private:
-  FMT_CONSTEXPR basic_format_arg<Context> get_arg(auto_id) {
-    return context_.next_arg();
+  auto fspecs = float_specs();
+  if (detail::signbit(value)) {
+    fspecs.sign = sign::minus;
+    value = -value;
   }
 
-  template <typename Id>
-  FMT_CONSTEXPR basic_format_arg<Context> get_arg(Id arg_id) {
-    context_.parse_context().check_arg_id(arg_id);
-    return context_.get_arg(arg_id);
+  constexpr auto specs = basic_format_specs<Char>();
+  uint mask = exponent_mask<floaty>();
+  if ((bits & mask) == mask)
+    return write_nonfinite(out, std::isinf(value), specs, fspecs);
+
+  auto dec = dragonbox::to_decimal(static_cast<floaty>(value));
+  return write_float(out, dec, specs, fspecs, {});
+}
+
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(std::is_floating_point<T>::value &&
+                        !is_fast_float<T>::value)>
+inline auto write(OutputIt out, T value) -> OutputIt {
+  return write(out, value, basic_format_specs<Char>());
+}
+
+template <typename Char, typename OutputIt>
+auto write(OutputIt out, monostate, basic_format_specs<Char> = {},
+           locale_ref = {}) -> OutputIt {
+  FMT_ASSERT(false, "");
+  return out;
+}
+
+template <typename Char, typename OutputIt>
+FMT_CONSTEXPR auto write(OutputIt out, basic_string_view<Char> value)
+    -> OutputIt {
+  auto it = reserve(out, value.size());
+  it = copy_str_noinline<Char>(value.begin(), value.end(), it);
+  return base_iterator(out, it);
+}
+
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(is_string<T>::value)>
+constexpr auto write(OutputIt out, const T& value) -> OutputIt {
+  return write<Char>(out, to_string_view(value));
+}
+
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(is_integral<T>::value &&
+                        !std::is_same<T, bool>::value &&
+                        !std::is_same<T, Char>::value)>
+FMT_CONSTEXPR auto write(OutputIt out, T value) -> OutputIt {
+  auto abs_value = static_cast<uint32_or_64_or_128_t<T>>(value);
+  bool negative = is_negative(value);
+  // Don't do -abs_value since it trips unsigned-integer-overflow sanitizer.
+  if (negative) abs_value = ~abs_value + 1;
+  int num_digits = count_digits(abs_value);
+  auto size = (negative ? 1 : 0) + static_cast<size_t>(num_digits);
+  auto it = reserve(out, size);
+  if (auto ptr = to_pointer<Char>(it, size)) {
+    if (negative) *ptr++ = static_cast<Char>('-');
+    format_decimal<Char>(ptr, abs_value, num_digits);
+    return out;
   }
+  if (negative) *it++ = static_cast<Char>('-');
+  it = format_decimal<Char>(it, abs_value, num_digits).end;
+  return base_iterator(out, it);
+}
 
-  Context &context_;
-};
+// FMT_ENABLE_IF() condition separated to workaround an MSVC bug.
+template <
+    typename Char, typename OutputIt, typename T,
+    bool check =
+        std::is_enum<T>::value && !std::is_same<T, Char>::value &&
+        mapped_type_constant<T, basic_format_context<OutputIt, Char>>::value !=
+            type::custom_type,
+    FMT_ENABLE_IF(check)>
+FMT_CONSTEXPR auto write(OutputIt out, T value) -> OutputIt {
+  return write<Char>(
+      out, static_cast<typename std::underlying_type<T>::type>(value));
+}
+
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(std::is_same<T, bool>::value)>
+FMT_CONSTEXPR auto write(OutputIt out, T value,
+                         const basic_format_specs<Char>& specs = {},
+                         locale_ref = {}) -> OutputIt {
+  return specs.type != presentation_type::none &&
+                 specs.type != presentation_type::string
+             ? write(out, value ? 1 : 0, specs, {})
+             : write_bytes(out, value ? "true" : "false", specs);
+}
+
+template <typename Char, typename OutputIt>
+FMT_CONSTEXPR auto write(OutputIt out, Char value) -> OutputIt {
+  auto it = reserve(out, 1);
+  *it++ = value;
+  return base_iterator(out, it);
+}
+
+template <typename Char, typename OutputIt>
+FMT_CONSTEXPR_CHAR_TRAITS auto write(OutputIt out, const Char* value)
+    -> OutputIt {
+  if (!value) {
+    throw_format_error("string pointer is null");
+  } else {
+    out = write(out, basic_string_view<Char>(value));
+  }
+  return out;
+}
 
-// An argument reference.
-template <typename Char>
-struct arg_ref {
-  enum Kind { NONE, INDEX, NAME };
+template <typename Char, typename OutputIt, typename T,
+          FMT_ENABLE_IF(std::is_same<T, void>::value)>
+auto write(OutputIt out, const T* value,
+           const basic_format_specs<Char>& specs = {}, locale_ref = {})
+    -> OutputIt {
+  check_pointer_type_spec(specs.type, error_handler());
+  return write_ptr<Char>(out, to_uintptr(value), &specs);
+}
+
+// A write overload that handles implicit conversions.
+template <typename Char, typename OutputIt, typename T,
+          typename Context = basic_format_context<OutputIt, Char>>
+FMT_CONSTEXPR auto write(OutputIt out, const T& value) -> enable_if_t<
+    std::is_class<T>::value && !is_string<T>::value &&
+        !std::is_same<T, Char>::value &&
+        !std::is_same<const T&,
+                      decltype(arg_mapper<Context>().map(value))>::value,
+    OutputIt> {
+  return write<Char>(out, arg_mapper<Context>().map(value));
+}
+
+template <typename Char, typename OutputIt, typename T,
+          typename Context = basic_format_context<OutputIt, Char>>
+FMT_CONSTEXPR auto write(OutputIt out, const T& value)
+    -> enable_if_t<mapped_type_constant<T, Context>::value == type::custom_type,
+                   OutputIt> {
+  using formatter_type =
+      conditional_t<has_formatter<T, Context>::value,
+                    typename Context::template formatter_type<T>,
+                    fallback_formatter<T, Char>>;
+  auto ctx = Context(out, {}, {});
+  return formatter_type().format(value, ctx);
+}
+
+// An argument visitor that formats the argument and writes it via the output
+// iterator. It's a class and not a generic lambda for compatibility with C++11.
+template <typename Char> struct default_arg_formatter {
+  using iterator = buffer_appender<Char>;
+  using context = buffer_context<Char>;
+
+  iterator out;
+  basic_format_args<context> args;
+  locale_ref loc;
+
+  template <typename T> auto operator()(T value) -> iterator {
+    return write<Char>(out, value);
+  }
+  auto operator()(typename basic_format_arg<context>::handle h) -> iterator {
+    basic_format_parse_context<Char> parse_ctx({});
+    context format_ctx(out, args, loc);
+    h.format(parse_ctx, format_ctx);
+    return format_ctx.out();
+  }
+};
+
+template <typename Char> struct arg_formatter {
+  using iterator = buffer_appender<Char>;
+  using context = buffer_context<Char>;
+
+  iterator out;
+  const basic_format_specs<Char>& specs;
+  locale_ref locale;
 
-  FMT_CONSTEXPR arg_ref() : kind(NONE), index(0) {}
-  FMT_CONSTEXPR explicit arg_ref(unsigned index) : kind(INDEX), index(index) {}
-  explicit arg_ref(basic_string_view<Char> nm) : kind(NAME) {
-    name = {nm.data(), nm.size()};
+  template <typename T>
+  FMT_CONSTEXPR FMT_INLINE auto operator()(T value) -> iterator {
+    return detail::write(out, value, specs, locale);
   }
-
-  FMT_CONSTEXPR arg_ref &operator=(unsigned idx) {
-    kind = INDEX;
-    index = idx;
-    return *this;
+  auto operator()(typename basic_format_arg<context>::handle) -> iterator {
+    // User-defined types are handled separately because they require access
+    // to the parse context.
+    return out;
   }
-
-  Kind kind;
-  union {
-    unsigned index;
-    string_value<Char> name;  // This is not string_view because of gcc 4.4.
-  };
-};
-
-// Format specifiers with width and precision resolved at formatting rather
-// than parsing time to allow re-using the same parsed specifiers with
-// differents sets of arguments (precompilation of format strings).
-template <typename Char>
-struct dynamic_format_specs : basic_format_specs<Char> {
-  arg_ref<Char> width_ref;
-  arg_ref<Char> precision_ref;
 };
 
-// Format spec handler that saves references to arguments representing dynamic
-// width and precision to be resolved at formatting time.
-template <typename ParseContext>
-class dynamic_specs_handler :
-    public specs_setter<typename ParseContext::char_type> {
- public:
-  typedef typename ParseContext::char_type char_type;
-
-  FMT_CONSTEXPR dynamic_specs_handler(
-      dynamic_format_specs<char_type> &specs, ParseContext &ctx)
-    : specs_setter<char_type>(specs), specs_(specs), context_(ctx) {}
-
-  FMT_CONSTEXPR dynamic_specs_handler(const dynamic_specs_handler &other)
-    : specs_setter<char_type>(other),
-      specs_(other.specs_), context_(other.context_) {}
-
-  template <typename Id>
-  FMT_CONSTEXPR void on_dynamic_width(Id arg_id) {
-    specs_.width_ref = make_arg_ref(arg_id);
+template <typename Char> struct custom_formatter {
+  basic_format_parse_context<Char>& parse_ctx;
+  buffer_context<Char>& ctx;
+
+  void operator()(
+      typename basic_format_arg<buffer_context<Char>>::handle h) const {
+    h.format(parse_ctx, ctx);
   }
+  template <typename T> void operator()(T) const {}
+};
 
-  template <typename Id>
-  FMT_CONSTEXPR void on_dynamic_precision(Id arg_id) {
-    specs_.precision_ref = make_arg_ref(arg_id);
+template <typename T>
+using is_integer =
+    bool_constant<is_integral<T>::value && !std::is_same<T, bool>::value &&
+                  !std::is_same<T, char>::value &&
+                  !std::is_same<T, wchar_t>::value>;
+
+template <typename ErrorHandler> class width_checker {
+ public:
+  explicit FMT_CONSTEXPR width_checker(ErrorHandler& eh) : handler_(eh) {}
+
+  template <typename T, FMT_ENABLE_IF(is_integer<T>::value)>
+  FMT_CONSTEXPR auto operator()(T value) -> unsigned long long {
+    if (is_negative(value)) handler_.on_error("negative width");
+    return static_cast<unsigned long long>(value);
   }
 
-  FMT_CONSTEXPR void on_error(const char *message) {
-    context_.on_error(message);
+  template <typename T, FMT_ENABLE_IF(!is_integer<T>::value)>
+  FMT_CONSTEXPR auto operator()(T) -> unsigned long long {
+    handler_.on_error("width is not integer");
+    return 0;
   }
 
  private:
-  typedef arg_ref<char_type> arg_ref_type;
-
-  template <typename Id>
-  FMT_CONSTEXPR arg_ref_type make_arg_ref(Id arg_id) {
-    context_.check_arg_id(arg_id);
-    return arg_ref_type(arg_id);
-  }
-
-  FMT_CONSTEXPR arg_ref_type make_arg_ref(auto_id) {
-    return arg_ref_type(context_.next_arg_id());
-  }
-
-  dynamic_format_specs<char_type> &specs_;
-  ParseContext &context_;
-};
-
-template <typename Char, typename IDHandler>
-FMT_CONSTEXPR const Char *parse_arg_id(
-    const Char *begin, const Char *end, IDHandler &&handler) {
-  assert(begin != end);
-  Char c = *begin;
-  if (c == '}' || c == ':')
-    return handler(), begin;
-  if (c >= '0' && c <= '9') {
-    unsigned index = parse_nonnegative_int(begin, end, handler);
-    if (begin == end || (*begin != '}' && *begin != ':'))
-      return handler.on_error("invalid format string"), begin;
-    handler(index);
-    return begin;
-  }
-  if (!is_name_start(c))
-    return handler.on_error("invalid format string"), begin;
-  auto it = begin;
-  do {
-    ++it;
-  } while (it != end && (is_name_start(c = *it) || ('0' <= c && c <= '9')));
-  handler(basic_string_view<Char>(begin, to_unsigned(it - begin)));
-  return it;
-}
-
-// Adapts SpecHandler to IDHandler API for dynamic width.
-template <typename SpecHandler, typename Char>
-struct width_adapter {
-  explicit FMT_CONSTEXPR width_adapter(SpecHandler &h) : handler(h) {}
-
-  FMT_CONSTEXPR void operator()() { handler.on_dynamic_width(auto_id()); }
-  FMT_CONSTEXPR void operator()(unsigned id) { handler.on_dynamic_width(id); }
-  FMT_CONSTEXPR void operator()(basic_string_view<Char> id) {
-    handler.on_dynamic_width(id);
-  }
-
-  FMT_CONSTEXPR void on_error(const char *message) {
-    handler.on_error(message);
-  }
-
-  SpecHandler &handler;
+  ErrorHandler& handler_;
 };
 
-// Adapts SpecHandler to IDHandler API for dynamic precision.
-template <typename SpecHandler, typename Char>
-struct precision_adapter {
-  explicit FMT_CONSTEXPR precision_adapter(SpecHandler &h) : handler(h) {}
+template <typename ErrorHandler> class precision_checker {
+ public:
+  explicit FMT_CONSTEXPR precision_checker(ErrorHandler& eh) : handler_(eh) {}
 
-  FMT_CONSTEXPR void operator()() { handler.on_dynamic_precision(auto_id()); }
-  FMT_CONSTEXPR void operator()(unsigned id) {
-    handler.on_dynamic_precision(id);
-  }
-  FMT_CONSTEXPR void operator()(basic_string_view<Char> id) {
-    handler.on_dynamic_precision(id);
+  template <typename T, FMT_ENABLE_IF(is_integer<T>::value)>
+  FMT_CONSTEXPR auto operator()(T value) -> unsigned long long {
+    if (is_negative(value)) handler_.on_error("negative precision");
+    return static_cast<unsigned long long>(value);
   }
 
-  FMT_CONSTEXPR void on_error(const char *message) { handler.on_error(message); }
+  template <typename T, FMT_ENABLE_IF(!is_integer<T>::value)>
+  FMT_CONSTEXPR auto operator()(T) -> unsigned long long {
+    handler_.on_error("precision is not integer");
+    return 0;
+  }
 
-  SpecHandler &handler;
+ private:
+  ErrorHandler& handler_;
 };
 
-// Parses fill and alignment.
-template <typename Char, typename Handler>
-FMT_CONSTEXPR const Char *parse_align(
-    const Char *begin, const Char *end, Handler &&handler) {
-  FMT_ASSERT(begin != end, "");
-  alignment align = ALIGN_DEFAULT;
-  int i = 0;
-  if (begin + 1 != end) ++i;
-  do {
-    switch (static_cast<char>(begin[i])) {
-    case '<':
-      align = ALIGN_LEFT;
-      break;
-    case '>':
-      align = ALIGN_RIGHT;
-      break;
-    case '=':
-      align = ALIGN_NUMERIC;
-      break;
-    case '^':
-      align = ALIGN_CENTER;
-      break;
-    }
-    if (align != ALIGN_DEFAULT) {
-      if (i > 0) {
-        auto c = *begin;
-        if (c == '{')
-          return handler.on_error("invalid fill character '{'"), begin;
-        begin += 2;
-        handler.on_fill(c);
-      } else ++begin;
-      handler.on_align(align);
-      break;
-    }
-  } while (i-- > 0);
-  return begin;
-}
-
-template <typename Char, typename Handler>
-FMT_CONSTEXPR const Char *parse_width(
-    const Char *begin, const Char *end, Handler &&handler) {
-  FMT_ASSERT(begin != end, "");
-  if ('0' <= *begin && *begin <= '9') {
-    handler.on_width(parse_nonnegative_int(begin, end, handler));
-  } else if (*begin == '{') {
-    ++begin;
-    if (begin != end)
-      begin = parse_arg_id(begin, end, width_adapter<Handler, Char>(handler));
-    if (begin == end || *begin != '}')
-      return handler.on_error("invalid format string"), begin;
-    ++begin;
-  }
-  return begin;
-}
-
-// Parses standard format specifiers and sends notifications about parsed
-// components to handler.
-template <typename Char, typename SpecHandler>
-FMT_CONSTEXPR const Char *parse_format_specs(
-    const Char *begin, const Char *end, SpecHandler &&handler) {
-  if (begin == end || *begin == '}')
-    return begin;
+template <template <typename> class Handler, typename FormatArg,
+          typename ErrorHandler>
+FMT_CONSTEXPR auto get_dynamic_spec(FormatArg arg, ErrorHandler eh) -> int {
+  unsigned long long value = visit_format_arg(Handler<ErrorHandler>(eh), arg);
+  if (value > to_unsigned(max_value<int>())) eh.on_error("number is too big");
+  return static_cast<int>(value);
+}
+
+template <typename Context, typename ID>
+FMT_CONSTEXPR auto get_arg(Context& ctx, ID id) ->
+    typename Context::format_arg {
+  auto arg = ctx.arg(id);
+  if (!arg) ctx.on_error("argument not found");
+  return arg;
+}
 
-  begin = parse_align(begin, end, handler);
-  if (begin == end) return begin;
+// The standard format specifier handler with checking.
+template <typename Char> class specs_handler : public specs_setter<Char> {
+ private:
+  basic_format_parse_context<Char>& parse_context_;
+  buffer_context<Char>& context_;
 
-  // Parse sign.
-  switch (static_cast<char>(*begin)) {
-  case '+':
-    handler.on_plus();
-    ++begin;
-    break;
-  case '-':
-    handler.on_minus();
-    ++begin;
-    break;
-  case ' ':
-    handler.on_space();
-    ++begin;
-    break;
-  }
-  if (begin == end) return begin;
+  // This is only needed for compatibility with gcc 4.4.
+  using format_arg = basic_format_arg<buffer_context<Char>>;
 
-  if (*begin == '#') {
-    handler.on_hash();
-    if (++begin == end) return begin;
-  }
-
-  // Parse zero flag.
-  if (*begin == '0') {
-    handler.on_zero();
-    if (++begin == end) return begin;
-  }
-
-  begin = parse_width(begin, end, handler);
-  if (begin == end) return begin;
-
-  // Parse precision.
-  if (*begin == '.') {
-    ++begin;
-    auto c = begin != end ? *begin : 0;
-    if ('0' <= c && c <= '9') {
-      handler.on_precision(parse_nonnegative_int(begin, end, handler));
-    } else if (c == '{') {
-      ++begin;
-      if (begin != end) {
-        begin = parse_arg_id(
-              begin, end, precision_adapter<SpecHandler, Char>(handler));
-      }
-      if (begin == end || *begin++ != '}')
-        return handler.on_error("invalid format string"), begin;
-    } else {
-      return handler.on_error("missing precision specifier"), begin;
-    }
-    handler.end_precision();
+  FMT_CONSTEXPR auto get_arg(auto_id) -> format_arg {
+    return detail::get_arg(context_, parse_context_.next_arg_id());
   }
 
-  // Parse type.
-  if (begin != end && *begin != '}')
-    handler.on_type(*begin++);
-  return begin;
-}
-
-// Return the result via the out param to workaround gcc bug 77539.
-template <bool IS_CONSTEXPR, typename T, typename Ptr = const T*>
-FMT_CONSTEXPR bool find(Ptr first, Ptr last, T value, Ptr &out) {
-  for (out = first; out != last; ++out) {
-    if (*out == value)
-      return true;
+  FMT_CONSTEXPR auto get_arg(int arg_id) -> format_arg {
+    parse_context_.check_arg_id(arg_id);
+    return detail::get_arg(context_, arg_id);
   }
-  return false;
-}
 
-template <>
-inline bool find<false, char>(
-    const char *first, const char *last, char value, const char *&out) {
-  out = static_cast<const char*>(std::memchr(first, value, internal::to_unsigned(last - first)));
-  return out != FMT_NULL;
-}
-
-template <typename Handler, typename Char>
-struct id_adapter {
-  FMT_CONSTEXPR void operator()() { handler.on_arg_id(); }
-  FMT_CONSTEXPR void operator()(unsigned id) { handler.on_arg_id(id); }
-  FMT_CONSTEXPR void operator()(basic_string_view<Char> id) {
-    handler.on_arg_id(id);
-  }
-  FMT_CONSTEXPR void on_error(const char *message) {
-    handler.on_error(message);
-  }
-  Handler &handler;
-};
-
-template <bool IS_CONSTEXPR, typename Char, typename Handler>
-FMT_CONSTEXPR void parse_format_string(
-        basic_string_view<Char> format_str, Handler &&handler) {
-  struct writer {
-    FMT_CONSTEXPR void operator()(const Char *begin, const Char *end) {
-      if (begin == end) return;
-      for (;;) {
-        const Char *p = FMT_NULL;
-        if (!find<IS_CONSTEXPR>(begin, end, '}', p))
-          return handler_.on_text(begin, end);
-        ++p;
-        if (p == end || *p != '}')
-          return handler_.on_error("unmatched '}' in format string");
-        handler_.on_text(begin, p);
-        begin = p + 1;
-      }
-    }
-    Handler &handler_;
-  } write{handler};
-  auto begin = format_str.data();
-  auto end = begin + format_str.size();
-  while (begin != end) {
-    // Doing two passes with memchr (one for '{' and another for '}') is up to
-    // 2.5x faster than the naive one-pass implementation on big format strings.
-    const Char *p = begin;
-    if (*begin != '{' && !find<IS_CONSTEXPR>(begin, end, '{', p))
-      return write(begin, end);
-    write(begin, p);
-    ++p;
-    if (p == end)
-      return handler.on_error("invalid format string");
-    if (static_cast<char>(*p) == '}') {
-      handler.on_arg_id();
-      handler.on_replacement_field(p);
-    } else if (*p == '{') {
-      handler.on_text(p, p + 1);
-    } else {
-      p = parse_arg_id(p, end, id_adapter<Handler, Char>{handler});
-      Char c = p != end ? *p : Char();
-      if (c == '}') {
-        handler.on_replacement_field(p);
-      } else if (c == ':') {
-        p = handler.on_format_specs(p + 1, end);
-        if (p == end || *p != '}')
-          return handler.on_error("unknown format specifier");
-      } else {
-        return handler.on_error("missing '}' in format string");
-      }
-    }
-    begin = p + 1;
+  FMT_CONSTEXPR auto get_arg(basic_string_view<Char> arg_id) -> format_arg {
+    parse_context_.check_arg_id(arg_id);
+    return detail::get_arg(context_, arg_id);
   }
-}
-
-template <typename T, typename ParseContext>
-FMT_CONSTEXPR const typename ParseContext::char_type *
-    parse_format_specs(ParseContext &ctx) {
-  // GCC 7.2 requires initializer.
-  formatter<T, typename ParseContext::char_type> f{};
-  return f.parse(ctx);
-}
 
-template <typename Char, typename ErrorHandler, typename... Args>
-class format_string_checker {
  public:
-  explicit FMT_CONSTEXPR format_string_checker(
-      basic_string_view<Char> format_str, ErrorHandler eh)
-    : arg_id_((std::numeric_limits<unsigned>::max)()), context_(format_str, eh),
-      parse_funcs_{&parse_format_specs<Args, parse_context_type>...} {}
-
-  FMT_CONSTEXPR void on_text(const Char *, const Char *) {}
+  FMT_CONSTEXPR specs_handler(basic_format_specs<Char>& specs,
+                              basic_format_parse_context<Char>& parse_ctx,
+                              buffer_context<Char>& ctx)
+      : specs_setter<Char>(specs), parse_context_(parse_ctx), context_(ctx) {}
 
-  FMT_CONSTEXPR void on_arg_id() {
-    arg_id_ = context_.next_arg_id();
-    check_arg_id();
+  template <typename Id> FMT_CONSTEXPR void on_dynamic_width(Id arg_id) {
+    this->specs_.width = get_dynamic_spec<width_checker>(
+        get_arg(arg_id), context_.error_handler());
   }
-  FMT_CONSTEXPR void on_arg_id(unsigned id) {
-    arg_id_ = id;
-    context_.check_arg_id(id);
-    check_arg_id();
-  }
-  FMT_CONSTEXPR void on_arg_id(basic_string_view<Char>) {}
-
-  FMT_CONSTEXPR void on_replacement_field(const Char *) {}
-
-  FMT_CONSTEXPR const Char *on_format_specs(const Char *begin, const Char *) {
-    context_.advance_to(begin);
-    return arg_id_ < NUM_ARGS ?
-          parse_funcs_[arg_id_](context_) : begin;
-  }
-
-  FMT_CONSTEXPR void on_error(const char *message) {
-    context_.on_error(message);
-  }
-
- private:
-  typedef basic_parse_context<Char, ErrorHandler> parse_context_type;
-  enum { NUM_ARGS = sizeof...(Args) };
 
-  FMT_CONSTEXPR void check_arg_id() {
-    if (arg_id_ >= NUM_ARGS)
-      context_.on_error("argument index out of range");
+  template <typename Id> FMT_CONSTEXPR void on_dynamic_precision(Id arg_id) {
+    this->specs_.precision = get_dynamic_spec<precision_checker>(
+        get_arg(arg_id), context_.error_handler());
   }
 
-  // Format specifier parsing function.
-  typedef const Char *(*parse_func)(parse_context_type &);
-
-  unsigned arg_id_;
-  parse_context_type context_;
-  parse_func parse_funcs_[NUM_ARGS > 0 ? NUM_ARGS : 1];
+  void on_error(const char* message) { context_.on_error(message); }
 };
 
-template <typename Char, typename ErrorHandler, typename... Args>
-FMT_CONSTEXPR bool do_check_format_string(
-    basic_string_view<Char> s, ErrorHandler eh = ErrorHandler()) {
-  format_string_checker<Char, ErrorHandler, Args...> checker(s, eh);
-  parse_format_string<true>(s, checker);
-  return true;
-}
-
-template <typename... Args, typename S>
-typename std::enable_if<is_compile_string<S>::value>::type
-    check_format_string(S format_str) {
-  typedef typename S::char_type char_t;
-  FMT_CONSTEXPR_DECL bool invalid_format = internal::do_check_format_string<
-      char_t, internal::error_handler, Args...>(to_string_view(format_str));
-  (void)invalid_format;
-}
-
-// Specifies whether to format T using the standard formatter.
-// It is not possible to use get_type in formatter specialization directly
-// because of a bug in MSVC.
-template <typename Context, typename T>
-struct format_type :
-  std::integral_constant<bool, get_type<Context, T>::value != custom_type> {};
-
-template <template <typename> class Handler, typename Spec, typename Context>
-void handle_dynamic_spec(
-    Spec &value, arg_ref<typename Context::char_type> ref, Context &ctx) {
-  typedef typename Context::char_type char_type;
+template <template <typename> class Handler, typename Context>
+FMT_CONSTEXPR void handle_dynamic_spec(int& value,
+                                       arg_ref<typename Context::char_type> ref,
+                                       Context& ctx) {
   switch (ref.kind) {
-  case arg_ref<char_type>::NONE:
+  case arg_id_kind::none:
     break;
-  case arg_ref<char_type>::INDEX:
-    internal::set_dynamic_spec<Handler>(
-          value, ctx.get_arg(ref.index), ctx.error_handler());
+  case arg_id_kind::index:
+    value = detail::get_dynamic_spec<Handler>(ctx.arg(ref.val.index),
+                                              ctx.error_handler());
     break;
-  case arg_ref<char_type>::NAME:
-    internal::set_dynamic_spec<Handler>(
-          value, ctx.get_arg({ref.name.value, ref.name.size}),
-          ctx.error_handler());
+  case arg_id_kind::name:
+    value = detail::get_dynamic_spec<Handler>(ctx.arg(ref.val.name),
+                                              ctx.error_handler());
     break;
   }
 }
-}  // namespace internal
-
-/** The default argument formatter. */
-template <typename Range>
-class arg_formatter:
-  public internal::function<
-    typename internal::arg_formatter_base<Range>::iterator>,
-  public internal::arg_formatter_base<Range> {
- private:
-  typedef typename Range::value_type char_type;
-  typedef internal::arg_formatter_base<Range> base;
-  typedef basic_format_context<typename base::iterator, char_type> context_type;
-
-  context_type &ctx_;
-
- public:
-  typedef Range range;
-  typedef typename base::iterator iterator;
-  typedef typename base::format_specs format_specs;
-
-  /**
-    \rst
-    Constructs an argument formatter object.
-    *ctx* is a reference to the formatting context,
-    *spec* contains format specifier information for standard argument types.
-    \endrst
-   */
-  explicit arg_formatter(context_type &ctx, format_specs *spec = FMT_NULL)
-  : base(Range(ctx.out()), spec, ctx.locale()), ctx_(ctx) {}
 
-  // Deprecated.
-  arg_formatter(context_type &ctx, format_specs &spec)
-  : base(Range(ctx.out()), &spec), ctx_(ctx) {}
-
-  using base::operator();
-
-  /** Formats an argument of a user-defined type. */
-  iterator operator()(typename basic_format_arg<context_type>::handle handle) {
-    handle.format(ctx_);
-    return this->out();
-  }
-};
-
-/**
- An error returned by an operating system or a language runtime,
- for example a file opening error.
-*/
-class system_error : public std::runtime_error {
- private:
-  FMT_API void init(int err_code, string_view format_str, format_args args);
-
- protected:
-  int error_code_;
-
-  system_error() : std::runtime_error("") {}
-
- public:
-  /**
-   \rst
-   Constructs a :class:`fmt::system_error` object with a description
-   formatted with `fmt::format_system_error`. *message* and additional
-   arguments passed into the constructor are formatted similarly to
-   `fmt::format`.
-
-   **Example**::
-
-     // This throws a system_error with the description
-     //   cannot open file 'madeup': No such file or directory
-     // or similar (system message may vary).
-     const char *filename = "madeup";
-     std::FILE *file = std::fopen(filename, "r");
-     if (!file)
-       throw fmt::system_error(errno, "cannot open file '{}'", filename);
-   \endrst
-  */
-  template <typename... Args>
-  system_error(int error_code, string_view message, const Args &... args)
-    : std::runtime_error("") {
-    init(error_code, message, make_format_args(args...));
-  }
-
-  int error_code() const { return error_code_; }
-};
+#define FMT_STRING_IMPL(s, base, explicit)                                 \
+  [] {                                                                     \
+    /* Use the hidden visibility as a workaround for a GCC bug (#1973). */ \
+    /* Use a macro-like name to avoid shadowing warnings. */               \
+    struct FMT_GCC_VISIBILITY_HIDDEN FMT_COMPILE_STRING : base {           \
+      using char_type = fmt::remove_cvref_t<decltype(s[0])>;               \
+      FMT_MAYBE_UNUSED FMT_CONSTEXPR explicit                              \
+      operator fmt::basic_string_view<char_type>() const {                 \
+        return fmt::detail_exported::compile_string_to_view<char_type>(s); \
+      }                                                                    \
+    };                                                                     \
+    return FMT_COMPILE_STRING();                                           \
+  }()
 
 /**
   \rst
-  Formats an error returned by an operating system or a language runtime,
-  for example a file opening error, and writes it to *out* in the following
-  form:
+  Constructs a compile-time format string from a string literal *s*.
 
-  .. parsed-literal::
-     *<message>*: *<system-message>*
+  **Example**::
 
-  where *<message>* is the passed message and *<system-message>* is
-  the system message corresponding to the error code.
-  *error_code* is a system error code as given by ``errno``.
-  If *error_code* is not a valid error code such as -1, the system message
-  may look like "Unknown error -1" and is platform-dependent.
+    // A compile-time error because 'd' is an invalid specifier for strings.
+    std::string s = fmt::format(FMT_STRING("{:d}"), "foo");
   \endrst
  */
-FMT_API void format_system_error(internal::buffer &out, int error_code,
-                                 fmt::string_view message) FMT_NOEXCEPT;
-
-/**
-  This template provides operations for formatting and writing data into a
-  character range.
- */
-template <typename Range>
-class basic_writer {
- public:
-  typedef typename Range::value_type char_type;
-  typedef decltype(internal::declval<Range>().begin()) iterator;
-  typedef basic_format_specs<char_type> format_specs;
+#define FMT_STRING(s) FMT_STRING_IMPL(s, fmt::compile_string, )
 
- private:
-  iterator out_;  // Output iterator.
-  internal::locale_ref locale_;
+#if FMT_USE_USER_DEFINED_LITERALS
+template <typename Char> struct udl_formatter {
+  basic_string_view<Char> str;
 
-  // Attempts to reserve space for n extra characters in the output range.
-  // Returns a pointer to the reserved range or a reference to out_.
-  auto reserve(std::size_t n) -> decltype(internal::reserve(out_, n)) {
-    return internal::reserve(out_, n);
-  }
-
-  // Writes a value in the format
-  //   <left-padding><value><right-padding>
-  // where <value> is written by f(it).
-  template <typename F>
-  void write_padded(const align_spec &spec, F &&f) {
-    unsigned width = spec.width(); // User-perceived width (in code points).
-    size_t size = f.size(); // The number of code units.
-    size_t num_code_points = width != 0 ? f.width() : size;
-    if (width <= num_code_points)
-      return f(reserve(size));
-    auto &&it = reserve(width + (size - num_code_points));
-    char_type fill = static_cast<char_type>(spec.fill());
-    std::size_t padding = width - num_code_points;
-    if (spec.align() == ALIGN_RIGHT) {
-      it = std::fill_n(it, padding, fill);
-      f(it);
-    } else if (spec.align() == ALIGN_CENTER) {
-      std::size_t left_padding = padding / 2;
-      it = std::fill_n(it, left_padding, fill);
-      f(it);
-      it = std::fill_n(it, padding - left_padding, fill);
-    } else {
-      f(it);
-      it = std::fill_n(it, padding, fill);
-    }
+  template <typename... T>
+  auto operator()(T&&... args) const -> std::basic_string<Char> {
+    return vformat(str, fmt::make_args_checked<T...>(str, args...));
   }
+};
 
-  template <typename F>
-  struct padded_int_writer {
-    size_t size_;
-    string_view prefix;
-    char_type fill;
-    std::size_t padding;
-    F f;
-
-    size_t size() const { return size_; }
-    size_t width() const { return size_; }
-
-    template <typename It>
-    void operator()(It &&it) const {
-      if (prefix.size() != 0)
-        it = internal::copy_str<char_type>(prefix.begin(), prefix.end(), it);
-      it = std::fill_n(it, padding, fill);
-      f(it);
-    }
-  };
-
-  // Writes an integer in the format
-  //   <left-padding><prefix><numeric-padding><digits><right-padding>
-  // where <digits> are written by f(it).
-  template <typename Spec, typename F>
-  void write_int(int num_digits, string_view prefix,
-                 const Spec &spec, F f) {
-    std::size_t size = prefix.size() + internal::to_unsigned(num_digits);
-    char_type fill = static_cast<char_type>(spec.fill());
-    std::size_t padding = 0;
-    if (spec.align() == ALIGN_NUMERIC) {
-      if (spec.width() > size) {
-        padding = spec.width() - size;
-        size = spec.width();
-      }
-    } else if (spec.precision > num_digits) {
-      size = prefix.size() + internal::to_unsigned(spec.precision);
-      padding = internal::to_unsigned(spec.precision - num_digits);
-      fill = static_cast<char_type>('0');
-    }
-    align_spec as = spec;
-    if (spec.align() == ALIGN_DEFAULT)
-      as.align_ = ALIGN_RIGHT;
-    write_padded(as, padded_int_writer<F>{size, prefix, fill, padding, f});
-  }
-
-  // Writes a decimal integer.
-  template <typename Int>
-  void write_decimal(Int value) {
-    typedef typename internal::int_traits<Int>::main_type main_type;
-    main_type abs_value = static_cast<main_type>(value);
-    bool is_negative = internal::is_negative(value);
-    if (is_negative)
-      abs_value = 0 - abs_value;
-    int num_digits = internal::count_digits(abs_value);
-    auto &&it = reserve((is_negative ? 1 : 0) + static_cast<size_t>(num_digits));
-    if (is_negative)
-      *it++ = static_cast<char_type>('-');
-    it = internal::format_decimal<char_type>(it, abs_value, num_digits);
-  }
-
-  // The handle_int_type_spec handler that writes an integer.
-  template <typename Int, typename Spec>
-  struct int_writer {
-    typedef typename internal::int_traits<Int>::main_type unsigned_type;
-
-    basic_writer<Range> &writer;
-    const Spec &spec;
-    unsigned_type abs_value;
-    char prefix[4];
-    unsigned prefix_size;
-
-    string_view get_prefix() const { return string_view(prefix, prefix_size); }
-
-    // Counts the number of digits in abs_value. BITS = log2(radix).
-    template <unsigned BITS>
-    int count_digits() const {
-      unsigned_type n = abs_value;
-      int num_digits = 0;
-      do {
-        ++num_digits;
-      } while ((n >>= BITS) != 0);
-      return num_digits;
-    }
-
-    int_writer(basic_writer<Range> &w, Int value, const Spec &s)
-      : writer(w), spec(s), abs_value(static_cast<unsigned_type>(value)),
-        prefix_size(0) {
-      if (internal::is_negative(value)) {
-        prefix[0] = '-';
-        ++prefix_size;
-        abs_value = 0 - abs_value;
-      } else if (spec.has(SIGN_FLAG)) {
-        prefix[0] = spec.has(PLUS_FLAG) ? '+' : ' ';
-        ++prefix_size;
-      }
-    }
-
-    struct dec_writer {
-      unsigned_type abs_value;
-      int num_digits;
-
-      template <typename It>
-      void operator()(It &&it) const {
-        it = internal::format_decimal<char_type>(it, abs_value, num_digits);
-      }
-    };
-
-    void on_dec() {
-      int num_digits = internal::count_digits(abs_value);
-      writer.write_int(num_digits, get_prefix(), spec,
-                       dec_writer{abs_value, num_digits});
-    }
-
-    struct hex_writer {
-      int_writer &self;
-      int num_digits;
-
-      template <typename It>
-      void operator()(It &&it) const {
-        it = internal::format_uint<4, char_type>(
-              it, self.abs_value, num_digits, self.spec.type != 'x');
-      }
-    };
-
-    void on_hex() {
-      if (spec.has(HASH_FLAG)) {
-        prefix[prefix_size++] = '0';
-        prefix[prefix_size++] = static_cast<char>(spec.type);
-      }
-      int num_digits = count_digits<4>();
-      writer.write_int(num_digits, get_prefix(), spec,
-                       hex_writer{*this, num_digits});
-    }
-
-    template <int BITS>
-    struct bin_writer {
-      unsigned_type abs_value;
-      int num_digits;
-
-      template <typename It>
-      void operator()(It &&it) const {
-        it = internal::format_uint<BITS, char_type>(it, abs_value, num_digits);
-      }
-    };
-
-    void on_bin() {
-      if (spec.has(HASH_FLAG)) {
-        prefix[prefix_size++] = '0';
-        prefix[prefix_size++] = static_cast<char>(spec.type);
-      }
-      int num_digits = count_digits<1>();
-      writer.write_int(num_digits, get_prefix(), spec,
-                       bin_writer<1>{abs_value, num_digits});
-    }
-
-    void on_oct() {
-      int num_digits = count_digits<3>();
-      if (spec.has(HASH_FLAG) &&
-          spec.precision <= num_digits) {
-        // Octal prefix '0' is counted as a digit, so only add it if precision
-        // is not greater than the number of digits.
-        prefix[prefix_size++] = '0';
-      }
-      writer.write_int(num_digits, get_prefix(), spec,
-                       bin_writer<3>{abs_value, num_digits});
-    }
-
-    enum { SEP_SIZE = 1 };
-
-    struct num_writer {
-      unsigned_type abs_value;
-      int size;
-      char_type sep;
-
-      template <typename It>
-      void operator()(It &&it) const {
-        basic_string_view<char_type> s(&sep, SEP_SIZE);
-        it = internal::format_decimal<char_type>(
-              it, abs_value, size, internal::add_thousands_sep<char_type>(s));
-      }
-    };
-
-    void on_num() {
-      int num_digits = internal::count_digits(abs_value);
-      char_type sep = internal::thousands_sep<char_type>(writer.locale_);
-      int size = num_digits + SEP_SIZE * ((num_digits - 1) / 3);
-      writer.write_int(size, get_prefix(), spec,
-                       num_writer{abs_value, size, sep});
-    }
-
-    void on_error() {
-      FMT_THROW(format_error("invalid type specifier"));
-    }
-  };
-
-  // Writes a formatted integer.
-  template <typename T, typename Spec>
-  void write_int(T value, const Spec &spec) {
-    internal::handle_int_type_spec(spec.type,
-                                   int_writer<T, Spec>(*this, value, spec));
-  }
-
-  enum {INF_SIZE = 3}; // This is an enum to workaround a bug in MSVC.
-
-  struct inf_or_nan_writer {
-    char sign;
-    const char *str;
-
-    size_t size() const {
-      return static_cast<std::size_t>(INF_SIZE + (sign ? 1 : 0));
-    }
-    size_t width() const { return size(); }
-
-    template <typename It>
-    void operator()(It &&it) const {
-      if (sign)
-        *it++ = static_cast<char_type>(sign);
-      it = internal::copy_str<char_type>(
-            str, str + static_cast<std::size_t>(INF_SIZE), it);
-    }
-  };
-
-  struct double_writer {
-    size_t n;
-    char sign;
-    internal::buffer &buffer;
-
-    size_t size() const { return buffer.size() + (sign ? 1 : 0); }
-    size_t width() const { return size(); }
-
-    template <typename It>
-    void operator()(It &&it) {
-      if (sign) {
-        *it++ = static_cast<char_type>(sign);
-        --n;
-      }
-      it = internal::copy_str<char_type>(buffer.begin(), buffer.end(), it);
-    }
-  };
-
-  // Formats a floating-point number (double or long double).
-  template <typename T>
-  void write_double(T value, const format_specs &spec);
-
-  template <typename Char>
-  struct str_writer {
-    const Char *s;
-    size_t size_;
-
-    size_t size() const { return size_; }
-    size_t width() const {
-      return internal::count_code_points(basic_string_view<Char>(s, size_));
-    }
-
-    template <typename It>
-    void operator()(It &&it) const {
-      it = internal::copy_str<char_type>(s, s + size_, it);
-    }
-  };
-
-  template <typename Char>
-  friend class internal::arg_formatter_base;
+#  if FMT_USE_NONTYPE_TEMPLATE_PARAMETERS
+template <typename T, typename Char, size_t N,
+          fmt::detail_exported::fixed_string<Char, N> Str>
+struct statically_named_arg : view {
+  static constexpr auto name = Str.data;
 
- public:
-  /** Constructs a ``basic_writer`` object. */
-  explicit basic_writer(
-      Range out, internal::locale_ref loc = internal::locale_ref())
-    : out_(out.begin()), locale_(loc) {}
-
-  iterator out() const { return out_; }
-
-  void write(int value) { write_decimal(value); }
-  void write(long value) { write_decimal(value); }
-  void write(long long value) { write_decimal(value); }
-
-  void write(unsigned value) { write_decimal(value); }
-  void write(unsigned long value) { write_decimal(value); }
-  void write(unsigned long long value) { write_decimal(value); }
+  const T& value;
+  statically_named_arg(const T& v) : value(v) {}
+};
 
-  /**
-    \rst
-    Formats *value* and writes it to the buffer.
-    \endrst
-   */
-  template <typename T, typename FormatSpec, typename... FormatSpecs>
-  typename std::enable_if<std::is_integral<T>::value, void>::type
-      write(T value, FormatSpec spec, FormatSpecs... specs) {
-    format_specs s(spec, specs...);
-    s.align_ = ALIGN_RIGHT;
-    write_int(value, s);
-  }
+template <typename T, typename Char, size_t N,
+          fmt::detail_exported::fixed_string<Char, N> Str>
+struct is_named_arg<statically_named_arg<T, Char, N, Str>> : std::true_type {};
 
-  void write(double value) {
-    write_double(value, format_specs());
-  }
+template <typename T, typename Char, size_t N,
+          fmt::detail_exported::fixed_string<Char, N> Str>
+struct is_statically_named_arg<statically_named_arg<T, Char, N, Str>>
+    : std::true_type {};
 
-  /**
-    \rst
-    Formats *value* using the general format for floating-point numbers
-    (``'g'``) and writes it to the buffer.
-    \endrst
-   */
-  void write(long double value) {
-    write_double(value, format_specs());
-  }
-
-  /** Writes a character to the buffer. */
-  void write(char value) {
-    *reserve(1) = value;
-  }
-  void write(wchar_t value) {
-    static_assert(std::is_same<char_type, wchar_t>::value, "");
-    *reserve(1) = value;
-  }
-
-  /**
-    \rst
-    Writes *value* to the buffer.
-    \endrst
-   */
-  void write(string_view value) {
-    auto &&it = reserve(value.size());
-    it = internal::copy_str<char_type>(value.begin(), value.end(), it);
-  }
-  void write(wstring_view value) {
-    static_assert(std::is_same<char_type, wchar_t>::value, "");
-    auto &&it = reserve(value.size());
-    it = std::copy(value.begin(), value.end(), it);
-  }
-
-  // Writes a formatted string.
-  template <typename Char>
-  void write(const Char *s, std::size_t size, const align_spec &spec) {
-    write_padded(spec, str_writer<Char>{s, size});
-  }
-
-  template <typename Char>
-  void write(basic_string_view<Char> s,
-             const format_specs &spec = format_specs()) {
-    const Char *data = s.data();
-    std::size_t size = s.size();
-    if (spec.precision >= 0 && internal::to_unsigned(spec.precision) < size)
-      size = internal::to_unsigned(spec.precision);
-    write(data, size, spec);
+template <typename Char, size_t N,
+          fmt::detail_exported::fixed_string<Char, N> Str>
+struct udl_arg {
+  template <typename T> auto operator=(T&& value) const {
+    return statically_named_arg<T, Char, N, Str>(std::forward<T>(value));
   }
+};
+#  else
+template <typename Char> struct udl_arg {
+  const Char* str;
 
-  template <typename T>
-  typename std::enable_if<std::is_same<T, void>::value>::type
-      write(const T *p) {
-    format_specs specs;
-    specs.flags = HASH_FLAG;
-    specs.type = 'x';
-    write_int(reinterpret_cast<uintptr_t>(p), specs);
+  template <typename T> auto operator=(T&& value) const -> named_arg<Char, T> {
+    return {str, std::forward<T>(value)};
   }
 };
+#  endif
+#endif  // FMT_USE_USER_DEFINED_LITERALS
 
-struct float_spec_handler {
-  char type;
-  bool upper;
-
-  explicit float_spec_handler(char t) : type(t), upper(false) {}
-
-  void on_general() {
-    if (type == 'G')
-      upper = true;
-    else
-      type = 'g';
-  }
+template <typename Locale, typename Char>
+auto vformat(const Locale& loc, basic_string_view<Char> format_str,
+             basic_format_args<buffer_context<type_identity_t<Char>>> args)
+    -> std::basic_string<Char> {
+  basic_memory_buffer<Char> buffer;
+  detail::vformat_to(buffer, format_str, args, detail::locale_ref(loc));
+  return {buffer.data(), buffer.size()};
+}
 
-  void on_exp() {
-    if (type == 'E')
-      upper = true;
-  }
+using format_func = void (*)(detail::buffer<char>&, int, const char*);
 
-  void on_fixed() {
-    if (type == 'F') {
-      upper = true;
-#if FMT_MSC_VER
-      // MSVC's printf doesn't support 'F'.
-      type = 'f';
-#endif
-    }
-  }
+FMT_API void format_error_code(buffer<char>& out, int error_code,
+                               string_view message) FMT_NOEXCEPT;
 
-  void on_hex() {
-    if (type == 'A')
-      upper = true;
-  }
+FMT_API void report_error(format_func func, int error_code,
+                          const char* message) FMT_NOEXCEPT;
+FMT_END_DETAIL_NAMESPACE
 
-  void on_error() {
-    FMT_THROW(format_error("invalid type specifier"));
-  }
-};
+FMT_API auto vsystem_error(int error_code, string_view format_str,
+                           format_args args) -> std::system_error;
 
-template <typename Range>
-template <typename T>
-void basic_writer<Range>::write_double(T value, const format_specs &spec) {
-  // Check type.
-  float_spec_handler handler(static_cast<char>(spec.type));
-  internal::handle_float_type_spec(handler.type, handler);
-
-  char sign = 0;
-  // Use signbit instead of value < 0 because the latter is always
-  // false for NaN.
-  if (std::signbit(value)) {
-    sign = '-';
-    value = -value;
-  } else if (spec.has(SIGN_FLAG)) {
-    sign = spec.has(PLUS_FLAG) ? '+' : ' ';
-  }
+/**
+ \rst
+ Constructs :class:`std::system_error` with a message formatted with
+ ``fmt::format(fmt, args...)``.
+  *error_code* is a system error code as given by ``errno``.
 
-  struct write_inf_or_nan_t {
-    basic_writer &writer;
-    format_specs spec;
-    char sign;
-    void operator()(const char *str) const {
-      writer.write_padded(spec, inf_or_nan_writer{sign, str});
-    }
-  } write_inf_or_nan = {*this, spec, sign};
-
-  // Format NaN and ininity ourselves because sprintf's output is not consistent
-  // across platforms.
-  if (internal::fputil::isnotanumber(value))
-    return write_inf_or_nan(handler.upper ? "NAN" : "nan");
-  if (internal::fputil::isinfinity(value))
-    return write_inf_or_nan(handler.upper ? "INF" : "inf");
+ **Example**::
 
-  memory_buffer buffer;
-  bool use_grisu = FMT_USE_GRISU && sizeof(T) <= sizeof(double) &&
-      spec.type != 'a' && spec.type != 'A' &&
-      internal::grisu2_format(static_cast<double>(value), buffer, spec);
-  if (!use_grisu) {
-    format_specs normalized_spec(spec);
-    normalized_spec.type = handler.type;
-    internal::sprintf_format(value, buffer, normalized_spec);
-  }
-  size_t n = buffer.size();
-  align_spec as = spec;
-  if (spec.align() == ALIGN_NUMERIC) {
-    if (sign) {
-      auto &&it = reserve(1);
-      *it++ = static_cast<char_type>(sign);
-      sign = 0;
-      if (as.width_)
-        --as.width_;
-    }
-    as.align_ = ALIGN_RIGHT;
-  } else {
-    if (spec.align() == ALIGN_DEFAULT)
-      as.align_ = ALIGN_RIGHT;
-    if (sign)
-      ++n;
-  }
-  write_padded(as, double_writer{n, sign, buffer});
+   // This throws std::system_error with the description
+   //   cannot open file 'madeup': No such file or directory
+   // or similar (system message may vary).
+   const char* filename = "madeup";
+   std::FILE* file = std::fopen(filename, "r");
+   if (!file)
+     throw fmt::system_error(errno, "cannot open file '{}'", filename);
+ \endrst
+*/
+template <typename... T>
+auto system_error(int error_code, format_string<T...> fmt, T&&... args)
+    -> std::system_error {
+  return vsystem_error(error_code, fmt, fmt::make_format_args(args...));
 }
 
-// Reports a system error without throwing an exception.
-// Can be used to report errors from destructors.
-FMT_API void report_system_error(int error_code,
-                                 string_view message) FMT_NOEXCEPT;
-
-#if FMT_USE_WINDOWS_H
-
-/** A Windows error. */
-class windows_error : public system_error {
- private:
-  FMT_API void init(int error_code, string_view format_str, format_args args);
-
- public:
-  /**
-   \rst
-   Constructs a :class:`fmt::windows_error` object with the description
-   of the form
+/**
+  \rst
+  Formats an error message for an error returned by an operating system or a
+  language runtime, for example a file opening error, and writes it to *out*.
+  The format is the same as the one used by ``std::system_error(ec, message)``
+  where ``ec`` is ``std::error_code(error_code, std::generic_category()})``.
+  It is implementation-defined but normally looks like:
 
-   .. parsed-literal::
+  .. parsed-literal::
      *<message>*: *<system-message>*
 
-   where *<message>* is the formatted message and *<system-message>* is the
-   system message corresponding to the error code.
-   *error_code* is a Windows error code as given by ``GetLastError``.
-   If *error_code* is not a valid error code such as -1, the system message
-   will look like "error -1".
-
-   **Example**::
-
-     // This throws a windows_error with the description
-     //   cannot open file 'madeup': The system cannot find the file specified.
-     // or similar (system message may vary).
-     const char *filename = "madeup";
-     LPOFSTRUCT of = LPOFSTRUCT();
-     HFILE file = OpenFile(filename, &of, OF_READ);
-     if (file == HFILE_ERROR) {
-       throw fmt::windows_error(GetLastError(),
-                                "cannot open file '{}'", filename);
-     }
-   \endrst
-  */
-  template <typename... Args>
-  windows_error(int error_code, string_view message, const Args &... args) {
-    init(error_code, message, make_format_args(args...));
-  }
-};
+  where *<message>* is the passed message and *<system-message>* is the system
+  message corresponding to the error code.
+  *error_code* is a system error code as given by ``errno``.
+  \endrst
+ */
+FMT_API void format_system_error(detail::buffer<char>& out, int error_code,
+                                 const char* message) FMT_NOEXCEPT;
 
-// Reports a Windows error without throwing an exception.
+// Reports a system error without throwing an exception.
 // Can be used to report errors from destructors.
-FMT_API void report_windows_error(int error_code,
-                                  string_view message) FMT_NOEXCEPT;
-
-#endif
+FMT_API void report_system_error(int error_code,
+                                 const char* message) FMT_NOEXCEPT;
 
 /** Fast integer formatter. */
 class format_int {
  private:
   // Buffer should be large enough to hold all digits (digits10 + 1),
   // a sign and a null character.
-  enum {BUFFER_SIZE = std::numeric_limits<unsigned long long>::digits10 + 3};
-  mutable char buffer_[BUFFER_SIZE];
-  char *str_;
-
-  // Formats value in reverse and returns a pointer to the beginning.
-  char *format_decimal(unsigned long long value) {
-    char *ptr = buffer_ + (BUFFER_SIZE - 1);  // Parens to workaround MSVC bug.
-    while (value >= 100) {
-      // Integer division is slow so do it for a group of two digits instead
-      // of for every digit. The idea comes from the talk by Alexandrescu
-      // "Three Optimization Tips for C++". See speed-test for a comparison.
-      unsigned index = static_cast<unsigned>((value % 100) * 2);
-      value /= 100;
-      *--ptr = internal::data::DIGITS[index + 1];
-      *--ptr = internal::data::DIGITS[index];
-    }
-    if (value < 10) {
-      *--ptr = static_cast<char>('0' + value);
-      return ptr;
-    }
-    unsigned index = static_cast<unsigned>(value * 2);
-    *--ptr = internal::data::DIGITS[index + 1];
-    *--ptr = internal::data::DIGITS[index];
-    return ptr;
+  enum { buffer_size = std::numeric_limits<unsigned long long>::digits10 + 3 };
+  mutable char buffer_[buffer_size];
+  char* str_;
+
+  template <typename UInt> auto format_unsigned(UInt value) -> char* {
+    auto n = static_cast<detail::uint32_or_64_or_128_t<UInt>>(value);
+    return detail::format_decimal(buffer_, n, buffer_size - 1).begin;
   }
 
-  void format_signed(long long value) {
-    unsigned long long abs_value = static_cast<unsigned long long>(value);
+  template <typename Int> auto format_signed(Int value) -> char* {
+    auto abs_value = static_cast<detail::uint32_or_64_or_128_t<Int>>(value);
     bool negative = value < 0;
-    if (negative)
-      abs_value = 0 - abs_value;
-    str_ = format_decimal(abs_value);
-    if (negative)
-      *--str_ = '-';
+    if (negative) abs_value = 0 - abs_value;
+    auto begin = format_unsigned(abs_value);
+    if (negative) *--begin = '-';
+    return begin;
   }
 
  public:
-  explicit format_int(int value) { format_signed(value); }
-  explicit format_int(long value) { format_signed(value); }
-  explicit format_int(long long value) { format_signed(value); }
-  explicit format_int(unsigned value) : str_(format_decimal(value)) {}
-  explicit format_int(unsigned long value) : str_(format_decimal(value)) {}
-  explicit format_int(unsigned long long value) : str_(format_decimal(value)) {}
+  explicit format_int(int value) : str_(format_signed(value)) {}
+  explicit format_int(long value) : str_(format_signed(value)) {}
+  explicit format_int(long long value) : str_(format_signed(value)) {}
+  explicit format_int(unsigned value) : str_(format_unsigned(value)) {}
+  explicit format_int(unsigned long value) : str_(format_unsigned(value)) {}
+  explicit format_int(unsigned long long value)
+      : str_(format_unsigned(value)) {}
 
   /** Returns the number of characters written to the output buffer. */
-  std::size_t size() const {
-    return internal::to_unsigned(buffer_ - str_ + BUFFER_SIZE - 1);
+  auto size() const -> size_t {
+    return detail::to_unsigned(buffer_ - str_ + buffer_size - 1);
   }
 
   /**
     Returns a pointer to the output buffer content. No terminating null
     character is appended.
    */
-  const char *data() const { return str_; }
+  auto data() const -> const char* { return str_; }
 
   /**
     Returns a pointer to the output buffer content with terminating null
     character appended.
    */
-  const char *c_str() const {
-    buffer_[BUFFER_SIZE - 1] = '\0';
+  auto c_str() const -> const char* {
+    buffer_[buffer_size - 1] = '\0';
     return str_;
   }
 
   /**
     \rst
     Returns the content of the output buffer as an ``std::string``.
     \endrst
    */
-  std::string str() const { return std::string(str_, size()); }
+  auto str() const -> std::string { return std::string(str_, size()); }
 };
 
-// DEPRECATED!
-// Formats a decimal integer value writing into buffer and returns
-// a pointer to the end of the formatted string. This function doesn't
-// write a terminating null character.
-template <typename T>
-inline void format_decimal(char *&buffer, T value) {
-  typedef typename internal::int_traits<T>::main_type main_type;
-  main_type abs_value = static_cast<main_type>(value);
-  if (internal::is_negative(value)) {
-    *buffer++ = '-';
-    abs_value = 0 - abs_value;
-  }
-  if (abs_value < 100) {
-    if (abs_value < 10) {
-      *buffer++ = static_cast<char>('0' + abs_value);
-      return;
-    }
-    unsigned index = static_cast<unsigned>(abs_value * 2);
-    *buffer++ = internal::data::DIGITS[index];
-    *buffer++ = internal::data::DIGITS[index + 1];
-    return;
-  }
-  int num_digits = internal::count_digits(abs_value);
-  internal::format_decimal<char>(
-        internal::make_checked(buffer, internal::to_unsigned(num_digits)), abs_value, num_digits);
-  buffer += num_digits;
-}
-
-// Formatter of objects of type T.
 template <typename T, typename Char>
-struct formatter<
-    T, Char,
-    typename std::enable_if<internal::format_type<
-        typename buffer_context<Char>::type, T>::value>::type> {
+template <typename FormatContext>
+FMT_CONSTEXPR FMT_INLINE auto
+formatter<T, Char,
+          enable_if_t<detail::type_constant<T, Char>::value !=
+                      detail::type::custom_type>>::format(const T& val,
+                                                          FormatContext& ctx)
+    const -> decltype(ctx.out()) {
+  if (specs_.width_ref.kind != detail::arg_id_kind::none ||
+      specs_.precision_ref.kind != detail::arg_id_kind::none) {
+    auto specs = specs_;
+    detail::handle_dynamic_spec<detail::width_checker>(specs.width,
+                                                       specs.width_ref, ctx);
+    detail::handle_dynamic_spec<detail::precision_checker>(
+        specs.precision, specs.precision_ref, ctx);
+    return detail::write<Char>(ctx.out(), val, specs, ctx.locale());
+  }
+  return detail::write<Char>(ctx.out(), val, specs_, ctx.locale());
+}
+
+#define FMT_FORMAT_AS(Type, Base)                                        \
+  template <typename Char>                                               \
+  struct formatter<Type, Char> : formatter<Base, Char> {                 \
+    template <typename FormatContext>                                    \
+    auto format(Type const& val, FormatContext& ctx) const               \
+        -> decltype(ctx.out()) {                                         \
+      return formatter<Base, Char>::format(static_cast<Base>(val), ctx); \
+    }                                                                    \
+  }
+
+FMT_FORMAT_AS(signed char, int);
+FMT_FORMAT_AS(unsigned char, unsigned);
+FMT_FORMAT_AS(short, int);
+FMT_FORMAT_AS(unsigned short, unsigned);
+FMT_FORMAT_AS(long, long long);
+FMT_FORMAT_AS(unsigned long, unsigned long long);
+FMT_FORMAT_AS(Char*, const Char*);
+FMT_FORMAT_AS(std::basic_string<Char>, basic_string_view<Char>);
+FMT_FORMAT_AS(std::nullptr_t, const void*);
+FMT_FORMAT_AS(detail::byte, unsigned char);
+FMT_FORMAT_AS(detail::std_string_view<Char>, basic_string_view<Char>);
 
-  // Parses format specifiers stopping either at the end of the range or at the
-  // terminating '}'.
-  template <typename ParseContext>
-  FMT_CONSTEXPR typename ParseContext::iterator parse(ParseContext &ctx) {
-    typedef internal::dynamic_specs_handler<ParseContext> handler_type;
-    auto type = internal::get_type<
-      typename buffer_context<Char>::type, T>::value;
-    internal::specs_checker<handler_type>
-        handler(handler_type(specs_, ctx), type);
-    auto it = parse_format_specs(ctx.begin(), ctx.end(), handler);
-    auto type_spec = specs_.type;
-    auto eh = ctx.error_handler();
-    switch (type) {
-    case internal::none_type:
-    case internal::named_arg_type:
-      FMT_ASSERT(false, "invalid argument type");
-      break;
-    case internal::int_type:
-    case internal::uint_type:
-    case internal::long_long_type:
-    case internal::ulong_long_type:
-    case internal::bool_type:
-      handle_int_type_spec(
-            type_spec, internal::int_type_checker<decltype(eh)>(eh));
-      break;
-    case internal::char_type:
-      handle_char_specs(
-          &specs_,
-          internal::char_specs_checker<decltype(eh)>(type_spec, eh));
-      break;
-    case internal::double_type:
-    case internal::long_double_type:
-      handle_float_type_spec(
-            type_spec, internal::float_type_checker<decltype(eh)>(eh));
-      break;
-    case internal::cstring_type:
-      internal::handle_cstring_type_spec(
-            type_spec, internal::cstring_type_checker<decltype(eh)>(eh));
-      break;
-    case internal::string_type:
-      internal::check_string_type_spec(type_spec, eh);
-      break;
-    case internal::pointer_type:
-      internal::check_pointer_type_spec(type_spec, eh);
-      break;
-    case internal::custom_type:
-      // Custom format specifiers should be checked in parse functions of
-      // formatter specializations.
-      break;
-    }
-    return it;
+template <typename Char>
+struct formatter<void*, Char> : formatter<const void*, Char> {
+  template <typename FormatContext>
+  auto format(void* val, FormatContext& ctx) const -> decltype(ctx.out()) {
+    return formatter<const void*, Char>::format(val, ctx);
   }
+};
 
+template <typename Char, size_t N>
+struct formatter<Char[N], Char> : formatter<basic_string_view<Char>, Char> {
   template <typename FormatContext>
-  auto format(const T &val, FormatContext &ctx) -> decltype(ctx.out()) {
-    internal::handle_dynamic_spec<internal::width_checker>(
-      specs_.width_, specs_.width_ref, ctx);
-    internal::handle_dynamic_spec<internal::precision_checker>(
-      specs_.precision, specs_.precision_ref, ctx);
-    typedef output_range<typename FormatContext::iterator,
-                         typename FormatContext::char_type> range_type;
-    return visit_format_arg(arg_formatter<range_type>(ctx, &specs_),
-                      internal::make_arg<FormatContext>(val));
+  FMT_CONSTEXPR auto format(const Char* val, FormatContext& ctx) const
+      -> decltype(ctx.out()) {
+    return formatter<basic_string_view<Char>, Char>::format(val, ctx);
   }
-
- private:
-  internal::dynamic_format_specs<Char> specs_;
 };
 
 // A formatter for types known only at run time such as variant alternatives.
 //
 // Usage:
-//   typedef std::variant<int, std::string> variant;
+//   using variant = std::variant<int, std::string>;
 //   template <>
 //   struct formatter<variant>: dynamic_formatter<> {
-//     void format(buffer &buf, const variant &v, context &ctx) {
-//       visit([&](const auto &val) { format(buf, val, ctx); }, v);
+//     auto format(const variant& v, format_context& ctx) {
+//       return visit([&](const auto& val) {
+//           return dynamic_formatter<>::format(val, ctx);
+//       }, v);
 //     }
 //   };
-template <typename Char = char>
-class dynamic_formatter {
+template <typename Char = char> class dynamic_formatter {
  private:
-  struct null_handler: internal::error_handler {
-    void on_align(alignment) {}
-    void on_plus() {}
-    void on_minus() {}
-    void on_space() {}
+  detail::dynamic_format_specs<Char> specs_;
+  const Char* format_str_;
+
+  struct null_handler : detail::error_handler {
+    void on_align(align_t) {}
+    void on_sign(sign_t) {}
     void on_hash() {}
   };
 
+  template <typename Context> void handle_specs(Context& ctx) {
+    detail::handle_dynamic_spec<detail::width_checker>(specs_.width,
+                                                       specs_.width_ref, ctx);
+    detail::handle_dynamic_spec<detail::precision_checker>(
+        specs_.precision, specs_.precision_ref, ctx);
+  }
+
  public:
   template <typename ParseContext>
-  auto parse(ParseContext &ctx) -> decltype(ctx.begin()) {
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
+    format_str_ = ctx.begin();
     // Checks are deferred to formatting time when the argument type is known.
-    internal::dynamic_specs_handler<ParseContext> handler(specs_, ctx);
-    return parse_format_specs(ctx.begin(), ctx.end(), handler);
+    detail::dynamic_specs_handler<ParseContext> handler(specs_, ctx);
+    return detail::parse_format_specs(ctx.begin(), ctx.end(), handler);
   }
 
   template <typename T, typename FormatContext>
-  auto format(const T &val, FormatContext &ctx) -> decltype(ctx.out()) {
+  auto format(const T& val, FormatContext& ctx) -> decltype(ctx.out()) {
     handle_specs(ctx);
-    internal::specs_checker<null_handler>
-        checker(null_handler(), internal::get_type<FormatContext, T>::value);
-    checker.on_align(specs_.align());
-    if (specs_.flags == 0);  // Do nothing.
-    else if (specs_.has(SIGN_FLAG))
-      specs_.has(PLUS_FLAG) ? checker.on_plus() : checker.on_space();
-    else if (specs_.has(MINUS_FLAG))
-      checker.on_minus();
-    else if (specs_.has(HASH_FLAG))
-      checker.on_hash();
-    if (specs_.precision != -1)
-      checker.end_precision();
-    typedef output_range<typename FormatContext::iterator,
-                         typename FormatContext::char_type> range;
-    visit_format_arg(arg_formatter<range>(ctx, &specs_),
-               internal::make_arg<FormatContext>(val));
-    return ctx.out();
+    detail::specs_checker<null_handler> checker(
+        null_handler(), detail::mapped_type_constant<T, FormatContext>::value);
+    checker.on_align(specs_.align);
+    if (specs_.sign != sign::none) checker.on_sign(specs_.sign);
+    if (specs_.alt) checker.on_hash();
+    if (specs_.precision >= 0) checker.end_precision();
+    return detail::write<Char>(ctx.out(), val, specs_, ctx.locale());
   }
+};
 
- private:
-  template <typename Context>
-  void handle_specs(Context &ctx) {
-    internal::handle_dynamic_spec<internal::width_checker>(
-      specs_.width_, specs_.width_ref, ctx);
-    internal::handle_dynamic_spec<internal::precision_checker>(
-      specs_.precision, specs_.precision_ref, ctx);
-  }
-
-  internal::dynamic_format_specs<Char> specs_;
-};
-
-template <typename Range, typename Char>
-typename basic_format_context<Range, Char>::format_arg
-  basic_format_context<Range, Char>::get_arg(
-    basic_string_view<char_type> name) {
-  map_.init(this->args());
-  format_arg arg = map_.find(name);
-  if (arg.type() == internal::none_type)
-    this->on_error("argument not found");
-  return arg;
+/**
+  \rst
+  Converts ``p`` to ``const void*`` for pointer formatting.
+
+  **Example**::
+
+    auto s = fmt::format("{}", fmt::ptr(p));
+  \endrst
+ */
+template <typename T> auto ptr(T p) -> const void* {
+  static_assert(std::is_pointer<T>::value, "");
+  return detail::bit_cast<const void*>(p);
+}
+template <typename T> auto ptr(const std::unique_ptr<T>& p) -> const void* {
+  return p.get();
+}
+template <typename T> auto ptr(const std::shared_ptr<T>& p) -> const void* {
+  return p.get();
 }
 
-template <typename ArgFormatter, typename Char, typename Context>
-struct format_handler : internal::error_handler {
-  typedef typename ArgFormatter::range range;
-
-  format_handler(range r, basic_string_view<Char> str,
-                 basic_format_args<Context> format_args,
-                 internal::locale_ref loc)
-    : context(r.begin(), str, format_args, loc) {}
-
-  void on_text(const Char *begin, const Char *end) {
-    auto size = internal::to_unsigned(end - begin);
-    auto out = context.out();
-    auto &&it = internal::reserve(out, size);
-    it = std::copy_n(begin, size, it);
-    context.advance_to(out);
-  }
-
-  void on_arg_id() { arg = context.next_arg(); }
-  void on_arg_id(unsigned id) {
-    context.parse_context().check_arg_id(id);
-    arg = context.get_arg(id);
-  }
-  void on_arg_id(basic_string_view<Char> id) {
-    arg = context.get_arg(id);
-  }
-
-  void on_replacement_field(const Char *p) {
-    context.parse_context().advance_to(p);
-    internal::custom_formatter<Char, Context> f(context);
-    if (!visit_format_arg(f, arg))
-      context.advance_to(visit_format_arg(ArgFormatter(context), arg));
-  }
-
-  const Char *on_format_specs(const Char *begin, const Char *end) {
-    auto &parse_ctx = context.parse_context();
-    parse_ctx.advance_to(begin);
-    internal::custom_formatter<Char, Context> f(context);
-    if (visit_format_arg(f, arg))
-      return parse_ctx.begin();
-    basic_format_specs<Char> specs;
-    using internal::specs_handler;
-    internal::specs_checker<specs_handler<Context>>
-        handler(specs_handler<Context>(specs, context), arg.type());
-    begin = parse_format_specs(begin, end, handler);
-    if (begin == end || *begin != '}')
-      on_error("missing '}' in format string");
-    parse_ctx.advance_to(begin);
-    context.advance_to(visit_format_arg(ArgFormatter(context, &specs), arg));
-    return begin;
-  }
+class bytes {
+ private:
+  string_view data_;
+  friend struct formatter<bytes>;
 
-  Context context;
-  basic_format_arg<Context> arg;
+ public:
+  explicit bytes(string_view data) : data_(data) {}
 };
 
-/** Formats arguments and writes the output to the range. */
-template <typename ArgFormatter, typename Char, typename Context>
-typename Context::iterator vformat_to(
-    typename ArgFormatter::range out,
-    basic_string_view<Char> format_str,
-    basic_format_args<Context> args,
-    internal::locale_ref loc = internal::locale_ref()) {
-  format_handler<ArgFormatter, Char, Context> h(out, format_str, args, loc);
-  internal::parse_format_string<false>(format_str, h);
-  return h.context.out();
-}
-
-// Casts ``p`` to ``const void*`` for pointer formatting.
-// Example:
-//   auto s = format("{}", ptr(p));
-template <typename T>
-inline const void *ptr(const T *p) { return p; }
-
-template <typename It, typename Char>
-struct arg_join {
-  It begin;
-  It end;
-  basic_string_view<Char> sep;
+template <> struct formatter<bytes> {
+ private:
+  detail::dynamic_format_specs<char> specs_;
 
-  arg_join(It begin, It end, basic_string_view<Char> sep)
-    : begin(begin), end(end), sep(sep) {}
-};
+ public:
+  template <typename ParseContext>
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
+    using handler_type = detail::dynamic_specs_handler<ParseContext>;
+    detail::specs_checker<handler_type> handler(handler_type(specs_, ctx),
+                                                detail::type::string_type);
+    auto it = parse_format_specs(ctx.begin(), ctx.end(), handler);
+    detail::check_string_type_spec(specs_.type, ctx.error_handler());
+    return it;
+  }
 
-template <typename It, typename Char>
-struct formatter<arg_join<It, Char>, Char>:
-    formatter<typename std::iterator_traits<It>::value_type, Char> {
   template <typename FormatContext>
-  auto format(const arg_join<It, Char> &value, FormatContext &ctx)
-      -> decltype(ctx.out()) {
-    typedef formatter<typename std::iterator_traits<It>::value_type, Char> base;
-    auto it = value.begin;
-    auto out = ctx.out();
-    if (it != value.end) {
-      out = base::format(*it++, ctx);
-      while (it != value.end) {
-        out = std::copy(value.sep.begin(), value.sep.end(), out);
-        ctx.advance_to(out);
-        out = base::format(*it++, ctx);
-      }
-    }
-    return out;
+  auto format(bytes b, FormatContext& ctx) -> decltype(ctx.out()) {
+    detail::handle_dynamic_spec<detail::width_checker>(specs_.width,
+                                                       specs_.width_ref, ctx);
+    detail::handle_dynamic_spec<detail::precision_checker>(
+        specs_.precision, specs_.precision_ref, ctx);
+    return detail::write_bytes(ctx.out(), b.data_, specs_);
   }
 };
 
-template <typename It>
-arg_join<It, char> join(It begin, It end, string_view sep) {
-  return arg_join<It, char>(begin, end, sep);
-}
-
-template <typename It>
-arg_join<It, wchar_t> join(It begin, It end, wstring_view sep) {
-  return arg_join<It, wchar_t>(begin, end, sep);
-}
-
-// The following causes ICE in gcc 4.4.
-#if FMT_USE_TRAILING_RETURN && (!FMT_GCC_VERSION || FMT_GCC_VERSION >= 405)
-template <typename Range>
-auto join(const Range &range, string_view sep)
-    -> arg_join<decltype(internal::begin(range)), char> {
-  return join(internal::begin(range), internal::end(range), sep);
-}
-
-template <typename Range>
-auto join(const Range &range, wstring_view sep)
-    -> arg_join<decltype(internal::begin(range)), wchar_t> {
-  return join(internal::begin(range), internal::end(range), sep);
-}
-#endif
+// group_digits_view is not derived from view because it copies the argument.
+template <typename T> struct group_digits_view { T value; };
 
 /**
   \rst
-  Converts *value* to ``std::string`` using the default format for type *T*.
-  It doesn't support user-defined types with custom formatters.
+  Returns a view that formats an integer value using ',' as a locale-independent
+  thousands separator.
 
   **Example**::
 
-    #include <fmt/format.h>
-
-    std::string answer = fmt::to_string(42);
+    fmt::print("{}", fmt::group_digits(12345));
+    // Output: "12,345"
   \endrst
  */
-template <typename T>
-std::string to_string(const T &value) {
-  std::string str;
-  internal::container_buffer<std::string> buf(str);
-  writer(buf).write(value);
-  return str;
+template <typename T> auto group_digits(T value) -> group_digits_view<T> {
+  return {value};
 }
 
-/**
-  Converts *value* to ``std::wstring`` using the default format for type *T*.
- */
-template <typename T>
-std::wstring to_wstring(const T &value) {
-  std::wstring str;
-  internal::container_buffer<std::wstring> buf(str);
-  wwriter(buf).write(value);
-  return str;
-}
+template <typename T> struct formatter<group_digits_view<T>> : formatter<T> {
+ private:
+  detail::dynamic_format_specs<char> specs_;
 
-template <typename Char, std::size_t SIZE>
-std::basic_string<Char> to_string(const basic_memory_buffer<Char, SIZE> &buf) {
-  return std::basic_string<Char>(buf.data(), buf.size());
-}
+ public:
+  template <typename ParseContext>
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
+    using handler_type = detail::dynamic_specs_handler<ParseContext>;
+    detail::specs_checker<handler_type> handler(handler_type(specs_, ctx),
+                                                detail::type::int_type);
+    auto it = parse_format_specs(ctx.begin(), ctx.end(), handler);
+    detail::check_string_type_spec(specs_.type, ctx.error_handler());
+    return it;
+  }
 
-template <typename Char>
-typename buffer_context<Char>::type::iterator internal::vformat_to(
-    internal::basic_buffer<Char> &buf, basic_string_view<Char> format_str,
-    basic_format_args<typename buffer_context<Char>::type> args) {
-  typedef back_insert_range<internal::basic_buffer<Char> > range;
-  return vformat_to<arg_formatter<range>>(
-    buf, to_string_view(format_str), args);
-}
+  template <typename FormatContext>
+  auto format(group_digits_view<T> t, FormatContext& ctx)
+      -> decltype(ctx.out()) {
+    detail::handle_dynamic_spec<detail::width_checker>(specs_.width,
+                                                       specs_.width_ref, ctx);
+    detail::handle_dynamic_spec<detail::precision_checker>(
+        specs_.precision, specs_.precision_ref, ctx);
+    return detail::write_int_localized(
+        ctx.out(), static_cast<detail::uint64_or_128_t<T>>(t.value), 0, specs_,
+        detail::digit_grouping<char>({"\3", ','}));
+  }
+};
 
-template <typename S, typename Char = FMT_CHAR(S)>
-inline typename buffer_context<Char>::type::iterator vformat_to(
-    internal::basic_buffer<Char> &buf, const S &format_str,
-    basic_format_args<typename buffer_context<Char>::type> args) {
-  return internal::vformat_to(buf, to_string_view(format_str), args);
-}
+template <typename It, typename Sentinel, typename Char = char>
+struct join_view : detail::view {
+  It begin;
+  Sentinel end;
+  basic_string_view<Char> sep;
 
-template <
-    typename S, typename... Args,
-    std::size_t SIZE = inline_buffer_size,
-    typename Char = typename internal::char_t<S>::type>
-inline typename buffer_context<Char>::type::iterator format_to(
-    basic_memory_buffer<Char, SIZE> &buf, const S &format_str,
-    const Args &... args) {
-  internal::check_format_string<Args...>(format_str);
-  typedef typename buffer_context<Char>::type context;
-  format_arg_store<context, Args...> as{args...};
-  return internal::vformat_to(buf, to_string_view(format_str),
-                              basic_format_args<context>(as));
-}
-
-namespace internal {
-
-// Detect the iterator category of *any* given type in a SFINAE-friendly way.
-// Unfortunately, older implementations of std::iterator_traits are not safe
-// for use in a SFINAE-context.
-
-// the gist of C++17's void_t magic
-template<typename... Ts>
-struct void_ { typedef void type; };
+  join_view(It b, Sentinel e, basic_string_view<Char> s)
+      : begin(b), end(e), sep(s) {}
+};
 
-template <typename T, typename Enable = void>
-struct it_category : std::false_type {};
+template <typename It, typename Sentinel, typename Char>
+using arg_join FMT_DEPRECATED_ALIAS = join_view<It, Sentinel, Char>;
 
-template <typename T>
-struct it_category<T*> { typedef std::random_access_iterator_tag type; };
+template <typename It, typename Sentinel, typename Char>
+struct formatter<join_view<It, Sentinel, Char>, Char> {
+ private:
+  using value_type =
+#ifdef __cpp_lib_ranges
+      std::iter_value_t<It>;
+#else
+      typename std::iterator_traits<It>::value_type;
+#endif
+  using context = buffer_context<Char>;
+  using mapper = detail::arg_mapper<context>;
 
-template <typename T>
-struct it_category<T, typename void_<typename T::iterator_category>::type> {
-  typedef typename T::iterator_category type;
-};
+  template <typename T, FMT_ENABLE_IF(has_formatter<T, context>::value)>
+  static auto map(const T& value) -> const T& {
+    return value;
+  }
+  template <typename T, FMT_ENABLE_IF(!has_formatter<T, context>::value)>
+  static auto map(const T& value) -> decltype(mapper().map(value)) {
+    return mapper().map(value);
+  }
+
+  using formatter_type =
+      conditional_t<is_formattable<value_type, Char>::value,
+                    formatter<remove_cvref_t<decltype(map(
+                                  std::declval<const value_type&>()))>,
+                              Char>,
+                    detail::fallback_formatter<value_type, Char>>;
 
-// Detect if *any* given type models the OutputIterator concept.
-template <typename It>
-class is_output_iterator {
-  // Check for mutability because all iterator categories derived from
-  // std::input_iterator_tag *may* also meet the requirements of an
-  // OutputIterator, thereby falling into the category of 'mutable iterators'
-  // [iterator.requirements.general] clause 4.
-  // The compiler reveals this property only at the point of *actually
-  // dereferencing* the iterator!
-  template <typename U>
-  static decltype(*(internal::declval<U>())) test(std::input_iterator_tag);
-  template <typename U>
-  static char& test(std::output_iterator_tag);
-  template <typename U>
-  static const char& test(...);
+  formatter_type value_formatter_;
 
-  typedef decltype(test<It>(typename it_category<It>::type{})) type;
-  typedef typename std::remove_reference<type>::type result;
  public:
-  static const bool value = !std::is_const<result>::value;
+  template <typename ParseContext>
+  FMT_CONSTEXPR auto parse(ParseContext& ctx) -> decltype(ctx.begin()) {
+    return value_formatter_.parse(ctx);
+  }
+
+  template <typename FormatContext>
+  auto format(const join_view<It, Sentinel, Char>& value, FormatContext& ctx)
+      -> decltype(ctx.out()) {
+    auto it = value.begin;
+    auto out = ctx.out();
+    if (it != value.end) {
+      out = value_formatter_.format(map(*it), ctx);
+      ++it;
+      while (it != value.end) {
+        out = detail::copy_str<Char>(value.sep.begin(), value.sep.end(), out);
+        ctx.advance_to(out);
+        out = value_formatter_.format(map(*it), ctx);
+        ++it;
+      }
+    }
+    return out;
+  }
 };
-} // internal
 
-template <typename OutputIt, typename Char = char>
-//using format_context_t = basic_format_context<OutputIt, Char>;
-struct format_context_t { typedef basic_format_context<OutputIt, Char> type; };
-
-template <typename OutputIt, typename Char = char>
-//using format_args_t = basic_format_args<format_context_t<OutputIt, Char>>;
-struct format_args_t {
-  typedef basic_format_args<
-    typename format_context_t<OutputIt, Char>::type> type;
-};
-
-template <typename String, typename OutputIt, typename... Args>
-inline typename std::enable_if<internal::is_output_iterator<OutputIt>::value,
-                               OutputIt>::type
-    vformat_to(OutputIt out, const String &format_str,
-               typename format_args_t<OutputIt, FMT_CHAR(String)>::type args) {
-  typedef output_range<OutputIt, FMT_CHAR(String)> range;
-  return vformat_to<arg_formatter<range>>(range(out),
-                                          to_string_view(format_str), args);
+/**
+  Returns a view that formats the iterator range `[begin, end)` with elements
+  separated by `sep`.
+ */
+template <typename It, typename Sentinel>
+auto join(It begin, Sentinel end, string_view sep) -> join_view<It, Sentinel> {
+  return {begin, end, sep};
 }
 
 /**
- \rst
- Formats arguments, writes the result to the output iterator ``out`` and returns
- the iterator past the end of the output range.
+  \rst
+  Returns a view that formats `range` with elements separated by `sep`.
 
- **Example**::
+  **Example**::
 
-   std::vector<char> out;
-   fmt::format_to(std::back_inserter(out), "{}", 42);
- \endrst
- */
-template <typename OutputIt, typename S, typename... Args>
-inline FMT_ENABLE_IF_T(
-    internal::is_string<S>::value &&
-    internal::is_output_iterator<OutputIt>::value, OutputIt)
-    format_to(OutputIt out, const S &format_str, const Args &... args) {
-  internal::check_format_string<Args...>(format_str);
-  typedef typename format_context_t<OutputIt, FMT_CHAR(S)>::type context;
-  format_arg_store<context, Args...> as{args...};
-  return vformat_to(out, to_string_view(format_str),
-                    basic_format_args<context>(as));
-}
+    std::vector<int> v = {1, 2, 3};
+    fmt::print("{}", fmt::join(v, ", "));
+    // Output: "1, 2, 3"
 
-template <typename OutputIt>
-struct format_to_n_result {
-  /** Iterator past the end of the output range. */
-  OutputIt out;
-  /** Total (not truncated) output size. */
-  std::size_t size;
-};
-
-template <typename OutputIt, typename Char = typename OutputIt::value_type>
-struct format_to_n_context :
-  format_context_t<fmt::internal::truncating_iterator<OutputIt>, Char> {};
-
-template <typename OutputIt, typename Char = typename OutputIt::value_type>
-struct format_to_n_args {
-  typedef basic_format_args<
-    typename format_to_n_context<OutputIt, Char>::type> type;
-};
-
-template <typename OutputIt, typename Char, typename ...Args>
-inline format_arg_store<
-  typename format_to_n_context<OutputIt, Char>::type, Args...>
-    make_format_to_n_args(const Args &... args) {
-  return format_arg_store<
-    typename format_to_n_context<OutputIt, Char>::type, Args...>(args...);
-}
-
-template <typename OutputIt, typename Char, typename... Args>
-inline typename std::enable_if<
-    internal::is_output_iterator<OutputIt>::value,
-    format_to_n_result<OutputIt>>::type vformat_to_n(
-    OutputIt out, std::size_t n, basic_string_view<Char> format_str,
-    typename format_to_n_args<OutputIt, Char>::type args) {
-  typedef internal::truncating_iterator<OutputIt> It;
-  auto it = vformat_to(It(out, n), format_str, args);
-  return {it.base(), it.count()};
-}
+  ``fmt::join`` applies passed format specifiers to the range elements::
 
-/**
- \rst
- Formats arguments, writes up to ``n`` characters of the result to the output
- iterator ``out`` and returns the total output size and the iterator past the
- end of the output range.
- \endrst
+    fmt::print("{:02}", fmt::join(v, ", "));
+    // Output: "01, 02, 03"
+  \endrst
  */
-template <typename OutputIt, typename S, typename... Args>
-inline FMT_ENABLE_IF_T(
-    internal::is_string<S>::value &&
-    internal::is_output_iterator<OutputIt>::value,
-    format_to_n_result<OutputIt>)
-    format_to_n(OutputIt out, std::size_t n, const S &format_str,
-                const Args &... args) {
-  internal::check_format_string<Args...>(format_str);
-  typedef FMT_CHAR(S) Char;
-  format_arg_store<
-      typename format_to_n_context<OutputIt, Char>::type, Args...> as(args...);
-  return vformat_to_n(out, n, to_string_view(format_str),
-                      typename format_to_n_args<OutputIt, Char>::type(as));
-}
-
-template <typename Char>
-inline std::basic_string<Char> internal::vformat(
-    basic_string_view<Char> format_str,
-    basic_format_args<typename buffer_context<Char>::type> args) {
-  basic_memory_buffer<Char> buffer;
-  internal::vformat_to(buffer, format_str, args);
-  return fmt::to_string(buffer);
+template <typename Range>
+auto join(Range&& range, string_view sep)
+    -> join_view<detail::iterator_t<Range>, detail::sentinel_t<Range>> {
+  return join(std::begin(range), std::end(range), sep);
 }
 
 /**
-  Returns the number of characters in the output of
-  ``format(format_str, args...)``.
- */
-template <typename... Args>
-inline std::size_t formatted_size(string_view format_str,
-                                  const Args &... args) {
-  auto it = format_to(internal::counting_iterator<char>(), format_str, args...);
-  return it.count();
-}
+  \rst
+  Converts *value* to ``std::string`` using the default format for type *T*.
 
-#if FMT_USE_USER_DEFINED_LITERALS
-namespace internal {
+  **Example**::
 
-# if FMT_UDL_TEMPLATE
-template <typename Char, Char... CHARS>
-class udl_formatter {
- public:
-  template <typename... Args>
-  std::basic_string<Char> operator()(const Args &... args) const {
-    FMT_CONSTEXPR_DECL Char s[] = {CHARS..., '\0'};
-    FMT_CONSTEXPR_DECL bool invalid_format =
-        do_check_format_string<Char, error_handler, Args...>(
-          basic_string_view<Char>(s, sizeof...(CHARS)));
-    (void)invalid_format;
-    return format(s, args...);
-  }
-};
-# else
-template <typename Char>
-struct udl_formatter {
-  const Char *str;
+    #include <fmt/format.h>
 
-  template <typename... Args>
-  auto operator()(Args &&... args) const
-                  -> decltype(format(str, std::forward<Args>(args)...)) {
-    return format(str, std::forward<Args>(args)...);
-  }
-};
-# endif // FMT_UDL_TEMPLATE
+    std::string answer = fmt::to_string(42);
+  \endrst
+ */
+template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+inline auto to_string(const T& value) -> std::string {
+  auto result = std::string();
+  detail::write<char>(std::back_inserter(result), value);
+  return result;
+}
+
+template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+FMT_NODISCARD inline auto to_string(T value) -> std::string {
+  // The buffer should be large enough to store the number including the sign
+  // or "false" for bool.
+  constexpr int max_size = detail::digits10<T>() + 2;
+  char buffer[max_size > 5 ? static_cast<unsigned>(max_size) : 5];
+  char* begin = buffer;
+  return std::string(begin, detail::write<char>(begin, value));
+}
+
+template <typename Char, size_t SIZE>
+FMT_NODISCARD auto to_string(const basic_memory_buffer<Char, SIZE>& buf)
+    -> std::basic_string<Char> {
+  auto size = buf.size();
+  detail::assume(size < std::basic_string<Char>().max_size());
+  return std::basic_string<Char>(buf.data(), size);
+}
 
-template <typename Char>
-struct udl_arg {
-  const Char *str;
+FMT_BEGIN_DETAIL_NAMESPACE
 
-  template <typename T>
-  named_arg<T, Char> operator=(T &&value) const {
-    return {str, std::forward<T>(value)};
+template <typename Char>
+void vformat_to(
+    buffer<Char>& buf, basic_string_view<Char> fmt,
+    basic_format_args<FMT_BUFFER_CONTEXT(type_identity_t<Char>)> args,
+    locale_ref loc) {
+  // workaround for msvc bug regarding name-lookup in module
+  // link names into function scope
+  using detail::arg_formatter;
+  using detail::buffer_appender;
+  using detail::custom_formatter;
+  using detail::default_arg_formatter;
+  using detail::get_arg;
+  using detail::locale_ref;
+  using detail::parse_format_specs;
+  using detail::specs_checker;
+  using detail::specs_handler;
+  using detail::to_unsigned;
+  using detail::type;
+  using detail::write;
+  auto out = buffer_appender<Char>(buf);
+  if (fmt.size() == 2 && equal2(fmt.data(), "{}")) {
+    auto arg = args.get(0);
+    if (!arg) error_handler().on_error("argument not found");
+    visit_format_arg(default_arg_formatter<Char>{out, args, loc}, arg);
+    return;
   }
-};
-
-} // namespace internal
 
-inline namespace literals {
-
-# if FMT_UDL_TEMPLATE
-template <typename Char, Char... CHARS>
-FMT_CONSTEXPR internal::udl_formatter<Char, CHARS...> operator""_format() {
-  return {};
+  struct format_handler : error_handler {
+    basic_format_parse_context<Char> parse_context;
+    buffer_context<Char> context;
+
+    format_handler(buffer_appender<Char> out, basic_string_view<Char> str,
+                   basic_format_args<buffer_context<Char>> args, locale_ref loc)
+        : parse_context(str), context(out, args, loc) {}
+
+    void on_text(const Char* begin, const Char* end) {
+      auto text = basic_string_view<Char>(begin, to_unsigned(end - begin));
+      context.advance_to(write<Char>(context.out(), text));
+    }
+
+    FMT_CONSTEXPR auto on_arg_id() -> int {
+      return parse_context.next_arg_id();
+    }
+    FMT_CONSTEXPR auto on_arg_id(int id) -> int {
+      return parse_context.check_arg_id(id), id;
+    }
+    FMT_CONSTEXPR auto on_arg_id(basic_string_view<Char> id) -> int {
+      int arg_id = context.arg_id(id);
+      if (arg_id < 0) on_error("argument not found");
+      return arg_id;
+    }
+
+    FMT_INLINE void on_replacement_field(int id, const Char*) {
+      auto arg = get_arg(context, id);
+      context.advance_to(visit_format_arg(
+          default_arg_formatter<Char>{context.out(), context.args(),
+                                      context.locale()},
+          arg));
+    }
+
+    auto on_format_specs(int id, const Char* begin, const Char* end)
+        -> const Char* {
+      auto arg = get_arg(context, id);
+      if (arg.type() == type::custom_type) {
+        parse_context.advance_to(parse_context.begin() +
+                                 (begin - &*parse_context.begin()));
+        visit_format_arg(custom_formatter<Char>{parse_context, context}, arg);
+        return parse_context.begin();
+      }
+      auto specs = basic_format_specs<Char>();
+      specs_checker<specs_handler<Char>> handler(
+          specs_handler<Char>(specs, parse_context, context), arg.type());
+      begin = parse_format_specs(begin, end, handler);
+      if (begin == end || *begin != '}')
+        on_error("missing '}' in format string");
+      auto f = arg_formatter<Char>{context.out(), specs, context.locale()};
+      context.advance_to(visit_format_arg(f, arg));
+      return begin;
+    }
+  };
+  detail::parse_format_string<false>(fmt, format_handler(out, fmt, args, loc));
 }
-# else
-/**
-  \rst
-  User-defined literal equivalent of :func:`fmt::format`.
 
-  **Example**::
+#ifndef FMT_HEADER_ONLY
+extern template FMT_API auto thousands_sep_impl<char>(locale_ref)
+    -> thousands_sep_result<char>;
+extern template FMT_API auto thousands_sep_impl<wchar_t>(locale_ref)
+    -> thousands_sep_result<wchar_t>;
+extern template FMT_API auto decimal_point_impl(locale_ref) -> char;
+extern template FMT_API auto decimal_point_impl(locale_ref) -> wchar_t;
+extern template auto format_float<double>(double value, int precision,
+                                          float_specs specs, buffer<char>& buf)
+    -> int;
+extern template auto format_float<long double>(long double value, int precision,
+                                               float_specs specs,
+                                               buffer<char>& buf) -> int;
+void snprintf_float(float, int, float_specs, buffer<char>&) = delete;
+extern template auto snprintf_float<double>(double value, int precision,
+                                            float_specs specs,
+                                            buffer<char>& buf) -> int;
+extern template auto snprintf_float<long double>(long double value,
+                                                 int precision,
+                                                 float_specs specs,
+                                                 buffer<char>& buf) -> int;
+#endif  // FMT_HEADER_ONLY
 
-    using namespace fmt::literals;
-    std::string message = "The answer is {}"_format(42);
-  \endrst
- */
-inline internal::udl_formatter<char>
-operator"" _format(const char *s, std::size_t) { return {s}; }
-inline internal::udl_formatter<wchar_t>
-operator"" _format(const wchar_t *s, std::size_t) { return {s}; }
-# endif // FMT_UDL_TEMPLATE
+FMT_END_DETAIL_NAMESPACE
 
+#if FMT_USE_USER_DEFINED_LITERALS
+inline namespace literals {
 /**
   \rst
   User-defined literal equivalent of :func:`fmt::arg`.
 
   **Example**::
 
     using namespace fmt::literals;
     fmt::print("Elapsed time: {s:.2f} seconds", "s"_a=1.23);
   \endrst
  */
-inline internal::udl_arg<char>
-operator"" _a(const char *s, std::size_t) { return {s}; }
-inline internal::udl_arg<wchar_t>
-operator"" _a(const wchar_t *s, std::size_t) { return {s}; }
-} // inline namespace literals
-#endif // FMT_USE_USER_DEFINED_LITERALS
-FMT_END_NAMESPACE
-
-#define FMT_STRING(s) [] { \
-    typedef typename std::remove_cv<std::remove_pointer< \
-      typename std::decay<decltype(s)>::type>::type>::type ct; \
-    struct str : fmt::compile_string { \
-      typedef ct char_type; \
-      FMT_CONSTEXPR operator fmt::basic_string_view<ct>() const { \
-        return {s, sizeof(s) / sizeof(ct) - 1}; \
-      } \
-    }; \
-    return str{}; \
-  }()
+#  if FMT_USE_NONTYPE_TEMPLATE_PARAMETERS
+template <detail_exported::fixed_string Str>
+constexpr auto operator""_a()
+    -> detail::udl_arg<remove_cvref_t<decltype(Str.data[0])>,
+                       sizeof(Str.data) / sizeof(decltype(Str.data[0])), Str> {
+  return {};
+}
+#  else
+constexpr auto operator"" _a(const char* s, size_t) -> detail::udl_arg<char> {
+  return {s};
+}
+#  endif
 
-#if defined(FMT_STRING_ALIAS) && FMT_STRING_ALIAS
-/**
-  \rst
-  Constructs a compile-time format string. This macro is disabled by default to
-  prevent potential name collisions. To enable it define ``FMT_STRING_ALIAS`` to
-  1 before including ``fmt/format.h``.
+// DEPRECATED!
+// User-defined literal equivalent of fmt::format.
+FMT_DEPRECATED constexpr auto operator"" _format(const char* s, size_t n)
+    -> detail::udl_formatter<char> {
+  return {{s, n}};
+}
+}  // namespace literals
+#endif  // FMT_USE_USER_DEFINED_LITERALS
+
+template <typename Locale, FMT_ENABLE_IF(detail::is_locale<Locale>::value)>
+inline auto vformat(const Locale& loc, string_view fmt, format_args args)
+    -> std::string {
+  return detail::vformat(loc, fmt, args);
+}
+
+template <typename Locale, typename... T,
+          FMT_ENABLE_IF(detail::is_locale<Locale>::value)>
+inline auto format(const Locale& loc, format_string<T...> fmt, T&&... args)
+    -> std::string {
+  return vformat(loc, string_view(fmt), fmt::make_format_args(args...));
+}
+
+template <typename... T, size_t SIZE, typename Allocator>
+FMT_DEPRECATED auto format_to(basic_memory_buffer<char, SIZE, Allocator>& buf,
+                              format_string<T...> fmt, T&&... args)
+    -> appender {
+  detail::vformat_to(buf, string_view(fmt), fmt::make_format_args(args...));
+  return appender(buf);
+}
+
+template <typename OutputIt, typename Locale,
+          FMT_ENABLE_IF(detail::is_output_iterator<OutputIt, char>::value&&
+                            detail::is_locale<Locale>::value)>
+auto vformat_to(OutputIt out, const Locale& loc, string_view fmt,
+                format_args args) -> OutputIt {
+  using detail::get_buffer;
+  auto&& buf = get_buffer<char>(out);
+  detail::vformat_to(buf, fmt, args, detail::locale_ref(loc));
+  return detail::get_iterator(buf);
+}
+
+template <typename OutputIt, typename Locale, typename... T,
+          FMT_ENABLE_IF(detail::is_output_iterator<OutputIt, char>::value&&
+                            detail::is_locale<Locale>::value)>
+FMT_INLINE auto format_to(OutputIt out, const Locale& loc,
+                          format_string<T...> fmt, T&&... args) -> OutputIt {
+  return vformat_to(out, loc, fmt, fmt::make_format_args(args...));
+}
 
-  **Example**::
+FMT_MODULE_EXPORT_END
+FMT_END_NAMESPACE
 
-    #define FMT_STRING_ALIAS 1
-    #include <fmt/format.h>
-    // A compile-time error because 'd' is an invalid specifier for strings.
-    std::string s = format(fmt("{:d}"), "foo");
-  \endrst
- */
-# define fmt(s) FMT_STRING(s)
+#ifdef FMT_DEPRECATED_INCLUDE_XCHAR
+#  include "xchar.h"
 #endif
 
 #ifdef FMT_HEADER_ONLY
-# define FMT_FUNC inline
-# include "format-inl.h"
+#  define FMT_FUNC inline
+#  include "format-inl.h"
 #else
-# define FMT_FUNC
-#endif
-
-// Restore warnings.
-#if FMT_GCC_VERSION >= 406 || FMT_CLANG_VERSION
-# pragma GCC diagnostic pop
+#  define FMT_FUNC
 #endif
 
 #endif  // FMT_FORMAT_H_
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/ostream.h` & `spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/ostream.h`

 * *Files 19% similar despite different names*

```diff
@@ -4,150 +4,132 @@
 // All rights reserved.
 //
 // For the license information refer to format.h.
 
 #ifndef FMT_OSTREAM_H_
 #define FMT_OSTREAM_H_
 
-#include "format.h"
 #include <ostream>
 
-FMT_BEGIN_NAMESPACE
-namespace internal {
-
-template <class Char>
-class formatbuf : public std::basic_streambuf<Char> {
- private:
-  typedef typename std::basic_streambuf<Char>::int_type int_type;
-  typedef typename std::basic_streambuf<Char>::traits_type traits_type;
-
-  basic_buffer<Char> &buffer_;
+#include "format.h"
 
- public:
-  formatbuf(basic_buffer<Char> &buffer) : buffer_(buffer) {}
+FMT_BEGIN_NAMESPACE
 
- protected:
-  // The put-area is actually always empty. This makes the implementation
-  // simpler and has the advantage that the streambuf and the buffer are always
-  // in sync and sputc never writes into uninitialized memory. The obvious
-  // disadvantage is that each call to sputc always results in a (virtual) call
-  // to overflow. There is no disadvantage here for sputn since this always
-  // results in a call to xsputn.
-
-  int_type overflow(int_type ch = traits_type::eof()) FMT_OVERRIDE {
-    if (!traits_type::eq_int_type(ch, traits_type::eof()))
-      buffer_.push_back(static_cast<Char>(ch));
-    return ch;
-  }
+template <typename OutputIt, typename Char> class basic_printf_context;
 
-  std::streamsize xsputn(const Char *s, std::streamsize count) FMT_OVERRIDE {
-    buffer_.append(s, s + count);
-    return count;
-  }
-};
+namespace detail {
 
-template <typename Char>
-struct test_stream : std::basic_ostream<Char> {
- private:
-  struct null;
-  // Hide all operator<< from std::basic_ostream<Char>.
-  void operator<<(null);
-};
-
-// Checks if T has a user-defined operator<< (e.g. not a member of std::ostream).
-template <typename T, typename Char>
+// Checks if T has a user-defined operator<<.
+template <typename T, typename Char, typename Enable = void>
 class is_streamable {
  private:
   template <typename U>
-  static decltype(
-    internal::declval<test_stream<Char>&>()
-      << internal::declval<U>(), std::true_type()) test(int);
+  static auto test(int)
+      -> bool_constant<sizeof(std::declval<std::basic_ostream<Char>&>()
+                              << std::declval<U>()) != 0>;
 
-  template <typename>
-  static std::false_type test(...);
+  template <typename> static auto test(...) -> std::false_type;
 
-  typedef decltype(test<T>(0)) result;
+  using result = decltype(test<T>(0));
 
  public:
+  is_streamable() = default;
+
   static const bool value = result::value;
 };
 
+// Formatting of built-in types and arrays is intentionally disabled because
+// it's handled by standard (non-ostream) formatters.
+template <typename T, typename Char>
+struct is_streamable<
+    T, Char,
+    enable_if_t<
+        std::is_arithmetic<T>::value || std::is_array<T>::value ||
+        std::is_pointer<T>::value || std::is_same<T, char8_type>::value ||
+        std::is_same<T, std::basic_string<Char>>::value ||
+        std::is_same<T, std_string_view<Char>>::value ||
+        (std::is_convertible<T, int>::value && !std::is_enum<T>::value)>>
+    : std::false_type {};
+
 // Write the content of buf to os.
+// It is a separate function rather than a part of vprint to simplify testing.
 template <typename Char>
-void write(std::basic_ostream<Char> &os, basic_buffer<Char> &buf) {
-  const Char *data = buf.data();
-  typedef std::make_unsigned<std::streamsize>::type UnsignedStreamSize;
-  UnsignedStreamSize size = buf.size();
-  UnsignedStreamSize max_size =
-      internal::to_unsigned((std::numeric_limits<std::streamsize>::max)());
+void write_buffer(std::basic_ostream<Char>& os, buffer<Char>& buf) {
+  const Char* buf_data = buf.data();
+  using unsigned_streamsize = std::make_unsigned<std::streamsize>::type;
+  unsigned_streamsize size = buf.size();
+  unsigned_streamsize max_size = to_unsigned(max_value<std::streamsize>());
   do {
-    UnsignedStreamSize n = size <= max_size ? size : max_size;
-    os.write(data, static_cast<std::streamsize>(n));
-    data += n;
+    unsigned_streamsize n = size <= max_size ? size : max_size;
+    os.write(buf_data, static_cast<std::streamsize>(n));
+    buf_data += n;
     size -= n;
   } while (size != 0);
 }
 
 template <typename Char, typename T>
-void format_value(basic_buffer<Char> &buffer, const T &value) {
-  internal::formatbuf<Char> format_buf(buffer);
-  std::basic_ostream<Char> output(&format_buf);
-  output.exceptions(std::ios_base::failbit | std::ios_base::badbit);
+void format_value(buffer<Char>& buf, const T& value,
+                  locale_ref loc = locale_ref()) {
+  auto&& format_buf = formatbuf<std::basic_streambuf<Char>>(buf);
+  auto&& output = std::basic_ostream<Char>(&format_buf);
+#if !defined(FMT_STATIC_THOUSANDS_SEPARATOR)
+  if (loc) output.imbue(loc.get<std::locale>());
+#endif
   output << value;
-  buffer.resize(buffer.size());
+  output.exceptions(std::ios_base::failbit | std::ios_base::badbit);
+  buf.try_resize(buf.size());
 }
-}  // namespace internal
-
-// Disable conversion to int if T has an overloaded operator<< which is a free
-// function (not a member of std::ostream).
-template <typename T, typename Char>
-struct convert_to_int<T, Char, void> {
-  static const bool value =
-    convert_to_int<T, Char, int>::value &&
-    !internal::is_streamable<T, Char>::value;
-};
 
 // Formats an object of type T that has an overloaded ostream operator<<.
 template <typename T, typename Char>
-struct formatter<T, Char,
-    typename std::enable_if<
-      internal::is_streamable<T, Char>::value &&
-      !internal::format_type<
-        typename buffer_context<Char>::type, T>::value>::type>
-    : formatter<basic_string_view<Char>, Char> {
-
-  template <typename Context>
-  auto format(const T &value, Context &ctx) -> decltype(ctx.out()) {
-    basic_memory_buffer<Char> buffer;
-    internal::format_value(buffer, value);
-    basic_string_view<Char> str(buffer.data(), buffer.size());
-    return formatter<basic_string_view<Char>, Char>::format(str, ctx);
+struct fallback_formatter<T, Char, enable_if_t<is_streamable<T, Char>::value>>
+    : private formatter<basic_string_view<Char>, Char> {
+  using formatter<basic_string_view<Char>, Char>::parse;
+
+  template <typename OutputIt>
+  auto format(const T& value, basic_format_context<OutputIt, Char>& ctx)
+      -> OutputIt {
+    auto buffer = basic_memory_buffer<Char>();
+    format_value(buffer, value, ctx.locale());
+    return formatter<basic_string_view<Char>, Char>::format(
+        {buffer.data(), buffer.size()}, ctx);
+  }
+
+  // DEPRECATED!
+  template <typename OutputIt>
+  auto format(const T& value, basic_printf_context<OutputIt, Char>& ctx)
+      -> OutputIt {
+    auto buffer = basic_memory_buffer<Char>();
+    format_value(buffer, value, ctx.locale());
+    return std::copy(buffer.begin(), buffer.end(), ctx.out());
   }
 };
+}  // namespace detail
 
+FMT_MODULE_EXPORT
 template <typename Char>
-inline void vprint(std::basic_ostream<Char> &os,
-                   basic_string_view<Char> format_str,
-                   basic_format_args<typename buffer_context<Char>::type> args) {
-  basic_memory_buffer<Char> buffer;
-  internal::vformat_to(buffer, format_str, args);
-  internal::write(os, buffer);
+void vprint(std::basic_ostream<Char>& os, basic_string_view<Char> format_str,
+            basic_format_args<buffer_context<type_identity_t<Char>>> args) {
+  auto buffer = basic_memory_buffer<Char>();
+  detail::vformat_to(buffer, format_str, args);
+  detail::write_buffer(os, buffer);
 }
+
 /**
   \rst
   Prints formatted data to the stream *os*.
 
   **Example**::
 
     fmt::print(cerr, "Don't {}!", "panic");
   \endrst
  */
-template <typename S, typename... Args>
-inline typename std::enable_if<internal::is_string<S>::value>::type
-print(std::basic_ostream<FMT_CHAR(S)> &os, const S &format_str,
-      const Args & ... args) {
-  internal::checked_args<S, Args...> ca(format_str, args...);
-  vprint(os, to_string_view(format_str), *ca);
+FMT_MODULE_EXPORT
+template <typename S, typename... Args,
+          typename Char = enable_if_t<detail::is_string<S>::value, char_t<S>>>
+void print(std::basic_ostream<Char>& os, const S& format_str, Args&&... args) {
+  vprint(os, to_string_view(format_str),
+         fmt::make_args_checked<Args...>(format_str, args...));
 }
 FMT_END_NAMESPACE
 
 #endif  // FMT_OSTREAM_H_
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/fmt/bundled/printf.h` & `spdlog-2.0.6/spdlog/include/spdlog/fmt/bundled/printf.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,855 +1,657 @@
-// Formatting library for C++
+// Formatting library for C++ - legacy printf implementation
 //
 // Copyright (c) 2012 - 2016, Victor Zverovich
 // All rights reserved.
 //
 // For the license information refer to format.h.
 
 #ifndef FMT_PRINTF_H_
 #define FMT_PRINTF_H_
 
-#include <algorithm>  // std::fill_n
+#include <algorithm>  // std::max
 #include <limits>     // std::numeric_limits
+#include <ostream>
 
-#include "ostream.h"
+#include "format.h"
 
 FMT_BEGIN_NAMESPACE
-namespace internal {
+FMT_MODULE_EXPORT_BEGIN
 
-// An iterator that produces a null terminator on *end. This simplifies parsing
-// and allows comparing the performance of processing a null-terminated string
-// vs string_view.
-template <typename Char>
-class null_terminating_iterator {
- public:
-  typedef std::ptrdiff_t difference_type;
-  typedef Char value_type;
-  typedef const Char* pointer;
-  typedef const Char& reference;
-  typedef std::random_access_iterator_tag iterator_category;
-
-  null_terminating_iterator() : ptr_(0), end_(0) {}
-
-  FMT_CONSTEXPR null_terminating_iterator(const Char *ptr, const Char *end)
-    : ptr_(ptr), end_(end) {}
-
-  template <typename Range>
-  FMT_CONSTEXPR explicit null_terminating_iterator(const Range &r)
-    : ptr_(r.begin()), end_(r.end()) {}
-
-  FMT_CONSTEXPR null_terminating_iterator &operator=(const Char *ptr) {
-    assert(ptr <= end_);
-    ptr_ = ptr;
-    return *this;
-  }
-
-  FMT_CONSTEXPR Char operator*() const {
-    return ptr_ != end_ ? *ptr_ : Char();
-  }
+template <typename T> struct printf_formatter { printf_formatter() = delete; };
 
-  FMT_CONSTEXPR null_terminating_iterator operator++() {
-    ++ptr_;
-    return *this;
-  }
-
-  FMT_CONSTEXPR null_terminating_iterator operator++(int) {
-    null_terminating_iterator result(*this);
-    ++ptr_;
-    return result;
-  }
+template <typename Char>
+class basic_printf_parse_context : public basic_format_parse_context<Char> {
+  using basic_format_parse_context<Char>::basic_format_parse_context;
+};
 
-  FMT_CONSTEXPR null_terminating_iterator operator--() {
-    --ptr_;
-    return *this;
-  }
+template <typename OutputIt, typename Char> class basic_printf_context {
+ private:
+  OutputIt out_;
+  basic_format_args<basic_printf_context> args_;
 
-  FMT_CONSTEXPR null_terminating_iterator operator+(difference_type n) {
-    return null_terminating_iterator(ptr_ + n, end_);
-  }
+ public:
+  using char_type = Char;
+  using format_arg = basic_format_arg<basic_printf_context>;
+  using parse_context_type = basic_printf_parse_context<Char>;
+  template <typename T> using formatter_type = printf_formatter<T>;
 
-  FMT_CONSTEXPR null_terminating_iterator operator-(difference_type n) {
-    return null_terminating_iterator(ptr_ - n, end_);
-  }
+  /**
+    \rst
+    Constructs a ``printf_context`` object. References to the arguments are
+    stored in the context object so make sure they have appropriate lifetimes.
+    \endrst
+   */
+  basic_printf_context(OutputIt out,
+                       basic_format_args<basic_printf_context> args)
+      : out_(out), args_(args) {}
 
-  FMT_CONSTEXPR null_terminating_iterator operator+=(difference_type n) {
-    ptr_ += n;
-    return *this;
-  }
+  OutputIt out() { return out_; }
+  void advance_to(OutputIt it) { out_ = it; }
 
-  FMT_CONSTEXPR difference_type operator-(
-      null_terminating_iterator other) const {
-    return ptr_ - other.ptr_;
-  }
+  detail::locale_ref locale() { return {}; }
 
-  FMT_CONSTEXPR bool operator!=(null_terminating_iterator other) const {
-    return ptr_ != other.ptr_;
-  }
+  format_arg arg(int id) const { return args_.get(id); }
 
-  bool operator>=(null_terminating_iterator other) const {
-    return ptr_ >= other.ptr_;
+  FMT_CONSTEXPR void on_error(const char* message) {
+    detail::error_handler().on_error(message);
   }
-
-  // This should be a friend specialization pointer_from<Char> but the latter
-  // doesn't compile by gcc 5.1 due to a compiler bug.
-  template <typename CharT>
-  friend FMT_CONSTEXPR_DECL const CharT *pointer_from(
-      null_terminating_iterator<CharT> it);
-
- private:
-  const Char *ptr_;
-  const Char *end_;
 };
 
-template <typename T>
-FMT_CONSTEXPR const T *pointer_from(const T *p) { return p; }
-
-template <typename Char>
-FMT_CONSTEXPR const Char *pointer_from(null_terminating_iterator<Char> it) {
-  return it.ptr_;
-}
-
-// DEPRECATED: Parses the input as an unsigned integer. This function assumes
-// that the first character is a digit and presence of a non-digit character at
-// the end.
-// it: an iterator pointing to the beginning of the input range.
-template <typename Iterator, typename ErrorHandler>
-FMT_CONSTEXPR unsigned parse_nonnegative_int(Iterator &it, ErrorHandler &&eh) {
-  assert('0' <= *it && *it <= '9');
-  if (*it == '0') {
-    ++it;
-    return 0;
-  }
-  unsigned value = 0;
-  // Convert to unsigned to prevent a warning.
-  unsigned max_int = (std::numeric_limits<int>::max)();
-  unsigned big = max_int / 10;
-  do {
-    // Check for overflow.
-    if (value > big) {
-      value = max_int + 1;
-      break;
-    }
-    value = value * 10 + unsigned(*it - '0');
-    // Workaround for MSVC "setup_exception stack overflow" error:
-    auto next = it;
-    ++next;
-    it = next;
-  } while ('0' <= *it && *it <= '9');
-  if (value > max_int)
-    eh.on_error("number is too big");
-  return value;
-}
+FMT_BEGIN_DETAIL_NAMESPACE
 
 // Checks if a value fits in int - used to avoid warnings about comparing
 // signed and unsigned integers.
-template <bool IsSigned>
-struct int_checker {
-  template <typename T>
-  static bool fits_in_int(T value) {
-    unsigned max = std::numeric_limits<int>::max();
+template <bool IsSigned> struct int_checker {
+  template <typename T> static bool fits_in_int(T value) {
+    unsigned max = max_value<int>();
     return value <= max;
   }
   static bool fits_in_int(bool) { return true; }
 };
 
-template <>
-struct int_checker<true> {
-  template <typename T>
-  static bool fits_in_int(T value) {
-    return value >= std::numeric_limits<int>::min() &&
-           value <= std::numeric_limits<int>::max();
+template <> struct int_checker<true> {
+  template <typename T> static bool fits_in_int(T value) {
+    return value >= (std::numeric_limits<int>::min)() &&
+           value <= max_value<int>();
   }
   static bool fits_in_int(int) { return true; }
 };
 
-class printf_precision_handler: public function<int> {
+class printf_precision_handler {
  public:
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value, int>::type
-      operator()(T value) {
+  template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+  int operator()(T value) {
     if (!int_checker<std::numeric_limits<T>::is_signed>::fits_in_int(value))
       FMT_THROW(format_error("number is too big"));
-    return static_cast<int>(value);
+    return (std::max)(static_cast<int>(value), 0);
   }
 
-  template <typename T>
-  typename std::enable_if<!std::is_integral<T>::value, int>::type operator()(T) {
+  template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+  int operator()(T) {
     FMT_THROW(format_error("precision is not integer"));
     return 0;
   }
 };
 
 // An argument visitor that returns true iff arg is a zero integer.
-class is_zero_int: public function<bool> {
+class is_zero_int {
  public:
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value, bool>::type
-      operator()(T value) { return value == 0; }
+  template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+  bool operator()(T value) {
+    return value == 0;
+  }
 
-  template <typename T>
-  typename std::enable_if<!std::is_integral<T>::value, bool>::type
-      operator()(T) { return false; }
+  template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+  bool operator()(T) {
+    return false;
+  }
 };
 
-template <typename T>
-struct make_unsigned_or_bool : std::make_unsigned<T> {};
+template <typename T> struct make_unsigned_or_bool : std::make_unsigned<T> {};
 
-template <>
-struct make_unsigned_or_bool<bool> {
-  typedef bool type;
-};
+template <> struct make_unsigned_or_bool<bool> { using type = bool; };
 
-template <typename T, typename Context>
-class arg_converter: public function<void> {
+template <typename T, typename Context> class arg_converter {
  private:
-  typedef typename Context::char_type Char;
+  using char_type = typename Context::char_type;
 
-  basic_format_arg<Context> &arg_;
-  typename Context::char_type type_;
+  basic_format_arg<Context>& arg_;
+  char_type type_;
 
  public:
-  arg_converter(basic_format_arg<Context> &arg, Char type)
-    : arg_(arg), type_(type) {}
+  arg_converter(basic_format_arg<Context>& arg, char_type type)
+      : arg_(arg), type_(type) {}
 
   void operator()(bool value) {
-    if (type_ != 's')
-      operator()<bool>(value);
+    if (type_ != 's') operator()<bool>(value);
   }
 
-  template <typename U>
-  typename std::enable_if<std::is_integral<U>::value>::type
-      operator()(U value) {
+  template <typename U, FMT_ENABLE_IF(std::is_integral<U>::value)>
+  void operator()(U value) {
     bool is_signed = type_ == 'd' || type_ == 'i';
-    typedef typename std::conditional<
-        std::is_same<T, void>::value, U, T>::type TargetType;
-    if (const_check(sizeof(TargetType) <= sizeof(int))) {
+    using target_type = conditional_t<std::is_same<T, void>::value, U, T>;
+    if (const_check(sizeof(target_type) <= sizeof(int))) {
       // Extra casts are used to silence warnings.
       if (is_signed) {
-        arg_ = internal::make_arg<Context>(
-          static_cast<int>(static_cast<TargetType>(value)));
+        arg_ = detail::make_arg<Context>(
+            static_cast<int>(static_cast<target_type>(value)));
       } else {
-        typedef typename make_unsigned_or_bool<TargetType>::type Unsigned;
-        arg_ = internal::make_arg<Context>(
-          static_cast<unsigned>(static_cast<Unsigned>(value)));
+        using unsigned_type = typename make_unsigned_or_bool<target_type>::type;
+        arg_ = detail::make_arg<Context>(
+            static_cast<unsigned>(static_cast<unsigned_type>(value)));
       }
     } else {
       if (is_signed) {
         // glibc's printf doesn't sign extend arguments of smaller types:
         //   std::printf("%lld", -42);  // prints "4294967254"
         // but we don't have to do the same because it's a UB.
-        arg_ = internal::make_arg<Context>(static_cast<long long>(value));
+        arg_ = detail::make_arg<Context>(static_cast<long long>(value));
       } else {
-        arg_ = internal::make_arg<Context>(
-          static_cast<typename make_unsigned_or_bool<U>::type>(value));
+        arg_ = detail::make_arg<Context>(
+            static_cast<typename make_unsigned_or_bool<U>::type>(value));
       }
     }
   }
 
-  template <typename U>
-  typename std::enable_if<!std::is_integral<U>::value>::type operator()(U) {
-    // No coversion needed for non-integral types.
-  }
+  template <typename U, FMT_ENABLE_IF(!std::is_integral<U>::value)>
+  void operator()(U) {}  // No conversion needed for non-integral types.
 };
 
 // Converts an integer argument to T for printf, if T is an integral type.
 // If T is void, the argument is converted to corresponding signed or unsigned
 // type depending on the type specifier: 'd' and 'i' - signed, other -
 // unsigned).
 template <typename T, typename Context, typename Char>
-void convert_arg(basic_format_arg<Context> &arg, Char type) {
+void convert_arg(basic_format_arg<Context>& arg, Char type) {
   visit_format_arg(arg_converter<T, Context>(arg, type), arg);
 }
 
 // Converts an integer argument to char for printf.
-template <typename Context>
-class char_converter: public function<void> {
+template <typename Context> class char_converter {
  private:
-  basic_format_arg<Context> &arg_;
+  basic_format_arg<Context>& arg_;
 
  public:
-  explicit char_converter(basic_format_arg<Context> &arg) : arg_(arg) {}
+  explicit char_converter(basic_format_arg<Context>& arg) : arg_(arg) {}
 
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value>::type
-      operator()(T value) {
-    typedef typename Context::char_type Char;
-    arg_ = internal::make_arg<Context>(static_cast<Char>(value));
+  template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+  void operator()(T value) {
+    arg_ = detail::make_arg<Context>(
+        static_cast<typename Context::char_type>(value));
   }
 
-  template <typename T>
-  typename std::enable_if<!std::is_integral<T>::value>::type operator()(T) {
-    // No coversion needed for non-integral types.
-  }
+  template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+  void operator()(T) {}  // No conversion needed for non-integral types.
+};
+
+// An argument visitor that return a pointer to a C string if argument is a
+// string or null otherwise.
+template <typename Char> struct get_cstring {
+  template <typename T> const Char* operator()(T) { return nullptr; }
+  const Char* operator()(const Char* s) { return s; }
 };
 
 // Checks if an argument is a valid printf width specifier and sets
 // left alignment if it is negative.
-template <typename Char>
-class printf_width_handler: public function<unsigned> {
+template <typename Char> class printf_width_handler {
  private:
-  typedef basic_format_specs<Char> format_specs;
+  using format_specs = basic_format_specs<Char>;
 
-  format_specs &spec_;
+  format_specs& specs_;
 
  public:
-  explicit printf_width_handler(format_specs &spec) : spec_(spec) {}
+  explicit printf_width_handler(format_specs& specs) : specs_(specs) {}
 
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value, unsigned>::type
-      operator()(T value) {
-    typedef typename internal::int_traits<T>::main_type UnsignedType;
-    UnsignedType width = static_cast<UnsignedType>(value);
-    if (internal::is_negative(value)) {
-      spec_.align_ = ALIGN_LEFT;
+  template <typename T, FMT_ENABLE_IF(std::is_integral<T>::value)>
+  unsigned operator()(T value) {
+    auto width = static_cast<uint32_or_64_or_128_t<T>>(value);
+    if (detail::is_negative(value)) {
+      specs_.align = align::left;
       width = 0 - width;
     }
-    unsigned int_max = std::numeric_limits<int>::max();
-    if (width > int_max)
-      FMT_THROW(format_error("number is too big"));
+    unsigned int_max = max_value<int>();
+    if (width > int_max) FMT_THROW(format_error("number is too big"));
     return static_cast<unsigned>(width);
   }
 
-  template <typename T>
-  typename std::enable_if<!std::is_integral<T>::value, unsigned>::type
-      operator()(T) {
+  template <typename T, FMT_ENABLE_IF(!std::is_integral<T>::value)>
+  unsigned operator()(T) {
     FMT_THROW(format_error("width is not integer"));
     return 0;
   }
 };
 
-template <typename Char, typename Context>
-void printf(basic_buffer<Char> &buf, basic_string_view<Char> format,
-            basic_format_args<Context> args) {
-  Context(std::back_inserter(buf), format, args).format();
-}
-}  // namespace internal
-
-using internal::printf;  // For printing into memory_buffer.
-
-template <typename Range>
-class printf_arg_formatter;
-
-template <
-    typename OutputIt, typename Char,
-    typename ArgFormatter =
-      printf_arg_formatter<back_insert_range<internal::basic_buffer<Char>>>>
-class basic_printf_context;
-
-/**
-  \rst
-  The ``printf`` argument formatter.
-  \endrst
- */
-template <typename Range>
-class printf_arg_formatter:
-  public internal::function<
-    typename internal::arg_formatter_base<Range>::iterator>,
-  public internal::arg_formatter_base<Range> {
+// The ``printf`` argument formatter.
+template <typename OutputIt, typename Char>
+class printf_arg_formatter : public arg_formatter<Char> {
  private:
-  typedef typename Range::value_type char_type;
-  typedef decltype(internal::declval<Range>().begin()) iterator;
-  typedef internal::arg_formatter_base<Range> base;
-  typedef basic_printf_context<iterator, char_type> context_type;
-
-  context_type &context_;
-
-  void write_null_pointer(char) {
-    this->spec()->type = 0;
-    this->write("(nil)");
-  }
-
-  void write_null_pointer(wchar_t) {
-    this->spec()->type = 0;
-    this->write(L"(nil)");
+  using base = arg_formatter<Char>;
+  using context_type = basic_printf_context<OutputIt, Char>;
+  using format_specs = basic_format_specs<Char>;
+
+  context_type& context_;
+
+  OutputIt write_null_pointer(bool is_string = false) {
+    auto s = this->specs;
+    s.type = presentation_type::none;
+    return write_bytes(this->out, is_string ? "(null)" : "(nil)", s);
   }
 
  public:
-  typedef typename base::format_specs format_specs;
+  printf_arg_formatter(OutputIt iter, format_specs& s, context_type& ctx)
+      : base{iter, s, locale_ref()}, context_(ctx) {}
 
-  /**
-    \rst
-    Constructs an argument formatter object.
-    *buffer* is a reference to the output buffer and *spec* contains format
-    specifier information for standard argument types.
-    \endrst
-   */
-  printf_arg_formatter(internal::basic_buffer<char_type> &buffer,
-                       format_specs &spec, context_type &ctx)
-    : base(back_insert_range<internal::basic_buffer<char_type>>(buffer), &spec,
-           ctx.locale()),
-      context_(ctx) {}
-
-  template <typename T>
-  typename std::enable_if<std::is_integral<T>::value, iterator>::type
-      operator()(T value) {
-    // MSVC2013 fails to compile separate overloads for bool and char_type so
-    // use std::is_same instead.
-    if (std::is_same<T, bool>::value) {
-      format_specs &fmt_spec = *this->spec();
-      if (fmt_spec.type != 's')
-        return base::operator()(value ? 1 : 0);
-      fmt_spec.type = 0;
-      this->write(value != 0);
-    } else if (std::is_same<T, char_type>::value) {
-      format_specs &fmt_spec = *this->spec();
-      if (fmt_spec.type && fmt_spec.type != 'c')
+  OutputIt operator()(monostate value) { return base::operator()(value); }
+
+  template <typename T, FMT_ENABLE_IF(detail::is_integral<T>::value)>
+  OutputIt operator()(T value) {
+    // MSVC2013 fails to compile separate overloads for bool and Char so use
+    // std::is_same instead.
+    if (std::is_same<T, Char>::value) {
+      format_specs fmt_specs = this->specs;
+      if (fmt_specs.type != presentation_type::none &&
+          fmt_specs.type != presentation_type::chr) {
         return (*this)(static_cast<int>(value));
-      fmt_spec.flags = 0;
-      fmt_spec.align_ = ALIGN_RIGHT;
-      return base::operator()(value);
-    } else {
-      return base::operator()(value);
+      }
+      fmt_specs.sign = sign::none;
+      fmt_specs.alt = false;
+      fmt_specs.fill[0] = ' ';  // Ignore '0' flag for char types.
+      // align::numeric needs to be overwritten here since the '0' flag is
+      // ignored for non-numeric types
+      if (fmt_specs.align == align::none || fmt_specs.align == align::numeric)
+        fmt_specs.align = align::right;
+      return write<Char>(this->out, static_cast<Char>(value), fmt_specs);
     }
-    return this->out();
+    return base::operator()(value);
   }
 
-  template <typename T>
-  typename std::enable_if<std::is_floating_point<T>::value, iterator>::type
-      operator()(T value) {
+  template <typename T, FMT_ENABLE_IF(std::is_floating_point<T>::value)>
+  OutputIt operator()(T value) {
     return base::operator()(value);
   }
 
   /** Formats a null-terminated C string. */
-  iterator operator()(const char *value) {
-    if (value)
-      base::operator()(value);
-    else if (this->spec()->type == 'p')
-      write_null_pointer(char_type());
-    else
-      this->write("(null)");
-    return this->out();
+  OutputIt operator()(const char* value) {
+    if (value) return base::operator()(value);
+    return write_null_pointer(this->specs.type != presentation_type::pointer);
   }
 
   /** Formats a null-terminated wide C string. */
-  iterator operator()(const wchar_t *value) {
-    if (value)
-      base::operator()(value);
-    else if (this->spec()->type == 'p')
-      write_null_pointer(char_type());
-    else
-      this->write(L"(null)");
-    return this->out();
-  }
-
-  iterator operator()(basic_string_view<char_type> value) {
-    return base::operator()(value);
+  OutputIt operator()(const wchar_t* value) {
+    if (value) return base::operator()(value);
+    return write_null_pointer(this->specs.type != presentation_type::pointer);
   }
 
-  iterator operator()(monostate value) {
+  OutputIt operator()(basic_string_view<Char> value) {
     return base::operator()(value);
   }
 
   /** Formats a pointer. */
-  iterator operator()(const void *value) {
-    if (value)
-      return base::operator()(value);
-    this->spec()->type = 0;
-    write_null_pointer(char_type());
-    return this->out();
+  OutputIt operator()(const void* value) {
+    return value ? base::operator()(value) : write_null_pointer();
   }
 
   /** Formats an argument of a custom (user-defined) type. */
-  iterator operator()(typename basic_format_arg<context_type>::handle handle) {
-    handle.format(context_);
-    return this->out();
+  OutputIt operator()(typename basic_format_arg<context_type>::handle handle) {
+    auto parse_ctx =
+        basic_printf_parse_context<Char>(basic_string_view<Char>());
+    handle.format(parse_ctx, context_);
+    return this->out;
   }
 };
 
-template <typename T>
-struct printf_formatter {
-  template <typename ParseContext>
-  auto parse(ParseContext &ctx) -> decltype(ctx.begin()) { return ctx.begin(); }
-
-  template <typename FormatContext>
-  auto format(const T &value, FormatContext &ctx) -> decltype(ctx.out()) {
-    internal::format_value(internal::get_container(ctx.out()), value);
-    return ctx.out();
-  }
-};
-
-/** This template formats data and writes the output to a writer. */
-template <typename OutputIt, typename Char, typename ArgFormatter>
-class basic_printf_context :
-  // Inherit publicly as a workaround for the icc bug
-  // https://software.intel.com/en-us/forums/intel-c-compiler/topic/783476.
-  public internal::context_base<
-    OutputIt, basic_printf_context<OutputIt, Char, ArgFormatter>, Char> {
- public:
-  /** The character type for the output. */
-  typedef Char char_type;
-
-  template <typename T>
-  struct formatter_type { typedef printf_formatter<T> type; };
-
- private:
-  typedef internal::context_base<OutputIt, basic_printf_context, Char> base;
-  typedef typename base::format_arg format_arg;
-  typedef basic_format_specs<char_type> format_specs;
-  typedef internal::null_terminating_iterator<char_type> iterator;
-
-  void parse_flags(format_specs &spec, iterator &it);
-
-  // Returns the argument with specified index or, if arg_index is equal
-  // to the maximum unsigned value, the next argument.
-  format_arg get_arg(
-      iterator it,
-      unsigned arg_index = (std::numeric_limits<unsigned>::max)());
-
-  // Parses argument index, flags and width and returns the argument index.
-  unsigned parse_header(iterator &it, format_specs &spec);
-
- public:
-  /**
-   \rst
-   Constructs a ``printf_context`` object. References to the arguments and
-   the writer are stored in the context object so make sure they have
-   appropriate lifetimes.
-   \endrst
-   */
-  basic_printf_context(OutputIt out, basic_string_view<char_type> format_str,
-                       basic_format_args<basic_printf_context> args)
-    : base(out, format_str, args) {}
-
-  using base::parse_context;
-  using base::out;
-  using base::advance_to;
-
-  /** Formats stored arguments and writes the output to the range. */
-  void format();
-};
-
-template <typename OutputIt, typename Char, typename AF>
-void basic_printf_context<OutputIt, Char, AF>::parse_flags(
-    format_specs &spec, iterator &it) {
-  for (;;) {
-    switch (*it++) {
-      case '-':
-        spec.align_ = ALIGN_LEFT;
-        break;
-      case '+':
-        spec.flags |= SIGN_FLAG | PLUS_FLAG;
-        break;
-      case '0':
-        spec.fill_ = '0';
-        break;
-      case ' ':
-        spec.flags |= SIGN_FLAG;
-        break;
-      case '#':
-        spec.flags |= HASH_FLAG;
-        break;
-      default:
-        --it;
-        return;
+template <typename Char>
+void parse_flags(basic_format_specs<Char>& specs, const Char*& it,
+                 const Char* end) {
+  for (; it != end; ++it) {
+    switch (*it) {
+    case '-':
+      specs.align = align::left;
+      break;
+    case '+':
+      specs.sign = sign::plus;
+      break;
+    case '0':
+      specs.fill[0] = '0';
+      break;
+    case ' ':
+      if (specs.sign != sign::plus) {
+        specs.sign = sign::space;
+      }
+      break;
+    case '#':
+      specs.alt = true;
+      break;
+    default:
+      return;
     }
   }
 }
 
-template <typename OutputIt, typename Char, typename AF>
-typename basic_printf_context<OutputIt, Char, AF>::format_arg
-  basic_printf_context<OutputIt, Char, AF>::get_arg(
-    iterator it, unsigned arg_index) {
-  (void)it;
-  if (arg_index == std::numeric_limits<unsigned>::max())
-    return this->do_get_arg(this->parse_context().next_arg_id());
-  return base::get_arg(arg_index - 1);
-}
-
-template <typename OutputIt, typename Char, typename AF>
-unsigned basic_printf_context<OutputIt, Char, AF>::parse_header(
-  iterator &it, format_specs &spec) {
-  unsigned arg_index = std::numeric_limits<unsigned>::max();
-  char_type c = *it;
+template <typename Char, typename GetArg>
+int parse_header(const Char*& it, const Char* end,
+                 basic_format_specs<Char>& specs, GetArg get_arg) {
+  int arg_index = -1;
+  Char c = *it;
   if (c >= '0' && c <= '9') {
     // Parse an argument index (if followed by '$') or a width possibly
     // preceded with '0' flag(s).
-    internal::error_handler eh;
-    unsigned value = parse_nonnegative_int(it, eh);
-    if (*it == '$') {  // value is an argument index
+    int value = parse_nonnegative_int(it, end, -1);
+    if (it != end && *it == '$') {  // value is an argument index
       ++it;
-      arg_index = value;
+      arg_index = value != -1 ? value : max_value<int>();
     } else {
-      if (c == '0')
-        spec.fill_ = '0';
+      if (c == '0') specs.fill[0] = '0';
       if (value != 0) {
         // Nonzero value means that we parsed width and don't need to
         // parse it or flags again, so return now.
-        spec.width_ = value;
+        if (value == -1) FMT_THROW(format_error("number is too big"));
+        specs.width = value;
         return arg_index;
       }
     }
   }
-  parse_flags(spec, it);
+  parse_flags(specs, it, end);
   // Parse width.
-  if (*it >= '0' && *it <= '9') {
-    internal::error_handler eh;
-    spec.width_ = parse_nonnegative_int(it, eh);
-  } else if (*it == '*') {
-    ++it;
-    spec.width_ = visit_format_arg(
-          internal::printf_width_handler<char_type>(spec), get_arg(it));
+  if (it != end) {
+    if (*it >= '0' && *it <= '9') {
+      specs.width = parse_nonnegative_int(it, end, -1);
+      if (specs.width == -1) FMT_THROW(format_error("number is too big"));
+    } else if (*it == '*') {
+      ++it;
+      specs.width = static_cast<int>(visit_format_arg(
+          detail::printf_width_handler<Char>(specs), get_arg(-1)));
+    }
   }
   return arg_index;
 }
 
-template <typename OutputIt, typename Char, typename AF>
-void basic_printf_context<OutputIt, Char, AF>::format() {
-  auto &buffer = internal::get_container(this->out());
-  auto start = iterator(this->parse_context());
+template <typename Char, typename Context>
+void vprintf(buffer<Char>& buf, basic_string_view<Char> format,
+             basic_format_args<Context> args) {
+  using OutputIt = buffer_appender<Char>;
+  auto out = OutputIt(buf);
+  auto context = basic_printf_context<OutputIt, Char>(out, args);
+  auto parse_ctx = basic_printf_parse_context<Char>(format);
+
+  // Returns the argument with specified index or, if arg_index is -1, the next
+  // argument.
+  auto get_arg = [&](int arg_index) {
+    if (arg_index < 0)
+      arg_index = parse_ctx.next_arg_id();
+    else
+      parse_ctx.check_arg_id(--arg_index);
+    return detail::get_arg(context, arg_index);
+  };
+
+  const Char* start = parse_ctx.begin();
+  const Char* end = parse_ctx.end();
   auto it = start;
-  using internal::pointer_from;
-  while (*it) {
-    char_type c = *it++;
-    if (c != '%') continue;
-    if (*it == c) {
-      buffer.append(pointer_from(start), pointer_from(it));
+  while (it != end) {
+    if (!detail::find<false, Char>(it, end, '%', it)) {
+      it = end;  // detail::find leaves it == nullptr if it doesn't find '%'
+      break;
+    }
+    Char c = *it++;
+    if (it != end && *it == c) {
+      out = detail::write(
+          out, basic_string_view<Char>(start, detail::to_unsigned(it - start)));
       start = ++it;
       continue;
     }
-    buffer.append(pointer_from(start), pointer_from(it) - 1);
+    out = detail::write(out, basic_string_view<Char>(
+                                 start, detail::to_unsigned(it - 1 - start)));
 
-    format_specs spec;
-    spec.align_ = ALIGN_RIGHT;
+    basic_format_specs<Char> specs;
+    specs.align = align::right;
 
     // Parse argument index, flags and width.
-    unsigned arg_index = parse_header(it, spec);
+    int arg_index = parse_header(it, end, specs, get_arg);
+    if (arg_index == 0) parse_ctx.on_error("argument not found");
 
     // Parse precision.
-    if (*it == '.') {
+    if (it != end && *it == '.') {
       ++it;
-      if ('0' <= *it && *it <= '9') {
-        internal::error_handler eh;
-        spec.precision = static_cast<int>(parse_nonnegative_int(it, eh));
-      } else if (*it == '*') {
+      c = it != end ? *it : 0;
+      if ('0' <= c && c <= '9') {
+        specs.precision = parse_nonnegative_int(it, end, 0);
+      } else if (c == '*') {
         ++it;
-        spec.precision =
-            visit_format_arg(internal::printf_precision_handler(), get_arg(it));
+        specs.precision = static_cast<int>(
+            visit_format_arg(detail::printf_precision_handler(), get_arg(-1)));
       } else {
-        spec.precision = 0;
+        specs.precision = 0;
       }
     }
 
-    format_arg arg = get_arg(it, arg_index);
-    if (spec.has(HASH_FLAG) && visit_format_arg(internal::is_zero_int(), arg))
-      spec.flags = static_cast<uint_least8_t>(spec.flags & (~internal::to_unsigned<int>(HASH_FLAG)));
-    if (spec.fill_ == '0') {
-      if (arg.is_arithmetic())
-        spec.align_ = ALIGN_NUMERIC;
+    auto arg = get_arg(arg_index);
+    // For d, i, o, u, x, and X conversion specifiers, if a precision is
+    // specified, the '0' flag is ignored
+    if (specs.precision >= 0 && arg.is_integral())
+      specs.fill[0] =
+          ' ';  // Ignore '0' flag for non-numeric types or if '-' present.
+    if (specs.precision >= 0 && arg.type() == detail::type::cstring_type) {
+      auto str = visit_format_arg(detail::get_cstring<Char>(), arg);
+      auto str_end = str + specs.precision;
+      auto nul = std::find(str, str_end, Char());
+      arg = detail::make_arg<basic_printf_context<OutputIt, Char>>(
+          basic_string_view<Char>(
+              str, detail::to_unsigned(nul != str_end ? nul - str
+                                                      : specs.precision)));
+    }
+    if (specs.alt && visit_format_arg(detail::is_zero_int(), arg))
+      specs.alt = false;
+    if (specs.fill[0] == '0') {
+      if (arg.is_arithmetic() && specs.align != align::left)
+        specs.align = align::numeric;
       else
-        spec.fill_ = ' ';  // Ignore '0' flag for non-numeric types.
+        specs.fill[0] = ' ';  // Ignore '0' flag for non-numeric types or if '-'
+                              // flag is also present.
     }
 
     // Parse length and convert the argument to the required type.
-    using internal::convert_arg;
-    switch (*it++) {
+    c = it != end ? *it++ : 0;
+    Char t = it != end ? *it : 0;
+    using detail::convert_arg;
+    switch (c) {
     case 'h':
-      if (*it == 'h')
-        convert_arg<signed char>(arg, *++it);
-      else
-        convert_arg<short>(arg, *it);
+      if (t == 'h') {
+        ++it;
+        t = it != end ? *it : 0;
+        convert_arg<signed char>(arg, t);
+      } else {
+        convert_arg<short>(arg, t);
+      }
       break;
     case 'l':
-      if (*it == 'l')
-        convert_arg<long long>(arg, *++it);
-      else
-        convert_arg<long>(arg, *it);
+      if (t == 'l') {
+        ++it;
+        t = it != end ? *it : 0;
+        convert_arg<long long>(arg, t);
+      } else {
+        convert_arg<long>(arg, t);
+      }
       break;
     case 'j':
-      convert_arg<intmax_t>(arg, *it);
+      convert_arg<intmax_t>(arg, t);
       break;
     case 'z':
-      convert_arg<std::size_t>(arg, *it);
+      convert_arg<size_t>(arg, t);
       break;
     case 't':
-      convert_arg<std::ptrdiff_t>(arg, *it);
+      convert_arg<std::ptrdiff_t>(arg, t);
       break;
     case 'L':
       // printf produces garbage when 'L' is omitted for long double, no
       // need to do the same.
       break;
     default:
       --it;
-      convert_arg<void>(arg, *it);
+      convert_arg<void>(arg, c);
     }
 
     // Parse type.
-    if (!*it)
-      FMT_THROW(format_error("invalid format string"));
-    spec.type = static_cast<char>(*it++);
+    if (it == end) FMT_THROW(format_error("invalid format string"));
+    char type = static_cast<char>(*it++);
     if (arg.is_integral()) {
       // Normalize type.
-      switch (spec.type) {
-      case 'i': case 'u':
-        spec.type = 'd';
+      switch (type) {
+      case 'i':
+      case 'u':
+        type = 'd';
         break;
       case 'c':
-        // TODO: handle wchar_t better?
         visit_format_arg(
-              internal::char_converter<basic_printf_context>(arg), arg);
+            detail::char_converter<basic_printf_context<OutputIt, Char>>(arg),
+            arg);
         break;
       }
     }
+    specs.type = parse_presentation_type(type);
+    if (specs.type == presentation_type::none)
+      parse_ctx.on_error("invalid type specifier");
 
     start = it;
 
     // Format argument.
-    visit_format_arg(AF(buffer, spec, *this), arg);
+    out = visit_format_arg(
+        detail::printf_arg_formatter<OutputIt, Char>(out, specs, context), arg);
   }
-  buffer.append(pointer_from(start), pointer_from(it));
+  detail::write(out, basic_string_view<Char>(start, to_unsigned(it - start)));
 }
+FMT_END_DETAIL_NAMESPACE
 
-template <typename Buffer>
-struct basic_printf_context_t {
-  typedef basic_printf_context<
-    std::back_insert_iterator<Buffer>, typename Buffer::value_type> type;
-};
+template <typename Char>
+using basic_printf_context_t =
+    basic_printf_context<detail::buffer_appender<Char>, Char>;
 
-typedef basic_printf_context_t<internal::buffer>::type printf_context;
-typedef basic_printf_context_t<internal::wbuffer>::type wprintf_context;
+using printf_context = basic_printf_context_t<char>;
+using wprintf_context = basic_printf_context_t<wchar_t>;
 
-typedef basic_format_args<printf_context> printf_args;
-typedef basic_format_args<wprintf_context> wprintf_args;
+using printf_args = basic_format_args<printf_context>;
+using wprintf_args = basic_format_args<wprintf_context>;
 
 /**
   \rst
   Constructs an `~fmt::format_arg_store` object that contains references to
-  arguments and can be implicitly converted to `~fmt::printf_args`. 
+  arguments and can be implicitly converted to `~fmt::printf_args`.
   \endrst
  */
-template<typename... Args>
-inline format_arg_store<printf_context, Args...>
-  make_printf_args(const Args &... args) { return {args...}; }
+template <typename... T>
+inline auto make_printf_args(const T&... args)
+    -> format_arg_store<printf_context, T...> {
+  return {args...};
+}
 
 /**
   \rst
   Constructs an `~fmt::format_arg_store` object that contains references to
-  arguments and can be implicitly converted to `~fmt::wprintf_args`. 
+  arguments and can be implicitly converted to `~fmt::wprintf_args`.
   \endrst
  */
-template<typename... Args>
-inline format_arg_store<wprintf_context, Args...>
-  make_wprintf_args(const Args &... args) { return {args...}; }
-
-template <typename S, typename Char = FMT_CHAR(S)>
-inline std::basic_string<Char>
-vsprintf(const S &format,
-         basic_format_args<typename basic_printf_context_t<
-           internal::basic_buffer<Char>>::type> args) {
+template <typename... T>
+inline auto make_wprintf_args(const T&... args)
+    -> format_arg_store<wprintf_context, T...> {
+  return {args...};
+}
+
+template <typename S, typename Char = char_t<S>>
+inline auto vsprintf(
+    const S& fmt,
+    basic_format_args<basic_printf_context_t<type_identity_t<Char>>> args)
+    -> std::basic_string<Char> {
   basic_memory_buffer<Char> buffer;
-  printf(buffer, to_string_view(format), args);
+  vprintf(buffer, to_string_view(fmt), args);
   return to_string(buffer);
 }
 
 /**
   \rst
   Formats arguments and returns the result as a string.
 
   **Example**::
 
     std::string message = fmt::sprintf("The answer is %d", 42);
   \endrst
 */
-template <typename S, typename... Args>
-inline FMT_ENABLE_IF_T(
-    internal::is_string<S>::value, std::basic_string<FMT_CHAR(S)>)
-    sprintf(const S &format, const Args & ... args) {
-  internal::check_format_string<Args...>(format);
-  typedef internal::basic_buffer<FMT_CHAR(S)> buffer;
-  typedef typename basic_printf_context_t<buffer>::type context;
-  format_arg_store<context, Args...> as{ args... };
-  return vsprintf(to_string_view(format),
-                  basic_format_args<context>(as));
-}
-
-template <typename S, typename Char = FMT_CHAR(S)>
-inline int vfprintf(std::FILE *f, const S &format,
-                    basic_format_args<typename basic_printf_context_t<
-                      internal::basic_buffer<Char>>::type> args) {
+template <typename S, typename... T,
+          typename Char = enable_if_t<detail::is_string<S>::value, char_t<S>>>
+inline auto sprintf(const S& fmt, const T&... args) -> std::basic_string<Char> {
+  using context = basic_printf_context_t<Char>;
+  return vsprintf(to_string_view(fmt), fmt::make_format_args<context>(args...));
+}
+
+template <typename S, typename Char = char_t<S>>
+inline auto vfprintf(
+    std::FILE* f, const S& fmt,
+    basic_format_args<basic_printf_context_t<type_identity_t<Char>>> args)
+    -> int {
   basic_memory_buffer<Char> buffer;
-  printf(buffer, to_string_view(format), args);
-  std::size_t size = buffer.size();
-  return std::fwrite(
-    buffer.data(), sizeof(Char), size, f) < size ? -1 : static_cast<int>(size);
+  vprintf(buffer, to_string_view(fmt), args);
+  size_t size = buffer.size();
+  return std::fwrite(buffer.data(), sizeof(Char), size, f) < size
+             ? -1
+             : static_cast<int>(size);
 }
 
 /**
   \rst
   Prints formatted data to the file *f*.
 
   **Example**::
 
     fmt::fprintf(stderr, "Don't %s!", "panic");
   \endrst
  */
-template <typename S, typename... Args>
-inline FMT_ENABLE_IF_T(internal::is_string<S>::value, int)
-    fprintf(std::FILE *f, const S &format, const Args & ... args) {
-  internal::check_format_string<Args...>(format);
-  typedef internal::basic_buffer<FMT_CHAR(S)> buffer;
-  typedef typename basic_printf_context_t<buffer>::type context;
-  format_arg_store<context, Args...> as{ args... };
-  return vfprintf(f, to_string_view(format),
-                  basic_format_args<context>(as));
-}
-
-template <typename S, typename Char = FMT_CHAR(S)>
-inline int vprintf(const S &format,
-                   basic_format_args<typename basic_printf_context_t<
-                    internal::basic_buffer<Char>>::type> args) {
-  return vfprintf(stdout, to_string_view(format), args);
+template <typename S, typename... T, typename Char = char_t<S>>
+inline auto fprintf(std::FILE* f, const S& fmt, const T&... args) -> int {
+  using context = basic_printf_context_t<Char>;
+  return vfprintf(f, to_string_view(fmt),
+                  fmt::make_format_args<context>(args...));
+}
+
+template <typename S, typename Char = char_t<S>>
+inline auto vprintf(
+    const S& fmt,
+    basic_format_args<basic_printf_context_t<type_identity_t<Char>>> args)
+    -> int {
+  return vfprintf(stdout, to_string_view(fmt), args);
 }
 
 /**
   \rst
   Prints formatted data to ``stdout``.
 
   **Example**::
 
     fmt::printf("Elapsed time: %.2f seconds", 1.23);
   \endrst
  */
-template <typename S, typename... Args>
-inline FMT_ENABLE_IF_T(internal::is_string<S>::value, int)
-    printf(const S &format_str, const Args & ... args) {
-  internal::check_format_string<Args...>(format_str);
-  typedef internal::basic_buffer<FMT_CHAR(S)> buffer;
-  typedef typename basic_printf_context_t<buffer>::type context;
-  format_arg_store<context, Args...> as{ args... };
-  return vprintf(to_string_view(format_str),
-                 basic_format_args<context>(as));
-}
-
-template <typename S, typename Char = FMT_CHAR(S)>
-inline int vfprintf(std::basic_ostream<Char> &os,
-                    const S &format,
-                    basic_format_args<typename basic_printf_context_t<
-                      internal::basic_buffer<Char>>::type> args) {
+template <typename S, typename... T, FMT_ENABLE_IF(detail::is_string<S>::value)>
+inline auto printf(const S& fmt, const T&... args) -> int {
+  return vprintf(
+      to_string_view(fmt),
+      fmt::make_format_args<basic_printf_context_t<char_t<S>>>(args...));
+}
+
+template <typename S, typename Char = char_t<S>>
+FMT_DEPRECATED auto vfprintf(
+    std::basic_ostream<Char>& os, const S& fmt,
+    basic_format_args<basic_printf_context_t<type_identity_t<Char>>> args)
+    -> int {
   basic_memory_buffer<Char> buffer;
-  printf(buffer, to_string_view(format), args);
-  internal::write(os, buffer);
+  vprintf(buffer, to_string_view(fmt), args);
+  os.write(buffer.data(), static_cast<std::streamsize>(buffer.size()));
   return static_cast<int>(buffer.size());
 }
-
-/**
-  \rst
-  Prints formatted data to the stream *os*.
-
-  **Example**::
-
-    fmt::fprintf(cerr, "Don't %s!", "panic");
-  \endrst
- */
-template <typename S, typename... Args>
-inline FMT_ENABLE_IF_T(internal::is_string<S>::value, int)
-    fprintf(std::basic_ostream<FMT_CHAR(S)> &os,
-            const S &format_str, const Args & ... args) {
-  internal::check_format_string<Args...>(format_str);
-  typedef internal::basic_buffer<FMT_CHAR(S)> buffer;
-  typedef typename basic_printf_context_t<buffer>::type context;
-  format_arg_store<context, Args...> as{ args... };
-  return vfprintf(os, to_string_view(format_str),
-                  basic_format_args<context>(as));
+template <typename S, typename... T, typename Char = char_t<S>>
+FMT_DEPRECATED auto fprintf(std::basic_ostream<Char>& os, const S& fmt,
+                            const T&... args) -> int {
+  return vfprintf(os, to_string_view(fmt),
+                  fmt::make_format_args<basic_printf_context_t<Char>>(args...));
 }
+
+FMT_MODULE_EXPORT_END
 FMT_END_NAMESPACE
 
 #endif  // FMT_PRINTF_H_
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/fmt/fmt.h` & `spdlog-2.0.6/spdlog/include/spdlog/fmt/fmt.h`

 * *Files 25% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 #pragma once
 
 //
 // Include a bundled header-only copy of fmtlib or an external one.
 // By default spdlog include its own copy.
 //
 
-#if !defined(SPDLOG_FMT_EXTERNAL)
-#ifndef FMT_HEADER_ONLY
-#define FMT_HEADER_ONLY
-#endif
-#ifndef FMT_USE_WINDOWS_H
-#define FMT_USE_WINDOWS_H 0
-#endif
-#include "bundled/core.h"
-#include "bundled/format.h"
-#else // external fmtlib
-#include <fmt/core.h>
-#include <fmt/format.h>
+#if defined(SPDLOG_USE_STD_FORMAT) // SPDLOG_USE_STD_FORMAT is defined - use std::format
+#    include <format>
+#elif !defined(SPDLOG_FMT_EXTERNAL)
+#    if !defined(SPDLOG_COMPILED_LIB) && !defined(FMT_HEADER_ONLY)
+#        define FMT_HEADER_ONLY
+#    endif
+#    ifndef FMT_USE_WINDOWS_H
+#        define FMT_USE_WINDOWS_H 0
+#    endif
+// enable the 'n' flag in for backward compatibility with fmt 6.x
+#    define FMT_DEPRECATED_N_SPECIFIER
+#    include <spdlog/fmt/bundled/core.h>
+#    include <spdlog/fmt/bundled/format.h>
+#else // SPDLOG_FMT_EXTERNAL is defined - use external fmtlib
+#    include <fmt/core.h>
+#    include <fmt/format.h>
 #endif
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/android_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/android_sink.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,57 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
-#endif
-
-#include "spdlog/details/fmt_helper.h"
-#include "spdlog/details/null_mutex.h"
-#include "spdlog/details/os.h"
-#include "spdlog/sinks/base_sink.h"
-
-#include <android/log.h>
-#include <chrono>
-#include <mutex>
-#include <string>
-#include <thread>
-
-#if !defined(SPDLOG_ANDROID_RETRIES)
-#define SPDLOG_ANDROID_RETRIES 2
-#endif
+#ifdef __ANDROID__
+
+#    include <spdlog/details/fmt_helper.h>
+#    include <spdlog/details/null_mutex.h>
+#    include <spdlog/details/os.h>
+#    include <spdlog/sinks/base_sink.h>
+#    include <spdlog/details/synchronous_factory.h>
+
+#    include <android/log.h>
+#    include <chrono>
+#    include <mutex>
+#    include <string>
+#    include <thread>
+
+#    if !defined(SPDLOG_ANDROID_RETRIES)
+#        define SPDLOG_ANDROID_RETRIES 2
+#    endif
 
 namespace spdlog {
 namespace sinks {
 
 /*
  * Android sink (logging using __android_log_write)
  */
 template<typename Mutex>
 class android_sink final : public base_sink<Mutex>
 {
 public:
     explicit android_sink(std::string tag = "spdlog", bool use_raw_msg = false)
         : tag_(std::move(tag))
         , use_raw_msg_(use_raw_msg)
-    {
-    }
+    {}
 
 protected:
     void sink_it_(const details::log_msg &msg) override
     {
         const android_LogPriority priority = convert_to_android_(msg.level);
-        fmt::memory_buffer formatted;
+        memory_buf_t formatted;
         if (use_raw_msg_)
         {
             details::fmt_helper::append_string_view(msg.payload, formatted);
         }
         else
         {
-            sink::formatter_->format(msg, formatted);
+            base_sink<Mutex>::formatter_->format(msg, formatted);
         }
         formatted.push_back('\0');
         const char *msg_output = formatted.data();
 
         // See system/core/liblog/logger_write.c for explanation of return value
         int ret = __android_log_write(priority, tag_.c_str(), msg_output);
         int retry_count = 0;
@@ -64,15 +60,15 @@
             details::os::sleep_for_millis(5);
             ret = __android_log_write(priority, tag_.c_str(), msg_output);
             retry_count++;
         }
 
         if (ret < 0)
         {
-            throw spdlog_ex("__android_log_write() failed", ret);
+            throw_spdlog_ex("__android_log_write() failed", ret);
         }
     }
 
     void flush_() override {}
 
 private:
     static android_LogPriority convert_to_android_(spdlog::level::level_enum level)
@@ -102,20 +98,22 @@
 
 using android_sink_mt = android_sink<std::mutex>;
 using android_sink_st = android_sink<details::null_mutex>;
 } // namespace sinks
 
 // Create and register android syslog logger
 
-template<typename Factory = default_factory>
+template<typename Factory = spdlog::synchronous_factory>
 inline std::shared_ptr<logger> android_logger_mt(const std::string &logger_name, const std::string &tag = "spdlog")
 {
     return Factory::template create<sinks::android_sink_mt>(logger_name, tag);
 }
 
-template<typename Factory = default_factory>
+template<typename Factory = spdlog::synchronous_factory>
 inline std::shared_ptr<logger> android_logger_st(const std::string &logger_name, const std::string &tag = "spdlog")
 {
     return Factory::template create<sinks::android_sink_st>(logger_name, tag);
 }
 
 } // namespace spdlog
+
+#endif // __ANDROID__
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/base_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/base_sink-inl.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,63 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
-//
-// base sink templated over a mutex (either dummy or real)
-// concrete implementation should override the sink_it_() and flush_()  methods.
-// locking is taken care of in this class - no locking needed by the
-// implementers..
-//
-
-#include "spdlog/common.h"
-#include "spdlog/details/log_msg.h"
-#include "spdlog/formatter.h"
-#include "spdlog/sinks/sink.h"
-
-namespace spdlog {
-namespace sinks {
-template<typename Mutex>
-class base_sink : public sink
-{
-public:
-    base_sink() = default;
-    base_sink(const base_sink &) = delete;
-    base_sink &operator=(const base_sink &) = delete;
-
-    void log(const details::log_msg &msg) final
-    {
-        std::lock_guard<Mutex> lock(mutex_);
-        sink_it_(msg);
-    }
-
-    void flush() final
-    {
-        std::lock_guard<Mutex> lock(mutex_);
-        flush_();
-    }
-
-    void set_pattern(const std::string &pattern) final
-    {
-        std::lock_guard<Mutex> lock(mutex_);
-        set_pattern_(pattern);
-    }
-
-    void set_formatter(std::unique_ptr<spdlog::formatter> sink_formatter) final
-    {
-        std::lock_guard<Mutex> lock(mutex_);
-        set_formatter_(std::move(sink_formatter));
-    }
-
-protected:
-    virtual void sink_it_(const details::log_msg &msg) = 0;
-    virtual void flush_() = 0;
-
-    virtual void set_pattern_(const std::string &pattern)
-    {
-        set_formatter_(details::make_unique<spdlog::pattern_formatter>(pattern));
-    }
-
-    virtual void set_formatter_(std::unique_ptr<spdlog::formatter> sink_formatter)
-    {
-        formatter_ = std::move(sink_formatter);
-    }
-    Mutex mutex_;
-};
-} // namespace sinks
-} // namespace spdlog
+
+#ifndef SPDLOG_HEADER_ONLY
+#    include <spdlog/sinks/base_sink.h>
+#endif
+
+#include <spdlog/common.h>
+#include <spdlog/pattern_formatter.h>
+
+#include <memory>
+
+template<typename Mutex>
+SPDLOG_INLINE spdlog::sinks::base_sink<Mutex>::base_sink()
+    : formatter_{details::make_unique<spdlog::pattern_formatter>()}
+{}
+
+template<typename Mutex>
+SPDLOG_INLINE spdlog::sinks::base_sink<Mutex>::base_sink(std::unique_ptr<spdlog::formatter> formatter)
+    : formatter_{std::move(formatter)}
+{}
+
+template<typename Mutex>
+void SPDLOG_INLINE spdlog::sinks::base_sink<Mutex>::log(const details::log_msg &msg)
+{
+    std::lock_guard<Mutex> lock(mutex_);
+    sink_it_(msg);
+}
+
+template<typename Mutex>
+void SPDLOG_INLINE spdlog::sinks::base_sink<Mutex>::flush()
+{
+    std::lock_guard<Mutex> lock(mutex_);
+    flush_();
+}
+
+template<typename Mutex>
+void SPDLOG_INLINE spdlog::sinks::base_sink<Mutex>::set_pattern(const std::string &pattern)
+{
+    std::lock_guard<Mutex> lock(mutex_);
+    set_pattern_(pattern);
+}
+
+template<typename Mutex>
+void SPDLOG_INLINE spdlog::sinks::base_sink<Mutex>::set_formatter(std::unique_ptr<spdlog::formatter> sink_formatter)
+{
+    std::lock_guard<Mutex> lock(mutex_);
+    set_formatter_(std::move(sink_formatter));
+}
+
+template<typename Mutex>
+void SPDLOG_INLINE spdlog::sinks::base_sink<Mutex>::set_pattern_(const std::string &pattern)
+{
+    set_formatter_(details::make_unique<spdlog::pattern_formatter>(pattern));
+}
+
+template<typename Mutex>
+void SPDLOG_INLINE spdlog::sinks::base_sink<Mutex>::set_formatter_(std::unique_ptr<spdlog::formatter> sink_formatter)
+{
+    formatter_ = std::move(sink_formatter);
+}
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/basic_file_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/basic_file_sink.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,60 @@
-//
-// Copyright(c) 2015-2018 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
-#endif
-
-#include "spdlog/details/file_helper.h"
-#include "spdlog/details/null_mutex.h"
-#include "spdlog/sinks/base_sink.h"
+#include <spdlog/details/file_helper.h>
+#include <spdlog/details/null_mutex.h>
+#include <spdlog/sinks/base_sink.h>
+#include <spdlog/details/synchronous_factory.h>
 
 #include <mutex>
 #include <string>
 
 namespace spdlog {
 namespace sinks {
 /*
  * Trivial file sink with single file as target
  */
 template<typename Mutex>
 class basic_file_sink final : public base_sink<Mutex>
 {
 public:
-    explicit basic_file_sink(const filename_t &filename, bool truncate = false)
-    {
-        file_helper_.open(filename, truncate);
-    }
+    explicit basic_file_sink(const filename_t &filename, bool truncate = false, const file_event_handlers &event_handlers = {});
+    const filename_t &filename() const;
 
 protected:
-    void sink_it_(const details::log_msg &msg) override
-    {
-        fmt::memory_buffer formatted;
-        sink::formatter_->format(msg, formatted);
-        file_helper_.write(formatted);
-    }
-
-    void flush_() override
-    {
-        file_helper_.flush();
-    }
+    void sink_it_(const details::log_msg &msg) override;
+    void flush_() override;
 
 private:
     details::file_helper file_helper_;
 };
 
 using basic_file_sink_mt = basic_file_sink<std::mutex>;
 using basic_file_sink_st = basic_file_sink<details::null_mutex>;
 
 } // namespace sinks
 
 //
 // factory functions
 //
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> basic_logger_mt(const std::string &logger_name, const filename_t &filename, bool truncate = false)
+template<typename Factory = spdlog::synchronous_factory>
+inline std::shared_ptr<logger> basic_logger_mt(
+    const std::string &logger_name, const filename_t &filename, bool truncate = false, const file_event_handlers &event_handlers = {})
 {
-    return Factory::template create<sinks::basic_file_sink_mt>(logger_name, filename, truncate);
+    return Factory::template create<sinks::basic_file_sink_mt>(logger_name, filename, truncate, event_handlers);
 }
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> basic_logger_st(const std::string &logger_name, const filename_t &filename, bool truncate = false)
+template<typename Factory = spdlog::synchronous_factory>
+inline std::shared_ptr<logger> basic_logger_st(
+    const std::string &logger_name, const filename_t &filename, bool truncate = false, const file_event_handlers &event_handlers = {})
 {
-    return Factory::template create<sinks::basic_file_sink_st>(logger_name, filename, truncate);
+    return Factory::template create<sinks::basic_file_sink_st>(logger_name, filename, truncate, event_handlers);
 }
 
 } // namespace spdlog
+
+#ifdef SPDLOG_HEADER_ONLY
+#    include "basic_file_sink-inl.h"
+#endif
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/dist_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/dist_sink.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-//
-// Copyright (c) 2015 David Schury, Gabi Melman
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
-#endif
-
 #include "base_sink.h"
-#include "spdlog/details/log_msg.h"
-#include "spdlog/details/null_mutex.h"
+#include <spdlog/details/log_msg.h>
+#include <spdlog/details/null_mutex.h>
+#include <spdlog/pattern_formatter.h>
 
 #include <algorithm>
 #include <memory>
 #include <mutex>
 #include <vector>
 
 // Distribution sink (mux). Stores a vector of sinks which get called when log
@@ -25,14 +20,18 @@
 namespace sinks {
 
 template<typename Mutex>
 class dist_sink : public base_sink<Mutex>
 {
 public:
     dist_sink() = default;
+    explicit dist_sink(std::vector<std::shared_ptr<sink>> sinks)
+        : sinks_(sinks)
+    {}
+
     dist_sink(const dist_sink &) = delete;
     dist_sink &operator=(const dist_sink &) = delete;
 
     void add_sink(std::shared_ptr<sink> sink)
     {
         std::lock_guard<Mutex> lock(base_sink<Mutex>::mutex_);
         sinks_.push_back(sink);
@@ -46,18 +45,22 @@
 
     void set_sinks(std::vector<std::shared_ptr<sink>> sinks)
     {
         std::lock_guard<Mutex> lock(base_sink<Mutex>::mutex_);
         sinks_ = std::move(sinks);
     }
 
+    std::vector<std::shared_ptr<sink>> &sinks()
+    {
+        return sinks_;
+    }
+
 protected:
     void sink_it_(const details::log_msg &msg) override
     {
-
         for (auto &sink : sinks_)
         {
             if (sink->should_log(msg.level))
             {
                 sink->log(msg);
             }
         }
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/msvc_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/msvc_sink.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-//
 // Copyright(c) 2016 Alexander Dalshov.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
-#endif
-
 #if defined(_WIN32)
 
-#include "spdlog/details/null_mutex.h"
-#include "spdlog/sinks/base_sink.h"
+#    include <spdlog/details/null_mutex.h>
+#    include <spdlog/sinks/base_sink.h>
 
-#include <winbase.h>
+#    include <mutex>
+#    include <string>
 
-#include <mutex>
-#include <string>
+// Avoid including windows.h (https://stackoverflow.com/a/30741042)
+extern "C" __declspec(dllimport) void __stdcall OutputDebugStringA(const char *lpOutputString);
 
 namespace spdlog {
 namespace sinks {
 /*
  * MSVC sink (logging using OutputDebugStringA)
  */
 template<typename Mutex>
 class msvc_sink : public base_sink<Mutex>
 {
 public:
-    explicit msvc_sink() {}
+    msvc_sink() = default;
 
 protected:
     void sink_it_(const details::log_msg &msg) override
     {
-
-        fmt::memory_buffer formatted;
-        sink::formatter_->format(msg, formatted);
+        memory_buf_t formatted;
+        base_sink<Mutex>::formatter_->format(msg, formatted);
+#    ifdef SPDLOG_USE_STD_FORMAT
+        OutputDebugStringA(formatted.c_str());
+#    else
         OutputDebugStringA(fmt::to_string(formatted).c_str());
+#    endif
     }
 
     void flush_() override {}
 };
 
 using msvc_sink_mt = msvc_sink<std::mutex>;
 using msvc_sink_st = msvc_sink<details::null_mutex>;
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/null_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/null_sink.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
-#endif
-
-#include "spdlog/details/null_mutex.h"
-#include "spdlog/sinks/base_sink.h"
+#include <spdlog/details/null_mutex.h>
+#include <spdlog/sinks/base_sink.h>
+#include <spdlog/details/synchronous_factory.h>
 
 #include <mutex>
 
 namespace spdlog {
 namespace sinks {
 
 template<typename Mutex>
 class null_sink : public base_sink<Mutex>
 {
 protected:
     void sink_it_(const details::log_msg &) override {}
     void flush_() override {}
 };
 
-using null_sink_mt = null_sink<std::mutex>;
+using null_sink_mt = null_sink<details::null_mutex>;
 using null_sink_st = null_sink<details::null_mutex>;
 
 } // namespace sinks
 
-template<typename Factory = default_factory>
+template<typename Factory = spdlog::synchronous_factory>
 inline std::shared_ptr<logger> null_logger_mt(const std::string &logger_name)
 {
     auto null_logger = Factory::template create<sinks::null_sink_mt>(logger_name);
     null_logger->set_level(level::off);
     return null_logger;
 }
 
-template<typename Factory = default_factory>
+template<typename Factory = spdlog::synchronous_factory>
 inline std::shared_ptr<logger> null_logger_st(const std::string &logger_name)
 {
     auto null_logger = Factory::template create<sinks::null_sink_st>(logger_name);
     null_logger->set_level(level::off);
     return null_logger;
 }
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/ostream_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/ostream_sink.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,36 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
-#endif
-
-#include "spdlog/details/null_mutex.h"
-#include "spdlog/sinks/base_sink.h"
+#include <spdlog/details/null_mutex.h>
+#include <spdlog/sinks/base_sink.h>
 
 #include <mutex>
 #include <ostream>
 
 namespace spdlog {
 namespace sinks {
 template<typename Mutex>
 class ostream_sink final : public base_sink<Mutex>
 {
 public:
     explicit ostream_sink(std::ostream &os, bool force_flush = false)
         : ostream_(os)
         , force_flush_(force_flush)
-    {
-    }
+    {}
     ostream_sink(const ostream_sink &) = delete;
     ostream_sink &operator=(const ostream_sink &) = delete;
 
 protected:
     void sink_it_(const details::log_msg &msg) override
     {
-        fmt::memory_buffer formatted;
-        sink::formatter_->format(msg, formatted);
+        memory_buf_t formatted;
+        base_sink<Mutex>::formatter_->format(msg, formatted);
         ostream_.write(formatted.data(), static_cast<std::streamsize>(formatted.size()));
         if (force_flush_)
         {
             ostream_.flush();
         }
     }
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/rotating_file_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/rotating_file_sink-inl.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,155 +1,152 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
+#ifndef SPDLOG_HEADER_ONLY
+#    include <spdlog/sinks/rotating_file_sink.h>
 #endif
 
-#include "spdlog/details/file_helper.h"
-#include "spdlog/details/null_mutex.h"
-#include "spdlog/fmt/fmt.h"
-#include "spdlog/sinks/base_sink.h"
+#include <spdlog/common.h>
+
+#include <spdlog/details/file_helper.h>
+#include <spdlog/details/null_mutex.h>
+#include <spdlog/fmt/fmt.h>
 
 #include <cerrno>
 #include <chrono>
 #include <ctime>
 #include <mutex>
 #include <string>
 #include <tuple>
 
 namespace spdlog {
 namespace sinks {
 
-//
-// Rotating file sink based on size
-//
 template<typename Mutex>
-class rotating_file_sink final : public base_sink<Mutex>
+SPDLOG_INLINE rotating_file_sink<Mutex>::rotating_file_sink(
+    filename_t base_filename, std::size_t max_size, std::size_t max_files, bool rotate_on_open, const file_event_handlers &event_handlers)
+    : base_filename_(std::move(base_filename))
+    , max_size_(max_size)
+    , max_files_(max_files)
+    , file_helper_{event_handlers}
 {
-public:
-    rotating_file_sink(filename_t base_filename, std::size_t max_size, std::size_t max_files)
-        : base_filename_(std::move(base_filename))
-        , max_size_(max_size)
-        , max_files_(max_files)
+    if (max_size == 0)
     {
-        file_helper_.open(calc_filename(base_filename_, 0));
-        current_size_ = file_helper_.size(); // expensive. called only once
+        throw_spdlog_ex("rotating sink constructor: max_size arg cannot be zero");
     }
 
-    // calc filename according to index and file extension if exists.
-    // e.g. calc_filename("logs/mylog.txt, 3) => "logs/mylog.3.txt".
-    static filename_t calc_filename(const filename_t &filename, std::size_t index)
+    if (max_files > 200000)
     {
-        typename std::conditional<std::is_same<filename_t::value_type, char>::value, fmt::memory_buffer, fmt::wmemory_buffer>::type w;
-        if (index != 0u)
-        {
-            filename_t basename, ext;
-            std::tie(basename, ext) = details::file_helper::split_by_extension(filename);
-            fmt::format_to(w, SPDLOG_FILENAME_T("{}.{}{}"), basename, index, ext);
-        }
-        else
-        {
-            fmt::format_to(w, SPDLOG_FILENAME_T("{}"), filename);
-        }
-        return fmt::to_string(w);
+        throw_spdlog_ex("rotating sink constructor: max_files arg cannot exceed 200000");
     }
-
-protected:
-    void sink_it_(const details::log_msg &msg) override
+    file_helper_.open(calc_filename(base_filename_, 0));
+    current_size_ = file_helper_.size(); // expensive. called only once
+    if (rotate_on_open && current_size_ > 0)
     {
-        fmt::memory_buffer formatted;
-        sink::formatter_->format(msg, formatted);
-        current_size_ += formatted.size();
-        if (current_size_ > max_size_)
-        {
-            rotate_();
-            current_size_ = formatted.size();
-        }
-        file_helper_.write(formatted);
+        rotate_();
+        current_size_ = 0;
     }
+}
 
-    void flush_() override
+// calc filename according to index and file extension if exists.
+// e.g. calc_filename("logs/mylog.txt, 3) => "logs/mylog.3.txt".
+template<typename Mutex>
+SPDLOG_INLINE filename_t rotating_file_sink<Mutex>::calc_filename(const filename_t &filename, std::size_t index)
+{
+    if (index == 0u)
     {
-        file_helper_.flush();
+        return filename;
     }
 
-private:
-    // Rotate files:
-    // log.txt -> log.1.txt
-    // log.1.txt -> log.2.txt
-    // log.2.txt -> log.3.txt
-    // log.3.txt -> delete
-    void rotate_()
-    {
-        using details::os::filename_to_str;
-        file_helper_.close();
-        for (auto i = max_files_; i > 0; --i)
-        {
-            filename_t src = calc_filename(base_filename_, i - 1);
-            if (!details::file_helper::file_exists(src))
-            {
-                continue;
-            }
-            filename_t target = calc_filename(base_filename_, i);
+    filename_t basename, ext;
+    std::tie(basename, ext) = details::file_helper::split_by_extension(filename);
+    return fmt_lib::format(SPDLOG_FILENAME_T("{}.{}{}"), basename, index, ext);
+}
 
-            if (!rename_file(src, target))
-            {
-                // if failed try again after a small delay.
-                // this is a workaround to a windows issue, where very high rotation
-                // rates can cause the rename to fail with permission denied (because of antivirus?).
-                details::os::sleep_for_millis(100);
-                if (!rename_file(src, target))
-                {
-                    file_helper_.reopen(true); // truncate the log file anyway to prevent it to grow beyond its limit!
-                    current_size_ = 0;
-                    throw spdlog_ex(
-                        "rotating_file_sink: failed renaming " + filename_to_str(src) + " to " + filename_to_str(target), errno);
-                }
-            }
-        }
-        file_helper_.reopen(true);
-    }
+template<typename Mutex>
+SPDLOG_INLINE filename_t rotating_file_sink<Mutex>::filename()
+{
+    std::lock_guard<Mutex> lock(base_sink<Mutex>::mutex_);
+    return file_helper_.filename();
+}
 
-    // delete the target if exists, and rename the src file  to target
-    // return true on success, false otherwise.
-    bool rename_file(const filename_t &src_filename, const filename_t &target_filename)
+template<typename Mutex>
+SPDLOG_INLINE void rotating_file_sink<Mutex>::sink_it_(const details::log_msg &msg)
+{
+    memory_buf_t formatted;
+    base_sink<Mutex>::formatter_->format(msg, formatted);
+    auto new_size = current_size_ + formatted.size();
+
+    // rotate if the new estimated file size exceeds max size.
+    // rotate only if the real size > 0 to better deal with full disk (see issue #2261).
+    // we only check the real size when new_size > max_size_ because it is relatively expensive.
+    if (new_size > max_size_)
     {
-        // try to delete the target file in case it already exists.
-        (void)details::os::remove(target_filename);
-        return details::os::rename(src_filename, target_filename) == 0;
+        file_helper_.flush();
+        if (file_helper_.size() > 0)
+        {
+            rotate_();
+            new_size = formatted.size();
+        }
     }
+    file_helper_.write(formatted);
+    current_size_ = new_size;
+}
 
-    filename_t base_filename_;
-    std::size_t max_size_;
-    std::size_t max_files_;
-    std::size_t current_size_;
-    details::file_helper file_helper_;
-};
-
-using rotating_file_sink_mt = rotating_file_sink<std::mutex>;
-using rotating_file_sink_st = rotating_file_sink<details::null_mutex>;
+template<typename Mutex>
+SPDLOG_INLINE void rotating_file_sink<Mutex>::flush_()
+{
+    file_helper_.flush();
+}
 
-} // namespace sinks
+// Rotate files:
+// log.txt -> log.1.txt
+// log.1.txt -> log.2.txt
+// log.2.txt -> log.3.txt
+// log.3.txt -> delete
+template<typename Mutex>
+SPDLOG_INLINE void rotating_file_sink<Mutex>::rotate_()
+{
+    using details::os::filename_to_str;
+    using details::os::path_exists;
 
-//
-// factory functions
-//
+    file_helper_.close();
+    for (auto i = max_files_; i > 0; --i)
+    {
+        filename_t src = calc_filename(base_filename_, i - 1);
+        if (!path_exists(src))
+        {
+            continue;
+        }
+        filename_t target = calc_filename(base_filename_, i);
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> rotating_logger_mt(
-    const std::string &logger_name, const filename_t &filename, size_t max_file_size, size_t max_files)
-{
-    return Factory::template create<sinks::rotating_file_sink_mt>(logger_name, filename, max_file_size, max_files);
+        if (!rename_file_(src, target))
+        {
+            // if failed try again after a small delay.
+            // this is a workaround to a windows issue, where very high rotation
+            // rates can cause the rename to fail with permission denied (because of antivirus?).
+            details::os::sleep_for_millis(100);
+            if (!rename_file_(src, target))
+            {
+                file_helper_.reopen(true); // truncate the log file anyway to prevent it to grow beyond its limit!
+                current_size_ = 0;
+                throw_spdlog_ex("rotating_file_sink: failed renaming " + filename_to_str(src) + " to " + filename_to_str(target), errno);
+            }
+        }
+    }
+    file_helper_.reopen(true);
 }
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> rotating_logger_st(
-    const std::string &logger_name, const filename_t &filename, size_t max_file_size, size_t max_files)
+// delete the target if exists, and rename the src file  to target
+// return true on success, false otherwise.
+template<typename Mutex>
+SPDLOG_INLINE bool rotating_file_sink<Mutex>::rename_file_(const filename_t &src_filename, const filename_t &target_filename)
 {
-    return Factory::template create<sinks::rotating_file_sink_st>(logger_name, filename, max_file_size, max_files);
+    // try to delete the target file in case it already exists.
+    (void)details::os::remove(target_filename);
+    return details::os::rename(src_filename, target_filename) == 0;
 }
+
+} // namespace sinks
 } // namespace spdlog
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/stdout_color_sinks.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/stdout_color_sinks-inl.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,38 @@
-//
-// Copyright(c) 2018 spdlog
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
+#ifndef SPDLOG_HEADER_ONLY
+#    include <spdlog/sinks/stdout_color_sinks.h>
 #endif
 
-#ifdef _WIN32
-#include "spdlog/sinks/wincolor_sink.h"
-#else
-#include "spdlog/sinks/ansicolor_sink.h"
-#endif
+#include <spdlog/logger.h>
+#include <spdlog/common.h>
 
 namespace spdlog {
-namespace sinks {
-#ifdef _WIN32
-using stdout_color_sink_mt = wincolor_stdout_sink_mt;
-using stdout_color_sink_st = wincolor_stdout_sink_st;
-using stderr_color_sink_mt = wincolor_stderr_sink_mt;
-using stderr_color_sink_st = wincolor_stderr_sink_st;
-#else
-using stdout_color_sink_mt = ansicolor_stdout_sink_mt;
-using stdout_color_sink_st = ansicolor_stdout_sink_st;
-using stderr_color_sink_mt = ansicolor_stderr_sink_mt;
-using stderr_color_sink_st = ansicolor_stderr_sink_st;
-#endif
-} // namespace sinks
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> stdout_color_mt(const std::string &logger_name)
+template<typename Factory>
+SPDLOG_INLINE std::shared_ptr<logger> stdout_color_mt(const std::string &logger_name, color_mode mode)
 {
-    return Factory::template create<sinks::stdout_color_sink_mt>(logger_name);
+    return Factory::template create<sinks::stdout_color_sink_mt>(logger_name, mode);
 }
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> stdout_color_st(const std::string &logger_name)
+template<typename Factory>
+SPDLOG_INLINE std::shared_ptr<logger> stdout_color_st(const std::string &logger_name, color_mode mode)
 {
-    return Factory::template create<sinks::stdout_color_sink_st>(logger_name);
+    return Factory::template create<sinks::stdout_color_sink_st>(logger_name, mode);
 }
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> stderr_color_mt(const std::string &logger_name)
+template<typename Factory>
+SPDLOG_INLINE std::shared_ptr<logger> stderr_color_mt(const std::string &logger_name, color_mode mode)
 {
-    return Factory::template create<sinks::stderr_color_sink_mt>(logger_name);
+    return Factory::template create<sinks::stderr_color_sink_mt>(logger_name, mode);
 }
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> stderr_color_st(const std::string &logger_name)
+template<typename Factory>
+SPDLOG_INLINE std::shared_ptr<logger> stderr_color_st(const std::string &logger_name, color_mode mode)
 {
-    return Factory::template create<sinks::stderr_color_sink_mt>(logger_name);
+    return Factory::template create<sinks::stderr_color_sink_st>(logger_name, mode);
 }
 } // namespace spdlog
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/stdout_sinks.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/stdout_sinks.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,87 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
-#endif
-
-#include "spdlog/details/console_globals.h"
-#include "spdlog/details/null_mutex.h"
-
+#include <spdlog/details/console_globals.h>
+#include <spdlog/details/synchronous_factory.h>
+#include <spdlog/sinks/sink.h>
 #include <cstdio>
-#include <memory>
-#include <mutex>
+
+#ifdef _WIN32
+#    include <spdlog/details/windows_include.h>
+#endif
 
 namespace spdlog {
 
 namespace sinks {
 
-template<typename TargetStream, typename ConsoleMutex>
-class stdout_sink final : public sink
+template<typename ConsoleMutex>
+class stdout_sink_base : public sink
 {
 public:
     using mutex_t = typename ConsoleMutex::mutex_t;
-    stdout_sink()
-        : mutex_(ConsoleMutex::mutex())
-        , file_(TargetStream::stream())
-    {
-    }
-    ~stdout_sink() override = default;
-
-    stdout_sink(const stdout_sink &other) = delete;
-    stdout_sink &operator=(const stdout_sink &other) = delete;
-
-    void log(const details::log_msg &msg) override
-    {
-        std::lock_guard<mutex_t> lock(mutex_);
-        fmt::memory_buffer formatted;
-        formatter_->format(msg, formatted);
-        fwrite(formatted.data(), sizeof(char), formatted.size(), file_);
-        fflush(TargetStream::stream());
-    }
-
-    void flush() override
-    {
-        std::lock_guard<mutex_t> lock(mutex_);
-        fflush(file_);
-    }
-
-    void set_pattern(const std::string &pattern) override
-    {
-        std::lock_guard<mutex_t> lock(mutex_);
-        formatter_ = std::unique_ptr<spdlog::formatter>(new pattern_formatter(pattern));
-    }
-
-    void set_formatter(std::unique_ptr<spdlog::formatter> sink_formatter) override
-    {
-        std::lock_guard<mutex_t> lock(mutex_);
-        formatter_ = std::move(sink_formatter);
-    }
+    explicit stdout_sink_base(FILE *file);
+    ~stdout_sink_base() override = default;
+
+    stdout_sink_base(const stdout_sink_base &other) = delete;
+    stdout_sink_base(stdout_sink_base &&other) = delete;
 
-private:
+    stdout_sink_base &operator=(const stdout_sink_base &other) = delete;
+    stdout_sink_base &operator=(stdout_sink_base &&other) = delete;
+
+    void log(const details::log_msg &msg) override;
+    void flush() override;
+    void set_pattern(const std::string &pattern) override;
+
+    void set_formatter(std::unique_ptr<spdlog::formatter> sink_formatter) override;
+
+protected:
     mutex_t &mutex_;
     FILE *file_;
+    std::unique_ptr<spdlog::formatter> formatter_;
+#ifdef _WIN32
+    HANDLE handle_;
+#endif // WIN32
+};
+
+template<typename ConsoleMutex>
+class stdout_sink : public stdout_sink_base<ConsoleMutex>
+{
+public:
+    stdout_sink();
+};
+
+template<typename ConsoleMutex>
+class stderr_sink : public stdout_sink_base<ConsoleMutex>
+{
+public:
+    stderr_sink();
 };
 
-using stdout_sink_mt = stdout_sink<details::console_stdout, details::console_mutex>;
-using stdout_sink_st = stdout_sink<details::console_stdout, details::console_nullmutex>;
+using stdout_sink_mt = stdout_sink<details::console_mutex>;
+using stdout_sink_st = stdout_sink<details::console_nullmutex>;
 
-using stderr_sink_mt = stdout_sink<details::console_stderr, details::console_mutex>;
-using stderr_sink_st = stdout_sink<details::console_stderr, details::console_nullmutex>;
+using stderr_sink_mt = stderr_sink<details::console_mutex>;
+using stderr_sink_st = stderr_sink<details::console_nullmutex>;
 
 } // namespace sinks
 
 // factory methods
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> stdout_logger_mt(const std::string &logger_name)
-{
-    return Factory::template create<sinks::stdout_sink_mt>(logger_name);
-}
+template<typename Factory = spdlog::synchronous_factory>
+std::shared_ptr<logger> stdout_logger_mt(const std::string &logger_name);
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> stdout_logger_st(const std::string &logger_name)
-{
-    return Factory::template create<sinks::stdout_sink_st>(logger_name);
-}
+template<typename Factory = spdlog::synchronous_factory>
+std::shared_ptr<logger> stdout_logger_st(const std::string &logger_name);
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> stderr_logger_mt(const std::string &logger_name)
-{
-    return Factory::template create<sinks::stderr_sink_mt>(logger_name);
-}
+template<typename Factory = spdlog::synchronous_factory>
+std::shared_ptr<logger> stderr_logger_mt(const std::string &logger_name);
+
+template<typename Factory = spdlog::synchronous_factory>
+std::shared_ptr<logger> stderr_logger_st(const std::string &logger_name);
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> stderr_logger_st(const std::string &logger_name)
-{
-    return Factory::template create<sinks::stderr_sink_st>(logger_name);
-}
 } // namespace spdlog
+
+#ifdef SPDLOG_HEADER_ONLY
+#    include "stdout_sinks-inl.h"
+#endif
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/syslog_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/syslog_sink.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
-#endif
-
-#include "spdlog/sinks/base_sink.h"
+#include <spdlog/sinks/base_sink.h>
+#include <spdlog/details/null_mutex.h>
+#include <spdlog/details/synchronous_factory.h>
 
 #include <array>
 #include <string>
 #include <syslog.h>
 
 namespace spdlog {
 namespace sinks {
 /**
  * Sink that write to syslog using the `syscall()` library call.
- *
- * Locking is not needed, as `syslog()` itself is thread-safe.
  */
 template<typename Mutex>
 class syslog_sink : public base_sink<Mutex>
 {
+
 public:
-    //
-    explicit syslog_sink(std::string ident = "", int syslog_option = 0, int syslog_facility = LOG_USER)
-        : ident_(std::move(ident))
+    syslog_sink(std::string ident, int syslog_option, int syslog_facility, bool enable_formatting)
+        : enable_formatting_{enable_formatting}
+        , syslog_levels_{{/* spdlog::level::trace      */ LOG_DEBUG,
+              /* spdlog::level::debug      */ LOG_DEBUG,
+              /* spdlog::level::info       */ LOG_INFO,
+              /* spdlog::level::warn       */ LOG_WARNING,
+              /* spdlog::level::err        */ LOG_ERR,
+              /* spdlog::level::critical   */ LOG_CRIT,
+              /* spdlog::level::off        */ LOG_INFO}}
+        , ident_{std::move(ident)}
     {
-        priorities_[static_cast<size_t>(level::trace)] = LOG_DEBUG;
-        priorities_[static_cast<size_t>(level::debug)] = LOG_DEBUG;
-        priorities_[static_cast<size_t>(level::info)] = LOG_INFO;
-        priorities_[static_cast<size_t>(level::warn)] = LOG_WARNING;
-        priorities_[static_cast<size_t>(level::err)] = LOG_ERR;
-        priorities_[static_cast<size_t>(level::critical)] = LOG_CRIT;
-        priorities_[static_cast<size_t>(level::off)] = LOG_INFO;
-
         // set ident to be program name if empty
         ::openlog(ident_.empty() ? nullptr : ident_.c_str(), syslog_option, syslog_facility);
     }
 
     ~syslog_sink() override
     {
         ::closelog();
@@ -49,46 +43,67 @@
 
     syslog_sink(const syslog_sink &) = delete;
     syslog_sink &operator=(const syslog_sink &) = delete;
 
 protected:
     void sink_it_(const details::log_msg &msg) override
     {
-        ::syslog(syslog_prio_from_level(msg), "%s", fmt::to_string(msg.payload).c_str());
+        string_view_t payload;
+        memory_buf_t formatted;
+        if (enable_formatting_)
+        {
+            base_sink<Mutex>::formatter_->format(msg, formatted);
+            payload = string_view_t(formatted.data(), formatted.size());
+        }
+        else
+        {
+            payload = msg.payload;
+        }
+
+        size_t length = payload.size();
+        // limit to max int
+        if (length > static_cast<size_t>(std::numeric_limits<int>::max()))
+        {
+            length = static_cast<size_t>(std::numeric_limits<int>::max());
+        }
+
+        ::syslog(syslog_prio_from_level(msg), "%.*s", static_cast<int>(length), payload.data());
     }
 
     void flush_() override {}
+    bool enable_formatting_ = false;
 
 private:
-    std::array<int, 7> priorities_;
+    using levels_array = std::array<int, 7>;
+    levels_array syslog_levels_;
     // must store the ident because the man says openlog might use the pointer as
     // is and not a string copy
     const std::string ident_;
 
     //
     // Simply maps spdlog's log level to syslog priority level.
     //
     int syslog_prio_from_level(const details::log_msg &msg) const
     {
-        return priorities_[static_cast<size_t>(msg.level)];
+        return syslog_levels_.at(static_cast<levels_array::size_type>(msg.level));
     }
 };
 
 using syslog_sink_mt = syslog_sink<std::mutex>;
 using syslog_sink_st = syslog_sink<details::null_mutex>;
 } // namespace sinks
 
 // Create and register a syslog logger
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> syslog_logger_mt(
-    const std::string &logger_name, const std::string &syslog_ident = "", int syslog_option = 0, int syslog_facility = (1 << 3))
+template<typename Factory = spdlog::synchronous_factory>
+inline std::shared_ptr<logger> syslog_logger_mt(const std::string &logger_name, const std::string &syslog_ident = "", int syslog_option = 0,
+    int syslog_facility = LOG_USER, bool enable_formatting = false)
 {
-    return Factory::template create<sinks::syslog_sink_mt>(logger_name, syslog_ident, syslog_option, syslog_facility);
+    return Factory::template create<sinks::syslog_sink_mt>(logger_name, syslog_ident, syslog_option, syslog_facility, enable_formatting);
 }
 
-template<typename Factory = default_factory>
-inline std::shared_ptr<logger> syslog_logger_st(
-    const std::string &logger_name, const std::string &syslog_ident = "", int syslog_option = 0, int syslog_facility = (1 << 3))
+template<typename Factory = spdlog::synchronous_factory>
+inline std::shared_ptr<logger> syslog_logger_st(const std::string &logger_name, const std::string &syslog_ident = "", int syslog_option = 0,
+    int syslog_facility = LOG_USER, bool enable_formatting = false)
 {
-    return Factory::template create<sinks::syslog_sink_st>(logger_name, syslog_ident, syslog_option, syslog_facility);
+    return Factory::template create<sinks::syslog_sink_st>(logger_name, syslog_ident, syslog_option, syslog_facility, enable_formatting);
 }
 } // namespace spdlog
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/sinks/wincolor_sink.h` & `spdlog-2.0.6/spdlog/include/spdlog/sinks/wincolor_sink-inl.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,175 @@
-//
-// Copyright(c) 2016 spdlog
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
-#ifndef SPDLOG_H
-#include "spdlog/spdlog.h"
+#ifndef SPDLOG_HEADER_ONLY
+#    include <spdlog/sinks/wincolor_sink.h>
 #endif
 
-#include "spdlog/common.h"
-#include "spdlog/details/console_globals.h"
-#include "spdlog/details/null_mutex.h"
-#include "spdlog/sinks/sink.h"
-
-#include <memory>
-#include <mutex>
-#include <string>
-#include <unordered_map>
+#include <spdlog/details/windows_include.h>
 #include <wincon.h>
 
+#include <spdlog/common.h>
+#include <spdlog/pattern_formatter.h>
+
 namespace spdlog {
 namespace sinks {
-/*
- * Windows color console sink. Uses WriteConsoleA to write to the console with
- * colors
- */
-template<typename OutHandle, typename ConsoleMutex>
-class wincolor_sink : public sink
+template<typename ConsoleMutex>
+SPDLOG_INLINE wincolor_sink<ConsoleMutex>::wincolor_sink(void *out_handle, color_mode mode)
+    : out_handle_(out_handle)
+    , mutex_(ConsoleMutex::mutex())
+    , formatter_(details::make_unique<spdlog::pattern_formatter>())
 {
-public:
-    const WORD BOLD = FOREGROUND_INTENSITY;
-    const WORD RED = FOREGROUND_RED;
-    const WORD GREEN = FOREGROUND_GREEN;
-    const WORD CYAN = FOREGROUND_GREEN | FOREGROUND_BLUE;
-    const WORD WHITE = FOREGROUND_RED | FOREGROUND_GREEN | FOREGROUND_BLUE;
-    const WORD YELLOW = FOREGROUND_RED | FOREGROUND_GREEN;
 
-    wincolor_sink()
-        : out_handle_(OutHandle::handle())
-        , mutex_(ConsoleMutex::mutex())
-    {
-        colors_[level::trace] = WHITE;
-        colors_[level::debug] = CYAN;
-        colors_[level::info] = GREEN;
-        colors_[level::warn] = YELLOW | BOLD;
-        colors_[level::err] = RED | BOLD;                         // red bold
-        colors_[level::critical] = BACKGROUND_RED | WHITE | BOLD; // white bold on red background
-        colors_[level::off] = 0;
-    }
+    set_color_mode_impl(mode);
+    // set level colors
+    colors_[level::trace] = FOREGROUND_RED | FOREGROUND_GREEN | FOREGROUND_BLUE;     // white
+    colors_[level::debug] = FOREGROUND_GREEN | FOREGROUND_BLUE;                      // cyan
+    colors_[level::info] = FOREGROUND_GREEN;                                         // green
+    colors_[level::warn] = FOREGROUND_RED | FOREGROUND_GREEN | FOREGROUND_INTENSITY; // intense yellow
+    colors_[level::err] = FOREGROUND_RED | FOREGROUND_INTENSITY;                     // intense red
+    colors_[level::critical] =
+        BACKGROUND_RED | FOREGROUND_RED | FOREGROUND_GREEN | FOREGROUND_BLUE | FOREGROUND_INTENSITY; // intense white on red background
+    colors_[level::off] = 0;
+}
 
-    ~wincolor_sink() override
-    {
-        this->flush();
-    }
+template<typename ConsoleMutex>
+SPDLOG_INLINE wincolor_sink<ConsoleMutex>::~wincolor_sink()
+{
+    this->flush();
+}
 
-    wincolor_sink(const wincolor_sink &other) = delete;
-    wincolor_sink &operator=(const wincolor_sink &other) = delete;
+// change the color for the given level
+template<typename ConsoleMutex>
+void SPDLOG_INLINE wincolor_sink<ConsoleMutex>::set_color(level::level_enum level, std::uint16_t color)
+{
+    std::lock_guard<mutex_t> lock(mutex_);
+    colors_[level] = color;
+}
 
-    // change the color for the given level
-    void set_color(level::level_enum level, WORD color)
+template<typename ConsoleMutex>
+void SPDLOG_INLINE wincolor_sink<ConsoleMutex>::log(const details::log_msg &msg)
+{
+    if (out_handle_ == nullptr || out_handle_ == INVALID_HANDLE_VALUE)
     {
-        std::lock_guard<mutex_t> lock(mutex_);
-        colors_[level] = color;
+        return;
     }
 
-    void log(const details::log_msg &msg) final override
+    std::lock_guard<mutex_t> lock(mutex_);
+    msg.color_range_start = 0;
+    msg.color_range_end = 0;
+    memory_buf_t formatted;
+    formatter_->format(msg, formatted);
+    if (should_do_colors_ && msg.color_range_end > msg.color_range_start)
     {
-        std::lock_guard<mutex_t> lock(mutex_);
-        fmt::memory_buffer formatted;
-        formatter_->format(msg, formatted);
-        if (msg.color_range_end > msg.color_range_start)
-        {
-            // before color range
-            print_range_(formatted, 0, msg.color_range_start);
-
-            // in color range
-            auto orig_attribs = set_console_attribs(colors_[msg.level]);
-            print_range_(formatted, msg.color_range_start, msg.color_range_end);
-            ::SetConsoleTextAttribute(out_handle_,
-                orig_attribs); // reset to orig colors
-                               // after color range
-            print_range_(formatted, msg.color_range_end, formatted.size());
-        }
-        else // print without colors if color range is invalid
-        {
-            print_range_(formatted, 0, formatted.size());
-        }
+        // before color range
+        print_range_(formatted, 0, msg.color_range_start);
+        // in color range
+        auto orig_attribs = static_cast<WORD>(set_foreground_color_(colors_[msg.level]));
+        print_range_(formatted, msg.color_range_start, msg.color_range_end);
+        // reset to orig colors
+        ::SetConsoleTextAttribute(static_cast<HANDLE>(out_handle_), orig_attribs);
+        print_range_(formatted, msg.color_range_end, formatted.size());
     }
-
-    void flush() final override
+    else // print without colors if color range is invalid (or color is disabled)
     {
-        // windows console always flushed?
+        write_to_file_(formatted);
     }
+}
+
+template<typename ConsoleMutex>
+void SPDLOG_INLINE wincolor_sink<ConsoleMutex>::flush()
+{
+    // windows console always flushed?
+}
+
+template<typename ConsoleMutex>
+void SPDLOG_INLINE wincolor_sink<ConsoleMutex>::set_pattern(const std::string &pattern)
+{
+    std::lock_guard<mutex_t> lock(mutex_);
+    formatter_ = std::unique_ptr<spdlog::formatter>(new pattern_formatter(pattern));
+}
+
+template<typename ConsoleMutex>
+void SPDLOG_INLINE wincolor_sink<ConsoleMutex>::set_formatter(std::unique_ptr<spdlog::formatter> sink_formatter)
+{
+    std::lock_guard<mutex_t> lock(mutex_);
+    formatter_ = std::move(sink_formatter);
+}
 
-    void set_pattern(const std::string &pattern) override final
+template<typename ConsoleMutex>
+void SPDLOG_INLINE wincolor_sink<ConsoleMutex>::set_color_mode(color_mode mode)
+{
+    std::lock_guard<mutex_t> lock(mutex_);
+    set_color_mode_impl(mode);
+}
+
+template<typename ConsoleMutex>
+void SPDLOG_INLINE wincolor_sink<ConsoleMutex>::set_color_mode_impl(color_mode mode)
+{
+    if (mode == color_mode::automatic)
     {
-        std::lock_guard<mutex_t> lock(mutex_);
-        formatter_ = std::unique_ptr<spdlog::formatter>(new pattern_formatter(pattern));
+        // should do colors only if out_handle_  points to actual console.
+        DWORD console_mode;
+        bool in_console = ::GetConsoleMode(static_cast<HANDLE>(out_handle_), &console_mode) != 0;
+        should_do_colors_ = in_console;
     }
-
-    void set_formatter(std::unique_ptr<spdlog::formatter> sink_formatter) override final
+    else
     {
-        std::lock_guard<mutex_t> lock(mutex_);
-        formatter_ = std::move(sink_formatter);
+        should_do_colors_ = mode == color_mode::always ? true : false;
     }
+}
 
-private:
-    using mutex_t = typename ConsoleMutex::mutex_t;
-    // set color and return the orig console attributes (for resetting later)
-    WORD set_console_attribs(WORD attribs)
+// set foreground color and return the orig console attributes (for resetting later)
+template<typename ConsoleMutex>
+std::uint16_t SPDLOG_INLINE wincolor_sink<ConsoleMutex>::set_foreground_color_(std::uint16_t attribs)
+{
+    CONSOLE_SCREEN_BUFFER_INFO orig_buffer_info;
+    if (!::GetConsoleScreenBufferInfo(static_cast<HANDLE>(out_handle_), &orig_buffer_info))
     {
-        CONSOLE_SCREEN_BUFFER_INFO orig_buffer_info;
-        ::GetConsoleScreenBufferInfo(out_handle_, &orig_buffer_info);
-        WORD back_color = orig_buffer_info.wAttributes;
-        // retrieve the current background color
-        back_color &= static_cast<WORD>(~(FOREGROUND_RED | FOREGROUND_GREEN | FOREGROUND_BLUE | FOREGROUND_INTENSITY));
-        // keep the background color unchanged
-        ::SetConsoleTextAttribute(out_handle_, attribs | back_color);
-        return orig_buffer_info.wAttributes; // return orig attribs
+        // just return white if failed getting console info
+        return FOREGROUND_RED | FOREGROUND_GREEN | FOREGROUND_BLUE;
     }
 
-    // print a range of formatted message to console
-    void print_range_(const fmt::memory_buffer &formatted, size_t start, size_t end)
+    // change only the foreground bits (lowest 4 bits)
+    auto new_attribs = static_cast<WORD>(attribs) | (orig_buffer_info.wAttributes & 0xfff0);
+    auto ignored = ::SetConsoleTextAttribute(static_cast<HANDLE>(out_handle_), static_cast<WORD>(new_attribs));
+    (void)(ignored);
+    return static_cast<std::uint16_t>(orig_buffer_info.wAttributes); // return orig attribs
+}
+
+// print a range of formatted message to console
+template<typename ConsoleMutex>
+void SPDLOG_INLINE wincolor_sink<ConsoleMutex>::print_range_(const memory_buf_t &formatted, size_t start, size_t end)
+{
+    if (end > start)
     {
         auto size = static_cast<DWORD>(end - start);
-        ::WriteConsoleA(out_handle_, formatted.data() + start, size, nullptr, nullptr);
+        auto ignored = ::WriteConsoleA(static_cast<HANDLE>(out_handle_), formatted.data() + start, size, nullptr, nullptr);
+        (void)(ignored);
     }
+}
 
-    HANDLE out_handle_;
-    mutex_t &mutex_;
-    std::unordered_map<level::level_enum, WORD, level::level_hasher> colors_;
-};
-
-using wincolor_stdout_sink_mt = wincolor_sink<details::console_stdout, details::console_mutex>;
-using wincolor_stdout_sink_st = wincolor_sink<details::console_stdout, details::console_nullmutex>;
-
-using wincolor_stderr_sink_mt = wincolor_sink<details::console_stderr, details::console_mutex>;
-using wincolor_stderr_sink_st = wincolor_sink<details::console_stderr, details::console_nullmutex>;
-
+template<typename ConsoleMutex>
+void SPDLOG_INLINE wincolor_sink<ConsoleMutex>::write_to_file_(const memory_buf_t &formatted)
+{
+    auto size = static_cast<DWORD>(formatted.size());
+    DWORD bytes_written = 0;
+    auto ignored = ::WriteFile(static_cast<HANDLE>(out_handle_), formatted.data(), size, &bytes_written, nullptr);
+    (void)(ignored);
+}
+
+// wincolor_stdout_sink
+template<typename ConsoleMutex>
+SPDLOG_INLINE wincolor_stdout_sink<ConsoleMutex>::wincolor_stdout_sink(color_mode mode)
+    : wincolor_sink<ConsoleMutex>(::GetStdHandle(STD_OUTPUT_HANDLE), mode)
+{}
+
+// wincolor_stderr_sink
+template<typename ConsoleMutex>
+SPDLOG_INLINE wincolor_stderr_sink<ConsoleMutex>::wincolor_stderr_sink(color_mode mode)
+    : wincolor_sink<ConsoleMutex>(::GetStdHandle(STD_ERROR_HANDLE), mode)
+{}
 } // namespace sinks
 } // namespace spdlog
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/spdlog.h` & `spdlog-2.0.6/spdlog/include/spdlog/spdlog.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,304 +1,281 @@
-//
-// Copyright(c) 2015-2018 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
+
 // spdlog main header file.
 // see example.cpp for usage example
 
 #ifndef SPDLOG_H
 #define SPDLOG_H
+
 #pragma once
 
-#include "spdlog/common.h"
-#include "spdlog/details/registry.h"
-#include "spdlog/logger.h"
-#include "spdlog/version.h"
+#include <spdlog/common.h>
+#include <spdlog/details/registry.h>
+#include <spdlog/logger.h>
+#include <spdlog/version.h>
+#include <spdlog/details/synchronous_factory.h>
 
 #include <chrono>
 #include <functional>
 #include <memory>
 #include <string>
 
 namespace spdlog {
 
-// Default logger factory-  creates synchronous loggers
-struct synchronous_factory
-{
-    template<typename Sink, typename... SinkArgs>
-    static std::shared_ptr<spdlog::logger> create(std::string logger_name, SinkArgs &&... args)
-    {
-        auto sink = std::make_shared<Sink>(std::forward<SinkArgs>(args)...);
-        auto new_logger = std::make_shared<logger>(std::move(logger_name), std::move(sink));
-        details::registry::instance().initialize_logger(new_logger);
-        return new_logger;
-    }
-};
-
 using default_factory = synchronous_factory;
 
 // Create and register a logger with a templated sink type
 // The logger's level, formatter and flush level will be set according the
 // global settings.
+//
 // Example:
-// spdlog::create<daily_file_sink_st>("logger_name", "dailylog_filename", 11, 59);
+//   spdlog::create<daily_file_sink_st>("logger_name", "dailylog_filename", 11, 59);
 template<typename Sink, typename... SinkArgs>
 inline std::shared_ptr<spdlog::logger> create(std::string logger_name, SinkArgs &&... sink_args)
 {
     return default_factory::create<Sink>(std::move(logger_name), std::forward<SinkArgs>(sink_args)...);
 }
 
+// Initialize and register a logger,
+// formatter and flush level will be set according the global settings.
+//
+// Useful for initializing manually created loggers with the global settings.
+//
+// Example:
+//   auto mylogger = std::make_shared<spdlog::logger>("mylogger", ...);
+//   spdlog::initialize_logger(mylogger);
+SPDLOG_API void initialize_logger(std::shared_ptr<logger> logger);
+
 // Return an existing logger or nullptr if a logger with such name doesn't
 // exist.
 // example: spdlog::get("my_logger")->info("hello {}", "world");
-inline std::shared_ptr<logger> get(const std::string &name)
-{
-    return details::registry::instance().get(name);
-}
+SPDLOG_API std::shared_ptr<logger> get(const std::string &name);
 
 // Set global formatter. Each sink in each logger will get a clone of this object
-inline void set_formatter(std::unique_ptr<spdlog::formatter> formatter)
-{
-    details::registry::instance().set_formatter(std::move(formatter));
-}
+SPDLOG_API void set_formatter(std::unique_ptr<spdlog::formatter> formatter);
 
 // Set global format string.
 // example: spdlog::set_pattern("%Y-%m-%d %H:%M:%S.%e %l : %v");
-inline void set_pattern(std::string pattern, pattern_time_type time_type = pattern_time_type::local)
-{
-    set_formatter(std::unique_ptr<spdlog::formatter>(new pattern_formatter(std::move(pattern), time_type)));
-}
+SPDLOG_API void set_pattern(std::string pattern, pattern_time_type time_type = pattern_time_type::local);
+
+// enable global backtrace support
+SPDLOG_API void enable_backtrace(size_t n_messages);
+
+// disable global backtrace support
+SPDLOG_API void disable_backtrace();
+
+// call dump backtrace on default logger
+SPDLOG_API void dump_backtrace();
+
+// Get global logging level
+SPDLOG_API level::level_enum get_level();
 
 // Set global logging level
-inline void set_level(level::level_enum log_level)
-{
-    details::registry::instance().set_level(log_level);
-}
+SPDLOG_API void set_level(level::level_enum log_level);
+
+// Determine whether the default logger should log messages with a certain level
+SPDLOG_API bool should_log(level::level_enum lvl);
 
 // Set global flush level
-inline void flush_on(level::level_enum log_level)
-{
-    details::registry::instance().flush_on(log_level);
-}
+SPDLOG_API void flush_on(level::level_enum log_level);
 
 // Start/Restart a periodic flusher thread
 // Warning: Use only if all your loggers are thread safe!
-inline void flush_every(std::chrono::seconds interval)
-{
-    details::registry::instance().flush_every(interval);
-}
+SPDLOG_API void flush_every(std::chrono::seconds interval);
 
 // Set global error handler
-inline void set_error_handler(log_err_handler handler)
-{
-    details::registry::instance().set_error_handler(std::move(handler));
-}
+SPDLOG_API void set_error_handler(void (*handler)(const std::string &msg));
 
 // Register the given logger with the given name
-inline void register_logger(std::shared_ptr<logger> logger)
-{
-    details::registry::instance().register_logger(std::move(logger));
-}
+SPDLOG_API void register_logger(std::shared_ptr<logger> logger);
 
 // Apply a user defined function on all registered loggers
 // Example:
 // spdlog::apply_all([&](std::shared_ptr<spdlog::logger> l) {l->flush();});
-inline void apply_all(const std::function<void(std::shared_ptr<logger>)> &fun)
-{
-    details::registry::instance().apply_all(fun);
-}
+SPDLOG_API void apply_all(const std::function<void(std::shared_ptr<logger>)> &fun);
 
 // Drop the reference to the given logger
-inline void drop(const std::string &name)
-{
-    details::registry::instance().drop(name);
-}
+SPDLOG_API void drop(const std::string &name);
 
 // Drop all references from the registry
-inline void drop_all()
-{
-    details::registry::instance().drop_all();
-}
+SPDLOG_API void drop_all();
 
 // stop any running threads started by spdlog and clean registry loggers
-inline void shutdown()
-{
-    details::registry::instance().shutdown();
-}
+SPDLOG_API void shutdown();
 
 // Automatic registration of loggers when using spdlog::create() or spdlog::create_async
-inline void set_automatic_registration(bool automatic_registation)
-{
-    details::registry::instance().set_automatic_registration(automatic_registation);
-}
+SPDLOG_API void set_automatic_registration(bool automatic_registration);
 
 // API for using default logger (stdout_color_mt),
 // e.g: spdlog::info("Message {}", 1);
 //
 // The default logger object can be accessed using the spdlog::default_logger():
 // For example, to add another sink to it:
-// spdlog::default_logger()->sinks()->push_back(some_sink);
+// spdlog::default_logger()->sinks().push_back(some_sink);
 //
 // The default logger can replaced using spdlog::set_default_logger(new_logger).
 // For example, to replace it with a file logger.
 //
 // IMPORTANT:
 // The default API is thread safe (for _mt loggers), but:
 // set_default_logger() *should not* be used concurrently with the default API.
 // e.g do not call set_default_logger() from one thread while calling spdlog::info() from another.
 
-inline std::shared_ptr<spdlog::logger> default_logger()
-{
-    return details::registry::instance().default_logger();
-}
+SPDLOG_API std::shared_ptr<spdlog::logger> default_logger();
 
-inline spdlog::logger *default_logger_raw()
-{
-    return details::registry::instance().get_default_raw();
-}
+SPDLOG_API spdlog::logger *default_logger_raw();
 
-inline void set_default_logger(std::shared_ptr<spdlog::logger> default_logger)
+SPDLOG_API void set_default_logger(std::shared_ptr<spdlog::logger> default_logger);
+
+template<typename... Args>
+inline void log(source_loc source, level::level_enum lvl, format_string_t<Args...> fmt, Args &&... args)
 {
-    details::registry::instance().set_default_logger(std::move(default_logger));
+    default_logger_raw()->log(source, lvl, fmt, std::forward<Args>(args)...);
 }
 
 template<typename... Args>
-inline void log(source_loc source, level::level_enum lvl, const char *fmt, const Args &... args)
+inline void log(level::level_enum lvl, format_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->log(source, lvl, fmt, args...);
+    default_logger_raw()->log(source_loc{}, lvl, fmt, std::forward<Args>(args)...);
 }
 
 template<typename... Args>
-inline void log(level::level_enum lvl, const char *fmt, const Args &... args)
+inline void trace(format_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->log(source_loc{}, lvl, fmt, args...);
+    default_logger_raw()->trace(fmt, std::forward<Args>(args)...);
 }
 
 template<typename... Args>
-inline void trace(const char *fmt, const Args &... args)
+inline void debug(format_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->trace(fmt, args...);
+    default_logger_raw()->debug(fmt, std::forward<Args>(args)...);
 }
 
 template<typename... Args>
-inline void debug(const char *fmt, const Args &... args)
+inline void info(format_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->debug(fmt, args...);
+    default_logger_raw()->info(fmt, std::forward<Args>(args)...);
 }
 
 template<typename... Args>
-inline void info(const char *fmt, const Args &... args)
+inline void warn(format_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->info(fmt, args...);
+    default_logger_raw()->warn(fmt, std::forward<Args>(args)...);
 }
 
 template<typename... Args>
-inline void warn(const char *fmt, const Args &... args)
+inline void error(format_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->warn(fmt, args...);
+    default_logger_raw()->error(fmt, std::forward<Args>(args)...);
 }
 
 template<typename... Args>
-inline void error(const char *fmt, const Args &... args)
+inline void critical(format_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->error(fmt, args...);
+    default_logger_raw()->critical(fmt, std::forward<Args>(args)...);
 }
 
-template<typename... Args>
-inline void critical(const char *fmt, const Args &... args)
+template<typename T>
+inline void log(source_loc source, level::level_enum lvl, const T &msg)
 {
-    default_logger_raw()->critical(fmt, args...);
+    default_logger_raw()->log(source, lvl, msg);
 }
 
 template<typename T>
 inline void log(level::level_enum lvl, const T &msg)
 {
     default_logger_raw()->log(lvl, msg);
 }
 
-template<typename T>
-inline void trace(const T &msg)
+#ifdef SPDLOG_WCHAR_TO_UTF8_SUPPORT
+template<typename... Args>
+inline void log(source_loc source, level::level_enum lvl, wformat_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->trace(msg);
+    default_logger_raw()->log(source, lvl, fmt, std::forward<Args>(args)...);
 }
 
-template<typename T>
-inline void debug(const T &msg)
+template<typename... Args>
+inline void log(level::level_enum lvl, wformat_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->debug(msg);
+    default_logger_raw()->log(source_loc{}, lvl, fmt, std::forward<Args>(args)...);
 }
 
-template<typename T>
-inline void info(const T &msg)
+template<typename... Args>
+inline void trace(wformat_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->info(msg);
+    default_logger_raw()->trace(fmt, std::forward<Args>(args)...);
 }
 
-template<typename T>
-inline void warn(const T &msg)
+template<typename... Args>
+inline void debug(wformat_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->warn(msg);
+    default_logger_raw()->debug(fmt, std::forward<Args>(args)...);
 }
 
-template<typename T>
-inline void error(const T &msg)
+template<typename... Args>
+inline void info(wformat_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->error(msg);
+    default_logger_raw()->info(fmt, std::forward<Args>(args)...);
 }
 
-template<typename T>
-inline void critical(const T &msg)
+template<typename... Args>
+inline void warn(wformat_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->critical(msg);
+    default_logger_raw()->warn(fmt, std::forward<Args>(args)...);
 }
 
-#ifdef SPDLOG_WCHAR_TO_UTF8_SUPPORT
 template<typename... Args>
-inline void log(level::level_enum lvl, const wchar_t *fmt, const Args &... args)
+inline void error(wformat_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->log(lvl, fmt, args...);
+    default_logger_raw()->error(fmt, std::forward<Args>(args)...);
 }
 
 template<typename... Args>
-inline void trace(const wchar_t *fmt, const Args &... args)
+inline void critical(wformat_string_t<Args...> fmt, Args &&... args)
 {
-    default_logger_raw()->trace(fmt, args...);
+    default_logger_raw()->critical(fmt, std::forward<Args>(args)...);
 }
+#endif
 
-template<typename... Args>
-inline void debug(const wchar_t *fmt, const Args &... args)
+template<typename T>
+inline void trace(const T &msg)
 {
-    default_logger_raw()->debug(fmt, args...);
+    default_logger_raw()->trace(msg);
 }
 
-template<typename... Args>
-inline void info(const wchar_t *fmt, const Args &... args)
+template<typename T>
+inline void debug(const T &msg)
 {
-    default_logger_raw()->info(fmt, args...);
+    default_logger_raw()->debug(msg);
 }
 
-template<typename... Args>
-inline void warn(const wchar_t *fmt, const Args &... args)
+template<typename T>
+inline void info(const T &msg)
 {
-    default_logger_raw()->warn(fmt, args...);
+    default_logger_raw()->info(msg);
 }
 
-template<typename... Args>
-inline void error(const wchar_t *fmt, const Args &... args)
+template<typename T>
+inline void warn(const T &msg)
 {
-    default_logger_raw()->error(fmt, args...);
+    default_logger_raw()->warn(msg);
 }
 
-template<typename... Args>
-inline void critical(const wchar_t *fmt, const Args &... args)
+template<typename T>
+inline void error(const T &msg)
 {
-    default_logger_raw()->critical(fmt, args...);
+    default_logger_raw()->error(msg);
 }
 
-#endif // SPDLOG_WCHAR_TO_UTF8_SUPPORT
+template<typename T>
+inline void critical(const T &msg)
+{
+    default_logger_raw()->critical(msg);
+}
 
 } // namespace spdlog
 
 //
 // enable/disable log calls at compile time according to global level.
 //
 // define SPDLOG_ACTIVE_LEVEL to one of those (before including spdlog.h):
@@ -307,60 +284,62 @@
 // SPDLOG_LEVEL_INFO,
 // SPDLOG_LEVEL_WARN,
 // SPDLOG_LEVEL_ERROR,
 // SPDLOG_LEVEL_CRITICAL,
 // SPDLOG_LEVEL_OFF
 //
 
-#define SPDLOG_LOGGER_CALL(logger, level, ...)                                                                                             \
-    if (logger->should_log(level))                                                                                                         \
-    logger->log(spdlog::source_loc{SPDLOG_FILE_BASENAME(__FILE__), __LINE__, SPDLOG_FUNCTION}, level, __VA_ARGS__)
+#define SPDLOG_LOGGER_CALL(logger, level, ...) (logger)->log(spdlog::source_loc{__FILE__, __LINE__, SPDLOG_FUNCTION}, level, __VA_ARGS__)
 
 #if SPDLOG_ACTIVE_LEVEL <= SPDLOG_LEVEL_TRACE
-#define SPDLOG_LOGGER_TRACE(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::trace, __VA_ARGS__)
-#define SPDLOG_TRACE(...) SPDLOG_LOGGER_TRACE(spdlog::default_logger_raw(), __VA_ARGS__)
+#    define SPDLOG_LOGGER_TRACE(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::trace, __VA_ARGS__)
+#    define SPDLOG_TRACE(...) SPDLOG_LOGGER_TRACE(spdlog::default_logger_raw(), __VA_ARGS__)
 #else
-#define SPDLOG_LOGGER_TRACE(logger, ...) (void)0
-#define SPDLOG_TRACE(...) (void)0
+#    define SPDLOG_LOGGER_TRACE(logger, ...) (void)0
+#    define SPDLOG_TRACE(...) (void)0
 #endif
 
 #if SPDLOG_ACTIVE_LEVEL <= SPDLOG_LEVEL_DEBUG
-#define SPDLOG_LOGGER_DEBUG(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::debug, __VA_ARGS__)
-#define SPDLOG_DEBUG(...) SPDLOG_LOGGER_DEBUG(spdlog::default_logger_raw(), __VA_ARGS__)
+#    define SPDLOG_LOGGER_DEBUG(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::debug, __VA_ARGS__)
+#    define SPDLOG_DEBUG(...) SPDLOG_LOGGER_DEBUG(spdlog::default_logger_raw(), __VA_ARGS__)
 #else
-#define SPDLOG_LOGGER_DEBUG(logger, ...) (void)0
-#define SPDLOG_DEBUG(...) (void)0
+#    define SPDLOG_LOGGER_DEBUG(logger, ...) (void)0
+#    define SPDLOG_DEBUG(...) (void)0
 #endif
 
 #if SPDLOG_ACTIVE_LEVEL <= SPDLOG_LEVEL_INFO
-#define SPDLOG_LOGGER_INFO(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::info, __VA_ARGS__)
-#define SPDLOG_INFO(...) SPDLOG_LOGGER_INFO(spdlog::default_logger_raw(), __VA_ARGS__)
+#    define SPDLOG_LOGGER_INFO(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::info, __VA_ARGS__)
+#    define SPDLOG_INFO(...) SPDLOG_LOGGER_INFO(spdlog::default_logger_raw(), __VA_ARGS__)
 #else
-#define SPDLOG_LOGGER_INFO(logger, ...) (void)0
-#define SPDLOG_INFO(...) (void)0
+#    define SPDLOG_LOGGER_INFO(logger, ...) (void)0
+#    define SPDLOG_INFO(...) (void)0
 #endif
 
 #if SPDLOG_ACTIVE_LEVEL <= SPDLOG_LEVEL_WARN
-#define SPDLOG_LOGGER_WARN(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::warn, __VA_ARGS__)
-#define SPDLOG_WARN(...) SPDLOG_LOGGER_WARN(spdlog::default_logger_raw(), __VA_ARGS__)
+#    define SPDLOG_LOGGER_WARN(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::warn, __VA_ARGS__)
+#    define SPDLOG_WARN(...) SPDLOG_LOGGER_WARN(spdlog::default_logger_raw(), __VA_ARGS__)
 #else
-#define SPDLOG_LOGGER_WARN(logger, ...) (void)0
-#define SPDLOG_WARN(...) (void)0
+#    define SPDLOG_LOGGER_WARN(logger, ...) (void)0
+#    define SPDLOG_WARN(...) (void)0
 #endif
 
 #if SPDLOG_ACTIVE_LEVEL <= SPDLOG_LEVEL_ERROR
-#define SPDLOG_LOGGER_ERROR(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::err, __VA_ARGS__)
-#define SPDLOG_ERROR(...) SPDLOG_LOGGER_ERROR(spdlog::default_logger_raw(), __VA_ARGS__)
+#    define SPDLOG_LOGGER_ERROR(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::err, __VA_ARGS__)
+#    define SPDLOG_ERROR(...) SPDLOG_LOGGER_ERROR(spdlog::default_logger_raw(), __VA_ARGS__)
 #else
-#define SPDLOG_LOGGER_ERROR(logger, ...) (void)0
-#define SPDLOG_ERROR(...) (void)0
+#    define SPDLOG_LOGGER_ERROR(logger, ...) (void)0
+#    define SPDLOG_ERROR(...) (void)0
 #endif
 
 #if SPDLOG_ACTIVE_LEVEL <= SPDLOG_LEVEL_CRITICAL
-#define SPDLOG_LOGGER_CRITICAL(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::critical, __VA_ARGS__)
-#define SPDLOG_CRITICAL(...) SPDLOG_LOGGER_CRITICAL(spdlog::default_logger_raw(), __VA_ARGS__)
+#    define SPDLOG_LOGGER_CRITICAL(logger, ...) SPDLOG_LOGGER_CALL(logger, spdlog::level::critical, __VA_ARGS__)
+#    define SPDLOG_CRITICAL(...) SPDLOG_LOGGER_CRITICAL(spdlog::default_logger_raw(), __VA_ARGS__)
 #else
-#define SPDLOG_LOGGER_CRITICAL(logger, ...) (void)0
-#define SPDLOG_CRITICAL(...) (void)0
+#    define SPDLOG_LOGGER_CRITICAL(logger, ...) (void)0
+#    define SPDLOG_CRITICAL(...) (void)0
+#endif
+
+#ifdef SPDLOG_HEADER_ONLY
+#    include "spdlog-inl.h"
 #endif
 
 #endif // SPDLOG_H
```

### Comparing `spdlog-2.0.4/spdlog/include/spdlog/tweakme.h` & `spdlog-2.0.6/spdlog/include/spdlog/tweakme.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-//
-// Copyright(c) 2015 Gabi Melman.
+// Copyright(c) 2015-present, Gabi Melman & spdlog contributors.
 // Distributed under the MIT License (http://opensource.org/licenses/MIT)
-//
 
 #pragma once
 
 ///////////////////////////////////////////////////////////////////////////////
 //
 // Edit this file to squeeze more performance, and to customize supported
 // features
@@ -18,60 +16,33 @@
 // the kernel HZ.
 // Uncomment to use it instead of the regular clock.
 //
 // #define SPDLOG_CLOCK_COARSE
 ///////////////////////////////////////////////////////////////////////////////
 
 ///////////////////////////////////////////////////////////////////////////////
-// Uncomment if date/time logging is not needed and never appear in the log
-// pattern.
-// This will prevent spdlog from querying the clock on each log call.
-//
-// WARNING: If the log pattern contains any date/time while this flag is on, the
-// result is undefined.
-//          You must set new pattern(spdlog::set_pattern(..") without any
-//          date/time in it
-//
-// #define SPDLOG_NO_DATETIME
-///////////////////////////////////////////////////////////////////////////////
-
-///////////////////////////////////////////////////////////////////////////////
 // Uncomment if thread id logging is not needed (i.e. no %t in the log pattern).
 // This will prevent spdlog from querying the thread id on each log call.
 //
 // WARNING: If the log pattern contains thread id (i.e, %t) while this flag is
-// on, the result is undefined.
+// on, zero will be logged as thread id.
 //
 // #define SPDLOG_NO_THREAD_ID
 ///////////////////////////////////////////////////////////////////////////////
 
 ///////////////////////////////////////////////////////////////////////////////
 // Uncomment to prevent spdlog from using thread local storage.
 //
 // WARNING: if your program forks, UNCOMMENT this flag to prevent undefined
 // thread ids in the children logs.
 //
 // #define SPDLOG_NO_TLS
 ///////////////////////////////////////////////////////////////////////////////
 
 ///////////////////////////////////////////////////////////////////////////////
-// Uncomment if logger name logging is not needed.
-// This will prevent spdlog from copying the logger name on each log call.
-//
-// #define SPDLOG_NO_NAME
-///////////////////////////////////////////////////////////////////////////////
-
-///////////////////////////////////////////////////////////////////////////////
-// Uncomment to enable the SPDLOG_DEBUG/SPDLOG_TRACE macros.
-//
-// #define SPDLOG_DEBUG_ON
-// #define SPDLOG_TRACE_ON
-///////////////////////////////////////////////////////////////////////////////
-
-///////////////////////////////////////////////////////////////////////////////
 // Uncomment to avoid spdlog's usage of atomic log levels
 // Use only if your code never modifies a logger's log levels concurrently by
 // different threads.
 //
 // #define SPDLOG_NO_ATOMIC_LEVELS
 ///////////////////////////////////////////////////////////////////////////////
 
@@ -84,45 +55,59 @@
 ///////////////////////////////////////////////////////////////////////////////
 // Uncomment to override default eol ("\n" or "\r\n" under Linux/Windows)
 //
 // #define SPDLOG_EOL ";-)\n"
 ///////////////////////////////////////////////////////////////////////////////
 
 ///////////////////////////////////////////////////////////////////////////////
+// Uncomment to override default folder separators ("/" or "\\/" under
+// Linux/Windows). Each character in the string is treated as a different
+// separator.
+//
+// #define SPDLOG_FOLDER_SEPS "\\"
+///////////////////////////////////////////////////////////////////////////////
+
+///////////////////////////////////////////////////////////////////////////////
 // Uncomment to use your own copy of the fmt library instead of spdlog's copy.
 // In this case spdlog will try to include <fmt/format.h> so set your -I flag
 // accordingly.
 //
 // #define SPDLOG_FMT_EXTERNAL
 ///////////////////////////////////////////////////////////////////////////////
 
 ///////////////////////////////////////////////////////////////////////////////
+// Uncomment to use C++20 std::format instead of fmt. This removes compile
+// time checking of format strings, but doesn't depend on the fmt library.
+//
+// #define SPDLOG_USE_STD_FORMAT
+///////////////////////////////////////////////////////////////////////////////
+
+///////////////////////////////////////////////////////////////////////////////
 // Uncomment to enable wchar_t support (convert to utf8)
 //
 // #define SPDLOG_WCHAR_TO_UTF8_SUPPORT
 ///////////////////////////////////////////////////////////////////////////////
 
 ///////////////////////////////////////////////////////////////////////////////
 // Uncomment to prevent child processes from inheriting log file descriptors
 //
 // #define SPDLOG_PREVENT_CHILD_FD
 ///////////////////////////////////////////////////////////////////////////////
 
 ///////////////////////////////////////////////////////////////////////////////
-// Uncomment to enable message counting feature.
-// Use the %i in the logger pattern to display log message sequence id.
+// Uncomment to customize level names (e.g. "MY TRACE")
 //
-// #define SPDLOG_ENABLE_MESSAGE_COUNTER
+// #define SPDLOG_LEVEL_NAMES { "MY TRACE", "MY DEBUG", "MY INFO", "MY WARNING", "MY ERROR", "MY CRITICAL", "OFF" }
 ///////////////////////////////////////////////////////////////////////////////
 
 ///////////////////////////////////////////////////////////////////////////////
-// Uncomment to customize level names (e.g. "MT TRACE")
+// Uncomment to customize short level names (e.g. "MT")
+// These can be longer than one character.
 //
-// #define SPDLOG_LEVEL_NAMES { "MY TRACE", "MY DEBUG", "MY INFO", "MY WARNING",
-// "MY ERROR", "MY CRITICAL", "OFF" }
+// #define SPDLOG_SHORT_LEVEL_NAMES { "T", "D", "I", "W", "E", "C", "O" }
 ///////////////////////////////////////////////////////////////////////////////
 
 ///////////////////////////////////////////////////////////////////////////////
 // Uncomment to disable default logger creation.
 // This might save some (very) small initialization time if no default logger is needed.
 //
 // #define SPDLOG_DISABLE_DEFAULT_LOGGER
@@ -137,9 +122,13 @@
 
 ///////////////////////////////////////////////////////////////////////////////
 // Uncomment (and change if desired) macro to use for function names.
 // This is compiler dependent.
 // __PRETTY_FUNCTION__ might be nicer in clang/gcc, and __FUNCTION__ in msvc.
 // Defaults to __FUNCTION__ (should work on all compilers) if not defined.
 //
-// #define SPDLOG_FUNCTION __PRETTY_FUNCTION__
-///////////////////////////////////////////////////////////////////////////////
+// #ifdef __PRETTY_FUNCTION__
+// # define SPDLOG_FUNCTION __PRETTY_FUNCTION__
+// #else
+// # define SPDLOG_FUNCTION __FUNCTION__
+// #endif
+///////////////////////////////////////////////////////////////////////////////
```

### Comparing `spdlog-2.0.4/spdlog.egg-info/SOURCES.txt` & `spdlog-2.0.6/spdlog.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,59 +6,107 @@
 spdlog.egg-info/PKG-INFO
 spdlog.egg-info/SOURCES.txt
 spdlog.egg-info/dependency_links.txt
 spdlog.egg-info/not-zip-safe
 spdlog.egg-info/requires.txt
 spdlog.egg-info/top_level.txt
 spdlog/include/spdlog/async.h
+spdlog/include/spdlog/async_logger-inl.h
 spdlog/include/spdlog/async_logger.h
+spdlog/include/spdlog/common-inl.h
 spdlog/include/spdlog/common.h
 spdlog/include/spdlog/formatter.h
+spdlog/include/spdlog/fwd.h
+spdlog/include/spdlog/logger-inl.h
 spdlog/include/spdlog/logger.h
+spdlog/include/spdlog/pattern_formatter-inl.h
+spdlog/include/spdlog/pattern_formatter.h
+spdlog/include/spdlog/spdlog-inl.h
 spdlog/include/spdlog/spdlog.h
+spdlog/include/spdlog/stopwatch.h
 spdlog/include/spdlog/tweakme.h
 spdlog/include/spdlog/version.h
-spdlog/include/spdlog/details/async_logger_impl.h
+spdlog/include/spdlog/cfg/argv.h
+spdlog/include/spdlog/cfg/env.h
+spdlog/include/spdlog/cfg/helpers-inl.h
+spdlog/include/spdlog/cfg/helpers.h
+spdlog/include/spdlog/details/backtracer-inl.h
+spdlog/include/spdlog/details/backtracer.h
 spdlog/include/spdlog/details/circular_q.h
 spdlog/include/spdlog/details/console_globals.h
+spdlog/include/spdlog/details/file_helper-inl.h
 spdlog/include/spdlog/details/file_helper.h
 spdlog/include/spdlog/details/fmt_helper.h
+spdlog/include/spdlog/details/log_msg-inl.h
 spdlog/include/spdlog/details/log_msg.h
-spdlog/include/spdlog/details/logger_impl.h
+spdlog/include/spdlog/details/log_msg_buffer-inl.h
+spdlog/include/spdlog/details/log_msg_buffer.h
 spdlog/include/spdlog/details/mpmc_blocking_q.h
 spdlog/include/spdlog/details/null_mutex.h
+spdlog/include/spdlog/details/os-inl.h
 spdlog/include/spdlog/details/os.h
-spdlog/include/spdlog/details/pattern_formatter.h
+spdlog/include/spdlog/details/periodic_worker-inl.h
 spdlog/include/spdlog/details/periodic_worker.h
+spdlog/include/spdlog/details/registry-inl.h
 spdlog/include/spdlog/details/registry.h
+spdlog/include/spdlog/details/synchronous_factory.h
+spdlog/include/spdlog/details/tcp_client-windows.h
+spdlog/include/spdlog/details/tcp_client.h
+spdlog/include/spdlog/details/thread_pool-inl.h
 spdlog/include/spdlog/details/thread_pool.h
+spdlog/include/spdlog/details/udp_client-windows.h
+spdlog/include/spdlog/details/udp_client.h
+spdlog/include/spdlog/details/windows_include.h
 spdlog/include/spdlog/fmt/bin_to_hex.h
+spdlog/include/spdlog/fmt/chrono.h
+spdlog/include/spdlog/fmt/compile.h
 spdlog/include/spdlog/fmt/fmt.h
 spdlog/include/spdlog/fmt/ostr.h
-spdlog/include/spdlog/fmt/bundled/LICENSE.rst
+spdlog/include/spdlog/fmt/ranges.h
+spdlog/include/spdlog/fmt/xchar.h
+spdlog/include/spdlog/fmt/bundled/args.h
 spdlog/include/spdlog/fmt/bundled/chrono.h
 spdlog/include/spdlog/fmt/bundled/color.h
+spdlog/include/spdlog/fmt/bundled/compile.h
 spdlog/include/spdlog/fmt/bundled/core.h
+spdlog/include/spdlog/fmt/bundled/fmt.license.rst
 spdlog/include/spdlog/fmt/bundled/format-inl.h
 spdlog/include/spdlog/fmt/bundled/format.h
 spdlog/include/spdlog/fmt/bundled/locale.h
+spdlog/include/spdlog/fmt/bundled/os.h
 spdlog/include/spdlog/fmt/bundled/ostream.h
-spdlog/include/spdlog/fmt/bundled/posix.h
 spdlog/include/spdlog/fmt/bundled/printf.h
 spdlog/include/spdlog/fmt/bundled/ranges.h
-spdlog/include/spdlog/fmt/bundled/time.h
+spdlog/include/spdlog/fmt/bundled/xchar.h
 spdlog/include/spdlog/sinks/android_sink.h
+spdlog/include/spdlog/sinks/ansicolor_sink-inl.h
 spdlog/include/spdlog/sinks/ansicolor_sink.h
+spdlog/include/spdlog/sinks/base_sink-inl.h
 spdlog/include/spdlog/sinks/base_sink.h
+spdlog/include/spdlog/sinks/basic_file_sink-inl.h
 spdlog/include/spdlog/sinks/basic_file_sink.h
 spdlog/include/spdlog/sinks/daily_file_sink.h
 spdlog/include/spdlog/sinks/dist_sink.h
+spdlog/include/spdlog/sinks/dup_filter_sink.h
+spdlog/include/spdlog/sinks/hourly_file_sink.h
+spdlog/include/spdlog/sinks/mongo_sink.h
 spdlog/include/spdlog/sinks/msvc_sink.h
 spdlog/include/spdlog/sinks/null_sink.h
 spdlog/include/spdlog/sinks/ostream_sink.h
+spdlog/include/spdlog/sinks/qt_sinks.h
+spdlog/include/spdlog/sinks/ringbuffer_sink.h
+spdlog/include/spdlog/sinks/rotating_file_sink-inl.h
 spdlog/include/spdlog/sinks/rotating_file_sink.h
+spdlog/include/spdlog/sinks/sink-inl.h
 spdlog/include/spdlog/sinks/sink.h
+spdlog/include/spdlog/sinks/stdout_color_sinks-inl.h
 spdlog/include/spdlog/sinks/stdout_color_sinks.h
+spdlog/include/spdlog/sinks/stdout_sinks-inl.h
 spdlog/include/spdlog/sinks/stdout_sinks.h
 spdlog/include/spdlog/sinks/syslog_sink.h
+spdlog/include/spdlog/sinks/systemd_sink.h
+spdlog/include/spdlog/sinks/tcp_sink.h
+spdlog/include/spdlog/sinks/udp_sink.h
+spdlog/include/spdlog/sinks/win_eventlog_sink.h
+spdlog/include/spdlog/sinks/wincolor_sink-inl.h
 spdlog/include/spdlog/sinks/wincolor_sink.h
 src/pyspdlog.cpp
```

### Comparing `spdlog-2.0.4/src/pyspdlog.cpp` & `spdlog-2.0.6/src/pyspdlog.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #include <spdlog/async_logger.h>
 #include <spdlog/sinks/basic_file_sink.h>
 #include <spdlog/sinks/daily_file_sink.h>
 #include <spdlog/sinks/null_sink.h>
 #include <spdlog/sinks/rotating_file_sink.h>
 #include <spdlog/sinks/stdout_color_sinks.h>
 #include <spdlog/sinks/stdout_sinks.h>
+#include <spdlog/sinks/tcp_sink.h>
 #ifndef _WIN32
 #include <spdlog/sinks/syslog_sink.h>
 #endif
 
 #include <iostream>
 #include <memory>
 #include <mutex>
@@ -246,28 +247,50 @@
 public:
     null_sink_mt()
     {
         _sink = std::make_shared<spdlog::sinks::null_sink_mt>();
     }
 };
 
+class tcp_sink_st : public Sink {
+public:
+    tcp_sink_st(std::string server_host, int server_port, bool lazy_connect)
+    {
+        struct spdlog::sinks::tcp_sink_config tcp_config(server_host, server_port);
+        tcp_config.lazy_connect = lazy_connect;
+
+        _sink = std::make_shared<spdlog::sinks::tcp_sink_st>(tcp_config);
+    }
+};
+
+class tcp_sink_mt : public Sink {
+public:
+    tcp_sink_mt(std::string server_host, int server_port, bool lazy_connect)
+    {
+        struct spdlog::sinks::tcp_sink_config tcp_config(server_host, server_port);
+        tcp_config.lazy_connect = lazy_connect;
+
+        _sink = std::make_shared<spdlog::sinks::tcp_sink_mt>(tcp_config);
+    }
+};
+
 #ifdef SPDLOG_ENABLE_SYSLOG
 class syslog_sink_st : public Sink {
 public:
-    syslog_sink_st(const std::string& ident = "", int syslog_option = 0, int syslog_facility = (1 << 3))
+    syslog_sink_st(const std::string& ident = "", int syslog_option = 0, int syslog_facility = (1 << 3), bool enable_formatting = true)
     {
-        _sink = std::make_shared<spdlog::sinks::syslog_sink_st>(ident, syslog_option, syslog_facility);
+        _sink = std::make_shared<spdlog::sinks::syslog_sink_st>(ident, syslog_option, syslog_facility, enable_formatting);
     }
 };
 
 class syslog_sink_mt : public Sink {
 public:
-    syslog_sink_mt(const std::string& ident = "", int syslog_option = 0, int syslog_facility = (1 << 3))
+    syslog_sink_mt(const std::string& ident = "", int syslog_option = 0, int syslog_facility = (1 << 3), bool enable_formatting = true)
     {
-        _sink = std::make_shared<spdlog::sinks::syslog_sink_mt>(ident, syslog_option, syslog_facility);
+        _sink = std::make_shared<spdlog::sinks::syslog_sink_mt>(ident, syslog_option, syslog_facility, enable_formatting);
     }
 };
 #endif
 
 class Logger {
 public:
     using async_factory_nb = spdlog::async_factory_impl<spdlog::async_overflow_policy::overrun_oldest>;
@@ -343,24 +366,19 @@
         std::vector<Sink> snks;
         for (const spd::sink_ptr& sink : _logger->sinks()) {
             snks.push_back(Sink(sink));
         }
         return snks;
     }
 
-    void set_error_handler(spd::log_err_handler handler)
+    void set_error_handler(spd::err_handler handler)
     {
         _logger->set_error_handler(handler);
     }
 
-    spd::log_err_handler error_handler()
-    {
-        return _logger->error_handler();
-    }
-
     std::shared_ptr<spdlog::logger> get_underlying_logger() {
         return _logger;
     }
 
 protected:
     const std::string _name;
     bool _async;
@@ -743,14 +761,26 @@
 
     py::class_<null_sink_st, Sink>(m, "null_sink_st")
         .def(py::init<>());
 
     py::class_<null_sink_mt, Sink>(m, "null_sink_mt")
         .def(py::init<>());
 
+    py::class_<tcp_sink_st, Sink>(m, "tcp_sink_st")
+        .def(py::init<std::string, int, bool>(),
+             py::arg("server_host"),
+             py::arg("server_port"),
+             py::arg("lazy_connect"));
+
+    py::class_<tcp_sink_mt, Sink>(m, "tcp_sink_mt")
+        .def(py::init<std::string, int, bool>(),
+             py::arg("server_host"),
+             py::arg("server_port"),
+             py::arg("lazy_connect"));
+
     py::class_<LogLevel>(m, "LogLevel")
         .def_property_readonly_static("TRACE", [](py::object) { return LogLevel::trace; })
         .def_property_readonly_static("DEBUG", [](py::object) { return LogLevel::debug; })
         .def_property_readonly_static("INFO", [](py::object) { return LogLevel::info; })
         .def_property_readonly_static("WARN", [](py::object) { return LogLevel::warn; })
         .def_property_readonly_static("ERR", [](py::object) { return LogLevel::err; })
         .def_property_readonly_static("CRITICAL", [](py::object) { return LogLevel::critical; })
@@ -774,22 +804,21 @@
         .def("error", &Logger::error)
         .def("critical", &Logger::critical)
         .def("name", &Logger::name)
         .def("should_log", &Logger::should_log)
         .def("set_level", &Logger::set_level)
         .def("level", &Logger::level)
         .def("set_pattern", &Logger::set_pattern,
-            py::arg("pattern"), py::arg("type") = spd::pattern_time_type::local)
+            py::arg("pattern"), py::arg("type") = spd::pattern_time_type::local, "type refers to time format and takes 'local' or 'utc'")
         .def("flush_on", &Logger::flush_on)
         .def("flush", &Logger::flush)
         .def("close", &Logger::close)
         .def("async_mode", &Logger::async)
         .def("sinks", &Logger::sinks)
         .def("set_error_handler", &Logger::set_error_handler)
-        .def("error_handler", &Logger::error_handler)
         .def("get_underlying_logger", &Logger::get_underlying_logger);
 
     py::class_<SinkLogger, Logger>(m, "SinkLogger")
     .def(py::init<const std::string&, const std::vector<Sink>&>(),
         py::arg("name"),
         py::arg("sinks"))
     .def(py::init<const std::string&, const std::vector<Sink>&, bool>(),
@@ -850,23 +879,25 @@
         py::arg("hour") = 0,
         py::arg("minute") = 0,
         py::arg("async_mode"));
 
 //SyslogLogger(const std::string& logger_name, const std::string& ident = "", int syslog_option = 0, int syslog_facilty = (1<<3))
 #ifdef SPDLOG_ENABLE_SYSLOG
 py::class_<syslog_sink_st, Sink>(m, "syslog_sink_st")
-    .def(py::init<std::string, int, int>(),
+    .def(py::init<std::string, int, int, bool>(),
         py::arg("ident") = "",
         py::arg("syslog_option") = 0,
-        py::arg("syslog_facility") = (1 << 3));
+        py::arg("syslog_facility") = (1 << 3),
+        py::arg("enable_formatting") = true);
 py::class_<syslog_sink_mt, Sink>(m, "syslog_sink_mt")
-    .def(py::init<std::string, int, int>(),
+    .def(py::init<std::string, int, int, bool>(),
         py::arg("ident") = "",
         py::arg("syslog_option") = 0,
-            py::arg("syslog_facility") = (1 << 3));
+        py::arg("syslog_facility") = (1 << 3),
+        py::arg("enable_formatting") = true);
     py::class_<SyslogLogger, Logger>(m, "SyslogLogger")
         .def(py::init<std::string, bool, std::string, int, int>(),
             py::arg("name"),
             py::arg("multithreaded") = false,
             py::arg("ident") = "",
             py::arg("syslog_option") = 0,
             py::arg("syslog_facility") = (1 << 3))
```

