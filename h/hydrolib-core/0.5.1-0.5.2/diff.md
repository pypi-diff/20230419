# Comparing `tmp/hydrolib_core-0.5.1.tar.gz` & `tmp/hydrolib_core-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrolib_core-0.5.1.tar", max compression
+gzip compressed data, was "hydrolib_core-0.5.2.tar", max compression
```

## Comparing `hydrolib_core-0.5.1.tar` & `hydrolib_core-0.5.2.tar`

### file list

```diff
@@ -1,87 +1,88 @@
--rw-r--r--   0        0        0       79 2023-03-15 10:07:16.193069 hydrolib_core-0.5.1/hydrolib/__init__.py
--rw-r--r--   0        0        0       23 2023-04-17 14:49:57.253849 hydrolib_core-0.5.1/hydrolib/core/__init__.py
--rw-r--r--   0        0        0      416 2023-04-14 13:35:23.823996 hydrolib_core-0.5.1/hydrolib/core/base.py
--rw-r--r--   0        0        0    52489 2023-04-14 14:04:30.109748 hydrolib_core-0.5.1/hydrolib/core/basemodel.py
--rw-r--r--   0        0        0      253 2023-03-15 10:07:16.194069 hydrolib_core-0.5.1/hydrolib/core/config.py
--rw-r--r--   0        0        0      441 2023-04-14 11:29:41.344831 hydrolib_core-0.5.1/hydrolib/core/dflowfm/__init__.py
--rw-r--r--   0        0        0      730 2023-03-15 10:07:16.194069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/bc/__init__.py
--rw-r--r--   0        0        0    32784 2023-04-14 13:35:23.824997 hydrolib_core-0.5.1/hydrolib/core/dflowfm/bc/models.py
--rw-r--r--   0        0        0       84 2023-04-14 11:29:41.344831 hydrolib_core-0.5.1/hydrolib/core/dflowfm/common/__init__.py
--rw-r--r--   0        0        0     1221 2023-04-14 11:29:41.345772 hydrolib_core-0.5.1/hydrolib/core/dflowfm/common/models.py
--rw-r--r--   0        0        0      546 2023-03-15 10:07:16.196069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/crosssection/__init__.py
--rw-r--r--   0        0        0    30678 2023-04-12 09:08:24.401033 hydrolib_core-0.5.1/hydrolib/core/dflowfm/crosssection/models.py
--rw-r--r--   0        0        0      169 2023-04-12 13:31:27.344166 hydrolib_core-0.5.1/hydrolib/core/dflowfm/ext/__init__.py
--rw-r--r--   0        0        0    11317 2023-04-12 14:24:51.270177 hydrolib_core-0.5.1/hydrolib/core/dflowfm/ext/models.py
--rw-r--r--   0        0        0      374 2023-04-14 11:29:41.345772 hydrolib_core-0.5.1/hydrolib/core/dflowfm/extold/__init__.py
--rw-r--r--   0        0        0      481 2023-04-14 11:29:41.345772 hydrolib_core-0.5.1/hydrolib/core/dflowfm/extold/common_io.py
--rw-r--r--   0        0        0    25071 2023-04-17 14:40:38.661861 hydrolib_core-0.5.1/hydrolib/core/dflowfm/extold/models.py
--rw-r--r--   0        0        0     4397 2023-04-14 13:35:23.826002 hydrolib_core-0.5.1/hydrolib/core/dflowfm/extold/parser.py
--rw-r--r--   0        0        0     3594 2023-04-14 13:35:23.826002 hydrolib_core-0.5.1/hydrolib/core/dflowfm/extold/serializer.py
--rw-r--r--   0        0        0      211 2023-03-15 10:07:16.197070 hydrolib_core-0.5.1/hydrolib/core/dflowfm/friction/__init__.py
--rw-r--r--   0        0        0     9410 2023-03-15 10:07:16.197070 hydrolib_core-0.5.1/hydrolib/core/dflowfm/friction/models.py
--rw-r--r--   0        0        0      131 2023-03-15 10:07:16.198070 hydrolib_core-0.5.1/hydrolib/core/dflowfm/gui/__init__.py
--rw-r--r--   0        0        0     4874 2023-03-15 10:07:16.198070 hydrolib_core-0.5.1/hydrolib/core/dflowfm/gui/models.py
--rw-r--r--   0        0        0        0 2023-03-15 10:07:16.198070 hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/__init__.py
--rw-r--r--   0        0        0     4826 2023-03-15 10:07:16.198070 hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/io_models.py
--rw-r--r--   0        0        0    10126 2023-04-13 10:06:37.641400 hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/models.py
--rw-r--r--   0        0        0    15080 2023-04-14 13:35:23.826998 hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/parser.py
--rw-r--r--   0        0        0    13840 2023-04-14 13:35:23.827997 hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/serializer.py
--rw-r--r--   0        0        0    24384 2023-04-12 18:16:17.251460 hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/util.py
--rw-r--r--   0        0        0      352 2023-04-14 11:29:41.347766 hydrolib_core-0.5.1/hydrolib/core/dflowfm/inifield/__init__.py
--rw-r--r--   0        0        0     8705 2023-04-14 11:29:41.347766 hydrolib_core-0.5.1/hydrolib/core/dflowfm/inifield/models.py
--rw-r--r--   0        0        0      962 2023-03-15 10:07:16.201069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/mdu/__init__.py
--rw-r--r--   0        0        0    96029 2023-04-14 13:35:23.827997 hydrolib_core-0.5.1/hydrolib/core/dflowfm/mdu/models.py
--rw-r--r--   0        0        0      194 2023-03-15 10:07:16.202069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/net/__init__.py
--rw-r--r--   0        0        0    48587 2023-04-06 07:04:22.343700 hydrolib_core-0.5.1/hydrolib/core/dflowfm/net/models.py
--rw-r--r--   0        0        0    11085 2023-03-15 10:07:16.202069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/net/reader.py
--rw-r--r--   0        0        0     4560 2023-04-12 18:16:17.253480 hydrolib_core-0.5.1/hydrolib/core/dflowfm/net/ugrid_conventions.json
--rw-r--r--   0        0        0    20587 2023-03-15 10:07:16.203069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/net/writer.py
--rw-r--r--   0        0        0      172 2023-03-15 10:07:16.203069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/obs/__init__.py
--rw-r--r--   0        0        0     4260 2023-04-03 11:51:20.714510 hydrolib_core-0.5.1/hydrolib/core/dflowfm/obs/models.py
--rw-r--r--   0        0        0      254 2023-03-15 10:07:16.204070 hydrolib_core-0.5.1/hydrolib/core/dflowfm/obscrosssection/__init__.py
--rw-r--r--   0        0        0     3868 2023-04-03 11:51:20.715510 hydrolib_core-0.5.1/hydrolib/core/dflowfm/obscrosssection/models.py
--rw-r--r--   0        0        0      178 2023-03-15 10:07:16.204070 hydrolib_core-0.5.1/hydrolib/core/dflowfm/onedfield/__init__.py
--rw-r--r--   0        0        0     4995 2023-03-15 10:07:16.204070 hydrolib_core-0.5.1/hydrolib/core/dflowfm/onedfield/models.py
--rw-r--r--   0        0        0      177 2023-03-15 10:07:16.205078 hydrolib_core-0.5.1/hydrolib/core/dflowfm/polyfile/__init__.py
--rw-r--r--   0        0        0     3233 2023-04-03 13:21:58.103586 hydrolib_core-0.5.1/hydrolib/core/dflowfm/polyfile/models.py
--rw-r--r--   0        0        0    20865 2023-04-14 13:35:23.828999 hydrolib_core-0.5.1/hydrolib/core/dflowfm/polyfile/parser.py
--rw-r--r--   0        0        0     3827 2023-04-14 13:35:23.828999 hydrolib_core-0.5.1/hydrolib/core/dflowfm/polyfile/serializer.py
--rw-r--r--   0        0        0      294 2023-03-15 10:07:16.206069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/storagenode/__init__.py
--rw-r--r--   0        0        0     9518 2023-04-03 11:51:20.718510 hydrolib_core-0.5.1/hydrolib/core/dflowfm/storagenode/models.py
--rw-r--r--   0        0        0      710 2023-03-15 10:07:16.206069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/structure/__init__.py
--rw-r--r--   0        0        0    47103 2023-04-17 14:40:32.114119 hydrolib_core-0.5.1/hydrolib/core/dflowfm/structure/models.py
--rw-r--r--   0        0        0       94 2023-04-17 14:40:38.662861 hydrolib_core-0.5.1/hydrolib/core/dflowfm/tim/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-17 14:40:38.662861 hydrolib_core-0.5.1/hydrolib/core/dflowfm/tim/models.py
--rw-r--r--   0        0        0     3930 2023-04-17 14:40:38.662861 hydrolib_core-0.5.1/hydrolib/core/dflowfm/tim/parser.py
--rw-r--r--   0        0        0     4988 2023-04-17 14:40:38.663861 hydrolib_core-0.5.1/hydrolib/core/dflowfm/tim/serializer.py
--rw-r--r--   0        0        0       92 2023-04-03 13:21:58.105587 hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyn/__init__.py
--rw-r--r--   0        0        0     1954 2023-04-17 14:40:38.663861 hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyn/models.py
--rw-r--r--   0        0        0     2602 2023-04-17 14:40:38.663861 hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyn/parser.py
--rw-r--r--   0        0        0     1638 2023-04-14 13:35:23.831997 hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyn/serializer.py
--rw-r--r--   0        0        0       92 2023-03-15 10:07:16.207069 hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyz/__init__.py
--rw-r--r--   0        0        0     1711 2023-04-12 13:31:27.348984 hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyz/models.py
--rw-r--r--   0        0        0     1693 2023-04-14 13:35:23.831997 hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyz/parser.py
--rw-r--r--   0        0        0     1432 2023-04-14 13:35:23.831997 hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyz/serializer.py
--rw-r--r--   0        0        0      592 2023-03-15 10:07:16.208069 hydrolib_core-0.5.1/hydrolib/core/dimr/__init__.py
--rw-r--r--   0        0        0    10577 2023-04-12 09:08:24.402032 hydrolib_core-0.5.1/hydrolib/core/dimr/models.py
--rw-r--r--   0        0        0     1913 2023-03-15 10:07:16.209070 hydrolib_core-0.5.1/hydrolib/core/dimr/parser.py
--rw-r--r--   0        0        0     3232 2023-04-14 11:15:00.138188 hydrolib_core-0.5.1/hydrolib/core/dimr/serializer.py
--rw-r--r--   0        0        0        2 2023-03-15 10:07:16.209070 hydrolib_core-0.5.1/hydrolib/core/geometry/__init__ .py
--rw-r--r--   0        0        0        2 2023-03-15 10:07:16.210070 hydrolib_core-0.5.1/hydrolib/core/modeldata/__init__ .py
--rw-r--r--   0        0        0       88 2023-03-15 10:07:16.210070 hydrolib_core-0.5.1/hydrolib/core/rr/__init__.py
--rw-r--r--   0        0        0      104 2023-03-15 10:07:16.210070 hydrolib_core-0.5.1/hydrolib/core/rr/meteo/__init__.py
--rw-r--r--   0        0        0     3194 2023-04-03 13:21:58.108587 hydrolib_core-0.5.1/hydrolib/core/rr/meteo/models.py
--rw-r--r--   0        0        0     6251 2023-03-15 10:07:16.211070 hydrolib_core-0.5.1/hydrolib/core/rr/meteo/parser.py
--rw-r--r--   0        0        0     8518 2023-04-03 13:21:58.108587 hydrolib_core-0.5.1/hydrolib/core/rr/meteo/serializer.py
--rw-r--r--   0        0        0    23015 2023-04-03 13:21:58.109598 hydrolib_core-0.5.1/hydrolib/core/rr/models.py
--rw-r--r--   0        0        0     1684 2023-04-14 13:35:23.832997 hydrolib_core-0.5.1/hydrolib/core/rr/parser.py
--rw-r--r--   0        0        0    14333 2023-04-14 13:35:23.832997 hydrolib_core-0.5.1/hydrolib/core/rr/serializer.py
--rw-r--r--   0        0        0      130 2023-03-15 10:07:16.212070 hydrolib_core-0.5.1/hydrolib/core/rr/topology/__init__.py
--rw-r--r--   0        0        0     6172 2023-04-03 13:21:58.110596 hydrolib_core-0.5.1/hydrolib/core/rr/topology/models.py
--rw-r--r--   0        0        0     2116 2023-04-14 13:35:23.833997 hydrolib_core-0.5.1/hydrolib/core/rr/topology/parser.py
--rw-r--r--   0        0        0     2839 2023-04-14 13:35:23.833997 hydrolib_core-0.5.1/hydrolib/core/rr/topology/serializer.py
--rw-r--r--   0        0        0     8831 2023-04-03 13:21:58.110596 hydrolib_core-0.5.1/hydrolib/core/utils.py
--rw-r--r--   0        0        0     1086 2023-03-15 10:07:16.160448 hydrolib_core-0.5.1/LICENSE
--rw-r--r--   0        0        0     2230 2023-04-17 14:49:57.254848 hydrolib_core-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1917 2023-03-15 10:07:16.160448 hydrolib_core-0.5.1/README.md
--rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 hydrolib_core-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       79 2022-11-25 07:07:38.494440 hydrolib_core-0.5.2/hydrolib/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-19 12:18:54.965993 hydrolib_core-0.5.2/hydrolib/core/__init__.py
+-rw-r--r--   0        0        0      416 2023-04-14 13:54:07.463910 hydrolib_core-0.5.2/hydrolib/core/base.py
+-rw-r--r--   0        0        0    52489 2023-04-14 11:13:48.562025 hydrolib_core-0.5.2/hydrolib/core/basemodel.py
+-rw-r--r--   0        0        0      253 2022-11-25 07:07:38.498443 hydrolib_core-0.5.2/hydrolib/core/config.py
+-rw-r--r--   0        0        0      441 2023-04-14 13:54:07.464910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/__init__.py
+-rw-r--r--   0        0        0      730 2022-12-16 15:33:47.602589 hydrolib_core-0.5.2/hydrolib/core/dflowfm/bc/__init__.py
+-rw-r--r--   0        0        0    32784 2023-04-14 13:54:07.464910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/bc/models.py
+-rw-r--r--   0        0        0       84 2023-04-14 13:54:07.465911 hydrolib_core-0.5.2/hydrolib/core/dflowfm/common/__init__.py
+-rw-r--r--   0        0        0     1221 2023-04-14 13:54:07.465911 hydrolib_core-0.5.2/hydrolib/core/dflowfm/common/models.py
+-rw-r--r--   0        0        0      546 2022-12-16 15:33:47.603589 hydrolib_core-0.5.2/hydrolib/core/dflowfm/crosssection/__init__.py
+-rw-r--r--   0        0        0    30678 2023-04-14 11:13:48.564025 hydrolib_core-0.5.2/hydrolib/core/dflowfm/crosssection/models.py
+-rw-r--r--   0        0        0      169 2023-04-14 11:13:48.564025 hydrolib_core-0.5.2/hydrolib/core/dflowfm/ext/__init__.py
+-rw-r--r--   0        0        0    11317 2023-04-14 11:13:48.564025 hydrolib_core-0.5.2/hydrolib/core/dflowfm/ext/models.py
+-rw-r--r--   0        0        0      374 2023-04-14 13:54:07.466911 hydrolib_core-0.5.2/hydrolib/core/dflowfm/extold/__init__.py
+-rw-r--r--   0        0        0      481 2023-04-14 13:54:07.466911 hydrolib_core-0.5.2/hydrolib/core/dflowfm/extold/common_io.py
+-rw-r--r--   0        0        0    25101 2023-04-19 12:16:37.782768 hydrolib_core-0.5.2/hydrolib/core/dflowfm/extold/models.py
+-rw-r--r--   0        0        0     4397 2023-04-14 13:54:07.467910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/extold/parser.py
+-rw-r--r--   0        0        0     3594 2023-04-14 13:54:07.467910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/extold/serializer.py
+-rw-r--r--   0        0        0      211 2022-12-16 15:33:47.605591 hydrolib_core-0.5.2/hydrolib/core/dflowfm/friction/__init__.py
+-rw-r--r--   0        0        0     9410 2023-03-10 13:38:25.779863 hydrolib_core-0.5.2/hydrolib/core/dflowfm/friction/models.py
+-rw-r--r--   0        0        0      131 2022-12-16 15:33:47.605591 hydrolib_core-0.5.2/hydrolib/core/dflowfm/gui/__init__.py
+-rw-r--r--   0        0        0     4874 2022-12-16 15:33:47.606594 hydrolib_core-0.5.2/hydrolib/core/dflowfm/gui/models.py
+-rw-r--r--   0        0        0        0 2022-12-16 15:33:47.606594 hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/__init__.py
+-rw-r--r--   0        0        0     4826 2022-12-16 15:33:47.607592 hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/io_models.py
+-rw-r--r--   0        0        0    10126 2023-04-14 11:13:48.565025 hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/models.py
+-rw-r--r--   0        0        0    15084 2023-04-19 12:16:37.783769 hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/parser.py
+-rw-r--r--   0        0        0    13840 2023-04-14 13:54:07.468910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/serializer.py
+-rw-r--r--   0        0        0    24384 2023-04-14 11:13:48.566026 hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/util.py
+-rw-r--r--   0        0        0      352 2023-04-14 13:54:07.469910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/inifield/__init__.py
+-rw-r--r--   0        0        0     8705 2023-04-14 13:54:07.469910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/inifield/models.py
+-rw-r--r--   0        0        0      962 2022-12-16 15:33:47.609591 hydrolib_core-0.5.2/hydrolib/core/dflowfm/mdu/__init__.py
+-rw-r--r--   0        0        0    96098 2023-04-19 12:16:37.785768 hydrolib_core-0.5.2/hydrolib/core/dflowfm/mdu/models.py
+-rw-r--r--   0        0        0      194 2022-12-16 15:33:47.610623 hydrolib_core-0.5.2/hydrolib/core/dflowfm/net/__init__.py
+-rw-r--r--   0        0        0    48587 2023-04-07 09:26:37.764409 hydrolib_core-0.5.2/hydrolib/core/dflowfm/net/models.py
+-rw-r--r--   0        0        0    11085 2022-12-16 15:33:47.611590 hydrolib_core-0.5.2/hydrolib/core/dflowfm/net/reader.py
+-rw-r--r--   0        0        0     4560 2023-04-14 11:13:48.568024 hydrolib_core-0.5.2/hydrolib/core/dflowfm/net/ugrid_conventions.json
+-rw-r--r--   0        0        0    20587 2022-12-16 15:33:47.611590 hydrolib_core-0.5.2/hydrolib/core/dflowfm/net/writer.py
+-rw-r--r--   0        0        0      172 2022-12-16 15:33:47.612625 hydrolib_core-0.5.2/hydrolib/core/dflowfm/obs/__init__.py
+-rw-r--r--   0        0        0     4260 2023-03-17 10:46:48.878436 hydrolib_core-0.5.2/hydrolib/core/dflowfm/obs/models.py
+-rw-r--r--   0        0        0      254 2022-12-16 15:33:47.612625 hydrolib_core-0.5.2/hydrolib/core/dflowfm/obscrosssection/__init__.py
+-rw-r--r--   0        0        0     3868 2023-03-10 08:41:16.684176 hydrolib_core-0.5.2/hydrolib/core/dflowfm/obscrosssection/models.py
+-rw-r--r--   0        0        0      178 2022-12-16 15:33:47.613590 hydrolib_core-0.5.2/hydrolib/core/dflowfm/onedfield/__init__.py
+-rw-r--r--   0        0        0     4995 2022-12-16 15:33:47.613590 hydrolib_core-0.5.2/hydrolib/core/dflowfm/onedfield/models.py
+-rw-r--r--   0        0        0      177 2022-12-16 15:33:47.613590 hydrolib_core-0.5.2/hydrolib/core/dflowfm/polyfile/__init__.py
+-rw-r--r--   0        0        0     3233 2023-04-03 07:38:39.155382 hydrolib_core-0.5.2/hydrolib/core/dflowfm/polyfile/models.py
+-rw-r--r--   0        0        0    20865 2023-04-14 13:54:07.471910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/polyfile/parser.py
+-rw-r--r--   0        0        0     3827 2023-04-14 13:54:07.472911 hydrolib_core-0.5.2/hydrolib/core/dflowfm/polyfile/serializer.py
+-rw-r--r--   0        0        0      294 2022-12-16 15:33:47.615590 hydrolib_core-0.5.2/hydrolib/core/dflowfm/storagenode/__init__.py
+-rw-r--r--   0        0        0     9518 2023-03-10 08:41:16.685175 hydrolib_core-0.5.2/hydrolib/core/dflowfm/storagenode/models.py
+-rw-r--r--   0        0        0      710 2022-12-16 15:33:47.616590 hydrolib_core-0.5.2/hydrolib/core/dflowfm/structure/__init__.py
+-rw-r--r--   0        0        0    47103 2023-04-14 11:13:48.568024 hydrolib_core-0.5.2/hydrolib/core/dflowfm/structure/models.py
+-rw-r--r--   0        0        0       94 2023-04-17 07:33:25.739287 hydrolib_core-0.5.2/hydrolib/core/dflowfm/tim/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-17 07:33:25.740325 hydrolib_core-0.5.2/hydrolib/core/dflowfm/tim/models.py
+-rw-r--r--   0        0        0     3930 2023-04-17 07:33:25.740325 hydrolib_core-0.5.2/hydrolib/core/dflowfm/tim/parser.py
+-rw-r--r--   0        0        0     4988 2023-04-17 07:33:25.741286 hydrolib_core-0.5.2/hydrolib/core/dflowfm/tim/serializer.py
+-rw-r--r--   0        0        0       92 2023-04-03 07:38:39.157379 hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyn/__init__.py
+-rw-r--r--   0        0        0     1954 2023-04-17 12:31:08.941008 hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyn/models.py
+-rw-r--r--   0        0        0     2602 2023-04-17 12:31:08.941008 hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyn/parser.py
+-rw-r--r--   0        0        0     1638 2023-04-14 13:54:07.475910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyn/serializer.py
+-rw-r--r--   0        0        0       92 2022-12-16 15:33:47.616590 hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyz/__init__.py
+-rw-r--r--   0        0        0     1711 2023-04-14 11:13:48.572028 hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyz/models.py
+-rw-r--r--   0        0        0     1693 2023-04-14 13:54:07.476910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyz/parser.py
+-rw-r--r--   0        0        0     1432 2023-04-14 13:54:07.476910 hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyz/serializer.py
+-rw-r--r--   0        0        0      592 2022-12-16 15:33:47.618590 hydrolib_core-0.5.2/hydrolib/core/dimr/__init__.py
+-rw-r--r--   0        0        0    10577 2023-04-14 11:13:48.572028 hydrolib_core-0.5.2/hydrolib/core/dimr/models.py
+-rw-r--r--   0        0        0     1913 2023-03-31 12:38:47.867932 hydrolib_core-0.5.2/hydrolib/core/dimr/parser.py
+-rw-r--r--   0        0        0     3232 2023-04-14 11:13:43.910579 hydrolib_core-0.5.2/hydrolib/core/dimr/serializer.py
+-rw-r--r--   0        0        0        2 2022-11-25 07:07:38.499450 hydrolib_core-0.5.2/hydrolib/core/geometry/__init__ .py
+-rw-r--r--   0        0        0        2 2022-11-25 07:07:38.549956 hydrolib_core-0.5.2/hydrolib/core/modeldata/__init__ .py
+-rw-r--r--   0        0        0       88 2022-12-16 15:33:47.619589 hydrolib_core-0.5.2/hydrolib/core/rr/__init__.py
+-rw-r--r--   0        0        0      104 2022-12-16 15:33:47.619589 hydrolib_core-0.5.2/hydrolib/core/rr/meteo/__init__.py
+-rw-r--r--   0        0        0     3194 2023-04-03 07:38:39.162303 hydrolib_core-0.5.2/hydrolib/core/rr/meteo/models.py
+-rw-r--r--   0        0        0     6251 2023-04-03 07:38:39.164304 hydrolib_core-0.5.2/hydrolib/core/rr/meteo/parser.py
+-rw-r--r--   0        0        0     8518 2023-04-03 07:38:39.164304 hydrolib_core-0.5.2/hydrolib/core/rr/meteo/serializer.py
+-rw-r--r--   0        0        0    23015 2023-04-03 07:38:39.165304 hydrolib_core-0.5.2/hydrolib/core/rr/models.py
+-rw-r--r--   0        0        0     1684 2023-04-14 13:54:07.477908 hydrolib_core-0.5.2/hydrolib/core/rr/parser.py
+-rw-r--r--   0        0        0    14333 2023-04-14 13:54:07.478911 hydrolib_core-0.5.2/hydrolib/core/rr/serializer.py
+-rw-r--r--   0        0        0      130 2022-12-16 15:33:47.622593 hydrolib_core-0.5.2/hydrolib/core/rr/topology/__init__.py
+-rw-r--r--   0        0        0     6172 2023-04-03 07:38:39.166309 hydrolib_core-0.5.2/hydrolib/core/rr/topology/models.py
+-rw-r--r--   0        0        0     2116 2023-04-14 13:54:07.478911 hydrolib_core-0.5.2/hydrolib/core/rr/topology/parser.py
+-rw-r--r--   0        0        0     2839 2023-04-14 13:54:07.479911 hydrolib_core-0.5.2/hydrolib/core/rr/topology/serializer.py
+-rw-r--r--   0        0        0     8831 2023-04-03 07:38:39.167308 hydrolib_core-0.5.2/hydrolib/core/utils.py
+-rw-r--r--   0        0        0     1086 2022-07-08 13:00:42.520836 hydrolib_core-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2230 2023-04-19 12:18:55.229987 hydrolib_core-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1917 2022-11-18 09:35:39.575195 hydrolib_core-0.5.2/README.md
+-rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 hydrolib_core-0.5.2/setup.py
+-rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 hydrolib_core-0.5.2/PKG-INFO
```

### Comparing `hydrolib_core-0.5.1/hydrolib/core/basemodel.py` & `hydrolib_core-0.5.2/hydrolib/core/basemodel.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/bc/__init__.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/bc/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/bc/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/bc/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/common/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/common/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/crosssection/__init__.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/crosssection/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/crosssection/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/crosssection/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/ext/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/ext/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/extold/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/extold/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
     """Wave significant height"""
     WavePeriod = "waveperiod"
     """Wave period"""
 
 
 class ExtOldFileType(IntEnum):
     """Enum class containing the valid values for the `filetype` attribute
-    in the [ExtForcing][hydrolib.core.dflowfm.extold.models.ExtForcing] class.
+    in the [ExtOldForcing][hydrolib.core.dflowfm.extold.models.ExtOldForcing] class.
     """
 
     TimeSeries = 1
     """1. Time series"""
     TimeSeriesMagnitudeAndDirection = 2
     """2. Time series magnitude and direction"""
     SpatiallyVaryingWindPressure = 3
@@ -270,15 +270,15 @@
     """11. NetCDF grid data (e.g. meteo fields)"""
     NetCDFWaveData = 14
     """14. NetCDF wave data"""
 
 
 class ExtOldMethod(IntEnum):
     """Enum class containing the valid values for the `method` attribute
-    in the [ExtForcing][hydrolib.core.dflowfm.extold.models.ExtForcing] class.
+    in the [ExtOldForcing][hydrolib.core.dflowfm.extold.models.ExtOldForcing] class.
     """
 
     PassThrough = 1
     """1. Pass through (no interpolation)"""
     InterpolateTimeAndSpace = 2
     """2. Interpolate time and space"""
     InterpolateTimeAndSpaceSaveWeights = 3
@@ -291,15 +291,15 @@
     """6. Averaging in space"""
     InterpolateExtrapolateTime = 7
     """7. Interpolate/Extrapolate time"""
 
 
 class ExtOldExtrapolationMethod(IntEnum):
     """Enum class containing the valid values for the `extrapolation_method` attribute
-    in the [ExtForcing][hydrolib.core.dflowfm.extold.models.ExtForcing] class.
+    in the [ExtOldForcing][hydrolib.core.dflowfm.extold.models.ExtOldForcing] class.
     """
 
     NoSpatialExtrapolation = 0
     """0. No spatial extrapolation."""
     SpatialExtrapolationOutsideOfSourceDataBoundingBox = 1
     """1. Do spatial extrapolation outside of source data bounding box."""
 
@@ -546,15 +546,15 @@
 
     This model is typically referenced under a [FMModel][hydrolib.core.dflowfm.mdu.models.FMModel]`.external_forcing.extforcefile`.
     """
 
     comment: List[str] = HEADER.splitlines()[1:]
     """List[str]: The comments in the header of the external forcing file."""
     forcing: List[ExtOldForcing] = []
-    """List[ExtForcing]: The external forcing blocks in the external forcing file."""
+    """List[ExtOldForcing]: The external forcing/QUANTITY blocks in the external forcing file."""
 
     @classmethod
     def _ext(cls) -> str:
         return ".ext"
 
     @classmethod
     def _filename(cls) -> str:
```

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/extold/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/extold/parser.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/extold/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/extold/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/friction/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/friction/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/gui/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/gui/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/io_models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/io_models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
             config = ParserConfig()
         parser = cls(config)
 
         progline = re.compile(
             r"^([^#]*=\s*)([^#]*)(#.*)?"
         )  # matches whole line: "Field = Value Maybe more # optional comment"
         progfloat = re.compile(
-            r"([\d.]+)([dD])([+\-]?\d+)"
+            r"([\d.]+)([dD])([+\-]?\d{1,3})"
         )  # matches a float value: 1d9, 1D-3, 1.D+4, etc.
 
         with filepath.open(encoding="utf8") as f:
             for line in f:
                 # Replace Fortran scientific notation for doubles
                 # Match number d/D +/- number (e.g. 1d-05 or 1.23D+01 or 1.d-4)
                 match = progline.match(line)
```

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/ini/util.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/ini/util.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/inifield/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/inifield/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/mdu/__init__.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/mdu/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/mdu/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/mdu/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
     no = 0
     autostart = 1
     autostartstop = 2
 
 
 class General(INIGeneral):
+    """The MDU file's `[General]` section with file meta data."""
+
     class Comments(INIBasedModel.Comments):
         program: Optional[str] = Field("Program.", alias="program")
         version: Optional[str] = Field(
             "Version number of computational kernel", alias="version"
         )
         filetype: Optional[str] = Field("File type. Do not edit this", alias="fileType")
         fileversion: Optional[str] = Field(
@@ -1760,15 +1762,15 @@
         default_factory=lambda: DiskOnlyFileModel(None), alias="AreaFile"
     )
 
 
 class InfiltrationMethod(IntEnum):
     """
     Enum class containing the valid values for the Infiltrationmodel
-    attribute in the [Groundwater][hydrolib.core.dflowfm.mdu.models.Groundwater] class.
+    attribute in the [GroundWater][hydrolib.core.dflowfm.mdu.models.GroundWater] class.
     """
 
     NoInfiltration = 0
     InterceptionLayer = 1
     ConstantInfiltrationCapacity = 2
     ModelUnsaturatedSaturated = 3
     Horton = 4
```

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/net/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/net/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/net/reader.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/net/reader.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/net/ugrid_conventions.json` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/net/ugrid_conventions.json`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/net/writer.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/net/writer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/obs/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/obs/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/obscrosssection/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/obscrosssection/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/onedfield/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/onedfield/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/polyfile/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/polyfile/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/polyfile/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/polyfile/parser.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/polyfile/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/polyfile/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/storagenode/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/storagenode/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/structure/__init__.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/structure/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/structure/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/tim/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/tim/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/tim/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/tim/parser.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/tim/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/tim/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyn/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyn/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyn/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyn/parser.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyn/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyn/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyz/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyz/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyz/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyz/parser.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dflowfm/xyz/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/dflowfm/xyz/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dimr/__init__.py` & `hydrolib_core-0.5.2/hydrolib/core/dimr/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dimr/models.py` & `hydrolib_core-0.5.2/hydrolib/core/dimr/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dimr/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/dimr/parser.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/dimr/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/dimr/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/rr/meteo/models.py` & `hydrolib_core-0.5.2/hydrolib/core/rr/meteo/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/rr/meteo/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/rr/meteo/parser.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/rr/meteo/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/rr/meteo/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/rr/models.py` & `hydrolib_core-0.5.2/hydrolib/core/rr/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/rr/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/rr/parser.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/rr/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/rr/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/rr/topology/models.py` & `hydrolib_core-0.5.2/hydrolib/core/rr/topology/models.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/rr/topology/parser.py` & `hydrolib_core-0.5.2/hydrolib/core/rr/topology/parser.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/rr/topology/serializer.py` & `hydrolib_core-0.5.2/hydrolib/core/rr/topology/serializer.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/hydrolib/core/utils.py` & `hydrolib_core-0.5.2/hydrolib/core/utils.py`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/LICENSE` & `hydrolib_core-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/pyproject.toml` & `hydrolib_core-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydrolib-core"
-version = "0.5.1"
+version = "0.5.2"
 description = "Python wrappers around D-HYDRO Suite."
 authors = ["Deltares"]
 license = "MIT"
 packages = [
     { include = "hydrolib"},
 ]
 readme = "README.md"
@@ -46,15 +46,15 @@
 markupsafe = "<2.1"
 mkdocs-jupyter = "^0.21.0"
 jupyter = "^1.0.0"
 ipykernel = "^6.15.0"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.1"
+version = "0.5.2"
 tag_format = "$version"
 version_files = [
     "hydrolib/core/__init__.py",
     "pyproject.toml:version",
     "tests/data/reference/dimr/test_serialize.xml:createdBy",
     "tests/data/reference/model/test_dimr_model_save.xml:createdBy",
     "tests/data/reference/crosssection/crsloc.ini:HYDROLIB-core"
```

### Comparing `hydrolib_core-0.5.1/README.md` & `hydrolib_core-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hydrolib_core-0.5.1/PKG-INFO` & `hydrolib_core-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrolib-core
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python wrappers around D-HYDRO Suite.
 Home-page: https://deltares.github.io/HYDROLIB-core
 License: MIT
 Author: Deltares
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

