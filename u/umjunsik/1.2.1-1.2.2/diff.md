# Comparing `tmp/umjunsik-1.2.1.tar.gz` & `tmp/umjunsik-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umjunsik-1.2.1.tar", last modified: Wed Apr 19 04:32:37 2023, max compression
+gzip compressed data, was "umjunsik-1.2.2.tar", last modified: Wed Apr 19 13:12:00 2023, max compression
```

## Comparing `umjunsik-1.2.1.tar` & `umjunsik-1.2.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 04:32:37.415775 umjunsik-1.2.1/
--rw-r--r--   0 hiyabye    (501) staff       (20)     1062 2023-04-18 14:04:33.000000 umjunsik-1.2.1/LICENSE
--rw-r--r--   0 hiyabye    (501) staff       (20)      272 2023-04-19 04:32:37.415832 umjunsik-1.2.1/PKG-INFO
--rw-r--r--   0 hiyabye    (501) staff       (20)    17050 2023-04-17 07:54:45.000000 umjunsik-1.2.1/README.md
--rw-r--r--   0 hiyabye    (501) staff       (20)      102 2023-04-19 04:32:37.416033 umjunsik-1.2.1/setup.cfg
--rw-r--r--   0 hiyabye    (501) staff       (20)      403 2023-04-19 04:32:19.000000 umjunsik-1.2.1/setup.py
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 04:32:37.415677 umjunsik-1.2.1/umjunsik.egg-info/
--rw-r--r--   0 hiyabye    (501) staff       (20)      272 2023-04-19 04:32:37.000000 umjunsik-1.2.1/umjunsik.egg-info/PKG-INFO
--rw-r--r--   0 hiyabye    (501) staff       (20)      199 2023-04-19 04:32:37.000000 umjunsik-1.2.1/umjunsik.egg-info/SOURCES.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)        1 2023-04-19 04:32:37.000000 umjunsik-1.2.1/umjunsik.egg-info/dependency_links.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)       43 2023-04-19 04:32:37.000000 umjunsik-1.2.1/umjunsik.egg-info/entry_points.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)        1 2023-04-19 04:32:37.000000 umjunsik-1.2.1/umjunsik.egg-info/top_level.txt
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:12:00.995867 umjunsik-1.2.2/
+-rw-r--r--   0 hiyabye    (501) staff       (20)     1062 2023-04-18 14:04:33.000000 umjunsik-1.2.2/LICENSE
+-rw-r--r--   0 hiyabye    (501) staff       (20)      643 2023-04-19 13:12:00.995924 umjunsik-1.2.2/PKG-INFO
+-rw-r--r--   0 hiyabye    (501) staff       (20)    17050 2023-04-17 07:54:45.000000 umjunsik-1.2.2/README.md
+-rw-r--r--   0 hiyabye    (501) staff       (20)      103 2023-04-19 13:12:00.996105 umjunsik-1.2.2/setup.cfg
+-rw-r--r--   0 hiyabye    (501) staff       (20)      730 2023-04-19 13:11:20.000000 umjunsik-1.2.2/setup.py
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:12:00.995331 umjunsik-1.2.2/umjunsik/
+-rw-r--r--   0 hiyabye    (501) staff       (20)     2928 2023-04-19 12:55:10.000000 umjunsik-1.2.2/umjunsik/runtime.py
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:12:00.995755 umjunsik-1.2.2/umjunsik.egg-info/
+-rw-r--r--   0 hiyabye    (501) staff       (20)      643 2023-04-19 13:12:00.000000 umjunsik-1.2.2/umjunsik.egg-info/PKG-INFO
+-rw-r--r--   0 hiyabye    (501) staff       (20)      184 2023-04-19 13:12:00.000000 umjunsik-1.2.2/umjunsik.egg-info/SOURCES.txt
+-rw-r--r--   0 hiyabye    (501) staff       (20)        1 2023-04-19 13:12:00.000000 umjunsik-1.2.2/umjunsik.egg-info/dependency_links.txt
+-rw-r--r--   0 hiyabye    (501) staff       (20)        9 2023-04-19 13:12:00.000000 umjunsik-1.2.2/umjunsik.egg-info/top_level.txt
```

### Comparing `umjunsik-1.2.1/LICENSE` & `umjunsik-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `umjunsik-1.2.1/README.md` & `umjunsik-1.2.2/README.md`

 * *Files identical despite different names*

