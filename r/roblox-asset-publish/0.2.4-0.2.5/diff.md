# Comparing `tmp/roblox-asset-publish-0.2.4.tar.gz` & `tmp/roblox-asset-publish-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-asset-publish-0.2.4.tar", last modified: Wed Apr 19 12:18:15 2023, max compression
+gzip compressed data, was "roblox-asset-publish-0.2.5.tar", last modified: Wed Apr 19 12:22:37 2023, max compression
```

## Comparing `roblox-asset-publish-0.2.4.tar` & `roblox-asset-publish-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:18:15.309547 roblox-asset-publish-0.2.4/
--rw-rw-rw-   0        0        0    11558 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      454 2023-04-19 12:18:15.308856 roblox-asset-publish-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.4/README.md
--rw-rw-rw-   0        0        0      560 2023-04-19 12:17:41.000000 roblox-asset-publish-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 12:18:15.309547 roblox-asset-publish-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 12:18:15.256681 roblox-asset-publish-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 12:18:15.296056 roblox-asset-publish-0.2.4/src/roblox_asset_publish.egg-info/
--rw-rw-rw-   0        0        0      454 2023-04-19 12:18:15.000000 roblox-asset-publish-0.2.4/src/roblox_asset_publish.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-19 12:18:15.000000 roblox-asset-publish-0.2.4/src/roblox_asset_publish.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:18:15.000000 roblox-asset-publish-0.2.4/src/roblox_asset_publish.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-19 12:18:15.000000 roblox-asset-publish-0.2.4/src/roblox_asset_publish.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-19 12:18:15.000000 roblox-asset-publish-0.2.4/src/roblox_asset_publish.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 12:18:15.306882 roblox-asset-publish-0.2.4/src/ropublisher/
--rw-rw-rw-   0        0        0    10935 2023-04-19 12:07:55.000000 roblox-asset-publish-0.2.4/src/ropublisher/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:22:37.235587 roblox-asset-publish-0.2.5/
+-rw-rw-rw-   0        0        0    11558 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      454 2023-04-19 12:22:37.234588 roblox-asset-publish-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.5/README.md
+-rw-rw-rw-   0        0        0      560 2023-04-19 12:22:10.000000 roblox-asset-publish-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:22:37.236583 roblox-asset-publish-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 12:22:37.202978 roblox-asset-publish-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 12:22:37.231598 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 12:22:37.233591 roblox-asset-publish-0.2.5/src/ropublisher/
+-rw-rw-rw-   0        0        0    10935 2023-04-19 12:07:55.000000 roblox-asset-publish-0.2.5/src/ropublisher/__init__.py
```

### Comparing `roblox-asset-publish-0.2.4/LICENSE` & `roblox-asset-publish-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-asset-publish-0.2.4/pyproject.toml` & `roblox-asset-publish-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roblox-asset-publish"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"requests==2.28.2", 
 	"mutagen==1.46.0", 
 ]
```

### Comparing `roblox-asset-publish-0.2.4/src/ropublisher/__init__.py` & `roblox-asset-publish-0.2.5/src/ropublisher/__init__.py`

 * *Files identical despite different names*

