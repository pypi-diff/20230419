# Comparing `tmp/qtdark-0.1.3.tar.gz` & `tmp/qtdark-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdark-0.1.3.tar", last modified: Wed Apr 19 05:13:27 2023, max compression
+gzip compressed data, was "qtdark-0.1.4.tar", last modified: Wed Apr 19 05:25:12 2023, max compression
```

## Comparing `qtdark-0.1.3.tar` & `qtdark-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 05:13:27.607138 qtdark-0.1.3/
--rw-rw-rw-   0        0        0     1097 2023-04-19 04:49:12.000000 qtdark-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      276 2023-04-19 05:13:27.606156 qtdark-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-04-19 04:49:12.000000 qtdark-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 05:13:27.598162 qtdark-0.1.3/qtdark/
--rw-rw-rw-   0        0        0        0 2023-04-19 04:51:58.000000 qtdark-0.1.3/qtdark/__init__.py
--rw-rw-rw-   0        0        0      517 2023-04-19 05:11:13.000000 qtdark-0.1.3/qtdark/__main__.py
--rw-rw-rw-   0        0        0      143 2023-04-19 05:07:14.000000 qtdark-0.1.3/qtdark/init.py
--rw-rw-rw-   0        0        0      131 2023-04-19 05:06:36.000000 qtdark-0.1.3/qtdark/program.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:13:27.605145 qtdark-0.1.3/qtdark.egg-info/
--rw-rw-rw-   0        0        0      276 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 05:13:27.607138 qtdark-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      501 2023-04-19 05:13:07.000000 qtdark-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:25:12.139294 qtdark-0.1.4/
+-rw-rw-rw-   0        0        0     1097 2023-04-19 04:49:12.000000 qtdark-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-04-19 05:25:12.138299 qtdark-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-04-19 04:49:12.000000 qtdark-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 05:25:12.130328 qtdark-0.1.4/qtdark/
+-rw-rw-rw-   0        0        0      135 2023-04-19 05:24:17.000000 qtdark-0.1.4/qtdark/__init__.py
+-rw-rw-rw-   0        0        0      535 2023-04-19 05:21:07.000000 qtdark-0.1.4/qtdark/__main__.py
+-rw-rw-rw-   0        0        0      143 2023-04-19 05:07:14.000000 qtdark-0.1.4/qtdark/init.py
+-rw-rw-rw-   0        0        0      117 2023-04-19 05:24:11.000000 qtdark-0.1.4/qtdark/program.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:25:12.137300 qtdark-0.1.4/qtdark.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-04-19 05:25:12.000000 qtdark-0.1.4/qtdark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-19 05:25:12.000000 qtdark-0.1.4/qtdark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 05:25:12.000000 qtdark-0.1.4/qtdark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-19 05:25:12.000000 qtdark-0.1.4/qtdark.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-04-19 05:25:12.000000 qtdark-0.1.4/qtdark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 05:25:12.000000 qtdark-0.1.4/qtdark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 05:25:12.139294 qtdark-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      501 2023-04-19 05:21:51.000000 qtdark-0.1.4/setup.py
```

### Comparing `qtdark-0.1.3/LICENSE` & `qtdark-0.1.4/LICENSE`

 * *Files identical despite different names*

