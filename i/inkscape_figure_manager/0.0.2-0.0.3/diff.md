# Comparing `tmp/inkscape_figure_manager-0.0.2.tar.gz` & `tmp/inkscape_figure_manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkscape_figure_manager-0.0.2.tar", last modified: Mon Apr 17 19:04:08 2023, max compression
+gzip compressed data, was "inkscape_figure_manager-0.0.3.tar", last modified: Wed Apr 19 04:08:39 2023, max compression
```

## Comparing `inkscape_figure_manager-0.0.2.tar` & `inkscape_figure_manager-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.2/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/LICENSE
--rw-r--r--   0        0        0       55 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.2/MANIFEST.in
--rw-r--r--   0        0        0      224 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/Pipfile
--rw-r--r--   0        0        0    28263 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/Pipfile.lock
--rw-r--r--   0        0        0     1038 2023-04-15 21:12:40.220852 inkscape_figure_manager-0.0.2/README.md
--rw-r--r--   0        0        0      709 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/__init__.py
--rw-r--r--   0        0        0     7810 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/__main__.py
--rw-r--r--   0        0        0     4022 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/daemon.py
--rw-r--r--   0        0        0     1427 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/picker.py
--rw-r--r--   0        0        0     1892 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/template.svg
--rw-r--r--   0        0        0     3354 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/watcher.py
--rw-r--r--   0        0        0     2504 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/watcher_daemon.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 inkscape_figure_manager-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/LICENSE
+-rw-r--r--   0        0        0       55 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.3/MANIFEST.in
+-rw-r--r--   0        0        0      224 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/Pipfile
+-rw-r--r--   0        0        0    28263 2023-04-19 04:06:10.275214 inkscape_figure_manager-0.0.3/Pipfile.lock
+-rw-r--r--   0        0        0     1038 2023-04-15 21:12:40.220852 inkscape_figure_manager-0.0.3/README.md
+-rw-r--r--   0        0        0      709 2023-04-19 04:06:56.711626 inkscape_figure_manager-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/__init__.py
+-rw-r--r--   0        0        0     7922 2023-04-19 04:05:37.378728 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/__main__.py
+-rw-r--r--   0        0        0     4022 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/daemon.py
+-rw-r--r--   0        0        0     1427 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/picker.py
+-rw-r--r--   0        0        0     1892 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/template.svg
+-rw-r--r--   0        0        0     3354 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/watcher.py
+-rw-r--r--   0        0        0     2504 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/watcher_daemon.py
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 inkscape_figure_manager-0.0.3/PKG-INFO
```

### Comparing `inkscape_figure_manager-0.0.2/LICENSE` & `inkscape_figure_manager-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.2/Pipfile.lock` & `inkscape_figure_manager-0.0.3/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666666%*

 * *Differences: {"'default'": "{'psutil': {'hashes': "*

 * *              "['sha256:104a5cc0e31baa2bcf67900be36acde157756b9c44017b86b2c049f11957887d', "*

 * *              "'sha256:3c6f686f4225553615612f6d9bc21f1c0e305f75d7d8454f9b46e901778e7217', "*

 * *              "'sha256:4aef137f3345082a3d3232187aeb4ac4ef959ba3d7c10c33dd73763fbc063da4', "*

 * *              "'sha256:5410638e4df39c54d957fc51ce03048acd8e6d60abc0f5107af51e5fb566eb3c', "*

 * *              "'sha256:5b9b8cb93f507e8dbaf22af6a2fd0ccbe8244bf30b1baad6b3954e935157ae3f', "*

 * *             […]*

```diff
@@ -30,31 +30,31 @@
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
             "version": "==8.1.3"
         },
         "psutil": {
             "hashes": [
-                "sha256:149555f59a69b33f056ba1c4eb22bb7bf24332ce631c44a319cec09f876aaeff",
-                "sha256:16653106f3b59386ffe10e0bad3bb6299e169d5327d3f187614b1cb8f24cf2e1",
-                "sha256:3d7f9739eb435d4b1338944abe23f49584bde5395f27487d2ee25ad9a8774a62",
-                "sha256:3ff89f9b835100a825b14c2808a106b6fdcc4b15483141482a12c725e7f78549",
-                "sha256:54c0d3d8e0078b7666984e11b12b88af2db11d11249a8ac8920dd5ef68a66e08",
-                "sha256:54d5b184728298f2ca8567bf83c422b706200bcbbfafdc06718264f9393cfeb7",
-                "sha256:6001c809253a29599bc0dfd5179d9f8a5779f9dffea1da0f13c53ee568115e1e",
-                "sha256:68908971daf802203f3d37e78d3f8831b6d1014864d7a85937941bb35f09aefe",
-                "sha256:6b92c532979bafc2df23ddc785ed116fced1f492ad90a6830cf24f4d1ea27d24",
-                "sha256:852dd5d9f8a47169fe62fd4a971aa07859476c2ba22c2254d4a1baa4e10b95ad",
-                "sha256:9120cd39dca5c5e1c54b59a41d205023d436799b1c8c4d3ff71af18535728e94",
-                "sha256:c1ca331af862803a42677c120aff8a814a804e09832f166f226bfd22b56feee8",
-                "sha256:efeae04f9516907be44904cc7ce08defb6b665128992a56957abc9b61dca94b7",
-                "sha256:fd8522436a6ada7b4aad6638662966de0d61d241cb821239b2ae7013d41a43d4"
+                "sha256:104a5cc0e31baa2bcf67900be36acde157756b9c44017b86b2c049f11957887d",
+                "sha256:3c6f686f4225553615612f6d9bc21f1c0e305f75d7d8454f9b46e901778e7217",
+                "sha256:4aef137f3345082a3d3232187aeb4ac4ef959ba3d7c10c33dd73763fbc063da4",
+                "sha256:5410638e4df39c54d957fc51ce03048acd8e6d60abc0f5107af51e5fb566eb3c",
+                "sha256:5b9b8cb93f507e8dbaf22af6a2fd0ccbe8244bf30b1baad6b3954e935157ae3f",
+                "sha256:7a7dd9997128a0d928ed4fb2c2d57e5102bb6089027939f3b722f3a210f9a8da",
+                "sha256:89518112647f1276b03ca97b65cc7f64ca587b1eb0278383017c2a0dcc26cbe4",
+                "sha256:8c5f7c5a052d1d567db4ddd231a9d27a74e8e4a9c3f44b1032762bd7b9fdcd42",
+                "sha256:ab8ed1a1d77c95453db1ae00a3f9c50227ebd955437bcf2a574ba8adbf6a74d5",
+                "sha256:acf2aef9391710afded549ff602b5887d7a2349831ae4c26be7c807c0a39fac4",
+                "sha256:b258c0c1c9d145a1d5ceffab1134441c4c5113b2417fafff7315a917a026c3c9",
+                "sha256:be8929ce4313f9f8146caad4272f6abb8bf99fc6cf59344a3167ecd74f4f203f",
+                "sha256:c607bb3b57dc779d55e1554846352b4e358c10fff3abf3514a7a6601beebdb30",
+                "sha256:ea8518d152174e1249c4f2a1c89e3e6065941df2fa13a1ab45327716a23c2b48"
             ],
             "index": "pypi",
-            "version": "==5.9.4"
+            "version": "==5.9.5"
         },
         "watchdog": {
             "hashes": [
                 "sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a",
                 "sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100",
                 "sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8",
                 "sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc",
@@ -85,19 +85,19 @@
             "index": "pypi",
             "version": "==3.0.0"
         }
     },
     "develop": {
         "astroid": {
             "hashes": [
-                "sha256:6e61b85c891ec53b07471aec5878f4ac6446a41e590ede0f2ce095f39f7d49dd",
-                "sha256:dea89d9f99f491c66ac9c04ebddf91e4acf8bd711722175fe6245c0725cc19bb"
+                "sha256:44224ad27c54d770233751315fa7f74c46fa3ee0fab7beef1065f99f09897efe",
+                "sha256:f11e74658da0f2a14a8d19776a8647900870a63de71db83713a8e77a6af52662"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.2"
+            "version": "==2.15.3"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
```

### Comparing `inkscape_figure_manager-0.0.2/README.md` & `inkscape_figure_manager-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.2/pyproject.toml` & `inkscape_figure_manager-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = 'inkscape_figure_manager'
-version = '0.0.2'
+version = '0.0.3'
 authors = [
   { name="Silas Waxter" },
   { name="Gille Castel" },
 ]
 description = "An API for managing inkscape figures."
 readme = "README.md"
 classifiers = [
```

### Comparing `inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/__main__.py` & `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from pathlib import Path
 from shutil import copy
 
 import click
 from appdirs import user_config_dir
 
 from inkscape_figure_manager import picker
-from inkscape_figure_manager.watcher_daemon import WatcherDaemon
 from inkscape_figure_manager.watcher import EXPORT_EXTENSTION_NO_DOT, Watcher
+from inkscape_figure_manager.watcher_daemon import WatcherDaemon
 
 APPLICATION_NAME = "inkscape-figure-manager"
 # os-agnostic path to current user's configuration directory for this
 # application
 APP_USER_CONFIG_DIR = Path(user_config_dir(APPLICATION_NAME, False))
 ROOT_FILE_PATH = APP_USER_CONFIG_DIR / 'roots'
 TEMPLATE_FILE_PATH = APP_USER_CONFIG_DIR / 'template.svg'
@@ -27,14 +27,19 @@
 ERROR_CODE_GIT_REPO_DNE = 3
 ERROR_CODE_BAD_DIR_TO_WATCH = 4
 
 logging.basicConfig(level=os.environ.get("LOGLEVEL", "INFO"))
 log = logging.getLogger('inkscape-figures')
 
 
+def eprint(*args, **kwargs):
+    """Error print to stderr"""
+    print(*args, file=sys.stderr, **kwargs)
+
+
 def snake_case(string):
     """
     Returns the snake case form of the passed string. Spaces and
     dashes are replaced with underscores, and the string is made lowercase.
     """
     return string.lower().replace(' ', '_').replace('-', ' ')
 
@@ -79,19 +84,19 @@
     figure files (*.svg); exports the figure (*.png) when this occurs.
 
     WATCHED_DIR: directory to watch
     """
     if git:
         watched_dir = Watcher.find_git_root(watched_dir)
         if watched_dir is None:
-            print("WATCHED_DIR is not within a git repository")
+            eprint("WATCHED_DIR is not within a git repository")
             sys.exit(ERROR_CODE_GIT_REPO_DNE)
     else:
         if not Path(watched_dir).is_dir():
-            print("WATCHED_DIR is not an existing directory")
+            eprint("WATCHED_DIR is not an existing directory")
             sys.exit(ERROR_CODE_BAD_DIR_TO_WATCH)
     WatcherDaemon.ensure_watch(watched_dir)
 
 
 @cli.command()
 @click.argument('alternate_text')
 @click.option('-d', '--figure-dir',
@@ -136,16 +141,16 @@
 
     relative_figure = relative_path / figure_file_name
     relative_figure_exported = relative_path / figure_file_name_exported
     absolute_figure = (relative_from / relative_figure).absolute()
 
     # Ensure figure does not exist
     if relative_figure.exists():
-        print(f"A file with the same name already exists at "
-              f"'{relative_figure}'")
+        eprint(f"A file with the same name already exists at "
+               f"'{relative_figure}'")
         sys.exit(ERROR_CODE_CREATED_FILE_ALREADY_EXISTS)
 
     # Create and return inclusion text
     copy(str(TEMPLATE_FILE_PATH), str(absolute_figure))
     open_inkscape(absolute_figure)
     WatcherDaemon.ensure_watch(figure_dir)
     print(markdown_include_image_text(alternate_text,
@@ -166,15 +171,15 @@
     figures. When multiple figures are within the directory, a picker will
     be used for selection. Default is the current working directory.
     """
     path = Path(path).absolute()
 
     # ensure path exists
     if not path.exists():
-        print(f"The path does not exsist; received '{path}'.")
+        eprint(f"The path does not exsist; received '{path}'.")
         sys.exit(ERROR_CODE_EDITED_FILE_PATH_DOES_NOT_EXIST)
 
     selected_file = None
     if path.is_file():
         selected_file = path
 
     elif path.is_dir():
```

### Comparing `inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/daemon.py` & `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/daemon.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/picker.py` & `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/picker.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/template.svg` & `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/template.svg`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/watcher.py` & `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/watcher.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.2/src/inkscape_figure_manager/watcher_daemon.py` & `inkscape_figure_manager-0.0.3/src/inkscape_figure_manager/watcher_daemon.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.2/PKG-INFO` & `inkscape_figure_manager-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkscape_figure_manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: An API for managing inkscape figures.
 Author: Silas Waxter, Gille Castel
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Dist: click
 Requires-Dist: appdirs
```

