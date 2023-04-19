# Comparing `tmp/friebox-1.0.0.tar.gz` & `tmp/friebox-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "friebox-1.0.0.tar", last modified: Wed Apr 19 05:30:47 2023, max compression
+gzip compressed data, was "friebox-1.0.1.tar", last modified: Wed Apr 19 05:50:37 2023, max compression
```

## Comparing `friebox-1.0.0.tar` & `friebox-1.0.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.114318 friebox-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-19 05:30:34.000000 friebox-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 05:30:34.000000 friebox-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-19 05:30:47.114318 friebox-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-19 05:30:34.000000 friebox-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.082318 friebox-1.0.0/friebox/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.086318 friebox-1.0.0/friebox/public/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.082318 friebox-1.0.0/friebox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.086318 friebox-1.0.0/friebox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)  7933192 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.094318 friebox-1.0.0/friebox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.094318 friebox-1.0.0/friebox/public/adb/mac/
--rw-r--r--   0 runner    (1001) docker     (123)  7328624 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.098318 friebox-1.0.0/friebox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)    97792 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)    62976 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)  5992960 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23827 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.110318 friebox-1.0.0/friebox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30524 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41196 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39321 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31553 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.082318 friebox-1.0.0/friebox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.110318 friebox-1.0.0/friebox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.110318 friebox-1.0.0/friebox/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/images/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/images/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/images/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/images/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/images/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.114318 friebox-1.0.0/friebox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.114318 friebox-1.0.0/friebox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    47111 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    38304 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    88932 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55724 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.114318 friebox-1.0.0/friebox/view/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23190 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-19 05:30:34.000000 friebox-1.0.0/friebox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:30:47.086318 friebox-1.0.0/friebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-19 05:30:47.000000 friebox-1.0.0/friebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-19 05:30:47.000000 friebox-1.0.0/friebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 05:30:47.000000 friebox-1.0.0/friebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-19 05:30:47.000000 friebox-1.0.0/friebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 05:30:47.000000 friebox-1.0.0/friebox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 05:30:47.114318 friebox-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-19 05:30:34.000000 friebox-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.309948 friebox-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-19 05:50:24.000000 friebox-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 05:50:24.000000 friebox-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 05:50:37.309948 friebox-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-19 05:50:24.000000 friebox-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.277947 friebox-1.0.1/friebox/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 05:50:24.000000 friebox-1.0.1/friebox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 05:50:24.000000 friebox-1.0.1/friebox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-19 05:50:24.000000 friebox-1.0.1/friebox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.277947 friebox-1.0.1/friebox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-19 05:50:24.000000 friebox-1.0.1/friebox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-19 05:50:24.000000 friebox-1.0.1/friebox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.273947 friebox-1.0.1/friebox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.277947 friebox-1.0.1/friebox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)  7933192 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.285947 friebox-1.0.1/friebox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.285947 friebox-1.0.1/friebox/public/adb/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)  7328624 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.293947 friebox-1.0.1/friebox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)    97792 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    62976 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)  5992960 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-19 05:50:24.000000 friebox-1.0.1/friebox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23827 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.305947 friebox-1.0.1/friebox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30524 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41196 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39321 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31553 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.273947 friebox-1.0.1/friebox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.305947 friebox-1.0.1/friebox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.305947 friebox-1.0.1/friebox/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/images/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/images/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/images/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/images/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/images/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.309948 friebox-1.0.1/friebox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.309948 friebox-1.0.1/friebox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    47111 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38304 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    88932 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55724 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.309948 friebox-1.0.1/friebox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23190 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-19 05:50:25.000000 friebox-1.0.1/friebox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:50:37.277947 friebox-1.0.1/friebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 05:50:37.000000 friebox-1.0.1/friebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-19 05:50:37.000000 friebox-1.0.1/friebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 05:50:37.000000 friebox-1.0.1/friebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-19 05:50:37.000000 friebox-1.0.1/friebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 05:50:37.000000 friebox-1.0.1/friebox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 05:50:37.313948 friebox-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-19 05:50:25.000000 friebox-1.0.1/setup.py
```

### Comparing `friebox-1.0.0/LICENSE` & `friebox-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/PKG-INFO` & `friebox-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: friebox
-Version: 1.0.0
+Version: 1.0.1
 Summary: friebox - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/kamalyes/friebox
 Author: Kamalyes
 Author-email: mryu168@163.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <a href="#">
-<img src="./friebox/static/images/logo.svg" alt="friebox" width="150">
+<img src="https://cdn.jsdelivr.net/gh/kamalyes/friebox@master/friebox/static/images/logo.svg" alt="friebox" width="150">
 </a>
 
 </p>
 <p align="center">
 <a href="https://pypi.org/project/friebox/" target="__blank"><img src="https://img.shields.io/pypi/v/friebox" alt="friebox preview"></a>
 <a href="https://pypistats.org/packages/friebox" target="__blank"><img src="https://img.shields.io/pypi/dm/friebox"></a>
 <br>
@@ -31,17 +31,20 @@
 
 我们致力于解决低效、繁琐的测试执行问题，我们的目标是在【Simple Test In friebox】
 
 ## 📦环境
 
 - 安装 Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - 更新adb包（选择性）<https://developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn>
- Windows版本：<https://dl.google.com/android/repository/platform-tools-latest-windows.zip>
- Mac版本：<https://dl.google.com/android/repository/platform-tools-latest-windows.zip>
- Linux版本：<https://dl.google.com/android/repository/platform-tools-latest-linux.zip>
+
+```bash
+Windows版本：https://dl.google.com/android/repository/platform-tools-latest-windows.zip
+Mac版本：https://dl.google.com/android/repository/platform-tools-latest-windows.zip
+Linux版本：https://dl.google.com/android/repository/platform-tools-latest-linux.zip
+```
 
 💡 如果Windows用户需要测试iOS，请先安装Itunes.
 
 - Apple官网：<https://www.apple.com.cn/itunes/>
 - Windows版本：<https://apps.microsoft.com/store/detail/itunes/9PB2MZ1ZMB1S?hl=zh_CN&gl=cn&cid=appledotcom&rtc=1&activetab=pivot%3Aoverviewtab>
 - Mac版本：https://support.apple.com/kb/dl1977?locale=zh_CN
 
@@ -61,15 +64,15 @@
 python -m friebox --host={ip} --port={port} # 自定义
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿使用python收集
 
 ```python
 from friebox.public.apm import APM
-# friebox version >= 1.0.0
+# friebox version >= 1.0.1
 apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
 # noLog : False (Save test data to log file)
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
```

#### html2text {}

```diff
@@ -1,40 +1,38 @@
-Metadata-Version: 2.1 Name: friebox Version: 1.0.0 Summary: friebox - Real-time
+Metadata-Version: 2.1 Name: friebox Version: 1.0.1 Summary: friebox - Real-time
 collection tool for Android/iOS performance data. Home-page: https://
 github.com/kamalyes/friebox Author: Kamalyes Author-email: mryu168@163.com
 License: MIT Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Description-Content-Type: text/markdown
 License-File: LICENSE
                                    [friebox]
           [friebox_preview] [https://img.shields.io/pypi/dm/friebox]
 ## ðç®ä» friebox - Android/iOSæ§è½æ°æ®çå®æ¶ééå·¥å·ã
 æä»¬è´åäºè§£å³ä½æãç¹ççæµè¯æ§è¡é®é¢ï¼æä»¬çç®æ æ¯å¨ãSimple
 Test In frieboxã ## ð¦ç¯å¢ - å®è£ Python 3.10 + [**Download**](https://
 www.python.org/downloads/) - æ´æ°adbåï¼éæ©æ§ï¼
-developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn>
-Windowsçæ¬ï¼
-dl.google.com/android/repository/platform-tools-latest-windows.zip>
-Macçæ¬ï¼
-dl.google.com/android/repository/platform-tools-latest-windows.zip>
-Linuxçæ¬ï¼
-dl.google.com/android/repository/platform-tools-latest-linux.zip> ð¡
+developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn> ```bash
+Windowsçæ¬ï¼https://dl.google.com/android/repository/platform-tools-latest-
+windows.zip Macçæ¬ï¼https://dl.google.com/android/repository/platform-
+tools-latest-windows.zip Linuxçæ¬ï¼https://dl.google.com/android/
+repository/platform-tools-latest-linux.zip ``` ð¡
 å¦æWindowsç¨æ·éè¦æµè¯iOSï¼è¯·åå®è£Itunes. - Appleå®ç½ï¼
 www.apple.com.cn/itunes/> - Windowsçæ¬ï¼
 apps.microsoft.com/store/detail/itunes/
 9PB2MZ1ZMB1S?hl=zh_CN&gl=cn&cid=appledotcom&rtc=1&activetab=pivot%3Aoverviewtab>
 - Macçæ¬ï¼https://support.apple.com/kb/dl1977?locale=zh_CN ## ð¥å®è£
 ```shell pip install -U friebox # é»è®¤ pip install -i https://
 mirrors.ustc.edu.cn/pypi/web/simple -U friebox # éå ``` ð¡
 å¦æä½ çç½ç»æ æ³éè¿ [pip install -U friebox] ä¸è½½,
 å¯ä»¥å°è¯ä½¿ç¨éåä¸è½½ï¼ä½æ¯å¯è½ä¸æ¯ææ°çæ¬. ##
 ðå¯å¨friebox ```shell python -m friebox # é»è®¤ python -m friebox --host=
 {ip} --port={port} # èªå®ä¹ ``` ##
 ð´ó £ó ©ó £ó ­ó ¿ä½¿ç¨pythonæ¶é ```python from friebox.public.apm
-import APM # friebox version >= 1.0.0 apm = APM
+import APM # friebox version >= 1.0.1 apm = APM
 (pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
 surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
 platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
 (Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
 (Save test data to log file) cpu = apm.collectCpu() # % memory =
 apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
 apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
```

### Comparing `friebox-1.0.0/README.md` & `friebox-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center">
 <a href="#">
-<img src="./friebox/static/images/logo.svg" alt="friebox" width="150">
+<img src="https://cdn.jsdelivr.net/gh/kamalyes/friebox@master/friebox/static/images/logo.svg" alt="friebox" width="150">
 </a>
 
 </p>
 <p align="center">
 <a href="https://pypi.org/project/friebox/" target="__blank"><img src="https://img.shields.io/pypi/v/friebox" alt="friebox preview"></a>
 <a href="https://pypistats.org/packages/friebox" target="__blank"><img src="https://img.shields.io/pypi/dm/friebox"></a>
 <br>
@@ -16,17 +16,20 @@
 
 我们致力于解决低效、繁琐的测试执行问题，我们的目标是在【Simple Test In friebox】
 
 ## 📦环境
 
 - 安装 Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - 更新adb包（选择性）<https://developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn>
- Windows版本：<https://dl.google.com/android/repository/platform-tools-latest-windows.zip>
- Mac版本：<https://dl.google.com/android/repository/platform-tools-latest-windows.zip>
- Linux版本：<https://dl.google.com/android/repository/platform-tools-latest-linux.zip>
+
+```bash
+Windows版本：https://dl.google.com/android/repository/platform-tools-latest-windows.zip
+Mac版本：https://dl.google.com/android/repository/platform-tools-latest-windows.zip
+Linux版本：https://dl.google.com/android/repository/platform-tools-latest-linux.zip
+```
 
 💡 如果Windows用户需要测试iOS，请先安装Itunes.
 
 - Apple官网：<https://www.apple.com.cn/itunes/>
 - Windows版本：<https://apps.microsoft.com/store/detail/itunes/9PB2MZ1ZMB1S?hl=zh_CN&gl=cn&cid=appledotcom&rtc=1&activetab=pivot%3Aoverviewtab>
 - Mac版本：https://support.apple.com/kb/dl1977?locale=zh_CN
 
@@ -46,15 +49,15 @@
 python -m friebox --host={ip} --port={port} # 自定义
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿使用python收集
 
 ```python
 from friebox.public.apm import APM
-# friebox version >= 1.0.0
+# friebox version >= 1.0.1
 apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
 # noLog : False (Save test data to log file)
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
```

#### html2text {}

```diff
@@ -1,33 +1,31 @@
                                    [friebox]
           [friebox_preview] [https://img.shields.io/pypi/dm/friebox]
 ## ðç®ä» friebox - Android/iOSæ§è½æ°æ®çå®æ¶ééå·¥å·ã
 æä»¬è´åäºè§£å³ä½æãç¹ççæµè¯æ§è¡é®é¢ï¼æä»¬çç®æ æ¯å¨ãSimple
 Test In frieboxã ## ð¦ç¯å¢ - å®è£ Python 3.10 + [**Download**](https://
 www.python.org/downloads/) - æ´æ°adbåï¼éæ©æ§ï¼
-developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn>
-Windowsçæ¬ï¼
-dl.google.com/android/repository/platform-tools-latest-windows.zip>
-Macçæ¬ï¼
-dl.google.com/android/repository/platform-tools-latest-windows.zip>
-Linuxçæ¬ï¼
-dl.google.com/android/repository/platform-tools-latest-linux.zip> ð¡
+developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn> ```bash
+Windowsçæ¬ï¼https://dl.google.com/android/repository/platform-tools-latest-
+windows.zip Macçæ¬ï¼https://dl.google.com/android/repository/platform-
+tools-latest-windows.zip Linuxçæ¬ï¼https://dl.google.com/android/
+repository/platform-tools-latest-linux.zip ``` ð¡
 å¦æWindowsç¨æ·éè¦æµè¯iOSï¼è¯·åå®è£Itunes. - Appleå®ç½ï¼
 www.apple.com.cn/itunes/> - Windowsçæ¬ï¼
 apps.microsoft.com/store/detail/itunes/
 9PB2MZ1ZMB1S?hl=zh_CN&gl=cn&cid=appledotcom&rtc=1&activetab=pivot%3Aoverviewtab>
 - Macçæ¬ï¼https://support.apple.com/kb/dl1977?locale=zh_CN ## ð¥å®è£
 ```shell pip install -U friebox # é»è®¤ pip install -i https://
 mirrors.ustc.edu.cn/pypi/web/simple -U friebox # éå ``` ð¡
 å¦æä½ çç½ç»æ æ³éè¿ [pip install -U friebox] ä¸è½½,
 å¯ä»¥å°è¯ä½¿ç¨éåä¸è½½ï¼ä½æ¯å¯è½ä¸æ¯ææ°çæ¬. ##
 ðå¯å¨friebox ```shell python -m friebox # é»è®¤ python -m friebox --host=
 {ip} --port={port} # èªå®ä¹ ``` ##
 ð´ó £ó ©ó £ó ­ó ¿ä½¿ç¨pythonæ¶é ```python from friebox.public.apm
-import APM # friebox version >= 1.0.0 apm = APM
+import APM # friebox version >= 1.0.1 apm = APM
 (pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
 surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
 platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
 (Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
 (Save test data to log file) cpu = apm.collectCpu() # % memory =
 apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
 apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
```

### Comparing `friebox-1.0.0/friebox/debug.py` & `friebox-1.0.1/friebox/debug.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/_iosPerf.py` & `friebox-1.0.1/friebox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/adb/linux/adb` & `friebox-1.0.1/friebox/public/adb/linux/adb`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/adb/mac/adb` & `friebox-1.0.1/friebox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/adb/windows/AdbWinApi.dll` & `friebox-1.0.1/friebox/public/adb/windows/AdbWinApi.dll`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/adb/windows/AdbWinUsbApi.dll` & `friebox-1.0.1/friebox/public/adb/windows/AdbWinUsbApi.dll`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/adb/windows/adb.exe` & `friebox-1.0.1/friebox/public/adb/windows/adb.exe`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/adb.py` & `friebox-1.0.1/friebox/public/adb.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/apm.py` & `friebox-1.0.1/friebox/public/apm.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/apm_pk.py` & `friebox-1.0.1/friebox/public/apm_pk.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/common.py` & `friebox-1.0.1/friebox/public/common.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/fps.py` & `friebox-1.0.1/friebox/public/fps.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/__main__.py` & `friebox-1.0.1/friebox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_crash.py` & `friebox-1.0.1/friebox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_device.py` & `friebox-1.0.1/friebox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_hexdump.py` & `friebox-1.0.1/friebox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_imagemounter.py` & `friebox-1.0.1/friebox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_installation.py` & `friebox-1.0.1/friebox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_instruments.py` & `friebox-1.0.1/friebox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_ipautil.py` & `friebox-1.0.1/friebox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_perf.py` & `friebox-1.0.1/friebox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_proto.py` & `friebox-1.0.1/friebox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_relay.py` & `friebox-1.0.1/friebox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_safe_socket.py` & `friebox-1.0.1/friebox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_ssl.py` & `friebox-1.0.1/friebox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_sync.py` & `friebox-1.0.1/friebox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_types.py` & `friebox-1.0.1/friebox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_usbmux.py` & `friebox-1.0.1/friebox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_utils.py` & `friebox-1.0.1/friebox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/_wdaproxy.py` & `friebox-1.0.1/friebox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/bplist.py` & `friebox-1.0.1/friebox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/exceptions.py` & `friebox-1.0.1/friebox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/plistlib2.py` & `friebox-1.0.1/friebox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/requests_usbmux.py` & `friebox-1.0.1/friebox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/public/iosperf/struct2.py` & `friebox-1.0.1/friebox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/css/highlight.min.css` & `friebox-1.0.1/friebox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/css/select2-bootstrap-5-theme.min.css` & `friebox-1.0.1/friebox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `friebox-1.0.1/friebox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/css/select2.min.css` & `friebox-1.0.1/friebox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/css/sweetalert2.min.css` & `friebox-1.0.1/friebox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/css/tabler.demo.min.css` & `friebox-1.0.1/friebox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/css/tabler.min.css` & `friebox-1.0.1/friebox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/images/404.png` & `friebox-1.0.1/friebox/static/images/404.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/images/500.png` & `friebox-1.0.1/friebox/static/images/500.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/images/avatar.png` & `friebox-1.0.1/friebox/static/images/avatar.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/images/coffee.png` & `friebox-1.0.1/friebox/static/images/coffee.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/images/empty.png` & `friebox-1.0.1/friebox/static/images/empty.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/apexcharts.js` & `friebox-1.0.1/friebox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/gray.js` & `friebox-1.0.1/friebox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/highlight.min.js` & `friebox-1.0.1/friebox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/highstock.js` & `friebox-1.0.1/friebox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/html2canvas.min.js` & `friebox-1.0.1/friebox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/jquery.min.js` & `friebox-1.0.1/friebox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/select2.min.js` & `friebox-1.0.1/friebox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/socket.io.js` & `friebox-1.0.1/friebox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/sweetalert2.min.js` & `friebox-1.0.1/friebox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/tabler.demo.min.js` & `friebox-1.0.1/friebox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/static/js/tabler.min.js` & `friebox-1.0.1/friebox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/templates/404.html` & `friebox-1.0.1/friebox/templates/404.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/templates/500.html` & `friebox-1.0.1/friebox/templates/500.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/templates/analysis.html` & `friebox-1.0.1/friebox/templates/analysis.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/templates/analysis_pk.html` & `friebox-1.0.1/friebox/templates/analysis_pk.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/templates/base.html` & `friebox-1.0.1/friebox/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/kamalyes" class="link-secondary">friebox</a>.{% if lan == 'zh_CN' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/kamalyes/friebox/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'zh_CN' %} 版本 {% else %} Releases {% endif %} . V1.0.0
+                                {% if lan == 'zh_CN' %} 版本 {% else %} Releases {% endif %} . V1.0.1
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
@@ -23,15 +23,15 @@
 ***** {% block page_title %} {% endblock %} *****
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'zh_CN'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'zh_CN'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
     * Copyright ©  friebox.{% if lan == 'zh_CN' %} ä¿çæææå© {% else
       %} All rights reserved {% endif %}
-    * {%_if_lan_==_'zh_CN'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V1.0.0
+    * {%_if_lan_==_'zh_CN'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V1.0.1
 *****  {% if lan == 'zh_CN' %} è®¾ç½® {% else %} Setting {% endif %} *****
     * Warning_Value
     * Timer
     * Agent_ _{%_if_lan_==_'en_US'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'zh_CN' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [
 {{ cpuWarning }}    ]
 {% if lan == 'zh_CN' %} åå­åè­¦å¼ {% else %} Memory warning value {%
```

### Comparing `friebox-1.0.0/friebox/templates/index.html` & `friebox-1.0.1/friebox/templates/index.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/templates/pk.html` & `friebox-1.0.1/friebox/templates/pk.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/templates/report.html` & `friebox-1.0.1/friebox/templates/report.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/view/apis.py` & `friebox-1.0.1/friebox/view/apis.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/view/pages.py` & `friebox-1.0.1/friebox/view/pages.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox/web.py` & `friebox-1.0.1/friebox/web.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/friebox.egg-info/PKG-INFO` & `friebox-1.0.1/friebox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: friebox
-Version: 1.0.0
+Version: 1.0.1
 Summary: friebox - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/kamalyes/friebox
 Author: Kamalyes
 Author-email: mryu168@163.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <a href="#">
-<img src="./friebox/static/images/logo.svg" alt="friebox" width="150">
+<img src="https://cdn.jsdelivr.net/gh/kamalyes/friebox@master/friebox/static/images/logo.svg" alt="friebox" width="150">
 </a>
 
 </p>
 <p align="center">
 <a href="https://pypi.org/project/friebox/" target="__blank"><img src="https://img.shields.io/pypi/v/friebox" alt="friebox preview"></a>
 <a href="https://pypistats.org/packages/friebox" target="__blank"><img src="https://img.shields.io/pypi/dm/friebox"></a>
 <br>
@@ -31,17 +31,20 @@
 
 我们致力于解决低效、繁琐的测试执行问题，我们的目标是在【Simple Test In friebox】
 
 ## 📦环境
 
 - 安装 Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - 更新adb包（选择性）<https://developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn>
- Windows版本：<https://dl.google.com/android/repository/platform-tools-latest-windows.zip>
- Mac版本：<https://dl.google.com/android/repository/platform-tools-latest-windows.zip>
- Linux版本：<https://dl.google.com/android/repository/platform-tools-latest-linux.zip>
+
+```bash
+Windows版本：https://dl.google.com/android/repository/platform-tools-latest-windows.zip
+Mac版本：https://dl.google.com/android/repository/platform-tools-latest-windows.zip
+Linux版本：https://dl.google.com/android/repository/platform-tools-latest-linux.zip
+```
 
 💡 如果Windows用户需要测试iOS，请先安装Itunes.
 
 - Apple官网：<https://www.apple.com.cn/itunes/>
 - Windows版本：<https://apps.microsoft.com/store/detail/itunes/9PB2MZ1ZMB1S?hl=zh_CN&gl=cn&cid=appledotcom&rtc=1&activetab=pivot%3Aoverviewtab>
 - Mac版本：https://support.apple.com/kb/dl1977?locale=zh_CN
 
@@ -61,15 +64,15 @@
 python -m friebox --host={ip} --port={port} # 自定义
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿使用python收集
 
 ```python
 from friebox.public.apm import APM
-# friebox version >= 1.0.0
+# friebox version >= 1.0.1
 apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
 # noLog : False (Save test data to log file)
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
```

#### html2text {}

```diff
@@ -1,40 +1,38 @@
-Metadata-Version: 2.1 Name: friebox Version: 1.0.0 Summary: friebox - Real-time
+Metadata-Version: 2.1 Name: friebox Version: 1.0.1 Summary: friebox - Real-time
 collection tool for Android/iOS performance data. Home-page: https://
 github.com/kamalyes/friebox Author: Kamalyes Author-email: mryu168@163.com
 License: MIT Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Description-Content-Type: text/markdown
 License-File: LICENSE
                                    [friebox]
           [friebox_preview] [https://img.shields.io/pypi/dm/friebox]
 ## ðç®ä» friebox - Android/iOSæ§è½æ°æ®çå®æ¶ééå·¥å·ã
 æä»¬è´åäºè§£å³ä½æãç¹ççæµè¯æ§è¡é®é¢ï¼æä»¬çç®æ æ¯å¨ãSimple
 Test In frieboxã ## ð¦ç¯å¢ - å®è£ Python 3.10 + [**Download**](https://
 www.python.org/downloads/) - æ´æ°adbåï¼éæ©æ§ï¼
-developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn>
-Windowsçæ¬ï¼
-dl.google.com/android/repository/platform-tools-latest-windows.zip>
-Macçæ¬ï¼
-dl.google.com/android/repository/platform-tools-latest-windows.zip>
-Linuxçæ¬ï¼
-dl.google.com/android/repository/platform-tools-latest-linux.zip> ð¡
+developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn> ```bash
+Windowsçæ¬ï¼https://dl.google.com/android/repository/platform-tools-latest-
+windows.zip Macçæ¬ï¼https://dl.google.com/android/repository/platform-
+tools-latest-windows.zip Linuxçæ¬ï¼https://dl.google.com/android/
+repository/platform-tools-latest-linux.zip ``` ð¡
 å¦æWindowsç¨æ·éè¦æµè¯iOSï¼è¯·åå®è£Itunes. - Appleå®ç½ï¼
 www.apple.com.cn/itunes/> - Windowsçæ¬ï¼
 apps.microsoft.com/store/detail/itunes/
 9PB2MZ1ZMB1S?hl=zh_CN&gl=cn&cid=appledotcom&rtc=1&activetab=pivot%3Aoverviewtab>
 - Macçæ¬ï¼https://support.apple.com/kb/dl1977?locale=zh_CN ## ð¥å®è£
 ```shell pip install -U friebox # é»è®¤ pip install -i https://
 mirrors.ustc.edu.cn/pypi/web/simple -U friebox # éå ``` ð¡
 å¦æä½ çç½ç»æ æ³éè¿ [pip install -U friebox] ä¸è½½,
 å¯ä»¥å°è¯ä½¿ç¨éåä¸è½½ï¼ä½æ¯å¯è½ä¸æ¯ææ°çæ¬. ##
 ðå¯å¨friebox ```shell python -m friebox # é»è®¤ python -m friebox --host=
 {ip} --port={port} # èªå®ä¹ ``` ##
 ð´ó £ó ©ó £ó ­ó ¿ä½¿ç¨pythonæ¶é ```python from friebox.public.apm
-import APM # friebox version >= 1.0.0 apm = APM
+import APM # friebox version >= 1.0.1 apm = APM
 (pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
 surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
 platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
 (Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
 (Save test data to log file) cpu = apm.collectCpu() # % memory =
 apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
 apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
```

### Comparing `friebox-1.0.0/friebox.egg-info/SOURCES.txt` & `friebox-1.0.1/friebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `friebox-1.0.0/setup.py` & `friebox-1.0.1/setup.py`

 * *Files identical despite different names*

