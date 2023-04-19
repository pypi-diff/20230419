# Comparing `tmp/friebox-1.0.2.tar.gz` & `tmp/friebox-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "friebox-1.0.2.tar", last modified: Wed Apr 19 06:23:38 2023, max compression
+gzip compressed data, was "friebox-1.0.3.tar", last modified: Wed Apr 19 07:22:26 2023, max compression
```

## Comparing `friebox-1.0.2.tar` & `friebox-1.0.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.698747 friebox-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-19 06:23:26.000000 friebox-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 06:23:26.000000 friebox-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 06:23:38.698747 friebox-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-19 06:23:26.000000 friebox-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.662746 friebox-1.0.2/friebox/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 06:23:26.000000 friebox-1.0.2/friebox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 06:23:26.000000 friebox-1.0.2/friebox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-19 06:23:26.000000 friebox-1.0.2/friebox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.662746 friebox-1.0.2/friebox/public/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-19 06:23:26.000000 friebox-1.0.2/friebox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-19 06:23:26.000000 friebox-1.0.2/friebox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.658746 friebox-1.0.2/friebox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.662746 friebox-1.0.2/friebox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)  7933192 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.670746 friebox-1.0.2/friebox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.670746 friebox-1.0.2/friebox/public/adb/mac/
--rw-r--r--   0 runner    (1001) docker     (123)  7328624 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.678747 friebox-1.0.2/friebox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)    97792 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)    62976 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)  5992960 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-19 06:23:26.000000 friebox-1.0.2/friebox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23827 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.690747 friebox-1.0.2/friebox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30524 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41196 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39321 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31553 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.658746 friebox-1.0.2/friebox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.690747 friebox-1.0.2/friebox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.690747 friebox-1.0.2/friebox/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/images/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/images/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/images/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/images/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/images/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.694747 friebox-1.0.2/friebox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.698747 friebox-1.0.2/friebox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    47111 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    38304 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34830 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    88932 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55724 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34971 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.698747 friebox-1.0.2/friebox/view/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23190 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-19 06:23:27.000000 friebox-1.0.2/friebox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:23:38.662746 friebox-1.0.2/friebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 06:23:38.000000 friebox-1.0.2/friebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-19 06:23:38.000000 friebox-1.0.2/friebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:23:38.000000 friebox-1.0.2/friebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-19 06:23:38.000000 friebox-1.0.2/friebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 06:23:38.000000 friebox-1.0.2/friebox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 06:23:38.698747 friebox-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-19 06:23:27.000000 friebox-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.056654 friebox-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-19 07:22:13.000000 friebox-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 07:22:13.000000 friebox-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 07:22:26.056654 friebox-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-19 07:22:13.000000 friebox-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.020650 friebox-1.0.3/friebox/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.024650 friebox-1.0.3/friebox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.016649 friebox-1.0.3/friebox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.024650 friebox-1.0.3/friebox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)  7933192 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.028651 friebox-1.0.3/friebox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.028651 friebox-1.0.3/friebox/public/adb/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)  7328624 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.040652 friebox-1.0.3/friebox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)    97792 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    62976 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)  5992960 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23827 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.048653 friebox-1.0.3/friebox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30524 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41196 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39321 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31553 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.016649 friebox-1.0.3/friebox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.048653 friebox-1.0.3/friebox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.052654 friebox-1.0.3/friebox/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/images/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/images/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/images/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/images/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/images/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.056654 friebox-1.0.3/friebox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.056654 friebox-1.0.3/friebox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    47111 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38304 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34830 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    88932 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55724 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34971 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.056654 friebox-1.0.3/friebox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23190 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-19 07:22:13.000000 friebox-1.0.3/friebox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:22:26.020650 friebox-1.0.3/friebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 07:22:25.000000 friebox-1.0.3/friebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-19 07:22:26.000000 friebox-1.0.3/friebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:22:25.000000 friebox-1.0.3/friebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-19 07:22:25.000000 friebox-1.0.3/friebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 07:22:25.000000 friebox-1.0.3/friebox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 07:22:26.056654 friebox-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-19 07:22:13.000000 friebox-1.0.3/setup.py
```

### Comparing `friebox-1.0.2/LICENSE` & `friebox-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/PKG-INFO` & `friebox-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: friebox
-Version: 1.0.2
+Version: 1.0.3
 Summary: friebox - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/kamalyes/friebox
 Author: Kamalyes
 Author-email: mryu168@163.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -64,15 +64,15 @@
 python -m friebox --host={ip} --port={port} # 自定义
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿使用python收集
 
 ```python
 from friebox.public.apm import APM
-# friebox version >= 1.0.2
+# friebox version >= 1.0.3
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: friebox Version: 1.0.2 Summary: friebox - Real-time
+Metadata-Version: 2.1 Name: friebox Version: 1.0.3 Summary: friebox - Real-time
 collection tool for Android/iOS performance data. Home-page: https://
 github.com/kamalyes/friebox Author: Kamalyes Author-email: mryu168@163.com
 License: MIT Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Description-Content-Type: text/markdown
 License-File: LICENSE
                                    [friebox]
@@ -24,15 +24,15 @@
 ```shell pip install -U friebox # é»è®¤ pip install -i https://
 mirrors.ustc.edu.cn/pypi/web/simple -U friebox # éå ``` ð¡
 å¦æä½ çç½ç»æ æ³éè¿ [pip install -U friebox] ä¸è½½,
 å¯ä»¥å°è¯ä½¿ç¨éåä¸è½½ï¼ä½æ¯å¯è½ä¸æ¯ææ°çæ¬. ##
 ðå¯å¨friebox ```shell python -m friebox # é»è®¤ python -m friebox --host=
 {ip} --port={port} # èªå®ä¹ ``` ##
 ð´ó £ó ©ó £ó ­ó ¿ä½¿ç¨pythonæ¶é ```python from friebox.public.apm
-import APM # friebox version >= 1.0.2 apm = APM
+import APM # friebox version >= 1.0.3 apm = APM
 (pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
 surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
 platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
 (Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
 (Save test data to log file) cpu = apm.collectCpu() # % memory =
 apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
 apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
```

### Comparing `friebox-1.0.2/README.md` & `friebox-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 python -m friebox --host={ip} --port={port} # 自定义
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿使用python收集
 
 ```python
 from friebox.public.apm import APM
-# friebox version >= 1.0.2
+# friebox version >= 1.0.3
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
@@ -17,15 +17,15 @@
 ```shell pip install -U friebox # é»è®¤ pip install -i https://
 mirrors.ustc.edu.cn/pypi/web/simple -U friebox # éå ``` ð¡
 å¦æä½ çç½ç»æ æ³éè¿ [pip install -U friebox] ä¸è½½,
 å¯ä»¥å°è¯ä½¿ç¨éåä¸è½½ï¼ä½æ¯å¯è½ä¸æ¯ææ°çæ¬. ##
 ðå¯å¨friebox ```shell python -m friebox # é»è®¤ python -m friebox --host=
 {ip} --port={port} # èªå®ä¹ ``` ##
 ð´ó £ó ©ó £ó ­ó ¿ä½¿ç¨pythonæ¶é ```python from friebox.public.apm
-import APM # friebox version >= 1.0.2 apm = APM
+import APM # friebox version >= 1.0.3 apm = APM
 (pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
 surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
 platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
 (Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
 (Save test data to log file) cpu = apm.collectCpu() # % memory =
 apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
 apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
```

### Comparing `friebox-1.0.2/friebox/debug.py` & `friebox-1.0.3/friebox/debug.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/_iosPerf.py` & `friebox-1.0.3/friebox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/adb/linux/adb` & `friebox-1.0.3/friebox/public/adb/linux/adb`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/adb/mac/adb` & `friebox-1.0.3/friebox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/adb/windows/AdbWinApi.dll` & `friebox-1.0.3/friebox/public/adb/windows/AdbWinApi.dll`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/adb/windows/AdbWinUsbApi.dll` & `friebox-1.0.3/friebox/public/adb/windows/AdbWinUsbApi.dll`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/adb/windows/adb.exe` & `friebox-1.0.3/friebox/public/adb/windows/adb.exe`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/adb.py` & `friebox-1.0.3/friebox/public/adb.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/apm.py` & `friebox-1.0.3/friebox/public/apm.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/apm_pk.py` & `friebox-1.0.3/friebox/public/apm_pk.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/common.py` & `friebox-1.0.3/friebox/public/common.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/fps.py` & `friebox-1.0.3/friebox/public/fps.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/__main__.py` & `friebox-1.0.3/friebox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_crash.py` & `friebox-1.0.3/friebox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_device.py` & `friebox-1.0.3/friebox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_hexdump.py` & `friebox-1.0.3/friebox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_imagemounter.py` & `friebox-1.0.3/friebox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_installation.py` & `friebox-1.0.3/friebox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_instruments.py` & `friebox-1.0.3/friebox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_ipautil.py` & `friebox-1.0.3/friebox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_perf.py` & `friebox-1.0.3/friebox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_proto.py` & `friebox-1.0.3/friebox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_relay.py` & `friebox-1.0.3/friebox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_safe_socket.py` & `friebox-1.0.3/friebox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_ssl.py` & `friebox-1.0.3/friebox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_sync.py` & `friebox-1.0.3/friebox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_types.py` & `friebox-1.0.3/friebox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_usbmux.py` & `friebox-1.0.3/friebox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_utils.py` & `friebox-1.0.3/friebox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/_wdaproxy.py` & `friebox-1.0.3/friebox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/bplist.py` & `friebox-1.0.3/friebox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/exceptions.py` & `friebox-1.0.3/friebox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/plistlib2.py` & `friebox-1.0.3/friebox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/requests_usbmux.py` & `friebox-1.0.3/friebox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/public/iosperf/struct2.py` & `friebox-1.0.3/friebox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/css/highlight.min.css` & `friebox-1.0.3/friebox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/css/select2-bootstrap-5-theme.min.css` & `friebox-1.0.3/friebox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `friebox-1.0.3/friebox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/css/select2.min.css` & `friebox-1.0.3/friebox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/css/sweetalert2.min.css` & `friebox-1.0.3/friebox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/css/tabler.demo.min.css` & `friebox-1.0.3/friebox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/css/tabler.min.css` & `friebox-1.0.3/friebox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/images/404.png` & `friebox-1.0.3/friebox/static/images/404.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/images/500.png` & `friebox-1.0.3/friebox/static/images/500.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/images/avatar.png` & `friebox-1.0.3/friebox/static/images/avatar.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/images/coffee.png` & `friebox-1.0.3/friebox/static/images/coffee.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/images/empty.png` & `friebox-1.0.3/friebox/static/images/empty.png`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/apexcharts.js` & `friebox-1.0.3/friebox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/gray.js` & `friebox-1.0.3/friebox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/highlight.min.js` & `friebox-1.0.3/friebox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/highstock.js` & `friebox-1.0.3/friebox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/html2canvas.min.js` & `friebox-1.0.3/friebox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/jquery.min.js` & `friebox-1.0.3/friebox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/select2.min.js` & `friebox-1.0.3/friebox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/socket.io.js` & `friebox-1.0.3/friebox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/sweetalert2.min.js` & `friebox-1.0.3/friebox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/tabler.demo.min.js` & `friebox-1.0.3/friebox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/static/js/tabler.min.js` & `friebox-1.0.3/friebox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/templates/404.html` & `friebox-1.0.3/friebox/templates/404.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/templates/500.html` & `friebox-1.0.3/friebox/templates/500.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/templates/analysis.html` & `friebox-1.0.3/friebox/templates/analysis.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/templates/analysis_pk.html` & `friebox-1.0.3/friebox/templates/analysis_pk.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/templates/base.html` & `friebox-1.0.3/friebox/templates/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/kamalyes" class="link-secondary">friebox</a>.{% if lan == 'zh_CN' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/kamalyes/friebox/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'zh_CN' %} 版本 {% else %} Releases {% endif %} . V1.0.2
+                                {% if lan == 'zh_CN' %} 版本 {% else %} Releases {% endif %} . V1.0.3
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
-    * {%_if_lan_==_'zh_CN'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V1.0.2
+    * {%_if_lan_==_'zh_CN'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V1.0.3
 *****  {% if lan == 'zh_CN' %} è®¾ç½® {% else %} Setting {% endif %} *****
     * Warning_Value
     * Timer
     * Agent_ _{%_if_lan_==_'en_US'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'zh_CN' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [
 {{ cpuWarning }}    ]
 {% if lan == 'zh_CN' %} åå­åè­¦å¼ {% else %} Memory warning value {%
```

### Comparing `friebox-1.0.2/friebox/templates/index.html` & `friebox-1.0.3/friebox/templates/index.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/templates/pk.html` & `friebox-1.0.3/friebox/templates/pk.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/templates/report.html` & `friebox-1.0.3/friebox/templates/report.html`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/view/apis.py` & `friebox-1.0.3/friebox/view/apis.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/view/pages.py` & `friebox-1.0.3/friebox/view/pages.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox/web.py` & `friebox-1.0.3/friebox/web.py`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/friebox.egg-info/PKG-INFO` & `friebox-1.0.3/friebox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: friebox
-Version: 1.0.2
+Version: 1.0.3
 Summary: friebox - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/kamalyes/friebox
 Author: Kamalyes
 Author-email: mryu168@163.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -64,15 +64,15 @@
 python -m friebox --host={ip} --port={port} # 自定义
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿使用python收集
 
 ```python
 from friebox.public.apm import APM
-# friebox version >= 1.0.2
+# friebox version >= 1.0.3
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: friebox Version: 1.0.2 Summary: friebox - Real-time
+Metadata-Version: 2.1 Name: friebox Version: 1.0.3 Summary: friebox - Real-time
 collection tool for Android/iOS performance data. Home-page: https://
 github.com/kamalyes/friebox Author: Kamalyes Author-email: mryu168@163.com
 License: MIT Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Description-Content-Type: text/markdown
 License-File: LICENSE
                                    [friebox]
@@ -24,15 +24,15 @@
 ```shell pip install -U friebox # é»è®¤ pip install -i https://
 mirrors.ustc.edu.cn/pypi/web/simple -U friebox # éå ``` ð¡
 å¦æä½ çç½ç»æ æ³éè¿ [pip install -U friebox] ä¸è½½,
 å¯ä»¥å°è¯ä½¿ç¨éåä¸è½½ï¼ä½æ¯å¯è½ä¸æ¯ææ°çæ¬. ##
 ðå¯å¨friebox ```shell python -m friebox # é»è®¤ python -m friebox --host=
 {ip} --port={port} # èªå®ä¹ ``` ##
 ð´ó £ó ©ó £ó ­ó ¿ä½¿ç¨pythonæ¶é ```python from friebox.public.apm
-import APM # friebox version >= 1.0.2 apm = APM
+import APM # friebox version >= 1.0.3 apm = APM
 (pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android',
 surfaceview=True, noLog=True) # apm = APM(pkgName='com.bilibili.app.in',
 platform='iOS') only supports one device # surfaceviewï¼ False = gfxinfo
 (Developer - GPU rendering mode - adb shell dumpsys gfxinfo) # noLog : False
 (Save test data to log file) cpu = apm.collectCpu() # % memory =
 apm.collectMemory() # MB flow = apm.collectFlow(wifi=True) # KB fps =
 apm.collectFps() # HZ battery = apm.collectBattery() # level:% temperature:Â°C
```

### Comparing `friebox-1.0.2/friebox.egg-info/SOURCES.txt` & `friebox-1.0.3/friebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `friebox-1.0.2/setup.py` & `friebox-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import setuptools
 from friebox import __version__
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    install_requires=['flask>=2.2.3', 'httpio>=0.3.0', 'requests>=2.28.2',
+    install_requires=['flask>=2.1.3', 'httpio>=0.3.0', 'requests>=2.28.2',
                       'logzero>=1.7.0', 'tidevice>=0.10.7', 'tqdm>=4.65.0', 'xlwt>=1.3.0',
-                      'flask_socketio>=5.3.3', 'fire>=0.5.0'],
+                      'flask_socketio>=5.3.3', 'fire>=0.5.0', 'werkzeug==2.0.3', 'Jinja2==3.0.1'],
     version=__version__,
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="friebox - Real-time collection tool for Android/iOS performance data.",
     packages=setuptools.find_namespace_packages(include=["friebox", "friebox.*"], ),
     include_package_data=True
 )
```

