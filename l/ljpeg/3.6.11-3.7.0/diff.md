# Comparing `tmp/ljpeg-3.6.11.tar.gz` & `tmp/ljpeg-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ljpeg-3.6.11.tar", last modified: Sun Feb 26 00:27:54 2023, max compression
+gzip compressed data, was "ljpeg-3.7.0.tar", last modified: Wed Apr 19 06:43:01 2023, max compression
```

## Comparing `ljpeg-3.6.11.tar` & `ljpeg-3.7.0.tar`

### file list

```diff
@@ -1,80 +1,83 @@
-drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-02-26 00:27:54.986640 ljpeg-3.6.11/
--rw-r--r--   0 cest      (1001) cest      (1001)      588 2023-02-25 19:28:47.000000 ljpeg-3.6.11/.coveragerc
--rw-r--r--   0 cest      (1001) cest      (1001)     1055 2023-02-25 22:52:09.000000 ljpeg-3.6.11/.gitignore
--rw-r--r--   0 cest      (1001) cest      (1001)     1488 2023-02-25 20:11:19.000000 ljpeg-3.6.11/.pre-commit-config.yaml
--rw-r--r--   0 cest      (1001) cest      (1001)      530 2023-02-25 19:28:47.000000 ljpeg-3.6.11/.readthedocs.yml
--rw-r--r--   0 cest      (1001) cest      (1001)      110 2023-02-25 19:28:47.000000 ljpeg-3.6.11/AUTHORS.rst
--rw-r--r--   0 cest      (1001) cest      (1001)      138 2023-02-25 19:45:31.000000 ljpeg-3.6.11/CHANGELOG.rst
--rw-r--r--   0 cest      (1001) cest      (1001)    11063 2023-02-25 19:47:47.000000 ljpeg-3.6.11/CONTRIBUTING.rst
--rw-r--r--   0 cest      (1001) cest      (1001)     1291 2023-02-25 07:30:12.000000 ljpeg-3.6.11/LICENSE
--rw-r--r--   0 cest      (1001) cest      (1001)     1082 2023-02-25 19:28:47.000000 ljpeg-3.6.11/LICENSE.txt
--rw-r--r--   0 cest      (1001) cest      (1001)     4481 2023-02-26 00:27:54.986640 ljpeg-3.6.11/PKG-INFO
--rw-r--r--   0 cest      (1001) cest      (1001)     3605 2023-02-25 23:32:24.000000 ljpeg-3.6.11/README.rst
-drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-02-26 00:27:54.953306 ljpeg-3.6.11/docs/
--rw-r--r--   0 cest      (1001) cest      (1001)     1154 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/Makefile
-drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-02-26 00:27:54.953306 ljpeg-3.6.11/docs/_static/
--rw-r--r--   0 cest      (1001) cest      (1001)       18 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/_static/.gitignore
--rw-r--r--   0 cest      (1001) cest      (1001)       41 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/authors.rst
--rw-r--r--   0 cest      (1001) cest      (1001)       43 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/changelog.rst
--rw-r--r--   0 cest      (1001) cest      (1001)     9730 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/conf.py
--rw-r--r--   0 cest      (1001) cest      (1001)       33 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/contributing.rst
--rw-r--r--   0 cest      (1001) cest      (1001)     2305 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/index.rst
--rw-r--r--   0 cest      (1001) cest      (1001)       67 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/license.rst
--rw-r--r--   0 cest      (1001) cest      (1001)       39 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/readme.rst
--rw-r--r--   0 cest      (1001) cest      (1001)      233 2023-02-25 19:28:47.000000 ljpeg-3.6.11/docs/requirements.txt
--rw-r--r--   0 cest      (1001) cest      (1001)     1381 2023-02-25 22:37:04.000000 ljpeg-3.6.11/index.html
--rw-r--r--   0 cest      (1001) cest      (1001)      346 2023-02-25 19:28:47.000000 ljpeg-3.6.11/pyproject.toml
--rw-r--r--   0 cest      (1001) cest      (1001)      438 2023-02-25 21:15:55.000000 ljpeg-3.6.11/requirements.txt
--rw-r--r--   0 cest      (1001) cest      (1001)     1547 2023-02-26 00:27:54.986640 ljpeg-3.6.11/setup.cfg
--rw-r--r--   0 cest      (1001) cest      (1001)      700 2023-02-26 00:16:18.000000 ljpeg-3.6.11/setup.py
-drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-02-26 00:27:54.946639 ljpeg-3.6.11/src/
-drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-02-26 00:27:54.956639 ljpeg-3.6.11/src/ljpeg/
--rw-r--r--   0 cest      (1001) cest      (1001)      577 2023-02-25 20:09:46.000000 ljpeg-3.6.11/src/ljpeg/__init__.py
-drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-02-26 00:27:54.983306 ljpeg-3.6.11/src/ljpeg/jpegdir/
--rw-r--r--   0 cest      (1001) cest      (1001)     2642 2023-02-25 19:58:05.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/CHANGES
--rw-r--r--   0 cest      (1001) cest      (1001)      364 2023-02-25 19:58:05.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/PORTABILITY
--rw-r--r--   0 cest      (1001) cest      (1001)     7310 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/README
--rw-r--r--   0 cest      (1001) cest      (1001)     2599 2023-02-25 19:58:05.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/SETUP
--rw-r--r--   0 cest      (1001) cest      (1001)     2899 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/blkint.jpg
--rw-r--r--   0 cest      (1001) cest      (1001)    16384 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/blkint.jpg.1
--rw-r--r--   0 cest      (1001) cest      (1001)     8192 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/blkint.jpg.2
--rw-r--r--   0 cest      (1001) cest      (1001)     8192 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/blkint.jpg.3
--rw-r--r--   0 cest      (1001) cest      (1001)     8482 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/chendct.c
--rw-r--r--   0 cest      (1001) cest      (1001)    14847 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/codec.c
--rw-r--r--   0 cest      (1001) cest      (1001)     2147 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/csize.h
--rw-r--r--   0 cest      (1001) cest      (1001)     4348 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/dct.h
--rw-r--r--   0 cest      (1001) cest      (1001)   474078 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/doc.ps
--rw-r--r--   0 cest      (1001) cest      (1001)     7281 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/globals.h
--rw-r--r--   0 cest      (1001) cest      (1001)    16802 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/huffman.c
--rw-r--r--   0 cest      (1001) cest      (1001)    30459 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/io.c
--rw-r--r--   0 cest      (1001) cest      (1001)     6489 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/jpeg.1
--rw-r--r--   0 cest      (1001) cest      (1001)    67934 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/jpeg.c
--rwxr-xr-x   0 cest      (1001) cest      (1001)  1002056 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/jpeg_static
--rw-r--r--   0 cest      (1001) cest      (1001)     9200 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/leedct.c
--rw-r--r--   0 cest      (1001) cest      (1001)    28656 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/lexer.l
--rw-r--r--   0 cest      (1001) cest      (1001)     1633 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/makefile
--rw-r--r--   0 cest      (1001) cest      (1001)    17959 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/marker.c
--rw-r--r--   0 cest      (1001) cest      (1001)     1783 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/marker.h
--rw-r--r--   0 cest      (1001) cest      (1001)     2922 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/nonint.jpg
--rw-r--r--   0 cest      (1001) cest      (1001)     3941 2023-02-25 19:58:05.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/param.h
--rw-r--r--   0 cest      (1001) cest      (1001)     5106 2023-02-25 19:58:05.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/prototypes.h
--rw-r--r--   0 cest      (1001) cest      (1001)    24432 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/stream.c
--rw-r--r--   0 cest      (1001) cest      (1001)     1547 2023-02-25 19:58:05.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/stream.h
--rw-r--r--   0 cest      (1001) cest      (1001)     3677 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/system.h
--rw-r--r--   0 cest      (1001) cest      (1001)     4706 2023-02-25 07:30:12.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/tables.h
--rw-r--r--   0 cest      (1001) cest      (1001)      623 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/test.3stream
--rw-r--r--   0 cest      (1001) cest      (1001)     3788 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/test.huff
--rw-r--r--   0 cest      (1001) cest      (1001)      592 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/test.q
--rw-r--r--   0 cest      (1001) cest      (1001)    11617 2023-02-25 19:58:00.000000 ljpeg-3.6.11/src/ljpeg/jpegdir/transform.c
--rwxr-xr-x   0 cest      (1001) cest      (1001)     3800 2023-02-26 00:19:21.000000 ljpeg-3.6.11/src/ljpeg/ljpeg.py
-drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-02-26 00:27:54.956639 ljpeg-3.6.11/src/ljpeg.egg-info/
--rw-r--r--   0 cest      (1001) cest      (1001)     4481 2023-02-26 00:27:54.000000 ljpeg-3.6.11/src/ljpeg.egg-info/PKG-INFO
--rw-r--r--   0 cest      (1001) cest      (1001)     1634 2023-02-26 00:27:54.000000 ljpeg-3.6.11/src/ljpeg.egg-info/SOURCES.txt
--rw-r--r--   0 cest      (1001) cest      (1001)        1 2023-02-26 00:27:54.000000 ljpeg-3.6.11/src/ljpeg.egg-info/dependency_links.txt
--rw-r--r--   0 cest      (1001) cest      (1001)       42 2023-02-26 00:27:54.000000 ljpeg-3.6.11/src/ljpeg.egg-info/entry_points.txt
--rw-r--r--   0 cest      (1001) cest      (1001)        1 2023-02-25 19:30:26.000000 ljpeg-3.6.11/src/ljpeg.egg-info/not-zip-safe
--rw-r--r--   0 cest      (1001) cest      (1001)      128 2023-02-26 00:27:54.000000 ljpeg-3.6.11/src/ljpeg.egg-info/requires.txt
--rw-r--r--   0 cest      (1001) cest      (1001)        6 2023-02-26 00:27:54.000000 ljpeg-3.6.11/src/ljpeg.egg-info/top_level.txt
-drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-02-26 00:27:54.986640 ljpeg-3.6.11/tests/
--rw-r--r--   0 cest      (1001) cest      (1001)      273 2023-02-25 19:28:47.000000 ljpeg-3.6.11/tests/conftest.py
--rw-r--r--   0 cest      (1001) cest      (1001)     2851 2023-02-25 19:28:47.000000 ljpeg-3.6.11/tox.ini
+drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-04-19 06:43:01.664291 ljpeg-3.7.0/
+-rw-r--r--   0 cest      (1001) cest      (1001)      588 2023-02-25 19:28:47.000000 ljpeg-3.7.0/.coveragerc
+-rw-r--r--   0 cest      (1001) cest      (1001)     1055 2023-02-25 22:52:09.000000 ljpeg-3.7.0/.gitignore
+-rw-r--r--   0 cest      (1001) cest      (1001)     1488 2023-02-25 20:11:19.000000 ljpeg-3.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 cest      (1001) cest      (1001)      530 2023-02-25 19:28:47.000000 ljpeg-3.7.0/.readthedocs.yml
+-rw-r--r--   0 cest      (1001) cest      (1001)      110 2023-02-25 19:28:47.000000 ljpeg-3.7.0/AUTHORS.rst
+-rw-r--r--   0 cest      (1001) cest      (1001)      138 2023-02-25 19:45:31.000000 ljpeg-3.7.0/CHANGELOG.rst
+-rw-r--r--   0 cest      (1001) cest      (1001)    11063 2023-02-25 19:47:47.000000 ljpeg-3.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 cest      (1001) cest      (1001)     1291 2023-02-25 07:30:12.000000 ljpeg-3.7.0/LICENSE
+-rw-r--r--   0 cest      (1001) cest      (1001)     1082 2023-02-25 19:28:47.000000 ljpeg-3.7.0/LICENSE.txt
+-rw-r--r--   0 cest      (1001) cest      (1001)     4728 2023-04-19 06:43:01.664291 ljpeg-3.7.0/PKG-INFO
+-rw-r--r--   0 cest      (1001) cest      (1001)     3853 2023-04-19 06:36:27.000000 ljpeg-3.7.0/README.rst
+drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-04-19 06:43:01.654290 ljpeg-3.7.0/docs/
+-rw-r--r--   0 cest      (1001) cest      (1001)     1154 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/Makefile
+drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-04-19 06:43:01.654290 ljpeg-3.7.0/docs/_static/
+-rw-r--r--   0 cest      (1001) cest      (1001)       18 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/_static/.gitignore
+-rw-r--r--   0 cest      (1001) cest      (1001)       41 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/authors.rst
+-rw-r--r--   0 cest      (1001) cest      (1001)       43 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/changelog.rst
+-rw-r--r--   0 cest      (1001) cest      (1001)     9730 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/conf.py
+-rw-r--r--   0 cest      (1001) cest      (1001)       33 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/contributing.rst
+-rw-r--r--   0 cest      (1001) cest      (1001)     2305 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/index.rst
+-rw-r--r--   0 cest      (1001) cest      (1001)       67 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/license.rst
+-rw-r--r--   0 cest      (1001) cest      (1001)       39 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/readme.rst
+-rw-r--r--   0 cest      (1001) cest      (1001)      233 2023-02-25 19:28:47.000000 ljpeg-3.7.0/docs/requirements.txt
+-rw-r--r--   0 cest      (1001) cest      (1001)      346 2023-02-25 19:28:47.000000 ljpeg-3.7.0/pyproject.toml
+-rw-r--r--   0 cest      (1001) cest      (1001)      438 2023-02-25 21:15:55.000000 ljpeg-3.7.0/requirements.txt
+-rw-r--r--   0 cest      (1001) cest      (1001)     1547 2023-04-19 06:43:01.667624 ljpeg-3.7.0/setup.cfg
+-rw-r--r--   0 cest      (1001) cest      (1001)      700 2023-02-26 00:16:18.000000 ljpeg-3.7.0/setup.py
+drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-04-19 06:43:01.647624 ljpeg-3.7.0/src/
+drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-04-19 06:43:01.654290 ljpeg-3.7.0/src/ljpeg/
+-rw-r--r--   0 cest      (1001) cest      (1001)      577 2023-02-25 20:09:46.000000 ljpeg-3.7.0/src/ljpeg/__init__.py
+drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-04-19 06:43:01.664291 ljpeg-3.7.0/src/ljpeg/jpegdir/
+-rw-r--r--   0 cest      (1001) cest      (1001)     2642 2023-02-25 19:58:05.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/CHANGES
+-rw-r--r--   0 cest      (1001) cest      (1001)      364 2023-02-25 19:58:05.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/PORTABILITY
+-rw-r--r--   0 cest      (1001) cest      (1001)     7310 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/README
+-rw-r--r--   0 cest      (1001) cest      (1001)     2599 2023-02-25 19:58:05.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/SETUP
+-rw-r--r--   0 cest      (1001) cest      (1001)     2899 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/blkint.jpg
+-rw-r--r--   0 cest      (1001) cest      (1001)    16384 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/blkint.jpg.1
+-rw-r--r--   0 cest      (1001) cest      (1001)     8192 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/blkint.jpg.2
+-rw-r--r--   0 cest      (1001) cest      (1001)     8192 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/blkint.jpg.3
+-rw-r--r--   0 cest      (1001) cest      (1001)     8482 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/chendct.c
+-rw-r--r--   0 cest      (1001) cest      (1001)    14847 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/codec.c
+-rw-r--r--   0 cest      (1001) cest      (1001)     2147 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/csize.h
+-rw-r--r--   0 cest      (1001) cest      (1001)     4348 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/dct.h
+-rw-r--r--   0 cest      (1001) cest      (1001)   474078 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/doc.ps
+-rw-r--r--   0 cest      (1001) cest      (1001)     7281 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/globals.h
+-rw-r--r--   0 cest      (1001) cest      (1001)    16802 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/huffman.c
+-rw-r--r--   0 cest      (1001) cest      (1001)    30459 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/io.c
+-rw-r--r--   0 cest      (1001) cest      (1001)     6489 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/jpeg.1
+-rw-r--r--   0 cest      (1001) cest      (1001)    67934 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/jpeg.c
+-rwxr-xr-x   0 cest      (1001) cest      (1001)  1002056 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/jpeg_static
+-rw-r--r--   0 cest      (1001) cest      (1001)     9200 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/leedct.c
+-rw-r--r--   0 cest      (1001) cest      (1001)    28656 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/lexer.l
+-rw-r--r--   0 cest      (1001) cest      (1001)     1633 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/makefile
+-rw-r--r--   0 cest      (1001) cest      (1001)    17959 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/marker.c
+-rw-r--r--   0 cest      (1001) cest      (1001)     1783 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/marker.h
+-rw-r--r--   0 cest      (1001) cest      (1001)     2922 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/nonint.jpg
+-rw-r--r--   0 cest      (1001) cest      (1001)     3941 2023-02-25 19:58:05.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/param.h
+-rw-r--r--   0 cest      (1001) cest      (1001)     5106 2023-02-25 19:58:05.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/prototypes.h
+-rw-r--r--   0 cest      (1001) cest      (1001)    24432 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/stream.c
+-rw-r--r--   0 cest      (1001) cest      (1001)     1547 2023-02-25 19:58:05.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/stream.h
+-rw-r--r--   0 cest      (1001) cest      (1001)     3677 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/system.h
+-rw-r--r--   0 cest      (1001) cest      (1001)     4706 2023-02-25 07:30:12.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/tables.h
+-rw-r--r--   0 cest      (1001) cest      (1001)      623 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/test.3stream
+-rw-r--r--   0 cest      (1001) cest      (1001)     3788 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/test.huff
+-rw-r--r--   0 cest      (1001) cest      (1001)      592 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/test.q
+-rw-r--r--   0 cest      (1001) cest      (1001)    11617 2023-02-25 19:58:00.000000 ljpeg-3.7.0/src/ljpeg/jpegdir/transform.c
+-rwxr-xr-x   0 cest      (1001) cest      (1001)     5040 2023-04-19 06:26:09.000000 ljpeg-3.7.0/src/ljpeg/ljpeg.py
+-rw-r--r--   0 cest      (1001) cest      (1001)     3542 2023-04-19 06:32:01.000000 ljpeg-3.7.0/src/ljpeg/utils.py
+drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-04-19 06:43:01.654290 ljpeg-3.7.0/src/ljpeg.egg-info/
+-rw-r--r--   0 cest      (1001) cest      (1001)     4728 2023-04-19 06:43:01.000000 ljpeg-3.7.0/src/ljpeg.egg-info/PKG-INFO
+-rw-r--r--   0 cest      (1001) cest      (1001)     1688 2023-04-19 06:43:01.000000 ljpeg-3.7.0/src/ljpeg.egg-info/SOURCES.txt
+-rw-r--r--   0 cest      (1001) cest      (1001)        1 2023-04-19 06:43:01.000000 ljpeg-3.7.0/src/ljpeg.egg-info/dependency_links.txt
+-rw-r--r--   0 cest      (1001) cest      (1001)       42 2023-04-19 06:43:01.000000 ljpeg-3.7.0/src/ljpeg.egg-info/entry_points.txt
+-rw-r--r--   0 cest      (1001) cest      (1001)        1 2023-02-25 19:30:26.000000 ljpeg-3.7.0/src/ljpeg.egg-info/not-zip-safe
+-rw-r--r--   0 cest      (1001) cest      (1001)      128 2023-04-19 06:43:01.000000 ljpeg-3.7.0/src/ljpeg.egg-info/requires.txt
+-rw-r--r--   0 cest      (1001) cest      (1001)        6 2023-04-19 06:43:01.000000 ljpeg-3.7.0/src/ljpeg.egg-info/top_level.txt
+drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-04-19 06:43:01.664291 ljpeg-3.7.0/tests/
+drwxr-xr-x   0 cest      (1001) cest      (1001)        0 2023-04-19 06:43:01.664291 ljpeg-3.7.0/tests/case4606/
+-rw-r--r--   0 cest      (1001) cest      (1001)      511 2023-04-19 06:22:27.000000 ljpeg-3.7.0/tests/case4606/D-4606-1.ics
+-rw-r--r--   0 cest      (1001) cest      (1001)      273 2023-02-25 19:28:47.000000 ljpeg-3.7.0/tests/conftest.py
+-rw-r--r--   0 cest      (1001) cest      (1001)     2331 2023-04-19 06:36:05.000000 ljpeg-3.7.0/tests/test_cli.py
+-rw-r--r--   0 cest      (1001) cest      (1001)     2851 2023-02-25 19:28:47.000000 ljpeg-3.7.0/tox.ini
```

### Comparing `ljpeg-3.6.11/.coveragerc` & `ljpeg-3.7.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/.gitignore` & `ljpeg-3.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/.pre-commit-config.yaml` & `ljpeg-3.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/.readthedocs.yml` & `ljpeg-3.7.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/CONTRIBUTING.rst` & `ljpeg-3.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/LICENSE` & `ljpeg-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/LICENSE.txt` & `ljpeg-3.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/PKG-INFO` & `ljpeg-3.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ljpeg
-Version: 3.6.11
+Version: 3.7.0
 Summary: Read and transform LJPEG images
 Home-page: https://github.com/sanchezcarlosjr/ljpeg
 Author: sanchezcarlosjr
 Author-email: 24639141+sanchezcarlosjr@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://github.com/sanchezcarlosjr/ljpeg
 Platform: Mac
@@ -57,46 +57,57 @@
     :target: https://pyscaffold.org/
 
 |
 
 ============
 ljpeg
 ============
+     Read and transform LJPEG images into modern formats.
 
+Installation
+============
+Warning: You must have installed the flex parser on your operating system::
 
-     Read and transform LJPEG images into modern formats.
+    pip install ljpeg
 
-Warning: You must have installed flex on your operating system.
+By default, we offer you a binary called jpeg_static. However, you can produce your jpeg binary::
+
+    cd jpegdir && make
+
+Getting started
+=================
+Download a set of mammograms with::
+
+     wget -r -q ftp://figment.csee.usf.edu:21/pub/DDSM/cases/normals/normal_08/case4606/
+
+Transform a lot of mammograms parallely::
+
+     find . -type f -name '*.LJPEG' | parallel -j+0 "ljpeg {} $(pwd)/{/.}.tiff --verify"
 
 Convert to TIFF (requires the .ics file in the same directory as LJPEG)::
 
      ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.tiff
 
 
 Convert to TIFF and verify that no information has been lost::
 
       ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.tiff --verify
 
 Convert to jpeg for visualization with down-sizing scale=0.3 (16-bit TIFF is not good for direct visualization)::
 
       ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.jpg --visual --scale 0.3
 
-Note that output file can be any format that's supported by OpenCV (which includes all common types). Most file formats only support 8-bit images, so directly saving into such file formats will cause problems. Add "--visual" to normalize color into 8-bit before saving to such file formats.
+Convert to TIFF and map gray levels to optical density level::
 
-The Stanford ljpeg code is in public domain and is therefore OK to be included here. I did minor modification to make the code compile under modern Linux.
-
-Getting started
-=================
-Download a set of mammograms with::
+      ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.jpg --od-correct
 
-     wget -q ftp://figment.csee.usf.edu:21/pub/DDSM/cases/normals/normal_08/case4606/ && cat index.html | grep -oP '"ftp.*"' | sed s/\"//g | parallel wget
+Note that output file can be any format that's supported by OpenCV (which includes all common types). Most file formats only support 8-bit images, so directly saving into such file formats will cause problems. Add "--visual" to normalize color into 8-bit before saving to such file formats.
 
-Transform a lot of mammograms parallely::
+The Stanford ljpeg code is in public domain and is therefore OK to be included here. I did minor modification to make the code compile under modern Linux.
 
-     find "$(pwd)" -type f -name '*.LJPEG' | parallel -j+0 "ljpeg {} $(pwd)/{/.}.tiff --verify"
 
 Making Changes & Contributing
 =============================
 
 This project uses `pre-commit`_, please make sure to install it before making any
 changes::
```

### Comparing `ljpeg-3.6.11/README.rst` & `ljpeg-3.7.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -32,46 +32,57 @@
     :target: https://pyscaffold.org/
 
 |
 
 ============
 ljpeg
 ============
+     Read and transform LJPEG images into modern formats.
 
+Installation
+============
+Warning: You must have installed the flex parser on your operating system::
 
-     Read and transform LJPEG images into modern formats.
+    pip install ljpeg
 
-Warning: You must have installed flex on your operating system.
+By default, we offer you a binary called jpeg_static. However, you can produce your jpeg binary::
+
+    cd jpegdir && make
+
+Getting started
+=================
+Download a set of mammograms with::
+
+     wget -r -q ftp://figment.csee.usf.edu:21/pub/DDSM/cases/normals/normal_08/case4606/
+
+Transform a lot of mammograms parallely::
+
+     find . -type f -name '*.LJPEG' | parallel -j+0 "ljpeg {} $(pwd)/{/.}.tiff --verify"
 
 Convert to TIFF (requires the .ics file in the same directory as LJPEG)::
 
      ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.tiff
 
 
 Convert to TIFF and verify that no information has been lost::
 
       ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.tiff --verify
 
 Convert to jpeg for visualization with down-sizing scale=0.3 (16-bit TIFF is not good for direct visualization)::
 
       ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.jpg --visual --scale 0.3
 
-Note that output file can be any format that's supported by OpenCV (which includes all common types). Most file formats only support 8-bit images, so directly saving into such file formats will cause problems. Add "--visual" to normalize color into 8-bit before saving to such file formats.
+Convert to TIFF and map gray levels to optical density level::
 
-The Stanford ljpeg code is in public domain and is therefore OK to be included here. I did minor modification to make the code compile under modern Linux.
-
-Getting started
-=================
-Download a set of mammograms with::
+      ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.jpg --od-correct
 
-     wget -q ftp://figment.csee.usf.edu:21/pub/DDSM/cases/normals/normal_08/case4606/ && cat index.html | grep -oP '"ftp.*"' | sed s/\"//g | parallel wget
+Note that output file can be any format that's supported by OpenCV (which includes all common types). Most file formats only support 8-bit images, so directly saving into such file formats will cause problems. Add "--visual" to normalize color into 8-bit before saving to such file formats.
 
-Transform a lot of mammograms parallely::
+The Stanford ljpeg code is in public domain and is therefore OK to be included here. I did minor modification to make the code compile under modern Linux.
 
-     find "$(pwd)" -type f -name '*.LJPEG' | parallel -j+0 "ljpeg {} $(pwd)/{/.}.tiff --verify"
 
 Making Changes & Contributing
 =============================
 
 This project uses `pre-commit`_, please make sure to install it before making any
 changes::
```

### Comparing `ljpeg-3.6.11/docs/Makefile` & `ljpeg-3.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/docs/conf.py` & `ljpeg-3.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/docs/index.rst` & `ljpeg-3.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/setup.cfg` & `ljpeg-3.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/setup.py` & `ljpeg-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/__init__.py` & `ljpeg-3.7.0/src/ljpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/CHANGES` & `ljpeg-3.7.0/src/ljpeg/jpegdir/CHANGES`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/README` & `ljpeg-3.7.0/src/ljpeg/jpegdir/README`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/SETUP` & `ljpeg-3.7.0/src/ljpeg/jpegdir/SETUP`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/blkint.jpg` & `ljpeg-3.7.0/src/ljpeg/jpegdir/blkint.jpg`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/blkint.jpg.1` & `ljpeg-3.7.0/src/ljpeg/jpegdir/blkint.jpg.1`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/blkint.jpg.2` & `ljpeg-3.7.0/src/ljpeg/jpegdir/blkint.jpg.2`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/blkint.jpg.3` & `ljpeg-3.7.0/src/ljpeg/jpegdir/blkint.jpg.3`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/chendct.c` & `ljpeg-3.7.0/src/ljpeg/jpegdir/chendct.c`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/codec.c` & `ljpeg-3.7.0/src/ljpeg/jpegdir/codec.c`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/csize.h` & `ljpeg-3.7.0/src/ljpeg/jpegdir/csize.h`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/dct.h` & `ljpeg-3.7.0/src/ljpeg/jpegdir/dct.h`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/doc.ps` & `ljpeg-3.7.0/src/ljpeg/jpegdir/doc.ps`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/globals.h` & `ljpeg-3.7.0/src/ljpeg/jpegdir/globals.h`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/huffman.c` & `ljpeg-3.7.0/src/ljpeg/jpegdir/huffman.c`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/io.c` & `ljpeg-3.7.0/src/ljpeg/jpegdir/io.c`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/jpeg.1` & `ljpeg-3.7.0/src/ljpeg/jpegdir/jpeg.1`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/jpeg.c` & `ljpeg-3.7.0/src/ljpeg/jpegdir/jpeg.c`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/jpeg_static` & `ljpeg-3.7.0/src/ljpeg/jpegdir/jpeg_static`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/leedct.c` & `ljpeg-3.7.0/src/ljpeg/jpegdir/leedct.c`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/lexer.l` & `ljpeg-3.7.0/src/ljpeg/jpegdir/lexer.l`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/makefile` & `ljpeg-3.7.0/src/ljpeg/jpegdir/makefile`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/marker.c` & `ljpeg-3.7.0/src/ljpeg/jpegdir/marker.c`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/marker.h` & `ljpeg-3.7.0/src/ljpeg/jpegdir/marker.h`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/nonint.jpg` & `ljpeg-3.7.0/src/ljpeg/jpegdir/nonint.jpg`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/param.h` & `ljpeg-3.7.0/src/ljpeg/jpegdir/param.h`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/prototypes.h` & `ljpeg-3.7.0/src/ljpeg/jpegdir/prototypes.h`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/stream.c` & `ljpeg-3.7.0/src/ljpeg/jpegdir/stream.c`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/stream.h` & `ljpeg-3.7.0/src/ljpeg/jpegdir/stream.h`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/system.h` & `ljpeg-3.7.0/src/ljpeg/jpegdir/system.h`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/tables.h` & `ljpeg-3.7.0/src/ljpeg/jpegdir/tables.h`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/test.3stream` & `ljpeg-3.7.0/src/ljpeg/jpegdir/test.3stream`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/test.huff` & `ljpeg-3.7.0/src/ljpeg/jpegdir/test.huff`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/test.q` & `ljpeg-3.7.0/src/ljpeg/jpegdir/test.q`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/jpegdir/transform.c` & `ljpeg-3.7.0/src/ljpeg/jpegdir/transform.c`

 * *Files identical despite different names*

### Comparing `ljpeg-3.6.11/src/ljpeg/ljpeg.py` & `ljpeg-3.7.0/src/ljpeg/ljpeg.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import subprocess
 import sys
 
 import cv2
 import numpy
 
 from ljpeg import __version__
+from ljpeg.utils import get_ics_info
 
 __author__ = "sanchezcarlosjr"
 __copyright__ = "sanchezcarlosjr"
 __license__ = "MIT"
 
 _logger = logging.getLogger(__name__)
 
@@ -26,14 +27,40 @@
 # sample output
 # > GW:1979  GH:4349  R:0
 # >> C:1  N:xx.ljpeg.1  W:1979  H:4349  hf:1  vf:1
 
 PATTERN = re.compile(r"\sC:(\d+)\s+N:(\S+)\s+W:(\d+)\s+H:(\d+)\s")
 
 
+def od_correct(im, ics_info):
+    """
+    Map gray levels to optical density level
+    :param im: image (numpy)
+    :return: optical density image
+    """
+    im_od = numpy.zeros_like(im, dtype=numpy.float64)
+
+    if (ics_info['scan_institution'] == 'MGH') and (ics_info['scanner_type'] == 'DBA'):
+        im_od = (numpy.log10(im + 1) - 4.80662) / -1.07553
+    elif (ics_info['scan_institution'] == 'MGH') \
+            and (ics_info['scanner_type'] == 'HOWTEK'):
+        im_od = (-0.00094568 * im) + 3.789
+    elif (ics_info['scan_institution'] == 'WFU') \
+            and (ics_info['scanner_type'] == 'LUMISYS'):
+        im_od = (im - 4096.99) / -1009.01
+    elif (ics_info['scan_institution'] == 'ISMD') \
+            and (ics_info['scanner_type'] == 'HOWTEK'):
+        im_od = (-0.00099055807612 * im) + 3.96604095240593
+
+    # perform heath noise correction
+    im_od[im_od < 0.05] = 0.05
+    im_od[im_od > 3.0] = 3.0
+    return im_od
+
+
 def read(path):
     cmd = "{} -d -s {}".format(BIN, path)
     output = subprocess.check_output(cmd, shell=True)
     _logger.debug(output)
     m = re.search(PATTERN, output.decode())
     C = int(m.group(1))  # I suppose this is # channels
     F = m.group(2)
@@ -71,14 +98,20 @@
         action="store_const",
         const=logging.DEBUG,
     )
     parser.add_argument("ljpeg", nargs=1)
     parser.add_argument("output", nargs=1)
     parser.add_argument("--verify", action="store_true")
     parser.add_argument("--visual", action="store_true")
+    parser.add_argument("--ics_info",
+                        action="store_true",
+                        help="display ics info as dict")
+    parser.add_argument("--od_correct",
+                        action="store_true",
+                        help="map gray levels to optical density level")
     parser.add_argument("--scale", type=float)
 
     args = parser.parse_args()
     path = args.ljpeg[0]
     tiff = args.output[0]
 
     assert "LJPEG" in path
@@ -91,52 +124,51 @@
     # read ICS
     _logger.info(glob.glob(root + "/*.ics"))
     ics = glob.glob(root + "/*.ics")[0]
     name = path.split(".")[-2]
 
     W = None
     H = None
-    # find the shape of image
-    for line in open(ics, "r"):
-        line = line.strip().split(" ")
-        if len(line) < 7:
-            continue
-        if line[0] == name:
-            W = int(line[4])
-            H = int(line[2])
-            bps = int(line[6])
-            if bps != 12:
-                _logger.warning("BPS != 12: %s" % path)
-            break
+    ics_info = get_ics_info(ics)
+    W = ics_info[name]['width']
+    H = ics_info[name]['height']
+    if ics_info[name]['bpp'] != 12:
+        _logger.warning("BPS != 12: %s" % path)
+
+    if args.ics_info:
+        print(ics_info)
 
     assert W is not None
     assert H is not None
 
     image = read(path)
 
     if W != image.shape[1]:
         _logger.warning("reshape: %s" % path)
         image = image.reshape((H, W))
 
     raw = image
 
+    if args.od_correct:
+        image = od_correct(image, ics_info)
+        image = numpy.interp(image, (0.0, 4.0), (255, 0))
+        image = image.astype(numpy.uint8)
+
     if args.visual:
         _logger.warning("normalizing color, will lose information")
         if args.verify:
             _logger.error("verification is going to fail")
         if args.scale:
             rows, cols = image.shape
             image = cv2.resize(image, (int(cols * args.scale), int(rows * args.scale)))
         image = cv2.normalize(image, None, 0, 255, cv2.NORM_MINMAX)
         image = numpy.uint8(image)
     elif args.scale:
         _logger.error("--scale must be used with --visual")
         sys.exit(1)
-        # image = cv2.equalizeHist(image)
-    # tiff = stem + '.TIFF'
     cv2.imwrite(tiff, image)
 
     if args.verify:
         verify = cv2.imread(tiff, -1)
         if numpy.all(raw == verify):
             print("Verification successful, conversion is lossless")
         else:
```

### Comparing `ljpeg-3.6.11/src/ljpeg.egg-info/PKG-INFO` & `ljpeg-3.7.0/src/ljpeg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ljpeg
-Version: 3.6.11
+Version: 3.7.0
 Summary: Read and transform LJPEG images
 Home-page: https://github.com/sanchezcarlosjr/ljpeg
 Author: sanchezcarlosjr
 Author-email: 24639141+sanchezcarlosjr@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://github.com/sanchezcarlosjr/ljpeg
 Platform: Mac
@@ -57,46 +57,57 @@
     :target: https://pyscaffold.org/
 
 |
 
 ============
 ljpeg
 ============
+     Read and transform LJPEG images into modern formats.
 
+Installation
+============
+Warning: You must have installed the flex parser on your operating system::
 
-     Read and transform LJPEG images into modern formats.
+    pip install ljpeg
 
-Warning: You must have installed flex on your operating system.
+By default, we offer you a binary called jpeg_static. However, you can produce your jpeg binary::
+
+    cd jpegdir && make
+
+Getting started
+=================
+Download a set of mammograms with::
+
+     wget -r -q ftp://figment.csee.usf.edu:21/pub/DDSM/cases/normals/normal_08/case4606/
+
+Transform a lot of mammograms parallely::
+
+     find . -type f -name '*.LJPEG' | parallel -j+0 "ljpeg {} $(pwd)/{/.}.tiff --verify"
 
 Convert to TIFF (requires the .ics file in the same directory as LJPEG)::
 
      ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.tiff
 
 
 Convert to TIFF and verify that no information has been lost::
 
       ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.tiff --verify
 
 Convert to jpeg for visualization with down-sizing scale=0.3 (16-bit TIFF is not good for direct visualization)::
 
       ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.jpg --visual --scale 0.3
 
-Note that output file can be any format that's supported by OpenCV (which includes all common types). Most file formats only support 8-bit images, so directly saving into such file formats will cause problems. Add "--visual" to normalize color into 8-bit before saving to such file formats.
+Convert to TIFF and map gray levels to optical density level::
 
-The Stanford ljpeg code is in public domain and is therefore OK to be included here. I did minor modification to make the code compile under modern Linux.
-
-Getting started
-=================
-Download a set of mammograms with::
+      ljpeg $(pwd)/C_0029_1.LEFT_CC.LJPEG $(pwd)/output.jpg --od-correct
 
-     wget -q ftp://figment.csee.usf.edu:21/pub/DDSM/cases/normals/normal_08/case4606/ && cat index.html | grep -oP '"ftp.*"' | sed s/\"//g | parallel wget
+Note that output file can be any format that's supported by OpenCV (which includes all common types). Most file formats only support 8-bit images, so directly saving into such file formats will cause problems. Add "--visual" to normalize color into 8-bit before saving to such file formats.
 
-Transform a lot of mammograms parallely::
+The Stanford ljpeg code is in public domain and is therefore OK to be included here. I did minor modification to make the code compile under modern Linux.
 
-     find "$(pwd)" -type f -name '*.LJPEG' | parallel -j+0 "ljpeg {} $(pwd)/{/.}.tiff --verify"
 
 Making Changes & Contributing
 =============================
 
 This project uses `pre-commit`_, please make sure to install it before making any
 changes::
```

### Comparing `ljpeg-3.6.11/src/ljpeg.egg-info/SOURCES.txt` & `ljpeg-3.7.0/src/ljpeg.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 LICENSE.txt
 README.rst
-index.html
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/authors.rst
@@ -22,14 +21,15 @@
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 src/ljpeg/__init__.py
 src/ljpeg/ljpeg.py
+src/ljpeg/utils.py
 src/ljpeg.egg-info/PKG-INFO
 src/ljpeg.egg-info/SOURCES.txt
 src/ljpeg.egg-info/dependency_links.txt
 src/ljpeg.egg-info/entry_points.txt
 src/ljpeg.egg-info/not-zip-safe
 src/ljpeg.egg-info/requires.txt
 src/ljpeg.egg-info/top_level.txt
@@ -64,8 +64,10 @@
 src/ljpeg/jpegdir/stream.h
 src/ljpeg/jpegdir/system.h
 src/ljpeg/jpegdir/tables.h
 src/ljpeg/jpegdir/test.3stream
 src/ljpeg/jpegdir/test.huff
 src/ljpeg/jpegdir/test.q
 src/ljpeg/jpegdir/transform.c
-tests/conftest.py
+tests/conftest.py
+tests/test_cli.py
+tests/case4606/D-4606-1.ics
```

### Comparing `ljpeg-3.6.11/tox.ini` & `ljpeg-3.7.0/tox.ini`

 * *Files identical despite different names*

