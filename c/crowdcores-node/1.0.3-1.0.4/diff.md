# Comparing `tmp/crowdcores_node-1.0.3.tar.gz` & `tmp/crowdcores-node-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores_node-1.0.3.tar", last modified: Wed Apr 19 01:16:57 2023, max compression
+gzip compressed data, was "crowdcores-node-1.0.4.tar", last modified: Wed Apr 19 01:23:57 2023, max compression
```

## Comparing `crowdcores_node-1.0.3.tar` & `crowdcores-node-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:16:57.991298 crowdcores_node-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores_node-1.0.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 01:16:57.991298 crowdcores_node-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2023-04-19 01:01:15.000000 crowdcores_node-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:16:57.991298 crowdcores_node-1.0.3/crowdcores_node/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores_node-1.0.3/crowdcores_node/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3989 2023-04-18 22:11:04.000000 crowdcores_node-1.0.3/crowdcores_node/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:16:57.991298 crowdcores_node-1.0.3/crowdcores_node.egg-info/
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 01:16:57.000000 crowdcores_node-1.0.3/crowdcores_node.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-19 01:16:57.000000 crowdcores_node-1.0.3/crowdcores_node.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 01:16:57.000000 crowdcores_node-1.0.3/crowdcores_node.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 01:16:57.000000 crowdcores_node-1.0.3/crowdcores_node.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 01:16:57.000000 crowdcores_node-1.0.3/crowdcores_node.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 01:16:57.000000 crowdcores_node-1.0.3/crowdcores_node.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 01:16:57.991298 crowdcores_node-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-19 01:10:37.000000 crowdcores_node-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.0.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2023-04-19 01:01:15.000000 crowdcores-node-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/crowdcores_node/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.0.4/crowdcores_node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-04-18 22:11:04.000000 crowdcores-node-1.0.4/crowdcores_node/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/crowdcores_node.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 01:23:57.000000 crowdcores-node-1.0.4/crowdcores_node.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 01:23:57.488413 crowdcores-node-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-19 01:23:46.000000 crowdcores-node-1.0.4/setup.py
```

### Comparing `crowdcores_node-1.0.3/LICENSE.txt` & `crowdcores-node-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores_node-1.0.3/crowdcores_node/node.py` & `crowdcores-node-1.0.4/crowdcores_node/node.py`

 * *Files identical despite different names*

