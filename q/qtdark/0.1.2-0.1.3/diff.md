# Comparing `tmp/qtdark-0.1.2.tar.gz` & `tmp/qtdark-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdark-0.1.2.tar", last modified: Tue Apr 18 14:11:48 2023, max compression
+gzip compressed data, was "qtdark-0.1.3.tar", last modified: Wed Apr 19 05:13:27 2023, max compression
```

## Comparing `qtdark-0.1.2.tar` & `qtdark-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 14:11:48.653418 qtdark-0.1.2/
--rw-rw-rw-   0        0        0     1097 2023-04-18 12:59:58.000000 qtdark-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      560 2023-04-18 14:11:48.653418 qtdark-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-04-18 12:59:58.000000 qtdark-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 14:11:48.644442 qtdark-0.1.2/qtdark/
--rw-rw-rw-   0        0        0        0 2023-04-18 14:09:20.000000 qtdark-0.1.2/qtdark/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:11:48.652420 qtdark-0.1.2/qtdark/cli/
--rw-rw-rw-   0        0        0      445 2023-04-18 14:10:50.000000 qtdark-0.1.2/qtdark/cli/__init__.py
--rw-rw-rw-   0        0        0      143 2023-04-18 13:50:06.000000 qtdark-0.1.2/qtdark/init.py
--rw-rw-rw-   0        0        0      178 2023-04-18 13:56:20.000000 qtdark-0.1.2/qtdark/program.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:11:48.651425 qtdark-0.1.2/qtdark.egg-info/
--rw-rw-rw-   0        0        0      560 2023-04-18 14:11:48.000000 qtdark-0.1.2/qtdark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-04-18 14:11:48.000000 qtdark-0.1.2/qtdark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 14:11:48.000000 qtdark-0.1.2/qtdark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-18 14:11:48.000000 qtdark-0.1.2/qtdark.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-04-18 14:11:48.000000 qtdark-0.1.2/qtdark.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 14:11:48.000000 qtdark-0.1.2/qtdark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 14:11:48.654416 qtdark-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      773 2023-04-18 14:11:15.000000 qtdark-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:13:27.607138 qtdark-0.1.3/
+-rw-rw-rw-   0        0        0     1097 2023-04-19 04:49:12.000000 qtdark-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-04-19 05:13:27.606156 qtdark-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-04-19 04:49:12.000000 qtdark-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 05:13:27.598162 qtdark-0.1.3/qtdark/
+-rw-rw-rw-   0        0        0        0 2023-04-19 04:51:58.000000 qtdark-0.1.3/qtdark/__init__.py
+-rw-rw-rw-   0        0        0      517 2023-04-19 05:11:13.000000 qtdark-0.1.3/qtdark/__main__.py
+-rw-rw-rw-   0        0        0      143 2023-04-19 05:07:14.000000 qtdark-0.1.3/qtdark/init.py
+-rw-rw-rw-   0        0        0      131 2023-04-19 05:06:36.000000 qtdark-0.1.3/qtdark/program.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:13:27.605145 qtdark-0.1.3/qtdark.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 05:13:27.000000 qtdark-0.1.3/qtdark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 05:13:27.607138 qtdark-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      501 2023-04-19 05:13:07.000000 qtdark-0.1.3/setup.py
```

### Comparing `qtdark-0.1.2/LICENSE` & `qtdark-0.1.3/LICENSE`

 * *Files identical despite different names*

