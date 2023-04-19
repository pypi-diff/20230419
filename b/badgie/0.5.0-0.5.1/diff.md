# Comparing `tmp/badgie-0.5.0.tar.gz` & `tmp/badgie-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgie-0.5.0.tar", last modified: Wed Apr 19 05:24:19 2023, max compression
+gzip compressed data, was "badgie-0.5.1.tar", last modified: Wed Apr 19 05:53:50 2023, max compression
```

## Comparing `badgie-0.5.0.tar` & `badgie-0.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.548009 badgie-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-19 05:24:15.000000 badgie-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3936 2023-04-19 05:24:19.548009 badgie-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-04-19 05:24:15.000000 badgie-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.542008 badgie-0.5.0/badgie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-19 05:24:16.000000 badgie-0.5.0/badgie/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.546009 badgie-0.5.0/badgie/badges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/brettops.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/codestyle.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     5154 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.547009 badgie-0.5.0/badgie/detectors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/detectors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/detectors/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.547009 badgie-0.5.0/badgie/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/providers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/providers/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.548009 badgie-0.5.0/badgie/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/sources/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.544009 badgie-0.5.0/badgie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3936 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      677 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-19 05:24:19.549009 badgie-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-19 05:24:16.000000 badgie-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.019352 badgie-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-19 05:53:46.000000 badgie-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4482 2023-04-19 05:53:50.019352 badgie-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-04-19 05:53:46.000000 badgie-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.013352 badgie-0.5.1/badgie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-19 05:53:47.000000 badgie-0.5.1/badgie/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.017352 badgie-0.5.1/badgie/badges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/brettops.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/codestyle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/badges/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5154 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.018352 badgie-0.5.1/badgie/detectors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/detectors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/detectors/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.018352 badgie-0.5.1/badgie/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/providers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/providers/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.019352 badgie-0.5.1/badgie/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-04-19 05:53:46.000000 badgie-0.5.1/badgie/sources/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:53:50.015352 badgie-0.5.1/badgie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4482 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      677 2023-04-19 05:53:50.000000 badgie-0.5.1/badgie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 05:53:49.000000 badgie-0.5.1/badgie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-19 05:53:50.020352 badgie-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-19 05:53:47.000000 badgie-0.5.1/setup.py
```

### Comparing `badgie-0.5.0/LICENSE` & `badgie-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/PKG-INFO` & `badgie-0.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.5.0
+Version: 0.5.1
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge template markdown
 Platform: UNKNOWN
@@ -134,14 +134,47 @@
 
 [![pipeline status](brettops/containers/verible/badges/main/pipeline.svg)](brettops/containers/verible/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <!-- END BADGIE TIME -->
 ```
 
+### Use as a pre-commit hook
+
+Badgie can be used as a pre-commit hook, so you can get fresh badges on every
+commit.
+
+Add the following to a `.pre-commit-config.yaml` file. Note the empty
+`rev` tag:
+
+```yaml
+repos:
+  - repo: https://gitlab.com/brettops/tools/badgie
+    rev: ""
+    hooks:
+      - id: badgie
+```
+
+Run `pre-commit autoupdate` to pin to the latest version:
+
+```bash
+pre-commit autoupdate
+```
+
+Run `pre-commit` directly or install as a hook:
+
+```bash
+# directly
+pre-commit
+
+# as a Git hook
+pre-commit install
+git commit -m "..."
+```
+
 ## Caveats
 
 Badgie makes decisions on the assumption that you do sensible things with your
 repository structure. It does not try to work around bad practices. MRs that
 encourage this will be rejected.
```

### Comparing `badgie-0.5.0/README.md` & `badgie-0.5.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -109,12 +109,45 @@
 
 [![pipeline status](brettops/containers/verible/badges/main/pipeline.svg)](brettops/containers/verible/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <!-- END BADGIE TIME -->
 ```
 
+### Use as a pre-commit hook
+
+Badgie can be used as a pre-commit hook, so you can get fresh badges on every
+commit.
+
+Add the following to a `.pre-commit-config.yaml` file. Note the empty
+`rev` tag:
+
+```yaml
+repos:
+  - repo: https://gitlab.com/brettops/tools/badgie
+    rev: ""
+    hooks:
+      - id: badgie
+```
+
+Run `pre-commit autoupdate` to pin to the latest version:
+
+```bash
+pre-commit autoupdate
+```
+
+Run `pre-commit` directly or install as a hook:
+
+```bash
+# directly
+pre-commit
+
+# as a Git hook
+pre-commit install
+git commit -m "..."
+```
+
 ## Caveats
 
 Badgie makes decisions on the assumption that you do sensible things with your
 repository structure. It does not try to work around bad practices. MRs that
 encourage this will be rejected.
```

### Comparing `badgie-0.5.0/badgie/badges/_base.py` & `badgie-0.5.1/badgie/badges/_base.py`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/badgie/badges/brettops.py` & `badgie-0.5.1/badgie/badges/brettops.py`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/badgie/badges/codestyle.py` & `badgie-0.5.1/badgie/badges/codestyle.py`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/badgie/badges/gitlab.py` & `badgie-0.5.1/badgie/badges/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/badgie/cli.py` & `badgie-0.5.1/badgie/cli.py`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/badgie/detectors/precommit.py` & `badgie-0.5.1/badgie/detectors/precommit.py`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/badgie/parser.py` & `badgie-0.5.1/badgie/parser.py`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/badgie/providers/gitlab.py` & `badgie-0.5.1/badgie/providers/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/badgie/sources/base.py` & `badgie-0.5.1/badgie/sources/base.py`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/badgie.egg-info/PKG-INFO` & `badgie-0.5.1/badgie.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.5.0
+Version: 0.5.1
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge template markdown
 Platform: UNKNOWN
@@ -134,14 +134,47 @@
 
 [![pipeline status](brettops/containers/verible/badges/main/pipeline.svg)](brettops/containers/verible/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <!-- END BADGIE TIME -->
 ```
 
+### Use as a pre-commit hook
+
+Badgie can be used as a pre-commit hook, so you can get fresh badges on every
+commit.
+
+Add the following to a `.pre-commit-config.yaml` file. Note the empty
+`rev` tag:
+
+```yaml
+repos:
+  - repo: https://gitlab.com/brettops/tools/badgie
+    rev: ""
+    hooks:
+      - id: badgie
+```
+
+Run `pre-commit autoupdate` to pin to the latest version:
+
+```bash
+pre-commit autoupdate
+```
+
+Run `pre-commit` directly or install as a hook:
+
+```bash
+# directly
+pre-commit
+
+# as a Git hook
+pre-commit install
+git commit -m "..."
+```
+
 ## Caveats
 
 Badgie makes decisions on the assumption that you do sensible things with your
 repository structure. It does not try to work around bad practices. MRs that
 encourage this will be rejected.
```

### Comparing `badgie-0.5.0/badgie.egg-info/SOURCES.txt` & `badgie-0.5.1/badgie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badgie-0.5.0/setup.py` & `badgie-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

