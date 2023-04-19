# Comparing `tmp/spdlog-2.0.4.tar.gz` & `tmp/spdlog-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spdlog-2.0.4.tar", last modified: Fri Feb 12 18:08:31 2021, max compression
+gzip compressed data, was "spdlog-2.0.5.tar", last modified: Wed Apr 19 15:46:50 2023, max compression
```

## Comparing `spdlog-2.0.4.tar` & `spdlog-2.0.5.tar`

### file list

```diff
@@ -1,75 +1,16 @@
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
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 15:46:50.658833 spdlog-2.0.5/
+-rw-rw-r--   0 geri      (1000) geri      (1000)     1067 2023-04-19 15:44:54.000000 spdlog-2.0.5/LICENSE
+-rw-rw-r--   0 geri      (1000) geri      (1000)       83 2023-04-19 15:44:54.000000 spdlog-2.0.5/MANIFEST.in
+-rw-rw-r--   0 geri      (1000) geri      (1000)      419 2023-04-19 15:46:50.658833 spdlog-2.0.5/PKG-INFO
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2516 2023-04-19 15:44:54.000000 spdlog-2.0.5/README.md
+-rw-rw-r--   0 geri      (1000) geri      (1000)       63 2023-04-19 15:46:50.658833 spdlog-2.0.5/setup.cfg
+-rw-rw-r--   0 geri      (1000) geri      (1000)     2633 2023-04-19 15:44:54.000000 spdlog-2.0.5/setup.py
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 15:46:50.658833 spdlog-2.0.5/spdlog.egg-info/
+-rw-rw-r--   0 geri      (1000) geri      (1000)      419 2023-04-19 15:46:50.000000 spdlog-2.0.5/spdlog.egg-info/PKG-INFO
+-rw-rw-r--   0 geri      (1000) geri      (1000)      243 2023-04-19 15:46:50.000000 spdlog-2.0.5/spdlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 geri      (1000) geri      (1000)        1 2023-04-19 15:46:50.000000 spdlog-2.0.5/spdlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 geri      (1000) geri      (1000)        1 2023-04-19 15:45:59.000000 spdlog-2.0.5/spdlog.egg-info/not-zip-safe
+-rw-rw-r--   0 geri      (1000) geri      (1000)       14 2023-04-19 15:46:50.000000 spdlog-2.0.5/spdlog.egg-info/requires.txt
+-rw-rw-r--   0 geri      (1000) geri      (1000)        7 2023-04-19 15:46:50.000000 spdlog-2.0.5/spdlog.egg-info/top_level.txt
+drwxrwxr-x   0 geri      (1000) geri      (1000)        0 2023-04-19 15:46:50.658833 spdlog-2.0.5/src/
+-rw-rw-r--   0 geri      (1000) geri      (1000)    32096 2023-04-19 15:44:54.000000 spdlog-2.0.5/src/pyspdlog.cpp
```

### Comparing `spdlog-2.0.4/LICENSE` & `spdlog-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spdlog-2.0.4/README.md` & `spdlog-2.0.5/README.md`

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

### Comparing `spdlog-2.0.4/setup.py` & `spdlog-2.0.5/setup.py`

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
+    version='2.0.5',
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

### Comparing `spdlog-2.0.4/src/pyspdlog.cpp` & `spdlog-2.0.5/src/pyspdlog.cpp`

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

