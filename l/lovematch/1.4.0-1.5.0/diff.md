# Comparing `tmp/lovematch-1.4.0.tar.gz` & `tmp/lovematch-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lovematch-1.4.0.tar", last modified: Wed Apr 19 11:32:36 2023, max compression
+gzip compressed data, was "dist\lovematch-1.5.0.tar", last modified: Wed Apr 19 11:45:25 2023, max compression
```

## Comparing `lovematch-1.4.0.tar` & `lovematch-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 11:32:36.000000 lovematch-1.4.0/
--rw-rw-rw-   0        0        0     1094 2023-04-19 11:23:31.000000 lovematch-1.4.0/LICENSE
--rw-rw-rw-   0        0        0      596 2023-04-19 11:32:36.000000 lovematch-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-19 11:23:31.000000 lovematch-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 11:32:36.000000 lovematch-1.4.0/lovematch/
--rw-rw-rw-   0        0        0       92 2023-04-19 11:32:07.000000 lovematch-1.4.0/lovematch/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-04-19 11:31:55.000000 lovematch-1.4.0/lovematch/lovematch.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:32:36.000000 lovematch-1.4.0/lovematch.egg-info/
--rw-rw-rw-   0        0        0      596 2023-04-19 11:32:36.000000 lovematch-1.4.0/lovematch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-19 11:32:36.000000 lovematch-1.4.0/lovematch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 11:32:36.000000 lovematch-1.4.0/lovematch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 11:32:36.000000 lovematch-1.4.0/lovematch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 11:32:36.000000 lovematch-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-04-19 11:32:18.000000 lovematch-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:45:25.000000 lovematch-1.5.0/
+-rw-rw-rw-   0        0        0     1094 2023-04-19 11:23:31.000000 lovematch-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0      641 2023-04-19 11:45:25.000000 lovematch-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-19 11:23:31.000000 lovematch-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 11:45:25.000000 lovematch-1.5.0/Relation_Calculator/
+-rw-rw-rw-   0        0        0      101 2023-04-19 11:44:28.000000 lovematch-1.5.0/Relation_Calculator/__init__.py
+-rw-rw-rw-   0        0        0     3072 2023-04-19 11:45:17.000000 lovematch-1.5.0/Relation_Calculator/lovematch.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:45:25.000000 lovematch-1.5.0/lovematch.egg-info/
+-rw-rw-rw-   0        0        0      641 2023-04-19 11:45:24.000000 lovematch-1.5.0/lovematch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-19 11:45:25.000000 lovematch-1.5.0/lovematch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:45:24.000000 lovematch-1.5.0/lovematch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-19 11:45:24.000000 lovematch-1.5.0/lovematch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:45:25.000000 lovematch-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      943 2023-04-19 11:42:56.000000 lovematch-1.5.0/setup.py
```

### Comparing `lovematch-1.4.0/LICENSE` & `lovematch-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lovematch-1.4.0/lovematch/lovematch.py` & `lovematch-1.5.0/Relation_Calculator/lovematch.py`

 * *Files identical despite different names*

