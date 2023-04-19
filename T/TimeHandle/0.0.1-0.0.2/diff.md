# Comparing `tmp/TimeHandle-0.0.1.tar.gz` & `tmp/TimeHandle-0.0.2.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TimeHandle-0.0.1.tar", last modified: Wed Apr 19 09:45:58 2023, max compression
+gzip compressed data, was "/home/CahyPublic/dist/TimeHandle-0.0.2.linux-x86_64.tar", last modified: Wed Apr 19 11:09:35 2023, max compression
```

## Comparing `TimeHandle-0.0.1.tar` & `TimeHandle-0.0.2.linux-x86_64.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:45:58.000000 TimeHandle-0.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:45:58.000000 TimeHandle-0.0.1/CahyPublic/
--rw-r--r--   0 root         (0) root         (0)      653 2023-04-19 09:15:58.000000 TimeHandle-0.0.1/CahyPublic/TimeHandle.py
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-19 09:18:33.000000 TimeHandle-0.0.1/CahyPublic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      365 2023-04-19 09:45:58.000000 TimeHandle-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 09:31:05.000000 TimeHandle-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:45:58.000000 TimeHandle-0.0.1/TimeHandle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      365 2023-04-19 09:45:58.000000 TimeHandle-0.0.1/TimeHandle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-04-19 09:45:58.000000 TimeHandle-0.0.1/TimeHandle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:45:58.000000 TimeHandle-0.0.1/TimeHandle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 09:45:58.000000 TimeHandle-0.0.1/TimeHandle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 09:45:58.000000 TimeHandle-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      458 2023-04-19 09:30:10.000000 TimeHandle-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./usr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./usr/local/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/CahyPublic/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-04-19 09:15:58.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/CahyPublic/TimeHandle.py
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-19 09:18:33.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/CahyPublic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/CahyPublic/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/CahyPublic/__pycache__/TimeHandle.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      259 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/CahyPublic/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/TimeHandle-0.0.2-py3.7.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/TimeHandle-0.0.2-py3.7.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/TimeHandle-0.0.2-py3.7.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/TimeHandle-0.0.2-py3.7.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 11:09:35.000000 ./usr/local/python3.7.8/lib/python3.7/site-packages/TimeHandle-0.0.2-py3.7.egg-info/top_level.txt
```

### Comparing `TimeHandle-0.0.1/CahyPublic/TimeHandle.py` & `./usr/local/python3.7.8/lib/python3.7/site-packages/CahyPublic/TimeHandle.py`

 * *Files identical despite different names*

