# Comparing `tmp/roblox-asset-publish-0.2.5.tar.gz` & `tmp/roblox-asset-publish-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-asset-publish-0.2.5.tar", last modified: Wed Apr 19 12:22:37 2023, max compression
+gzip compressed data, was "roblox-asset-publish-0.2.6.tar", last modified: Wed Apr 19 12:42:00 2023, max compression
```

## Comparing `roblox-asset-publish-0.2.5.tar` & `roblox-asset-publish-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:22:37.235587 roblox-asset-publish-0.2.5/
--rw-rw-rw-   0        0        0    11558 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      454 2023-04-19 12:22:37.234588 roblox-asset-publish-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.5/README.md
--rw-rw-rw-   0        0        0      560 2023-04-19 12:22:10.000000 roblox-asset-publish-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 12:22:37.236583 roblox-asset-publish-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 12:22:37.202978 roblox-asset-publish-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 12:22:37.231598 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/
--rw-rw-rw-   0        0        0      454 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-19 12:22:37.000000 roblox-asset-publish-0.2.5/src/roblox_asset_publish.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 12:22:37.233591 roblox-asset-publish-0.2.5/src/ropublisher/
--rw-rw-rw-   0        0        0    10935 2023-04-19 12:07:55.000000 roblox-asset-publish-0.2.5/src/ropublisher/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:00.047176 roblox-asset-publish-0.2.6/
+-rw-rw-rw-   0        0        0    11558 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      454 2023-04-19 12:42:00.047176 roblox-asset-publish-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.6/README.md
+-rw-rw-rw-   0        0        0      560 2023-04-19 12:41:10.000000 roblox-asset-publish-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:42:00.048174 roblox-asset-publish-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:00.006400 roblox-asset-publish-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:00.043188 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 12:42:00.045182 roblox-asset-publish-0.2.6/src/ropublisher/
+-rw-rw-rw-   0        0        0    10935 2023-04-19 12:41:05.000000 roblox-asset-publish-0.2.6/src/ropublisher/__init__.py
```

### Comparing `roblox-asset-publish-0.2.5/LICENSE` & `roblox-asset-publish-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-asset-publish-0.2.5/pyproject.toml` & `roblox-asset-publish-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roblox-asset-publish"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"requests==2.28.2", 
 	"mutagen==1.46.0", 
 ]
```

### Comparing `roblox-asset-publish-0.2.5/src/ropublisher/__init__.py` & `roblox-asset-publish-0.2.6/src/ropublisher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
 				"Content-Type": "application/octet-stream",
 				"x-api-key": self.place_key,
 			}
 		)
 		print(x.text)
 
 
-	def post_decal(self, file_path: str, name: str | None = None, publish_to_group=True, description: str | None = None) -> int | None:
+	def post_image(self, file_path: str, name: str | None = None, publish_to_group=True, description: str | None = None) -> int | None:
 		if not name:
 			name = _get_name_from_path(file_path)
 
 		assert name, f"bad name for {file_path}"	
 
 		if not description:
 			description = f"{name} decal"
```

