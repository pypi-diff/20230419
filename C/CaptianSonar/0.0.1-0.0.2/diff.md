# Comparing `tmp/CaptianSonar-0.0.1.tar.gz` & `tmp/CaptianSonar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CaptianSonar-0.0.1.tar", last modified: Mon Apr 17 02:55:13 2023, max compression
+gzip compressed data, was "CaptianSonar-0.0.2.tar", last modified: Wed Apr 19 02:24:15 2023, max compression
```

## Comparing `CaptianSonar-0.0.1.tar` & `CaptianSonar-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 02:55:13.104586 CaptianSonar-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-17 02:55:13.090614 CaptianSonar-0.0.1/CaptianSonar/
--rw-rw-rw-   0        0        0   190896 2023-04-17 02:43:08.000000 CaptianSonar-0.0.1/CaptianSonar/Game.py
--rw-rw-rw-   0        0        0     3303 2023-04-17 00:53:12.000000 CaptianSonar-0.0.1/CaptianSonar/Server.py
--rw-rw-rw-   0        0        0   190916 2023-04-17 02:21:31.000000 CaptianSonar-0.0.1/CaptianSonar/client.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:55:13.101593 CaptianSonar-0.0.1/CaptianSonar.egg-info/
--rw-rw-rw-   0        0        0      355 2023-04-17 02:55:12.000000 CaptianSonar-0.0.1/CaptianSonar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-17 02:55:13.000000 CaptianSonar-0.0.1/CaptianSonar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 02:55:12.000000 CaptianSonar-0.0.1/CaptianSonar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 02:55:12.000000 CaptianSonar-0.0.1/CaptianSonar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 02:49:04.000000 CaptianSonar-0.0.1/CaptianSonar.egg-info/zip-safe
--rw-rw-rw-   0        0        0      355 2023-04-17 02:55:13.103583 CaptianSonar-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-17 02:55:13.104586 CaptianSonar-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-04-17 02:46:34.000000 CaptianSonar-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:24:15.164502 CaptianSonar-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-19 02:24:15.112322 CaptianSonar-0.0.2/CaptianSonar/
+-rw-rw-rw-   0        0        0    19813 2023-04-19 00:55:15.000000 CaptianSonar-0.0.2/CaptianSonar/Server.py
+-rw-rw-rw-   0        0        0  6082053 2023-04-19 02:10:08.000000 CaptianSonar-0.0.2/CaptianSonar/zip.py
+drwxrwxrwx   0        0        0        0 2023-04-19 02:24:15.152598 CaptianSonar-0.0.2/CaptianSonar.egg-info/
+-rw-rw-rw-   0        0        0      357 2023-04-19 02:24:14.000000 CaptianSonar-0.0.2/CaptianSonar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-19 02:24:14.000000 CaptianSonar-0.0.2/CaptianSonar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 02:24:14.000000 CaptianSonar-0.0.2/CaptianSonar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-19 02:24:14.000000 CaptianSonar-0.0.2/CaptianSonar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-19 02:24:14.000000 CaptianSonar-0.0.2/CaptianSonar.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      357 2023-04-19 02:24:15.161790 CaptianSonar-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-19 02:24:15.166161 CaptianSonar-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      494 2023-04-19 02:23:59.000000 CaptianSonar-0.0.2/setup.py
```

