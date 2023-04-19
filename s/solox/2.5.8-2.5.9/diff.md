# Comparing `tmp/solox-2.5.8.tar.gz` & `tmp/solox-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-17vxvja6/solox-2.5.8.tar", last modified: Mon Apr 10 09:54:58 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-f6gwnpz6/solox-2.5.9.tar", last modified: Wed Apr 19 09:34:31 2023, max compression
```

## Comparing `solox-2.5.8.tar` & `solox-2.5.9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-10 09:54:47.000000 solox-2.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-10 09:54:47.000000 solox-2.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-10 09:54:58.000000 solox-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-10 09:54:47.000000 solox-2.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-10 09:54:58.000000 solox-2.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-10 09:54:47.000000 solox-2.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 09:54:47.000000 solox-2.5.8/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-10 09:54:47.000000 solox-2.5.8/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-10 09:54:47.000000 solox-2.5.8/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16374 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23595 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39139 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-10 09:54:47.000000 solox-2.5.8/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-04-10 09:54:47.000000 solox-2.5.8/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    47094 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    35648 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    88804 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-04-10 09:54:47.000000 solox-2.5.8/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 09:54:47.000000 solox-2.5.8/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-04-10 09:54:47.000000 solox-2.5.8/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-10 09:54:47.000000 solox-2.5.8/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-10 09:54:47.000000 solox-2.5.8/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 09:54:58.000000 solox-2.5.8/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-19 09:34:19.000000 solox-2.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-19 09:34:19.000000 solox-2.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-19 09:34:31.000000 solox-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-19 09:34:19.000000 solox-2.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-19 09:34:31.000000 solox-2.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 09:34:19.000000 solox-2.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 09:34:19.000000 solox-2.5.9/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 09:34:19.000000 solox-2.5.9/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-19 09:34:19.000000 solox-2.5.9/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23736 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39139 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    47094 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35648 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    91984 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 09:34:19.000000 solox-2.5.9/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24225 2023-04-19 09:34:19.000000 solox-2.5.9/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-19 09:34:19.000000 solox-2.5.9/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-19 09:34:19.000000 solox-2.5.9/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/top_level.txt
```

### Comparing `solox-2.5.8/LICENSE` & `solox-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/PKG-INFO` & `solox-2.5.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: solox
-Version: 2.5.8
-Summary: SoloX - Real-time collection tool for Android/iOS performance data.
-Home-page: https://github.com/smart-test-ti/SoloX
-Author: Rafa Chen
-Author-email: rafacheninc@gamil.com
-License: MIT
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a>English</a> | <a href="./README.zh.md">中文</a>
 </p>
 
 <p align="center">
 <a href="#">
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1643364757640-b4529458-ec8d-42cc-a2d8-c0ce60fdf50f.png" alt="SoloX" width="150">
@@ -27,66 +12,85 @@
 </p>
 <p align="center">
 <a href="https://pypi.org/project/solox/" target="__blank"><img src="https://img.shields.io/pypi/v/solox" alt="solox preview"></a>
 <a href="https://pypistats.org/packages/solox" target="__blank"><img src="https://img.shields.io/pypi/dm/solox"></a>
 <br>
 </p>
 
-## Preview
+## 🔎Preview
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
-## Installation
+## 📦Requirements
+
+- Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
+
+💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
+
+💡 If Windows users need to test ios, install and start Itunes.
+
+## 📥Installation
+
+### default
 
 ```shell
-1.Python:3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
-2.pip install -U solox 
-3.pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox (China)
+pip install -U solox 
+```
 
-Note: If Windows users need to test ios, install and start Itunes
+### mirrors
+
+```shell
+pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
 
-## Startup SoloX
+💡 If your network is unable to download through [pip install -U solox], please try using mirrors to download, but the download of SoloX may not be the latest version.
+
+## 🚀Startup SoloX
 
 ### default
 
 ```shell
 python -m solox
 ```
 
 ### customize
 
 ```shell
 python -m solox --host={ip} --port={port}
 ```
 
-## Collect in python
+## 🏴󠁣󠁩󠁣󠁭󠁿Collect in python
 
 ```python
 from solox.public.apm import APM
+from solox.public.common import Devices
+
 # solox version >= 2.1.2
 
-apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True)
+d = Devices()
+pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in')
+
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True, pid=None)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
 # noLog : False (Save test data to log file)
 
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
 fps = apm.collectFps() # HZ
 battery = apm.collectBattery() # level:% temperature:°C current:mA voltage:mV power:w
 gpu = apm.collectGpu() # % only supports ios
 ```
 
-## Collect in API
+## 🏴󠁣󠁩󠁣󠁭󠁿Collect in API
 
 ### Start the service in the background
 
 ```
 # solox version >= 2.1.5
 
 macOS/Linux: nohup python3 -m solox &
@@ -98,28 +102,29 @@
 ```shell
 Android: http://{ip}:{port}/apm/collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu
 
 target in ['cpu','memory','network','fps','battery','gpu']
 ```
 
-## PK Model
-
-- 2-devices: test the same app on two different phones
-- 2-apps: test two different apps on two phones with the same configuration
-
-notice: only supports android
+## 🔥Features
 
-<img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%">
+* **No ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS devices. Efficiently solving the test and analysis challenges in Android & iOS performance.
+* **Data Integrality:** We provide the data about Screenshot, CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
+* **Beautiful report board:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
+* **Useful monitoring settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
+* **PK model:** Supports simultaneous comparative testing of two mobile devices.
+  🌱2-devices: test the same app on two different phones.
+  🌱2-apps: test two different apps on two phones with the same configuration.
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
 
 - windows: PowerShell
 - macOS：iTerm2 (https://iterm2.com/)
 
-## Thanks
+## 💕Thanks
 
 - https://github.com/alibaba/taobao-iphone-device
```

#### html2text {}

```diff
@@ -1,44 +1,51 @@
-Metadata-Version: 2.1 Name: solox Version: 2.5.8 Summary: SoloX - Real-time
-collection tool for Android/iOS performance data. Home-page: https://
-github.com/smart-test-ti/SoloX Author: Rafa Chen Author-email:
-rafacheninc@gamil.com License: MIT Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Description-
-Content-Type: text/markdown License-File: LICENSE
                                English | ä¸­æ
                                    [SoloX]
 
             [solox_preview] [https://img.shields.io/pypi/dm/solox]
-## Preview SoloX - Real-time collection tool for Android/iOS performance data.
-We are committed to solving inefficient, cumbersome test execution, and our
-goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/153412/
-1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
-process=image%2Fresize%2Cw_1500%2Climit_0] ## Installation ```shell 1.Python:
-3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
-2.pip install -U solox 3.pip install -i https://mirrors.ustc.edu.cn/pypi/web/
-simple -U solox (China) Note: If Windows users need to test ios, install and
-start Itunes ``` ## Startup SoloX ### default ```shell python -m solox ``` ###
-customize ```shell python -m solox --host={ip} --port={port} ``` ## Collect in
-python ```python from solox.public.apm import APM # solox version >= 2.1.2 apm
-= APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
-surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
-platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
-(Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
-(Save test data to log file) cpu = apm.collectCpu() # % memory =
-apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
-apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
-current:mA voltage:mV power:w gpu = apm.collectGpu() # % only supports ios ```
-## Collect in API ### Start the service in the background ``` # solox version
->= 2.1.5 macOS/Linux: nohup python3 -m solox & Windows: start /min python3 -
-m solox & ``` ### Request apm data from api ```shell Android: http://{ip}:
-{port}/apm/
+## ðPreview SoloX - Real-time collection tool for Android/iOS performance
+data. We are committed to solving inefficient, cumbersome test execution, and
+our goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/
+153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
+process=image%2Fresize%2Cw_1500%2Climit_0] ## ð¦Requirements - Install Python
+3.10 + [**Download**](https://www.python.org/downloads/) ð¡ Python 3.6 ~ 3.9
+, please download a version of solox lower than 2.5.4. ð¡ If Windows users
+need to test ios, install and start Itunes. ## ð¥Installation ### default
+```shell pip install -U solox ``` ### mirrors ```shell pip install -i https://
+mirrors.ustc.edu.cn/pypi/web/simple -U solox ``` ð¡ If your network is unable
+to download through [pip install -U solox], please try using mirrors to
+download, but the download of SoloX may not be the latest version. ##
+ðStartup SoloX ### default ```shell python -m solox ``` ### customize
+```shell python -m solox --host={ip} --port={port} ``` ##
+ð´ó £ó ©ó £ó ­ó ¿Collect in python ```python from solox.public.apm
+import APM from solox.public.common import Devices # solox version >= 2.1.2 d =
+Devices() pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in')
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
+surfaceview=True, noLog=True, pid=None) # apm = APM
+(pkgName='com.bilibili.app.in', platform='iOS') only supports one device #
+surfaceviewï¼ False = gfxinfo (Developer - GPU rendering mode - adb shell
+dumpsys gfxinfo) # noLog : False (Save test data to log file) cpu =
+apm.collectCpu() # % memory = apm.collectMemory() # MB flow = apm.collectFlow
+(wifi=True) # KB fps = apm.collectFps() # HZ battery = apm.collectBattery() #
+level:% temperature:Â°C current:mA voltage:mV power:w gpu = apm.collectGpu() #
+% only supports ios ``` ## ð´ó £ó ©ó £ó ­ó ¿Collect in API ### Start the
+service in the background ``` # solox version >= 2.1.5 macOS/Linux: nohup
+python3 -m solox & Windows: start /min python3 -m solox & ``` ### Request apm
+data from api ```shell Android: http://{ip}:{port}/apm/
 collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/
 collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu target in
-['cpu','memory','network','fps','battery','gpu'] ``` ## PK Model - 2-devices:
-test the same app on two different phones - 2-apps: test two different apps on
-two phones with the same configuration notice: only supports android [https://
-cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-
-0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0] ## Browser
-[Chrome] ## Terminal - windows: PowerShell - macOSï¼iTerm2 (https://
-iterm2.com/) ## Thanks - https://github.com/alibaba/taobao-iphone-device
+['cpu','memory','network','fps','battery','gpu'] ``` ## ð¥Features * **No
+ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS
+devices. Efficiently solving the test and analysis challenges in Android & iOS
+performance. * **Data Integrality:** We provide the data about Screenshot, CPU,
+GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get. *
+**Beautiful report board:** A beautiful and detailed report analysis, where to
+store, visualize, edit, manage, and download all the test cases collected with
+SoloX no matter where you are or when is it. * **Useful monitoring settings:**
+Support setting alarm values, collecting duration, and accessing mobile devices
+on other PC machines during the monitoring process. * **PK model:** Supports
+simultaneous comparative testing of two mobile devices. ð±2-devices: test the
+same app on two different phones. ð±2-apps: test two different apps on two
+phones with the same configuration. ## Browser [Chrome] ## Terminal - windows:
+PowerShell - macOSï¼iTerm2 (https://iterm2.com/) ## ðThanks - https://
+github.com/alibaba/taobao-iphone-device
```

### Comparing `solox-2.5.8/setup.py` & `solox-2.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/debug.py` & `solox-2.5.9/solox/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,31 +27,32 @@
 thread = True
 thread_lock = Lock()
 
 
 @socketio.on('connect', namespace='/logcat')
 def connect():
     socketio.emit('start connect', {'data': 'Connected'}, namespace='/logcat')
-    if not os.path.exists('adblog'):
-        os.mkdir('adblog')
+    logDir = os.path.join(os.getcwd(),'adblog')
+    if not os.path.exists(logDir):
+        os.mkdir(logDir)
     global thread
     thread = True
     with thread_lock:
         if thread:
             thread = socketio.start_background_task(target=backgroundThread)
 
 
 def backgroundThread():
     global thread
     try:
         current_time = time.strftime("%Y%m%d%H", time.localtime())
-        logcat = subprocess.Popen(f'adb logcat *:E > ./adblog/{current_time}_adb.log', stdout=subprocess.PIPE,
+        logPath = os.path.join(os.getcwd(),'adblog',f'{current_time}.log')
+        logcat = subprocess.Popen(f'adb logcat *:E > {logPath}', stdout=subprocess.PIPE,
                                   shell=True)
-        file = f"./adblog/{current_time}_adb.log"
-        with open(file, "r") as f:
+        with open(logPath, "r") as f:
             while thread:
                 socketio.sleep(1)
                 for line in f.readlines():
                     socketio.emit('message', {'data': line}, namespace='/logcat')
         if logcat.poll() == 0:
             thread = False
     except Exception:
```

### Comparing `solox-2.5.8/solox/public/_iosPerf.py` & `solox-2.5.9/solox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/adb/mac/adb` & `solox-2.5.9/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/adb.py` & `solox-2.5.9/solox/public/adb.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/apm.py` & `solox-2.5.9/solox/public/apm.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,23 +20,25 @@
     Battery = 'battery'
     Network = 'network'
     FPS = 'fps'
     GPU = 'gpu'
 
 class CPU(object):
 
-    def __init__(self, pkgName, deviceId, platform='Android'):
+    def __init__(self, pkgName, deviceId, platform=Platform.Android, pid=None):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
+        self.pid = pid
+        if self.pid is None and self.platform == Platform.Android:
+            self.pid = d.getPid(pkgName=self.pkgName, deviceId=self.deviceId)[0].split(':')[0]
 
     def getprocessCpuStat(self):
         """get the cpu usage of a process at a certain time"""
-        pid = d.getPid(pkgName=self.pkgName, deviceId=self.deviceId)
-        cmd = f'cat /proc/{pid}/stat'
+        cmd = f'cat /proc/{self.pid}/stat'
         result = adb.shell(cmd=cmd, deviceId=self.deviceId)
         r = re.compile("\\s+")
         toks = r.split(result)
         processCpu = float(int(toks[13]) + int(toks[14]) + int(toks[15]) + int(toks[16]))
         return processCpu
 
     def getTotalCpuStat(self):
@@ -66,59 +68,61 @@
         result = adb.shell(cmd=cmd, deviceId=self.deviceId)
         r = re.compile(r'(?<!cpu)\d+')
         toks = r.findall(result)
         ileCpu = int(toks[4])
         sysCpu = self.getTotalCpuStat() - ileCpu
         return sysCpu
 
-    def getAndroidCpuRate(self, sueApi=False):
+    def getAndroidCpuRate(self, noLog=False):
         """get the Android cpu rate of a process"""
         processCpuTime_1 = self.getprocessCpuStat()
         totalCpuTime_1 = self.getTotalCpuStat()
         sysCpuTime_1 = self.getSysCpuStat()
         time.sleep(1)
         processCpuTime_2 = self.getprocessCpuStat()
         totalCpuTime_2 = self.getTotalCpuStat()
         sysCpuTime_2 = self.getSysCpuStat()
         appCpuRate = round(float((processCpuTime_2 - processCpuTime_1) / (totalCpuTime_2 - totalCpuTime_1) * 100), 2)
         sysCpuRate = round(float((sysCpuTime_2 - sysCpuTime_1) / (totalCpuTime_2 - totalCpuTime_1) * 100), 2)
-        if sueApi is False:
+        if noLog is False:
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'cpu_app.log'), apm_time, appCpuRate)
             f.add_log(os.path.join(f.report_dir,'cpu_sys.log'), apm_time, sysCpuRate)
 
         return appCpuRate, sysCpuRate
 
-    def getiOSCpuRate(self, sueApi=False):
+    def getiOSCpuRate(self, noLog=False):
         """get the iOS cpu rate of a process, unit:%"""
         apm = iosAPM(self.pkgName)
         appCpuRate = round(float(apm.getPerformance(apm.cpu)[0]), 2)
         sysCpuRate = round(float(apm.getPerformance(apm.cpu)[1]), 2)
-        if sueApi is False:
+        if noLog is False:
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'cpu_app.log'), apm_time, appCpuRate)
             f.add_log(os.path.join(f.report_dir,'cpu_sys.log'), apm_time, sysCpuRate)
         return appCpuRate, sysCpuRate
 
     def getCpuRate(self, noLog=False):
         """Get the cpu rate of a process, unit:%"""
         appCpuRate, systemCpuRate = self.getAndroidCpuRate(noLog) if self.platform == Platform.Android else self.getiOSCpuRate(noLog)
         return appCpuRate, systemCpuRate
 
 
 class MEM(object):
-    def __init__(self, pkgName, deviceId, platform=Platform.Android):
+    def __init__(self, pkgName, deviceId, platform=Platform.Android, pid=None):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
+        self.pid = pid
+        if self.pid is None and self.platform == Platform.Android:
+            self.pid = d.getPid(pkgName=self.pkgName, deviceId=self.deviceId)[0].split(':')[0]
 
     def getAndroidMem(self):
         """Get the Android memory ,unit:MB"""
-        pid = d.getPid(pkgName=self.pkgName, deviceId=self.deviceId)
-        cmd = f'dumpsys meminfo {pid}'
+        cmd = f'dumpsys meminfo {self.pid}'
         output = adb.shell(cmd=cmd, deviceId=self.deviceId)
         m_total = re.search(r'TOTAL\s*(\d+)', output)
         m_native = re.search(r'Native Heap\s*(\d+)', output)
         m_dalvik = re.search(r'Dalvik Heap\s*(\d+)', output)
         totalPass = round(float(float(m_total.group(1))) / 1024, 2)
         nativePass = round(float(float(m_native.group(1))) / 1024, 2)
         dalvikPass = round(float(float(m_dalvik.group(1))) / 1024, 2)
@@ -196,24 +200,26 @@
         """Reset phone charging status"""
         cmd = 'dumpsys battery reset'
         adb.shell(cmd=cmd, deviceId=self.deviceId)
 
 
 class Flow(object):
 
-    def __init__(self, pkgName, deviceId, platform=Platform.Android):
+    def __init__(self, pkgName, deviceId, platform=Platform.Android, pid=None):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
+        self.pid = pid
+        if self.pid is None and self.platform == Platform.Android:
+            self.pid = d.getPid(pkgName=self.pkgName, deviceId=self.deviceId)[0].split(':')[0]
 
     def getAndroidNet(self, wifi=True):
         """Get Android send/recv data, unit:KB wlan0/rmnet0"""
         net = 'wlan0' if wifi else 'rmnet0'
-        pid = d.getPid(pkgName=self.pkgName, deviceId=self.deviceId)
-        cmd = f'cat /proc/{pid}/net/dev |{d.filterType()} {net}'
+        cmd = f'cat /proc/{self.pid}/net/dev |{d.filterType()} {net}'
         output_pre = adb.shell(cmd=cmd, deviceId=self.deviceId)
         m_pre = re.search(r'{}:\s*(\d+)\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*(\d+)'.format(net), output_pre)
         sendNum_pre = round(float(float(m_pre.group(2)) / 1024), 2)
         recNum_pre = round(float(float(m_pre.group(1)) / 1024), 2)
         time.sleep(1)
         output_final = adb.shell(cmd=cmd, deviceId=self.deviceId)
         m_final = re.search(r'{}:\s*(\d+)\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*(\d+)'.format(net), output_final)
@@ -221,16 +227,15 @@
         recNum_final = round(float(float(m_final.group(1)) / 1024), 2)
         sendNum = round(float(sendNum_final - sendNum_pre), 2)
         recNum = round(float(recNum_final - recNum_pre), 2)
         return sendNum, recNum
     
     def setAndroidNet(self, wifi=True):
         net = 'wlan0' if wifi else 'rmnet0'
-        pid = d.getPid(pkgName=self.pkgName, deviceId=self.deviceId)
-        cmd = f'cat /proc/{pid}/net/dev |{d.filterType()} {net}'
+        cmd = f'cat /proc/{self.pid}/net/dev |{d.filterType()} {net}'
         output_pre = adb.shell(cmd=cmd, deviceId=self.deviceId)
         m = re.search(r'{}:\s*(\d+)\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*(\d+)'.format(net), output_pre)
         sendNum = round(float(float(m.group(2)) / 1024), 2)
         recNum = round(float(float(m.group(1)) / 1024), 2)
         return sendNum, recNum
 
 
@@ -335,31 +340,32 @@
             perf_value = perf.start(self.pkgName, callback=self.callback)
         return perf_value
 
 
 class APM(object):
     """for python api"""
 
-    def __init__(self, pkgName, deviceId='', platform=Platform.Android, surfaceview=True, noLog=True):
+    def __init__(self, pkgName, deviceId=None, platform=Platform.Android, surfaceview=True, noLog=True, pid=None):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
         self.surfaceview = surfaceview
         self.noLog = noLog
+        self.pid = pid
         d.devicesCheck(platform=self.platform, deviceid=self.deviceId, pkgname=self.pkgName)
 
     def collectCpu(self):
-        _cpu = CPU(self.pkgName, self.deviceId, self.platform)
+        _cpu = CPU(self.pkgName, self.deviceId, self.platform, pid=self.pid)
         appCpuRate, systemCpuRate = _cpu.getCpuRate(noLog=self.noLog)
         result = {'appCpuRate': appCpuRate, 'systemCpuRate': systemCpuRate}
         logger.info(f'cpu: {result}')
         return result
 
     def collectMemory(self):
-        _memory = MEM(self.pkgName, self.deviceId, self.platform)
+        _memory = MEM(self.pkgName, self.deviceId, self.platform, pid=self.pid)
         totalPass, nativePass, dalvikPass = _memory.getProcessMem(noLog=self.noLog)
         result = {'totalPass': totalPass, 'nativePass': nativePass, 'dalvikPass': dalvikPass}
         logger.info(f'memory: {result}')
         return result
 
     def collectBattery(self):
         _battery = Battery(self.deviceId, self.platform)
@@ -368,15 +374,15 @@
             result = {'level': final[0], 'temperature': final[1]}
         else:
             result = {'temperature': final[0], 'current': final[1], 'voltage': final[2], 'power': final[3]}
         logger.info(f'battery: {result}')
         return result
 
     def collectFlow(self, wifi=True):
-        _flow = Flow(self.pkgName, self.deviceId, self.platform)
+        _flow = Flow(self.pkgName, self.deviceId, self.platform, pid=self.pid)
         upFlow, downFlow = _flow.getNetWorkData(wifi=wifi,noLog=self.noLog)
         result = {'upFlow': upFlow, 'downFlow': downFlow}
         logger.info(f'network: {result}')
         return result
 
     def collectFps(self):
         _fps = FPS(self.pkgName, self.deviceId, self.platform, self.surfaceview)
```

### Comparing `solox-2.5.8/solox/public/apm_pk.py` & `solox-2.5.9/solox/public/apm_pk.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/common.py` & `solox-2.5.9/solox/public/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,22 @@
         else:
             deviceId = deviceinfo.split(':')[1]
         return deviceId
 
     def getPid(self, deviceId, pkgName):
         """Get the pid corresponding to the Android package name"""
         result = os.popen(f"{self.adb} -s {deviceId} shell ps -ef | {self.filterType()} {pkgName}").readlines()
-        flag = len(result) > 0
         try:
-            pid = (0, result[0].split()[1])[flag]
+            processList = []
+            for process in result:
+                processInfo = '{}:{}'.format(process.split()[1],process.split()[7])
+                processList.append(processInfo)
         except Exception:
-            pid = None
-        return pid
+            logger.error('no pid found')
+        return processList
 
     def checkPkgname(self, pkgname):
         flag = True
         replace_list = ['com.google']
         for i in replace_list:
             if i in pkgname:
                 flag = False
```

### Comparing `solox-2.5.8/solox/public/fps.py` & `solox-2.5.9/solox/public/fps.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/__main__.py` & `solox-2.5.9/solox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_crash.py` & `solox-2.5.9/solox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_device.py` & `solox-2.5.9/solox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_hexdump.py` & `solox-2.5.9/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_imagemounter.py` & `solox-2.5.9/solox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_installation.py` & `solox-2.5.9/solox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_instruments.py` & `solox-2.5.9/solox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_ipautil.py` & `solox-2.5.9/solox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_perf.py` & `solox-2.5.9/solox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_proto.py` & `solox-2.5.9/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_relay.py` & `solox-2.5.9/solox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_safe_socket.py` & `solox-2.5.9/solox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_ssl.py` & `solox-2.5.9/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_sync.py` & `solox-2.5.9/solox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_types.py` & `solox-2.5.9/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_usbmux.py` & `solox-2.5.9/solox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_utils.py` & `solox-2.5.9/solox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/_wdaproxy.py` & `solox-2.5.9/solox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/bplist.py` & `solox-2.5.9/solox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/exceptions.py` & `solox-2.5.9/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/plistlib2.py` & `solox-2.5.9/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/requests_usbmux.py` & `solox-2.5.9/solox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/public/iosperf/struct2.py` & `solox-2.5.9/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/css/highlight.min.css` & `solox-2.5.9/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.5.9/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.5.9/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/css/select2.min.css` & `solox-2.5.9/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/css/sweetalert2.min.css` & `solox-2.5.9/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/css/tabler.demo.min.css` & `solox-2.5.9/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/css/tabler.min.css` & `solox-2.5.9/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/image/404.png` & `solox-2.5.9/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/image/500.png` & `solox-2.5.9/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/image/avatar.png` & `solox-2.5.9/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/image/coffee.png` & `solox-2.5.9/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/image/empty.png` & `solox-2.5.9/solox/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/image/readme/home.png` & `solox-2.5.9/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/image/readme/pk.png` & `solox-2.5.9/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/apexcharts.js` & `solox-2.5.9/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/gray.js` & `solox-2.5.9/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/highlight.min.js` & `solox-2.5.9/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/highstock.js` & `solox-2.5.9/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/html2canvas.min.js` & `solox-2.5.9/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/jquery.min.js` & `solox-2.5.9/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/select2.min.js` & `solox-2.5.9/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/socket.io.js` & `solox-2.5.9/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/sweetalert2.min.js` & `solox-2.5.9/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/tabler.demo.min.js` & `solox-2.5.9/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/js/tabler.min.js` & `solox-2.5.9/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/static/logo/logo.png` & `solox-2.5.9/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/templates/404.html` & `solox-2.5.9/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/templates/500.html` & `solox-2.5.9/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/templates/analysis.html` & `solox-2.5.9/solox/templates/analysis.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/templates/analysis_pk.html` & `solox-2.5.9/solox/templates/analysis_pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/templates/base.html` & `solox-2.5.9/solox/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/smart-test-ti" class="link-secondary">SoloX</a>.{% if lan == 'cn' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.5.8
+                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.5.9
                             </a>
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'cn'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
     * _{%_if_lan_==_'cn'_%}_åæ¯åå¡_{%_else_%}_Sponsor_{%_endif_%}
     * Copyright ©  SoloX.{% if lan == 'cn' %} ä¿çæææå© {% else %} All
       rights reserved {% endif %}
-    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.5.8
+    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.5.9
 *****  {% if lan == 'cn' %} è®¾ç½® {% else %} Setting {% endif %} *****
     * Warning_Value
     * Timer
     * Agent_ _{%_if_lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'cn' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [{
 { cpuWarning }}    ]
 {% if lan == 'cn' %} åå­åè­¦å¼ {% else %} Memory warning value {% endif
```

### Comparing `solox-2.5.8/solox/templates/index.html` & `solox-2.5.9/solox/templates/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -89,24 +89,36 @@
                 </div>
                 {% if lan == 'cn' %}
                 <select  class="select-device select2-selection--single" data-placeholder="请选择一台设备"></select>
                 {% else %}
                 <select  class="select-device select2-selection--single" data-placeholder="Please select a device"></select>
                 {% endif %}
             </div>
-            <div class="input-group" style="width: 93%;margin-left: 10px;">
+            <div class="input-group mb-3" style="width: 93%;margin-left: 10px;">
                 <div class="input-group-text">
                     <svg t="1645171258689" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2225" width="2000" height="2000"><path d="M352 96H224c-70.4 0-128 57.6-128 128v128c0 70.4 57.6 128 128 128h192c35.2 0 64-28.8 64-64V224c0-70.4-57.6-128-128-128z m64 319.9l-0.1 0.1H224c-17 0-33-6.7-45.1-18.9S160 369 160 352V224c0-17 6.7-33 18.9-45.1S207 160 224 160h128c17 0 33 6.7 45.1 18.9S416 207 416 224v191.9zM800 96H672c-70.4 0-128 57.6-128 128v192c0 35.2 28.8 64 64 64h192c70.4 0 128-57.6 128-128V224c0-70.4-57.6-128-128-128z m64 256c0 17-6.7 33-18.9 45.1S817 416 800 416H608.1l-0.1-0.1V224c0-17 6.7-33 18.9-45.1S655 160 672 160h128c17 0 33 6.7 45.1 18.9S864 207 864 224v128zM416 544H224c-70.4 0-128 57.6-128 128v128c0 70.4 57.6 128 128 128h128c70.4 0 128-57.6 128-128V608c0-35.2-28.8-64-64-64z m0 256c0 17-6.7 33-18.9 45.1S369 864 352 864H224c-17 0-33-6.7-45.1-18.9S160 817 160 800V672c0-17 6.7-33 18.9-45.1S207 608 224 608h191.9l0.1 0.1V800zM800 544H608c-35.2 0-64 28.8-64 64v192c0 70.4 57.6 128 128 128h128c70.4 0 128-57.6 128-128V672c0-70.4-57.6-128-128-128z m64 256c0 17-6.7 33-18.9 45.1S817 864 800 864H672c-17 0-33-6.7-45.1-18.9S608 817 608 800V608.1l0.1-0.1H800c17 0 33 6.7 45.1 18.9S864 655 864 672v128z" fill="#1875F0" p-id="2226"></path></svg>
                 </div>
                 {% if lan == 'cn' %}
                 <select  class="select-app select2-selection--single" data-placeholder="请选择一个APP"></select>
                 {% else %}
                 <select  class="select-app select2-selection--single" data-placeholder="Please select a package"></select>
                 {% endif %}
             </div>
+            {% if platform == 'Android' %}
+            <div class="input-group" style="width: 93%;margin-left: 10px;">
+                <div class="input-group-text">
+                    <svg t="1681890999535" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5737" width="50" height="50"><path d="M512 64.303538c-247.254314 0-447.696462 200.438055-447.696462 447.696462s200.442148 447.696462 447.696462 447.696462c247.258407 0 447.696462-200.438055 447.696462-447.696462S759.258407 64.303538 512 64.303538zM512 914.925792c-222.532259 0-402.926816-180.394556-402.926816-402.926816 0-222.532259 180.394556-402.926816 402.926816-402.926816 222.527143 0 402.926816 180.394556 402.926816 402.926816C914.926816 734.531236 734.528166 914.925792 512 914.925792zM512 243.382123c-148.352793 0-268.617877 120.265084-268.617877 268.617877s120.265084 268.617877 268.617877 268.617877 268.617877-120.265084 268.617877-268.617877S660.353816 243.382123 512 243.382123z" p-id="5738" data-spm-anchor-id="a313x.7781069.0.i3" class="selected" fill="#d81e06"></path></svg>
+                </div>
+                {% if lan == 'cn' %}
+                <select  class="select-pid select2-selection--single" data-placeholder="请选择一个进程"></select>
+                {% else %}
+                <select  class="select-pid select2-selection--single" data-placeholder="Please select a process"></select>
+                {% endif %}
+            </div>
+            {% endif %}
             <div class="card" style="margin-top: 13px;">
                 <div class="card-header">
                     <ul class="nav nav-tabs card-header-tabs" data-bs-toggle="tabs">
                         <li class="nav-item">
                             <a href="#tabs-apm-target" class="nav-link active" data-bs-toggle="tab">
                                 {% if lan == 'cn' %} 性能指标 {% else %} APM TARGET {% endif %}
                             </a>
@@ -307,14 +319,52 @@
                     }
                     swal.close();
                 }
             }
         });
     });
 
+    $('.select-app').change(function() {
+        $.ajax({
+            url: Host + "/package/pids",
+            type: "GET",
+            async: true,
+            cache: false,
+            data:{
+                platform:platform,
+                device:$('.select-device').val(),
+                pkgname:this.value
+            },
+            beforeSend: function () {
+                $('.select-pid').empty();
+                $('.select-pid').append('<option></option>');
+                if(lan == 'cn' ){
+                    SwalLoading('初始化','正在获取该APP上的所有进程, 请您稍等！');
+                }else{
+                    SwalLoading('Process initialization!','Initializing Process, please wait a mmoment.');
+                }
+                
+            },
+            success: function (data) {
+                if(data['status'] != 1 ) {
+                    if(lan == 'cn' ){
+                        SwalFire('error', '连接失败','请检查当前移动设备的是否连接了PC端', 2000);
+                    }else{
+                        SwalFire('error', 'Connet failed !', 'No pid found', 2000);
+                    } 
+                }else{
+                    for(var i=0;i<data['pids'].length;i++){
+                        $('.select-pid').append('<option>'+data['pids'][i]+'</option>')
+                    }
+                    swal.close();
+                }
+            }
+        });
+    });
+
 
     function initializeAPM(){
         $.ajax({
             url: Host + "/apm/initialize",
             type: "POST",
             async: true,
             cache: false,
@@ -377,15 +427,16 @@
             type: "GET",
             async: true,
             cache: false,
             data:{
                 model:'normal',
                 platform:platform,
                 pkgname:pkgname,
-                device:device
+                device:device,
+                process:$('.select-pid').val()
             },
             beforeSend: function () {
                window.clearTimeout(timerQ);
             },
             success: function (data) {
                 console.log(data)
                 if(stop == false){
@@ -506,15 +557,16 @@
             type: "GET",
             async: true,
             cache: false,
             data:{
                 model:'normal',
                 platform:platform,
                 pkgname:pkgname,
-                device:device
+                device:device,
+                process:$('.select-pid').val()
             },
             beforeSend: function () {
                window.clearTimeout(timerQ);
             },
             success: function (data) {
                 console.log(data)
                 if(stop == false){
@@ -558,15 +610,16 @@
             async: true,
             cache: false,
             data:{
                 platform:platform,
                 pkgname:pkgname,
                 device:device,
                 wifi_switch: net_switch,
-                type: type
+                type: type,
+                process:$('.select-pid').val()
             },
             success: function (data) {
                 if(data['status'] != 1){
                     SwalFire('error','something error',data['msg'],2000);
                 }
             },
             error: function(){
@@ -582,15 +635,16 @@
             async: true,
             cache: false,
             data:{
                 model:'normal',
                 platform:platform,
                 pkgname:pkgname,
                 device:device,
-                wifi_switch: net_switch
+                wifi_switch: net_switch,
+                process:$('.select-pid').val()
             },
             beforeSend: function () {
                window.clearTimeout(timerQ);
             },
             success: function (data) {
                 if(stop == false){
                     if(data['status'] == 1){
@@ -1250,15 +1304,16 @@
             async: true,
             cache: false,
             data:{
                 platform:platform,
                 model:'normal',
                 app:$('.select-app').val(),
                 devices:$('.select-device').val(),
-                wifi_switch:wifi_switch
+                wifi_switch:wifi_switch,
+                process:$('.select-pid').val()
             },
             beforeSend: function () {
                 
                 if(lan == 'cn'){
                     SwalLoading('保存数据','正在保存数据生成报告, 请不要离开页面.')
                 }else{
                     SwalLoading('Save data','Saving data to generate report, please do not leave.')
```

### Comparing `solox-2.5.8/solox/templates/pk.html` & `solox-2.5.9/solox/templates/pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/templates/report.html` & `solox-2.5.9/solox/templates/report.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/view/apis.py` & `solox-2.5.9/solox/view/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 devices = d.getDevices()
                 if len(deviceids) > 0:
                     pkgnames = d.getPkgname(deviceids[0])
                     device_detail = d.getDdeviceDetail(deviceId=deviceids[0], platform=platform)
                     result = {'status': 1, 
                               'deviceids': deviceids, 
                               'devices': devices,
-                              'pkgnames': pkgnames, 
+                              'pkgnames': pkgnames,
                               'device_detail': device_detail}
                 else:
                     result = {'status': 0, 'msg': 'no devices'}
             case Platform.iOS:
                 deviceinfos = d.getDeviceInfoByiOS()
                 if len(deviceinfos) > 0:
                     pkgnames = d.getPkgnameByiOS(deviceinfos[0].split(':')[1])
@@ -112,21 +112,36 @@
         case _:
             result = {'status': 0, 'msg': 'platform is undefined'}
             return result
     result = {'status': 1, 'pkgnames': pkgnames} if len(pkgnames) > 0 else  {'status': 0, 'msg': 'no pkgnames'} 
     return result
 
 
+@api.route('/package/pids', methods=['post', 'get'])
+def getPackagePids():
+    platform = method._request(request, 'platform')
+    device = method._request(request, 'device')
+    pkgname = method._request(request, 'pkgname')
+    try:
+        deviceId = d.getIdbyDevice(device, platform)
+        pids = d.getPid(deviceId, pkgname)
+        result = {'status': 1, 'pids': pids} 
+    except Exception:
+        traceback.print_exc()
+        result = {'status': 0, 'msg': 'no pid found'} 
+    return result        
+
 @api.route('/apm/cpu', methods=['post', 'get'])
 def getCpuRate():
     """get process cpu rate"""
     model = method._request(request, 'model')
     platform = method._request(request, 'platform')
     pkgname = method._request(request, 'pkgname')
     device = method._request(request, 'device')
+    process = method._request(request, 'process')
     try:
         match(model):
             case '2-devices':
                 pkgNameList = []
                 pkgNameList.append(pkgname)
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
@@ -138,15 +153,16 @@
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 cpu = CPU_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = cpu.getAndroidCpuRate()
                 result = {'status': 1, 'first': first, 'second': second}
             case _:
                 deviceId = d.getIdbyDevice(device, platform)
-                cpu = CPU(pkgName=pkgname, deviceId=deviceId, platform=platform)
+                pid = process.split(':')[0] if platform == Platform.Android else None
+                cpu = CPU(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
                 appCpuRate, systemCpuRate = cpu.getCpuRate()
                 result = {'status': 1, 'appCpuRate': appCpuRate, 'systemCpuRate': systemCpuRate}        
     except Exception:
         logger.error('get cpu failed')
         traceback.print_exc()
         result = {'status': 1, 'appCpuRate': 0, 'systemCpuRate': 0, 'first': 0, 'second': 0}
     return result
@@ -155,14 +171,15 @@
 @api.route('/apm/mem', methods=['post', 'get'])
 def getMEM():
     """get memery data"""
     model = method._request(request, 'model')
     platform = method._request(request, 'platform')
     pkgname = method._request(request, 'pkgname')
     device = method._request(request, 'device')
+    process = method._request(request, 'process')
     try:
         match(model):
             case '2-devices':
                 pkgNameList = []
                 pkgNameList.append(pkgname)
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
@@ -174,15 +191,16 @@
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 mem = MEM_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = mem.getProcessMem()
                 result = {'status': 1, 'first': first, 'second': second}
             case _:
                 deviceId = d.getIdbyDevice(device, platform)
-                mem = MEM(pkgName=pkgname, deviceId=deviceId, platform=platform)
+                pid = process.split(':')[0] if platform == Platform.Android else None
+                mem = MEM(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
                 totalPass, nativePass, dalvikPass = mem.getProcessMem()
                 result = {'status': 1, 'totalPass': totalPass, 'nativePass': nativePass, 'dalvikPass': dalvikPass}        
     except Exception:
         logger.error('get memory data failed')
         traceback.print_exc()
         result = {'status': 1, 'totalPass': 0, 'nativePass': 0, 'dalvikPass': 0, 'first': 0, 'second': 0}
     return result
@@ -191,18 +209,20 @@
 def setNetWorkData():
     """set network data"""
     platform = method._request(request, 'platform')
     pkgname = method._request(request, 'pkgname')
     device = method._request(request, 'device')
     wifi_switch = method._request(request, 'wifi_switch')
     type = method._request(request, 'type')
+    process = method._request(request, 'process')
     try:
         wifi = False if wifi_switch == 'false' else True
         deviceId = d.getIdbyDevice(device, platform)
-        flow = Flow(pkgName=pkgname, deviceId=deviceId, platform=platform)
+        pid = process.split(':')[0] if platform == Platform.Android else None
+        flow = Flow(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
         data = flow.setAndroidNet(wifi=wifi)
         f.record_net(type, data[0], data[1])
         result = {'status': 1, 'msg':'set network data success'}
     except Exception as e:
         traceback.print_exc()
         result = {'status': 0, 'msg':'set network data failed'}
     return result        
@@ -211,14 +231,15 @@
 def getNetWorkData():
     """get network data"""
     model = method._request(request, 'model')
     platform = method._request(request, 'platform')
     pkgname = method._request(request, 'pkgname')
     device = method._request(request, 'device')
     wifi_switch = method._request(request, 'wifi_switch')
+    process = method._request(request, 'process')
     try:
         wifi = False if wifi_switch == 'false' else True
         match(model):
             case '2-devices':
                 pkgNameList = []
                 pkgNameList.append(pkgname)
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
@@ -231,15 +252,16 @@
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 network = Flow_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = network.getNetWorkData()
                 result = {'status': 1, 'first': first, 'second': second}
             case _:
                 deviceId = d.getIdbyDevice(device, platform)
-                flow = Flow(pkgName=pkgname, deviceId=deviceId, platform=platform)
+                pid = process.split(':')[0] if platform == Platform.Android else None
+                flow = Flow(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
                 data = flow.getNetWorkData(wifi=wifi,noLog=False)
                 result = {'status': 1, 'upflow': data[0], 'downflow': data[1]}    
     except Exception:
         logger.error('get network data failed')
         traceback.print_exc()
         result = {'status': 1, 'upflow': 0, 'downflow': 0, 'first': 0, 'second': 0}    
     return result
@@ -325,27 +347,31 @@
     """Create test report records"""
     current_time = time.strftime("%Y-%m-%d-%H-%M-%S", time.localtime())
     platform = method._request(request, 'platform')
     app = method._request(request, 'app')
     model = method._request(request, 'model')
     devices = method._request(request, 'devices')
     wifi_switch = method._request(request, 'wifi_switch')
+    process = method._request(request, 'process')
     try:
         if platform == Platform.Android:
             deviceId = d.getIdbyDevice(devices, platform)
             battery_monitor = Battery(deviceId=deviceId)
             battery_monitor.recoverBattery()
             wifi = False if wifi_switch == 'false' else True
             deviceId = d.getIdbyDevice(devices, platform)
-            flow = Flow(pkgName=app, deviceId=deviceId, platform=platform)
+            pid = process.split(':')[0] if platform == Platform.Android else None
+            flow = Flow(pkgName=app, deviceId=deviceId, platform=platform, pid=pid)
             data = flow.setAndroidNet(wifi=wifi)
             f.record_net('end', data[0], data[1])
+            app = process
         file(fileroot=f'apm_{current_time}').make_report(app=app, devices=devices, platform=platform, model=model)
         result = {'status': 1}
     except Exception as e:
+        traceback.print_exc()
         result = {'status': 0, 'msg': str(e)}
     return result
 
 
 @api.route('/apm/edit/report', methods=['post', 'get'])
 def editReport():
     """Edit test report records"""
```

### Comparing `solox-2.5.8/solox/view/pages.py` & `solox-2.5.9/solox/view/pages.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.8/solox/web.py` & `solox-2.5.9/solox/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,31 +25,32 @@
 thread = True
 thread_lock = Lock()
 
 
 @socketio.on('connect', namespace='/logcat')
 def connect():
     socketio.emit('start connect', {'data': 'Connected'}, namespace='/logcat')
-    if not os.path.exists('adblog'):
-        os.mkdir('adblog')
+    logDir = os.path.join(os.getcwd(),'adblog')
+    if not os.path.exists(logDir):
+        os.mkdir(logDir)
     global thread
     thread = True
     with thread_lock:
         if thread:
             thread = socketio.start_background_task(target=backgroundThread)
 
 
 def backgroundThread():
     global thread
     try:
         current_time = time.strftime("%Y%m%d%H", time.localtime())
-        logcat = subprocess.Popen(f'adb logcat *:E > ./adblog/{current_time}_adb.log', stdout=subprocess.PIPE,
+        logPath = os.path.join(os.getcwd(),'adblog',f'{current_time}.log')
+        logcat = subprocess.Popen(f'adb logcat *:E > {logPath}', stdout=subprocess.PIPE,
                                   shell=True)
-        file = f"./adblog/{current_time}_adb.log"
-        with open(file, "r") as f:
+        with open(logPath, "r") as f:
             while thread:
                 socketio.sleep(1)
                 for line in f.readlines():
                     socketio.emit('message', {'data': line}, namespace='/logcat')
         if logcat.poll() == 0:
             thread = False
     except Exception:
```

### Comparing `solox-2.5.8/solox.egg-info/PKG-INFO` & `solox-2.5.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.5.8
+Version: 2.5.9
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -27,66 +27,85 @@
 </p>
 <p align="center">
 <a href="https://pypi.org/project/solox/" target="__blank"><img src="https://img.shields.io/pypi/v/solox" alt="solox preview"></a>
 <a href="https://pypistats.org/packages/solox" target="__blank"><img src="https://img.shields.io/pypi/dm/solox"></a>
 <br>
 </p>
 
-## Preview
+## 🔎Preview
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
-## Installation
+## 📦Requirements
+
+- Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
+
+💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
+
+💡 If Windows users need to test ios, install and start Itunes.
+
+## 📥Installation
+
+### default
 
 ```shell
-1.Python:3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
-2.pip install -U solox 
-3.pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox (China)
+pip install -U solox 
+```
 
-Note: If Windows users need to test ios, install and start Itunes
+### mirrors
+
+```shell
+pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
 
-## Startup SoloX
+💡 If your network is unable to download through [pip install -U solox], please try using mirrors to download, but the download of SoloX may not be the latest version.
+
+## 🚀Startup SoloX
 
 ### default
 
 ```shell
 python -m solox
 ```
 
 ### customize
 
 ```shell
 python -m solox --host={ip} --port={port}
 ```
 
-## Collect in python
+## 🏴󠁣󠁩󠁣󠁭󠁿Collect in python
 
 ```python
 from solox.public.apm import APM
+from solox.public.common import Devices
+
 # solox version >= 2.1.2
 
-apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True)
+d = Devices()
+pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in')
+
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True, pid=None)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
 # noLog : False (Save test data to log file)
 
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
 fps = apm.collectFps() # HZ
 battery = apm.collectBattery() # level:% temperature:°C current:mA voltage:mV power:w
 gpu = apm.collectGpu() # % only supports ios
 ```
 
-## Collect in API
+## 🏴󠁣󠁩󠁣󠁭󠁿Collect in API
 
 ### Start the service in the background
 
 ```
 # solox version >= 2.1.5
 
 macOS/Linux: nohup python3 -m solox &
@@ -98,28 +117,29 @@
 ```shell
 Android: http://{ip}:{port}/apm/collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu
 
 target in ['cpu','memory','network','fps','battery','gpu']
 ```
 
-## PK Model
-
-- 2-devices: test the same app on two different phones
-- 2-apps: test two different apps on two phones with the same configuration
-
-notice: only supports android
+## 🔥Features
 
-<img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%">
+* **No ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS devices. Efficiently solving the test and analysis challenges in Android & iOS performance.
+* **Data Integrality:** We provide the data about Screenshot, CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
+* **Beautiful report board:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
+* **Useful monitoring settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
+* **PK model:** Supports simultaneous comparative testing of two mobile devices.
+  🌱2-devices: test the same app on two different phones.
+  🌱2-apps: test two different apps on two phones with the same configuration.
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
 
 - windows: PowerShell
 - macOS：iTerm2 (https://iterm2.com/)
 
-## Thanks
+## 💕Thanks
 
 - https://github.com/alibaba/taobao-iphone-device
```

#### html2text {}

```diff
@@ -1,44 +1,58 @@
-Metadata-Version: 2.1 Name: solox Version: 2.5.8 Summary: SoloX - Real-time
+Metadata-Version: 2.1 Name: solox Version: 2.5.9 Summary: SoloX - Real-time
 collection tool for Android/iOS performance data. Home-page: https://
 github.com/smart-test-ti/SoloX Author: Rafa Chen Author-email:
 rafacheninc@gamil.com License: MIT Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE
                                English | ä¸­æ
                                    [SoloX]
 
             [solox_preview] [https://img.shields.io/pypi/dm/solox]
-## Preview SoloX - Real-time collection tool for Android/iOS performance data.
-We are committed to solving inefficient, cumbersome test execution, and our
-goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/153412/
-1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
-process=image%2Fresize%2Cw_1500%2Climit_0] ## Installation ```shell 1.Python:
-3.10+ (Python 3.6 ~ 3.9 Please download a version of solox lower than 2.5.4)
-2.pip install -U solox 3.pip install -i https://mirrors.ustc.edu.cn/pypi/web/
-simple -U solox (China) Note: If Windows users need to test ios, install and
-start Itunes ``` ## Startup SoloX ### default ```shell python -m solox ``` ###
-customize ```shell python -m solox --host={ip} --port={port} ``` ## Collect in
-python ```python from solox.public.apm import APM # solox version >= 2.1.2 apm
-= APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
-surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
-platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
-(Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
-(Save test data to log file) cpu = apm.collectCpu() # % memory =
-apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
-apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
-current:mA voltage:mV power:w gpu = apm.collectGpu() # % only supports ios ```
-## Collect in API ### Start the service in the background ``` # solox version
->= 2.1.5 macOS/Linux: nohup python3 -m solox & Windows: start /min python3 -
-m solox & ``` ### Request apm data from api ```shell Android: http://{ip}:
-{port}/apm/
+## ðPreview SoloX - Real-time collection tool for Android/iOS performance
+data. We are committed to solving inefficient, cumbersome test execution, and
+our goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/
+153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
+process=image%2Fresize%2Cw_1500%2Climit_0] ## ð¦Requirements - Install Python
+3.10 + [**Download**](https://www.python.org/downloads/) ð¡ Python 3.6 ~ 3.9
+, please download a version of solox lower than 2.5.4. ð¡ If Windows users
+need to test ios, install and start Itunes. ## ð¥Installation ### default
+```shell pip install -U solox ``` ### mirrors ```shell pip install -i https://
+mirrors.ustc.edu.cn/pypi/web/simple -U solox ``` ð¡ If your network is unable
+to download through [pip install -U solox], please try using mirrors to
+download, but the download of SoloX may not be the latest version. ##
+ðStartup SoloX ### default ```shell python -m solox ``` ### customize
+```shell python -m solox --host={ip} --port={port} ``` ##
+ð´ó £ó ©ó £ó ­ó ¿Collect in python ```python from solox.public.apm
+import APM from solox.public.common import Devices # solox version >= 2.1.2 d =
+Devices() pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in')
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
+surfaceview=True, noLog=True, pid=None) # apm = APM
+(pkgName='com.bilibili.app.in', platform='iOS') only supports one device #
+surfaceviewï¼ False = gfxinfo (Developer - GPU rendering mode - adb shell
+dumpsys gfxinfo) # noLog : False (Save test data to log file) cpu =
+apm.collectCpu() # % memory = apm.collectMemory() # MB flow = apm.collectFlow
+(wifi=True) # KB fps = apm.collectFps() # HZ battery = apm.collectBattery() #
+level:% temperature:Â°C current:mA voltage:mV power:w gpu = apm.collectGpu() #
+% only supports ios ``` ## ð´ó £ó ©ó £ó ­ó ¿Collect in API ### Start the
+service in the background ``` # solox version >= 2.1.5 macOS/Linux: nohup
+python3 -m solox & Windows: start /min python3 -m solox & ``` ### Request apm
+data from api ```shell Android: http://{ip}:{port}/apm/
 collect?platform=Android&deviceid=ca6bd5a5&pkgname=com.bilibili.app.in&target=cpu
 iOS: http://{ip}:{port}/apm/
 collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu target in
-['cpu','memory','network','fps','battery','gpu'] ``` ## PK Model - 2-devices:
-test the same app on two different phones - 2-apps: test two different apps on
-two phones with the same configuration notice: only supports android [https://
-cdn.nlark.com/yuque/0/2022/png/153412/1662348055024-96e38b5e-d6b4-4a06-8070-
-0707e2fbcd99.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0] ## Browser
-[Chrome] ## Terminal - windows: PowerShell - macOSï¼iTerm2 (https://
-iterm2.com/) ## Thanks - https://github.com/alibaba/taobao-iphone-device
+['cpu','memory','network','fps','battery','gpu'] ``` ## ð¥Features * **No
+ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS
+devices. Efficiently solving the test and analysis challenges in Android & iOS
+performance. * **Data Integrality:** We provide the data about Screenshot, CPU,
+GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get. *
+**Beautiful report board:** A beautiful and detailed report analysis, where to
+store, visualize, edit, manage, and download all the test cases collected with
+SoloX no matter where you are or when is it. * **Useful monitoring settings:**
+Support setting alarm values, collecting duration, and accessing mobile devices
+on other PC machines during the monitoring process. * **PK model:** Supports
+simultaneous comparative testing of two mobile devices. ð±2-devices: test the
+same app on two different phones. ð±2-apps: test two different apps on two
+phones with the same configuration. ## Browser [Chrome] ## Terminal - windows:
+PowerShell - macOSï¼iTerm2 (https://iterm2.com/) ## ðThanks - https://
+github.com/alibaba/taobao-iphone-device
```

### Comparing `solox-2.5.8/solox.egg-info/SOURCES.txt` & `solox-2.5.9/solox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

