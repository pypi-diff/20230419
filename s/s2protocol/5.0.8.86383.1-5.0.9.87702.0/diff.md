# Comparing `tmp/s2protocol-5.0.8.86383.1.tar.gz` & `tmp/s2protocol-5.0.9.87702.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/s2protocol-5.0.8.86383.1.tar", last modified: Wed Oct 20 17:14:40 2021, max compression
+gzip compressed data, was "dist/s2protocol-5.0.9.87702.0.tar", last modified: Wed Mar 16 01:40:42 2022, max compression
```

## Comparing `s2protocol-5.0.8.86383.1.tar` & `s2protocol-5.0.9.87702.0.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/_static/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/docs/_templates/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/_templates/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/docs/flags/
--rw-r--r--   0 root         (0) root         (0)     5289 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/flags/details.md
--rw-r--r--   0 root         (0) root         (0)    27843 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/flags/initdata.md
--rw-r--r--   0 root         (0) root         (0)     2863 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/flags/messageevents.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/docs/refs/
--rw-r--r--   0 root         (0) root         (0)      464 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/refs/s2protocol.rst
--rw-r--r--   0 root         (0) root         (0)     4606 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      890 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/README.md
--rw-r--r--   0 root         (0) root         (0)     7110 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      907 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/events.rst
--rw-r--r--   0 root         (0) root         (0)     1444 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     4519 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     2101 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/tutorial.rst
--rw-r--r--   0 root         (0) root         (0)     2890 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/docs/tutorial_API.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/s2protocol/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/
--rw-r--r--   0 root         (0) root         (0)     1941 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20520 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol15405.py
--rw-r--r--   0 root         (0) root         (0)    21293 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol16561.py
--rw-r--r--   0 root         (0) root         (0)    21293 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol16605.py
--rw-r--r--   0 root         (0) root         (0)    21293 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol16755.py
--rw-r--r--   0 root         (0) root         (0)    21293 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol16939.py
--rw-r--r--   0 root         (0) root         (0)    21560 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol17266.py
--rw-r--r--   0 root         (0) root         (0)    21560 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol17326.py
--rw-r--r--   0 root         (0) root         (0)    21560 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol18092.py
--rw-r--r--   0 root         (0) root         (0)    21560 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol18468.py
--rw-r--r--   0 root         (0) root         (0)    21560 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol18574.py
--rw-r--r--   0 root         (0) root         (0)    21616 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol19132.py
--rw-r--r--   0 root         (0) root         (0)    21711 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol19458.py
--rw-r--r--   0 root         (0) root         (0)    21711 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol19595.py
--rw-r--r--   0 root         (0) root         (0)    21711 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol19679.py
--rw-r--r--   0 root         (0) root         (0)    21711 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol21029.py
--rw-r--r--   0 root         (0) root         (0)    22871 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol22612.py
--rw-r--r--   0 root         (0) root         (0)    22871 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol23260.py
--rw-r--r--   0 root         (0) root         (0)    24026 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol24944.py
--rw-r--r--   0 root         (0) root         (0)    27458 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol26490.py
--rw-r--r--   0 root         (0) root         (0)    27753 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol27950.py
--rw-r--r--   0 root         (0) root         (0)    27753 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol28272.py
--rw-r--r--   0 root         (0) root         (0)    27753 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol28667.py
--rw-r--r--   0 root         (0) root         (0)    27775 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol32283.py
--rw-r--r--   0 root         (0) root         (0)    31174 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol51702.py
--rw-r--r--   0 root         (0) root         (0)    31174 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol52910.py
--rw-r--r--   0 root         (0) root         (0)    31174 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol53644.py
--rw-r--r--   0 root         (0) root         (0)    31260 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol54518.py
--rw-r--r--   0 root         (0) root         (0)    31563 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol55505.py
--rw-r--r--   0 root         (0) root         (0)    31563 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol55958.py
--rw-r--r--   0 root         (0) root         (0)    31563 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol56787.py
--rw-r--r--   0 root         (0) root         (0)    31563 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol57507.py
--rw-r--r--   0 root         (0) root         (0)    31563 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol58400.py
--rw-r--r--   0 root         (0) root         (0)    31078 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol59587.py
--rw-r--r--   0 root         (0) root         (0)    31078 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol60196.py
--rw-r--r--   0 root         (0) root         (0)    31078 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol60321.py
--rw-r--r--   0 root         (0) root         (0)    31078 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol62347.py
--rw-r--r--   0 root         (0) root         (0)    31078 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol62848.py
--rw-r--r--   0 root         (0) root         (0)    31078 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol63454.py
--rw-r--r--   0 root         (0) root         (0)    31078 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol64469.py
--rw-r--r--   0 root         (0) root         (0)    31078 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol65094.py
--rw-r--r--   0 root         (0) root         (0)    31078 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol65384.py
--rw-r--r--   0 root         (0) root         (0)    31349 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol65895.py
--rw-r--r--   0 root         (0) root         (0)    31349 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol66668.py
--rw-r--r--   0 root         (0) root         (0)    31349 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol67188.py
--rw-r--r--   0 root         (0) root         (0)    31349 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol67926.py
--rw-r--r--   0 root         (0) root         (0)    31349 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol69232.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol70154.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol71061.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol71523.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol71663.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol72282.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol73286.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol73559.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol73620.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol74071.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol74456.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol74741.py
--rw-r--r--   0 root         (0) root         (0)    31383 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol75025.py
--rw-r--r--   0 root         (0) root         (0)    31404 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol75689.py
--rw-r--r--   0 root         (0) root         (0)    31404 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol75800.py
--rw-r--r--   0 root         (0) root         (0)    31404 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol76052.py
--rw-r--r--   0 root         (0) root         (0)    31404 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol76114.py
--rw-r--r--   0 root         (0) root         (0)    31523 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol77379.py
--rw-r--r--   0 root         (0) root         (0)    31523 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol77535.py
--rw-r--r--   0 root         (0) root         (0)    31523 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol77661.py
--rw-r--r--   0 root         (0) root         (0)    31523 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol78285.py
--rw-r--r--   0 root         (0) root         (0)    31523 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol80669.py
--rw-r--r--   0 root         (0) root         (0)    31561 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol80949.py
--rw-r--r--   0 root         (0) root         (0)    31561 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol81009.py
--rw-r--r--   0 root         (0) root         (0)    31561 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol82457.py
--rw-r--r--   0 root         (0) root         (0)    31561 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol82893.py
--rw-r--r--   0 root         (0) root         (0)    31561 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol83830.py
--rw-r--r--   0 root         (0) root         (0)    31561 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol84643.py
--rw-r--r--   0 root         (0) root         (0)    31561 2021-10-20 17:14:36.000000 s2protocol-5.0.8.86383.1/s2protocol/versions/protocol86383.py
--rw-r--r--   0 root         (0) root         (0)      188 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1472 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/attributes.py
--rw-r--r--   0 root         (0) root         (0)      951 2021-10-20 17:14:37.000000 s2protocol-5.0.8.86383.1/s2protocol/build.py
--rw-r--r--   0 root         (0) root         (0)      326 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/compat.py
--rw-r--r--   0 root         (0) root         (0)    10010 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/decoders.py
--rw-r--r--   0 root         (0) root         (0)     2237 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/diff.py
--rw-r--r--   0 root         (0) root         (0)     9610 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/encoders.py
--rw-r--r--   0 root         (0) root         (0)       48 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/namespaces.py
--rwxr-xr-x   0 root         (0) root         (0)    13493 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/s2protocol/s2_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/s2protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)      833 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/s2protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3490 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/s2protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/s2protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/s2protocol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       27 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/s2protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/s2protocol.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1072 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       59 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3871 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1407 2021-10-20 17:14:30.000000 s2protocol-5.0.8.86383.1/setup.py
--rw-r--r--   0 root         (0) root         (0)      833 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       59 2021-10-20 17:14:40.000000 s2protocol-5.0.8.86383.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/_static/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/docs/_templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/_templates/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/docs/flags/
+-rw-r--r--   0 root         (0) root         (0)     5289 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/flags/details.md
+-rw-r--r--   0 root         (0) root         (0)    27843 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/flags/initdata.md
+-rw-r--r--   0 root         (0) root         (0)     2863 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/flags/messageevents.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/docs/refs/
+-rw-r--r--   0 root         (0) root         (0)      464 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/refs/s2protocol.rst
+-rw-r--r--   0 root         (0) root         (0)     4606 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      890 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/README.md
+-rw-r--r--   0 root         (0) root         (0)     7110 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      907 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/events.rst
+-rw-r--r--   0 root         (0) root         (0)     1444 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     4519 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     2101 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/tutorial.rst
+-rw-r--r--   0 root         (0) root         (0)     2890 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/docs/tutorial_API.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/s2protocol/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/
+-rw-r--r--   0 root         (0) root         (0)     1941 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20520 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol15405.py
+-rw-r--r--   0 root         (0) root         (0)    21293 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol16561.py
+-rw-r--r--   0 root         (0) root         (0)    21293 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol16605.py
+-rw-r--r--   0 root         (0) root         (0)    21293 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol16755.py
+-rw-r--r--   0 root         (0) root         (0)    21293 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol16939.py
+-rw-r--r--   0 root         (0) root         (0)    21560 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol17266.py
+-rw-r--r--   0 root         (0) root         (0)    21560 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol17326.py
+-rw-r--r--   0 root         (0) root         (0)    21560 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol18092.py
+-rw-r--r--   0 root         (0) root         (0)    21560 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol18468.py
+-rw-r--r--   0 root         (0) root         (0)    21560 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol18574.py
+-rw-r--r--   0 root         (0) root         (0)    21616 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol19132.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol19458.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol19595.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol19679.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol21029.py
+-rw-r--r--   0 root         (0) root         (0)    22871 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol22612.py
+-rw-r--r--   0 root         (0) root         (0)    22871 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol23260.py
+-rw-r--r--   0 root         (0) root         (0)    24026 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol24944.py
+-rw-r--r--   0 root         (0) root         (0)    27458 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol26490.py
+-rw-r--r--   0 root         (0) root         (0)    27753 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol27950.py
+-rw-r--r--   0 root         (0) root         (0)    27753 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol28272.py
+-rw-r--r--   0 root         (0) root         (0)    27753 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol28667.py
+-rw-r--r--   0 root         (0) root         (0)    27775 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol32283.py
+-rw-r--r--   0 root         (0) root         (0)    31174 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol51702.py
+-rw-r--r--   0 root         (0) root         (0)    31174 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol52910.py
+-rw-r--r--   0 root         (0) root         (0)    31174 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol53644.py
+-rw-r--r--   0 root         (0) root         (0)    31260 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol54518.py
+-rw-r--r--   0 root         (0) root         (0)    31563 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol55505.py
+-rw-r--r--   0 root         (0) root         (0)    31563 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol55958.py
+-rw-r--r--   0 root         (0) root         (0)    31563 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol56787.py
+-rw-r--r--   0 root         (0) root         (0)    31563 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol57507.py
+-rw-r--r--   0 root         (0) root         (0)    31563 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol58400.py
+-rw-r--r--   0 root         (0) root         (0)    31078 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol59587.py
+-rw-r--r--   0 root         (0) root         (0)    31078 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol60196.py
+-rw-r--r--   0 root         (0) root         (0)    31078 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol60321.py
+-rw-r--r--   0 root         (0) root         (0)    31078 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol62347.py
+-rw-r--r--   0 root         (0) root         (0)    31078 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol62848.py
+-rw-r--r--   0 root         (0) root         (0)    31078 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol63454.py
+-rw-r--r--   0 root         (0) root         (0)    31078 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol64469.py
+-rw-r--r--   0 root         (0) root         (0)    31078 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol65094.py
+-rw-r--r--   0 root         (0) root         (0)    31078 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol65384.py
+-rw-r--r--   0 root         (0) root         (0)    31349 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol65895.py
+-rw-r--r--   0 root         (0) root         (0)    31349 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol66668.py
+-rw-r--r--   0 root         (0) root         (0)    31349 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol67188.py
+-rw-r--r--   0 root         (0) root         (0)    31349 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol67926.py
+-rw-r--r--   0 root         (0) root         (0)    31349 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol69232.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol70154.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol71061.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol71523.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol71663.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol72282.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol73286.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol73559.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol73620.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol74071.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol74456.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol74741.py
+-rw-r--r--   0 root         (0) root         (0)    31383 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol75025.py
+-rw-r--r--   0 root         (0) root         (0)    31404 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol75689.py
+-rw-r--r--   0 root         (0) root         (0)    31404 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol75800.py
+-rw-r--r--   0 root         (0) root         (0)    31404 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol76052.py
+-rw-r--r--   0 root         (0) root         (0)    31404 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol76114.py
+-rw-r--r--   0 root         (0) root         (0)    31523 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol77379.py
+-rw-r--r--   0 root         (0) root         (0)    31523 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol77535.py
+-rw-r--r--   0 root         (0) root         (0)    31523 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol77661.py
+-rw-r--r--   0 root         (0) root         (0)    31523 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol78285.py
+-rw-r--r--   0 root         (0) root         (0)    31523 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol80669.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol80949.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol81009.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol82457.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol82893.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol83830.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol84643.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol86383.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2022-03-16 01:40:34.000000 s2protocol-5.0.9.87702.0/s2protocol/versions/protocol87702.py
+-rw-r--r--   0 root         (0) root         (0)      188 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/attributes.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-03-16 01:40:39.000000 s2protocol-5.0.9.87702.0/s2protocol/build.py
+-rw-r--r--   0 root         (0) root         (0)      326 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/compat.py
+-rw-r--r--   0 root         (0) root         (0)    10010 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/decoders.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/diff.py
+-rw-r--r--   0 root         (0) root         (0)     9610 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/encoders.py
+-rw-r--r--   0 root         (0) root         (0)       48 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/namespaces.py
+-rwxr-xr-x   0 root         (0) root         (0)    13493 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/s2protocol/s2_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/s2protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      833 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/s2protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3527 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/s2protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/s2protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/s2protocol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/s2protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/s2protocol.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1072 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       59 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3871 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1407 2022-03-16 01:40:24.000000 s2protocol-5.0.9.87702.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      833 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       59 2022-03-16 01:40:42.000000 s2protocol-5.0.9.87702.0/setup.cfg
```

### Comparing `s2protocol-5.0.8.86383.1/docs/flags/details.md` & `s2protocol-5.0.9.87702.0/docs/flags/details.md`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/flags/initdata.md` & `s2protocol-5.0.9.87702.0/docs/flags/initdata.md`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/flags/messageevents.md` & `s2protocol-5.0.9.87702.0/docs/flags/messageevents.md`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/Makefile` & `s2protocol-5.0.9.87702.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/README.md` & `s2protocol-5.0.9.87702.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/conf.py` & `s2protocol-5.0.9.87702.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/events.rst` & `s2protocol-5.0.9.87702.0/docs/events.rst`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/index.rst` & `s2protocol-5.0.9.87702.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/make.bat` & `s2protocol-5.0.9.87702.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/tutorial.rst` & `s2protocol-5.0.9.87702.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/docs/tutorial_API.rst` & `s2protocol-5.0.9.87702.0/docs/tutorial_API.rst`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/__init__.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol15405.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol15405.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol16561.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol16561.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol16605.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol16605.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol16755.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol16755.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol16939.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol16939.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol17266.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol17266.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol17326.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol17326.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol18092.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol18092.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol18468.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol18468.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol18574.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol18574.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol19132.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol19132.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol19458.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol19458.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol19595.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol19595.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol19679.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol19679.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol21029.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol21029.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol22612.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol22612.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol23260.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol23260.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol24944.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol24944.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol26490.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol26490.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol27950.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol27950.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol28272.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol28272.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol28667.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol28667.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol32283.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol32283.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol51702.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol51702.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol52910.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol52910.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol53644.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol53644.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol54518.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol54518.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol55505.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol55505.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol55958.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol55958.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol56787.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol56787.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol57507.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol57507.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol58400.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol58400.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol59587.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol59587.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol60196.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol60196.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol60321.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol60321.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol62347.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol62347.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol62848.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol62848.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol63454.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol63454.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol64469.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol64469.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol65094.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol65094.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol65384.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol65384.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol65895.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol65895.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol66668.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol66668.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol67188.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol67188.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol67926.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol67926.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol69232.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol69232.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol70154.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol70154.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol71061.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol71061.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol71523.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol71523.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol71663.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol71663.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol72282.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol72282.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol73286.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol73286.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol73559.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol73559.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol73620.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol73620.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol74071.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol74071.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol74456.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol74456.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol74741.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol74741.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol75025.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol75025.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol75689.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol75689.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol75800.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol75800.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol76052.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol76052.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol76114.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol76114.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol77379.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol77379.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol77535.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol77535.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol77661.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol77661.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol78285.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol78285.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol80669.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol80669.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol80949.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol80949.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol81009.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol81009.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol82457.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol82457.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol82893.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol82893.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol83830.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol83830.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol84643.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol84643.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/versions/protocol86383.py` & `s2protocol-5.0.9.87702.0/s2protocol/versions/protocol86383.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/attributes.py` & `s2protocol-5.0.9.87702.0/s2protocol/attributes.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/build.py` & `s2protocol-5.0.9.87702.0/s2protocol/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ##
 ## This file is auto-generated by ../s2client-api-build/buildpylib/update_version_file.py
 ##
 import subprocess
 
 def game_version():
-    return "5.0.8.86383.1"
+    return "5.0.9.87702.0"
 
 
 def read_command_output(cmd):
     lines = []
     handle = subprocess.Popen(cmd, stdout=subprocess.PIPE)
     while True:
         line = handle.stdout.readline()
```

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/decoders.py` & `s2protocol-5.0.9.87702.0/s2protocol/decoders.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/diff.py` & `s2protocol-5.0.9.87702.0/s2protocol/diff.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/encoders.py` & `s2protocol-5.0.9.87702.0/s2protocol/encoders.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol/s2_cli.py` & `s2protocol-5.0.9.87702.0/s2protocol/s2_cli.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/s2protocol.egg-info/PKG-INFO` & `s2protocol-5.0.9.87702.0/s2protocol.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: s2protocol
-Version: 5.0.8.86383.1
+Version: 5.0.9.87702.0
 Summary: Python library to decode StarCraft II replay protocols
 Home-page: https://github.com/Blizzard/s2protocol
 Author: Blizzard Entertainment
 Author-email: s2github@blizzard.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `s2protocol-5.0.8.86383.1/s2protocol.egg-info/SOURCES.txt` & `s2protocol-5.0.9.87702.0/s2protocol.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -101,8 +101,9 @@
 s2protocol/versions/protocol80669.py
 s2protocol/versions/protocol80949.py
 s2protocol/versions/protocol81009.py
 s2protocol/versions/protocol82457.py
 s2protocol/versions/protocol82893.py
 s2protocol/versions/protocol83830.py
 s2protocol/versions/protocol84643.py
-s2protocol/versions/protocol86383.py
+s2protocol/versions/protocol86383.py
+s2protocol/versions/protocol87702.py
```

### Comparing `s2protocol-5.0.8.86383.1/LICENSE` & `s2protocol-5.0.9.87702.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/README.md` & `s2protocol-5.0.9.87702.0/README.md`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/setup.py` & `s2protocol-5.0.9.87702.0/setup.py`

 * *Files identical despite different names*

### Comparing `s2protocol-5.0.8.86383.1/PKG-INFO` & `s2protocol-5.0.9.87702.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: s2protocol
-Version: 5.0.8.86383.1
+Version: 5.0.9.87702.0
 Summary: Python library to decode StarCraft II replay protocols
 Home-page: https://github.com/Blizzard/s2protocol
 Author: Blizzard Entertainment
 Author-email: s2github@blizzard.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

