# Comparing `tmp/signal-export-1.5.5.tar.gz` & `tmp/signal-export-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-export-1.5.5.tar", last modified: Sat Mar  4 20:29:26 2023, max compression
+gzip compressed data, was "signal-export-1.6.0.tar", last modified: Wed Apr 19 19:26:34 2023, max compression
```

## Comparing `signal-export-1.5.5.tar` & `signal-export-1.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.145009 signal-export-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-04 20:29:14.000000 signal-export-1.5.5/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.141009 signal-export-1.5.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-04 20:29:14.000000 signal-export-1.5.5/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.141009 signal-export-1.5.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-04 20:29:14.000000 signal-export-1.5.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-04 20:29:14.000000 signal-export-1.5.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.141009 signal-export-1.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-04 20:29:14.000000 signal-export-1.5.5/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-04 20:29:14.000000 signal-export-1.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-04 20:29:14.000000 signal-export-1.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-04 20:29:14.000000 signal-export-1.5.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-04 20:29:14.000000 signal-export-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-04 20:29:14.000000 signal-export-1.5.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-03-04 20:29:26.145009 signal-export-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-03-04 20:29:14.000000 signal-export-1.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-03-04 20:29:14.000000 signal-export-1.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 20:29:26.145009 signal-export-1.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.141009 signal-export-1.5.5/sigexport/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-04 20:29:14.000000 signal-export-1.5.5/sigexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-03-04 20:29:14.000000 signal-export-1.5.5/sigexport/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22947 2023-03-04 20:29:14.000000 signal-export-1.5.5/sigexport/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-04 20:29:14.000000 signal-export-1.5.5/sigexport/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-04 20:29:14.000000 signal-export-1.5.5/sigexport/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-04 20:29:14.000000 signal-export-1.5.5/sigexport/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.145009 signal-export-1.5.5/signal_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-03-04 20:29:26.000000 signal-export-1.5.5/signal_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-04 20:29:26.000000 signal-export-1.5.5/signal_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 20:29:26.000000 signal-export-1.5.5/signal_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-04 20:29:26.000000 signal-export-1.5.5/signal_export.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-04 20:29:26.000000 signal-export-1.5.5/signal_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-04 20:29:26.000000 signal-export-1.5.5/signal_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.145009 signal-export-1.5.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.145009 signal-export-1.5.5/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.145009 signal-export-1.5.5/tests/data/attachments.noindex/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-03-04 20:29:14.000000 signal-export-1.5.5/tests/data/attachments.noindex/image.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-03-04 20:29:14.000000 signal-export-1.5.5/tests/data/attachments.noindex/voicenote.m4a
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-04 20:29:14.000000 signal-export-1.5.5/tests/data/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 20:29:26.145009 signal-export-1.5.5/tests/data/sql/
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-03-04 20:29:14.000000 signal-export-1.5.5/tests/data/sql/db.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-03-04 20:29:14.000000 signal-export-1.5.5/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-04 20:29:14.000000 signal-export-1.5.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.481934 signal-export-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 19:26:22.000000 signal-export-1.6.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.477934 signal-export-1.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 19:26:22.000000 signal-export-1.6.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.477934 signal-export-1.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-19 19:26:22.000000 signal-export-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 19:26:22.000000 signal-export-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.477934 signal-export-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-19 19:26:22.000000 signal-export-1.6.0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-19 19:26:22.000000 signal-export-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-19 19:26:22.000000 signal-export-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-19 19:26:22.000000 signal-export-1.6.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-19 19:26:22.000000 signal-export-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 19:26:22.000000 signal-export-1.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-19 19:26:34.481934 signal-export-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-19 19:26:22.000000 signal-export-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-19 19:26:22.000000 signal-export-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:26:34.481934 signal-export-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.477934 signal-export-1.6.0/sigexport/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 19:26:22.000000 signal-export-1.6.0/sigexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-19 19:26:22.000000 signal-export-1.6.0/sigexport/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22947 2023-04-19 19:26:22.000000 signal-export-1.6.0/sigexport/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 19:26:22.000000 signal-export-1.6.0/sigexport/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-19 19:26:22.000000 signal-export-1.6.0/sigexport/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-19 19:26:22.000000 signal-export-1.6.0/sigexport/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.481934 signal-export-1.6.0/signal_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-19 19:26:34.000000 signal-export-1.6.0/signal_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-19 19:26:34.000000 signal-export-1.6.0/signal_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:26:34.000000 signal-export-1.6.0/signal_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 19:26:34.000000 signal-export-1.6.0/signal_export.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 19:26:34.000000 signal-export-1.6.0/signal_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 19:26:34.000000 signal-export-1.6.0/signal_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.481934 signal-export-1.6.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.481934 signal-export-1.6.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.481934 signal-export-1.6.0/tests/data/attachments.noindex/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-19 19:26:22.000000 signal-export-1.6.0/tests/data/attachments.noindex/image.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-04-19 19:26:22.000000 signal-export-1.6.0/tests/data/attachments.noindex/voicenote.m4a
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 19:26:22.000000 signal-export-1.6.0/tests/data/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:26:34.481934 signal-export-1.6.0/tests/data/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-04-19 19:26:22.000000 signal-export-1.6.0/tests/data/sql/db.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-04-19 19:26:22.000000 signal-export-1.6.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 19:26:22.000000 signal-export-1.6.0/tests/test_utils.py
```

### Comparing `signal-export-1.5.5/.github/workflows/cicd.yml` & `signal-export-1.6.0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/.gitignore` & `signal-export-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/.pre-commit-config.yaml` & `signal-export-1.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/Dockerfile` & `signal-export-1.6.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/LICENSE` & `signal-export-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/PKG-INFO` & `signal-export-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-export
-Version: 1.5.5
+Version: 1.6.0
 Summary: Export Signal conversations to Markdown and HTML
 Author-email: Chris Arderne <chris@rdrn.me>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/carderne/signal-export
 Project-URL: repository, https://github.com/carderne/signal-export
 Keywords: backup,chat,export
 Classifier: Environment :: Console
```

### Comparing `signal-export-1.5.5/README.md` & `signal-export-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/pyproject.toml` & `signal-export-1.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,18 +24,18 @@
   "Environment :: Console",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Unix",
   "Programming Language :: Python",
 ]
 
 dependencies = [
-    "beautifulsoup4>=4.11.1",
-    "emoji>=1.7.0",
-    "Markdown>=3.4.1",
-    "typer[all]>=0.7.0",
+    "beautifulsoup4 >= 4.11.1",
+    "emoji >= 1.7.0",
+    "Markdown >= 3.4.1",
+    "typer[all] >= 0.7.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
     "build",
     "mypy",
@@ -45,15 +45,16 @@
     "ruff",
     "setuptools-scm",
     "twine",
     "types-Markdown",
     "types-emoji",
 ]
 sql = [
-    "pysqlcipher3==1.1.0",
+    'pysqlcipher3 == 1.1.0; python_version < "3.11"',
+    'pysqlcipher3 >= 1.2.0; python_version >= "3.11"',
 ]
 
 [project.urls]
 homepage = "https://github.com/carderne/signal-export"
 repository = "https://github.com/carderne/signal-export"
 
 [tool.setuptools]
```

### Comparing `signal-export-1.5.5/sigexport/data.py` & `signal-export-1.6.0/sigexport/data.py`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/sigexport/main.py` & `signal-export-1.6.0/sigexport/main.py`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/sigexport/style.css` & `signal-export-1.6.0/sigexport/style.css`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/sigexport/templates.py` & `signal-export-1.6.0/sigexport/templates.py`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/signal_export.egg-info/PKG-INFO` & `signal-export-1.6.0/signal_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-export
-Version: 1.5.5
+Version: 1.6.0
 Summary: Export Signal conversations to Markdown and HTML
 Author-email: Chris Arderne <chris@rdrn.me>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/carderne/signal-export
 Project-URL: repository, https://github.com/carderne/signal-export
 Keywords: backup,chat,export
 Classifier: Environment :: Console
```

### Comparing `signal-export-1.5.5/signal_export.egg-info/SOURCES.txt` & `signal-export-1.6.0/signal_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/tests/data/attachments.noindex/image.jpeg` & `signal-export-1.6.0/tests/data/attachments.noindex/image.jpeg`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/tests/data/attachments.noindex/voicenote.m4a` & `signal-export-1.6.0/tests/data/attachments.noindex/voicenote.m4a`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/tests/data/sql/db.sqlite` & `signal-export-1.6.0/tests/data/sql/db.sqlite`

 * *Files identical despite different names*

### Comparing `signal-export-1.5.5/tests/test_integration.py` & `signal-export-1.6.0/tests/test_integration.py`

 * *Files identical despite different names*

