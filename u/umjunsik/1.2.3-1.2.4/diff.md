# Comparing `tmp/umjunsik-1.2.3.tar.gz` & `tmp/umjunsik-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umjunsik-1.2.3.tar", last modified: Wed Apr 19 13:16:16 2023, max compression
+gzip compressed data, was "umjunsik-1.2.4.tar", last modified: Wed Apr 19 13:37:13 2023, max compression
```

## Comparing `umjunsik-1.2.3.tar` & `umjunsik-1.2.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:16:16.534371 umjunsik-1.2.3/
--rw-r--r--   0 hiyabye    (501) staff       (20)     1062 2023-04-18 14:04:33.000000 umjunsik-1.2.3/LICENSE
--rw-r--r--   0 hiyabye    (501) staff       (20)      643 2023-04-19 13:16:16.534423 umjunsik-1.2.3/PKG-INFO
--rw-r--r--   0 hiyabye    (501) staff       (20)    17050 2023-04-17 07:54:45.000000 umjunsik-1.2.3/README.md
--rw-r--r--   0 hiyabye    (501) staff       (20)      103 2023-04-19 13:16:16.534596 umjunsik-1.2.3/setup.cfg
--rw-r--r--   0 hiyabye    (501) staff       (20)      730 2023-04-19 13:15:39.000000 umjunsik-1.2.3/setup.py
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:16:16.533749 umjunsik-1.2.3/umjunsik/
--rw-r--r--   0 hiyabye    (501) staff       (20)     3116 2023-04-19 13:15:29.000000 umjunsik-1.2.3/umjunsik/runtime.py
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:16:16.534262 umjunsik-1.2.3/umjunsik.egg-info/
--rw-r--r--   0 hiyabye    (501) staff       (20)      643 2023-04-19 13:16:16.000000 umjunsik-1.2.3/umjunsik.egg-info/PKG-INFO
--rw-r--r--   0 hiyabye    (501) staff       (20)      184 2023-04-19 13:16:16.000000 umjunsik-1.2.3/umjunsik.egg-info/SOURCES.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)        1 2023-04-19 13:16:16.000000 umjunsik-1.2.3/umjunsik.egg-info/dependency_links.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)        9 2023-04-19 13:16:16.000000 umjunsik-1.2.3/umjunsik.egg-info/top_level.txt
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:37:13.951809 umjunsik-1.2.4/
+-rw-r--r--   0 hiyabye    (501) staff       (20)     1062 2023-04-18 14:04:33.000000 umjunsik-1.2.4/LICENSE
+-rw-r--r--   0 hiyabye    (501) staff       (20)      807 2023-04-19 13:37:13.951874 umjunsik-1.2.4/PKG-INFO
+-rw-r--r--   0 hiyabye    (501) staff       (20)    17050 2023-04-17 07:54:45.000000 umjunsik-1.2.4/README.md
+-rw-r--r--   0 hiyabye    (501) staff       (20)      103 2023-04-19 13:37:13.952084 umjunsik-1.2.4/setup.cfg
+-rw-r--r--   0 hiyabye    (501) staff       (20)     1061 2023-04-19 13:35:29.000000 umjunsik-1.2.4/setup.py
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:37:13.950945 umjunsik-1.2.4/umjunsik/
+-rw-r--r--   0 hiyabye    (501) staff       (20)       21 2023-04-19 13:26:03.000000 umjunsik-1.2.4/umjunsik/__init__.py
+-rw-r--r--   0 hiyabye    (501) staff       (20)     3116 2023-04-19 13:25:48.000000 umjunsik-1.2.4/umjunsik/runtime.py
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:37:13.951649 umjunsik-1.2.4/umjunsik.egg-info/
+-rw-r--r--   0 hiyabye    (501) staff       (20)      807 2023-04-19 13:37:13.000000 umjunsik-1.2.4/umjunsik.egg-info/PKG-INFO
+-rw-r--r--   0 hiyabye    (501) staff       (20)      205 2023-04-19 13:37:13.000000 umjunsik-1.2.4/umjunsik.egg-info/SOURCES.txt
+-rw-r--r--   0 hiyabye    (501) staff       (20)        1 2023-04-19 13:37:13.000000 umjunsik-1.2.4/umjunsik.egg-info/dependency_links.txt
+-rw-r--r--   0 hiyabye    (501) staff       (20)        9 2023-04-19 13:37:13.000000 umjunsik-1.2.4/umjunsik.egg-info/top_level.txt
```

### Comparing `umjunsik-1.2.3/LICENSE` & `umjunsik-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `umjunsik-1.2.3/README.md` & `umjunsik-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `umjunsik-1.2.3/umjunsik/runtime.py` & `umjunsik-1.2.4/umjunsik/runtime.py`

 * *Files identical despite different names*

