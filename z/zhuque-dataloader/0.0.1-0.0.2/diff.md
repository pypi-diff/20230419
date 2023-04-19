# Comparing `tmp/zhuque-dataloader-0.0.1.tar.gz` & `tmp/zhuque-dataloader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhuque-dataloader-0.0.1.tar", last modified: Wed Apr 19 07:04:13 2023, max compression
+gzip compressed data, was "zhuque-dataloader-0.0.2.tar", last modified: Wed Apr 19 08:56:20 2023, max compression
```

## Comparing `zhuque-dataloader-0.0.1.tar` & `zhuque-dataloader-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:04:13.238132 zhuque-dataloader-0.0.1/
--rw-rw-rw-   0        0        0      192 2023-04-19 07:04:13.237132 zhuque-dataloader-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-19 07:04:13.238132 zhuque-dataloader-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      359 2023-04-19 06:59:03.000000 zhuque-dataloader-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:04:13.235132 zhuque-dataloader-0.0.1/zhuque_dataloader.egg-info/
--rw-rw-rw-   0        0        0      192 2023-04-19 07:04:13.000000 zhuque-dataloader-0.0.1/zhuque_dataloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-19 07:04:13.000000 zhuque-dataloader-0.0.1/zhuque_dataloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:04:13.000000 zhuque-dataloader-0.0.1/zhuque_dataloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:04:13.000000 zhuque-dataloader-0.0.1/zhuque_dataloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 08:56:20.384425 zhuque-dataloader-0.0.2/
+-rw-rw-rw-   0        0        0      192 2023-04-19 08:56:20.383425 zhuque-dataloader-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 08:56:20.373426 zhuque-dataloader-0.0.2/load/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:48:30.000000 zhuque-dataloader-0.0.2/load/__init__.py
+-rw-rw-rw-   0        0        0    13435 2023-04-19 07:33:46.000000 zhuque-dataloader-0.0.2/load/loader.py
+-rw-rw-rw-   0        0        0       42 2023-04-19 08:56:20.384425 zhuque-dataloader-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      491 2023-04-19 08:55:58.000000 zhuque-dataloader-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:56:20.380425 zhuque-dataloader-0.0.2/zhuque_dataloader.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-04-19 08:56:20.000000 zhuque-dataloader-0.0.2/zhuque_dataloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-04-19 08:56:20.000000 zhuque-dataloader-0.0.2/zhuque_dataloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 08:56:20.000000 zhuque-dataloader-0.0.2/zhuque_dataloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-19 08:56:20.000000 zhuque-dataloader-0.0.2/zhuque_dataloader.egg-info/top_level.txt
```

