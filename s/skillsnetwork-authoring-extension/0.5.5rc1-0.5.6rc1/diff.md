# Comparing `tmp/skillsnetwork-authoring-extension-0.5.5rc1.tar.gz` & `tmp/skillsnetwork-authoring-extension-0.5.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillsnetwork-authoring-extension-0.5.5rc1.tar", last modified: Thu Mar 30 23:53:21 2023, max compression
+gzip compressed data, was "skillsnetwork-authoring-extension-0.5.6rc1.tar", last modified: Wed Apr 19 14:41:47 2023, max compression
```

## Comparing `skillsnetwork-authoring-extension-0.5.5rc1.tar` & `skillsnetwork-authoring-extension-0.5.6rc1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.225798 skillsnetwork-authoring-extension-0.5.5rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-03-30 23:53:21.225798 skillsnetwork-authoring-extension-0.5.5rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.217797 skillsnetwork-authoring-extension-0.5.5rc1/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.221797 skillsnetwork-authoring-extension-0.5.5rc1/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.221797 skillsnetwork-authoring-extension-0.5.5rc1/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/jupyter-config/server-config/skillsnetwork_authoring_extension.json
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-03-30 23:52:05.000000 skillsnetwork-authoring-extension-0.5.5rc1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 23:53:21.225798 skillsnetwork-authoring-extension-0.5.5rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.221797 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.221797 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-03-30 23:53:20.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.221797 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-03-30 23:53:20.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/568.ce87b2f96464ec26573e.js
--rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-03-30 23:53:20.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-30 23:53:20.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-03-30 23:53:20.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.b585f71a139b6c522bd1.js
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-30 23:53:19.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-03-30 23:53:20.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.221797 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork_authoring_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-03-30 23:53:21.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-30 23:53:21.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 23:53:21.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 23:52:37.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork_authoring_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 23:53:21.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork_authoring_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 23:53:21.000000 skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork_authoring_extension.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.225798 skillsnetwork-authoring-extension-0.5.5rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.225798 skillsnetwork-authoring-extension-0.5.5rc1/src/button/
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/src/button/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/src/button/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/src/config.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/src/dialog.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.225798 skillsnetwork-authoring-extension-0.5.5rc1/src/menu/
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/src/menu/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/src/sn-file-library.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/src/tools.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 23:53:21.225798 skillsnetwork-authoring-extension-0.5.5rc1/style/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-30 23:52:04.000000 skillsnetwork-authoring-extension-0.5.5rc1/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)   218389 2023-03-30 23:53:07.000000 skillsnetwork-authoring-extension-0.5.5rc1/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.738331 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/jupyter-config/server-config/skillsnetwork_authoring_extension.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-19 14:40:32.000000 skillsnetwork-authoring-extension-0.5.6rc1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/568.d23144daea3f495050cb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.1ebb17cfc896e2585599.js
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-19 14:41:45.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:41:04.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 14:41:47.000000 skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.742331 skillsnetwork-authoring-extension-0.5.6rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/src/button/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/button/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/button/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/dialog.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/src/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/menu/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/sn-file-library.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/src/tools.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:41:47.746331 skillsnetwork-authoring-extension-0.5.6rc1/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-19 14:40:26.000000 skillsnetwork-authoring-extension-0.5.6rc1/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218440 2023-04-19 14:41:34.000000 skillsnetwork-authoring-extension-0.5.6rc1/yarn.lock
```

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/LICENSE` & `skillsnetwork-authoring-extension-0.5.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.6rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.5rc1
+Version: 0.5.6rc1
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/README.md` & `skillsnetwork-authoring-extension-0.5.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/package.json` & `skillsnetwork-authoring-extension-0.5.6rc1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.5.6-rc1'"}*

```diff
@@ -103,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.5-rc1"
+    "version": "0.5.6-rc1"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/pyproject.toml` & `skillsnetwork-authoring-extension-0.5.6rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/setup.py` & `skillsnetwork-authoring-extension-0.5.6rc1/setup.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/__init__.py` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/_version.py` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/_version.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/handlers.py` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/handlers.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/package.json` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.1ebb17cfc896e2585599.js'}}",*

 * * "'version'": "'0.5.6-rc1'"}*

```diff
@@ -54,15 +54,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b585f71a139b6c522bd1.js",
+            "load": "static/remoteEntry.1ebb17cfc896e2585599.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "skillsnetwork-authoring-extension/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
@@ -108,9 +108,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.5-rc1"
+    "version": "0.5.6-rc1"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/568.ce87b2f96464ec26573e.js` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/568.d23144daea3f495050cb.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,122 +1,135 @@
 "use strict";
 (self.webpackChunkskillsnetwork_authoring_extension = self.webpackChunkskillsnetwork_authoring_extension || []).push([
     [568], {
-        7953: (t, e, n) => {
-            n.a(t, (async (t, o) => {
+        7953: (t, e, o) => {
+            o.a(t, (async (t, n) => {
                 try {
-                    n.d(e, {
+                    o.d(e, {
                         Z: () => m
                     });
-                    var a = n(3619),
-                        l = n(2884),
-                        s = n(5923),
-                        i = n(9448),
-                        r = n(8623),
-                        c = n(3311),
-                        u = n(6973),
-                        d = n(405),
-                        h = n(5679),
-                        w = n(5449),
-                        b = t([d, r, c, w]);
-                    [d, r, c, w] = b.then ? (await b)() : b;
-                    const g = {
-                        activate: y,
+                    var a = o(7986),
+                        l = o(3033),
+                        i = o(5923),
+                        s = o(5344),
+                        r = o(8623),
+                        c = o(3311),
+                        u = o(6973),
+                        d = o(3619),
+                        h = o(1123),
+                        b = o(5449),
+                        w = t([d, r, c, b]);
+                    [d, r, c, b] = w.then ? (await w)() : w;
+                    const p = {
+                        activate: g,
                         id: "skillsnetwork-authoring-extension:plugin",
                         autoStart: !0,
-                        requires: [i.IMainMenu, h.INotebookTracker, a.IDocumentManager]
+                        requires: [s.IMainMenu, h.INotebookTracker, a.IDocumentManager]
                     };
-                    class p {
+                    class y {
                         createNew(t, e) {
-                            if (d.OH.SHOW_PUBLISH_BUTTON_FOR !== e.path) return new s.DisposableDelegate((() => {})); {
-                                const n = async () => {
-                                    const n = await (0, r.nu)(t, e),
-                                        o = d.OH.TOKENS.get(t.id);
-                                    void 0 !== o ? (0, c.nK)((0, c.SJ)(o), n) : console.log("No atlas token found for id", t.id)
-                                }, o = new l.ToolbarButton({
+                            if (d.OH.SHOW_PUBLISH_BUTTON_FOR !== e.path) return new i.DisposableDelegate((() => {})); {
+                                const o = async () => {
+                                    const o = await (0, r.nu)(t, e),
+                                        n = d.OH.TOKENS.get(t.id);
+                                    void 0 !== n ? (0, c.nK)((0, c.SJ)(n), o) : console.log("No atlas token found for id", t.id)
+                                }, n = async () => {
+                                    const o = await (0, r.nu)(t, e),
+                                        n = new Blob([o], {
+                                            type: "application/x-ipynb+json"
+                                        }),
+                                        a = URL.createObjectURL(n),
+                                        l = document.createElement("a");
+                                    l.setAttribute("download", e.path), l.setAttribute("href", a), document.body.appendChild(l), l.click(), document.body.removeChild(l), URL.revokeObjectURL(a)
+                                }, a = new l.ToolbarButton({
+                                    className: "download-lab-button",
+                                    label: "Download",
+                                    onClick: n,
+                                    tooltip: "Download Lab"
+                                }), s = new l.ToolbarButton({
                                     className: "publish-lab-button",
                                     label: "Publish on SN",
-                                    onClick: n,
+                                    onClick: o,
                                     tooltip: "Publish Lab"
-                                }), a = new l.ToolbarButton({
+                                }), u = new l.ToolbarButton({
                                     className: "sn-file-library-button",
                                     label: "SN File Library",
-                                    onClick: () => new w.E(t.id).launch(),
+                                    onClick: () => new b.E(t.id).launch(),
                                     tooltip: "Skills Network File Library"
                                 });
-                                return t.toolbar.insertItem(9, "sn-file-library", a), t.toolbar.insertItem(10, "publish", o), new s.DisposableDelegate((() => {
-                                    o.dispose(), a.dispose()
+                                return t.toolbar.insertItem(8, "download", a), t.toolbar.insertItem(9, "sn-file-library", u), t.toolbar.insertItem(10, "publish", s), new i.DisposableDelegate((() => {
+                                    a.dispose(), s.dispose(), u.dispose()
                                 }))
                             }
                         }
                     }
-                    async function y(t, e, n, o) {
+                    async function g(t, e, o, n) {
                         if (console.log("Activated skillsnetwork-authoring-extension button plugin!"), "learn" == await (0, d.IK)()) return;
                         const a = await (0, d.Nz)(),
-                            s = await (0, d.D2)();
-                        console.log("Using default kernel: ", d.OH.PY_KERNEL_NAME), t.docRegistry.addWidgetExtension("Notebook", new p), t.restored.then((async () => {
-                            if ("NO_TOKEN" !== a && "local" !== s) try {
-                                await (0, r._Y)(a, o)
+                            i = await (0, d.D2)();
+                        console.log("Using default kernel: ", d.OH.PY_KERNEL_NAME), t.docRegistry.addWidgetExtension("Notebook", new y), t.restored.then((async () => {
+                            if ("NO_TOKEN" !== a && "local" !== i) try {
+                                await (0, r._Y)(a, n)
                             } catch (t) {
                                 l.Dialog.flush(), (0, u.YZ)(), console.log(t)
                             }
                         }))
                     }
-                    const m = g;
-                    o()
+                    const m = p;
+                    n()
                 } catch (f) {
-                    o(f)
+                    n(f)
                 }
             }))
         },
-        405: (t, e, n) => {
-            n.a(t, (async (t, o) => {
+        3619: (t, e, o) => {
+            o.a(t, (async (t, n) => {
                 try {
-                    n.d(e, {
-                        CC: () => s,
+                    o.d(e, {
+                        CC: () => i,
                         D2: () => c,
-                        IK: () => i,
+                        IK: () => s,
                         Nz: () => r,
                         OH: () => d,
                         XM: () => l
                     });
-                    var a = n(5613);
+                    var a = o(8820);
                     const t = t => {
                             let e = t.baseUrl;
                             return e.endsWith("/") || (e += "/"), e
                         },
                         l = await (async () => {
                             const e = window.location.href,
-                                n = new URL(e).searchParams.get("atlas_base_url");
-                            if (null === n) {
+                                o = new URL(e).searchParams.get("atlas_base_url");
+                            if (null === o) {
                                 const e = {
                                         method: "GET"
                                     },
-                                    n = a.ServerConnection.makeSettings(),
-                                    o = t(n) + "skillsnetwork-authoring-extension/config",
-                                    l = await a.ServerConnection.makeRequest(o, e, n);
+                                    o = a.ServerConnection.makeSettings(),
+                                    n = t(o) + "skillsnetwork-authoring-extension/config",
+                                    l = await a.ServerConnection.makeRequest(n, e, o);
                                 return (await l.json()).ATLAS_BASE_URL
                             }
-                            return decodeURIComponent(n)
+                            return decodeURIComponent(o)
                         })(),
-                        s = await (async () => {
+                        i = await (async () => {
                             const e = window.location.href,
-                                n = new URL(e).searchParams.get("sn_file_library_url");
-                            if (null === n) {
+                                o = new URL(e).searchParams.get("sn_file_library_url");
+                            if (null === o) {
                                 const e = {
                                         method: "GET"
                                     },
-                                    n = a.ServerConnection.makeSettings(),
-                                    o = t(n) + "skillsnetwork-authoring-extension/config",
-                                    l = await a.ServerConnection.makeRequest(o, e, n);
+                                    o = a.ServerConnection.makeSettings(),
+                                    n = t(o) + "skillsnetwork-authoring-extension/config",
+                                    l = await a.ServerConnection.makeRequest(n, e, o);
                                 return (await l.json()).SN_FILE_LIBRARY_URL
                             }
-                            return decodeURIComponent(n)
+                            return decodeURIComponent(o)
                         })(),
-                        i = async () => {
+                        s = async () => {
                             const t = window.location.href;
                             let e = new URL(t).searchParams.get("mode");
                             return "learn" == e ? e : "author"
                         }, r = async () => {
                             const t = window.location.href,
                                 e = new URL(t).searchParams.get("atlas_token");
                             return null !== e ? e : "NO_TOKEN"
@@ -128,49 +141,49 @@
                             let t = await (await a.KernelSpecAPI.getSpecs()).kernelspecs,
                                 e = Object.keys(t).filter((function(t) {
                                     return t.includes("python")
                                 })).sort();
                             return e[e.length - 1]
                         };
                     class d {}
-                    d.TOKENS = new Map, d.SHOW_PUBLISH_BUTTON_FOR = void 0, o()
+                    d.TOKENS = new Map, d.SHOW_PUBLISH_BUTTON_FOR = void 0, n()
                 } catch (t) {
-                    o(t)
+                    n(t)
                 }
             }), 1)
         },
-        6973: (t, e, n) => {
-            n.d(e, {
-                Up: () => s,
+        6973: (t, e, o) => {
+            o.d(e, {
+                Up: () => i,
                 YZ: () => d,
                 fP: () => u,
                 ql: () => r,
                 wW: () => c,
-                wj: () => i
+                wj: () => s
             });
-            var o = n(1431),
-                a = n(2884);
-            class l extends o.Widget {
+            var n = o(8832),
+                a = o(3033);
+            class l extends n.Widget {
                 constructor() {
                     const t = document.createElement("div"),
                         e = new a.Spinner;
                     t.appendChild(e.node), t.style.padding = "15px", super({
                         node: t
                     })
                 }
             }
-            const s = t => {
+            const i = t => {
                     const e = new l;
                     (0, a.showDialog)({
                         title: t,
                         body: e,
                         buttons: [a.Dialog.cancelButton()]
                     })
                 },
-                i = t => {
+                s = t => {
                     const e = new l;
                     return (0, a.showDialog)({
                         title: t,
                         body: e,
                         buttons: []
                     })
                 },
@@ -199,245 +212,245 @@
                     (0, a.showDialog)({
                         title: "Failed to Load Lab",
                         body: "This lab failed to load.",
                         buttons: [a.Dialog.okButton()]
                     }).then((t => {})).catch((t => {}))
                 }
         },
-        3311: (t, e, n) => {
-            n.a(t, (async (t, o) => {
+        3311: (t, e, o) => {
+            o.a(t, (async (t, n) => {
                 try {
-                    n.d(e, {
+                    o.d(e, {
                         B4: () => d,
                         SJ: () => u,
                         nK: () => h
                     });
-                    var a = n(6973),
-                        l = n(2884),
-                        s = n(405),
-                        i = n(9581),
-                        r = n.n(i),
-                        c = t([s]);
-                    s = (c.then ? (await c)() : c)[0];
+                    var a = o(6973),
+                        l = o(3033),
+                        i = o(3619),
+                        s = o(9581),
+                        r = o.n(s),
+                        c = t([i]);
+                    i = (c.then ? (await c)() : c)[0];
                     const u = t => r().create({
-                            baseURL: s.XM,
+                            baseURL: i.XM,
                             headers: {
                                 Authorization: `Bearer ${t}`,
                                 "Content-Type": "application/json",
                                 "Access-Control-Allow-Origin": "*",
                                 Accept: "application/json"
                             }
                         }),
                         d = t => t.get("v1/labs").then((t => (l.Dialog.flush(), t.data))).catch((t => {
                             throw console.log(t), "Failed to fetch notebook"
                         })),
                         h = async (t, e) => {
-                            if (await (0, a.ql)("Publishing your lab onto Skills Network...").then((t => !0)).catch((t => !1))) return (0, a.wj)("Publishing your changes..."), new Promise((async (n, o) => {
+                            if (await (0, a.ql)("Publishing your lab onto Skills Network...").then((t => !0)).catch((t => !1))) return (0, a.wj)("Publishing your changes..."), new Promise((async (o, n) => {
                                 await t.post("v1/labs", {
                                     body: e
                                 }).then((t => {
                                     console.log("SUCCESSFULLY PUSHED", t), l.Dialog.flush(), (0, a.wW)()
                                 })).catch((t => {
                                     console.log(t), l.Dialog.flush(), (0, a.fP)()
                                 }))
                             }))
                         };
-                    o()
+                    n()
                 } catch (t) {
-                    o(t)
+                    n(t)
                 }
             }))
         },
-        1568: (t, e, n) => {
-            n.a(t, (async (t, o) => {
+        1568: (t, e, o) => {
+            o.a(t, (async (t, n) => {
                 try {
-                    n.r(e), n.d(e, {
-                        default: () => i
+                    o.r(e), o.d(e, {
+                        default: () => s
                     });
-                    var a = n(4822),
-                        l = n(7953),
-                        s = t([l, a]);
-                    [l, a] = s.then ? (await s)() : s;
-                    const i = [l.Z, a.G];
-                    o()
+                    var a = o(4822),
+                        l = o(7953),
+                        i = t([l, a]);
+                    [l, a] = i.then ? (await i)() : i;
+                    const s = [l.Z, a.G];
+                    n()
                 } catch (t) {
-                    o(t)
+                    n(t)
                 }
             }))
         },
-        4822: (t, e, n) => {
-            n.a(t, (async (t, o) => {
+        4822: (t, e, o) => {
+            o.a(t, (async (t, n) => {
                 try {
-                    n.d(e, {
-                        G: () => w
+                    o.d(e, {
+                        G: () => b
                     });
-                    var a = n(9448),
-                        l = n(1431),
-                        s = n(2884),
-                        i = n(5679),
-                        r = n(3619),
-                        c = n(6973),
-                        u = n(405),
-                        d = n(8623),
+                    var a = o(5344),
+                        l = o(8832),
+                        i = o(3033),
+                        s = o(1123),
+                        r = o(7986),
+                        c = o(6973),
+                        u = o(3619),
+                        d = o(8623),
                         h = t([u, d]);
                     [u, d] = h.then ? (await h)() : h;
-                    const w = {
+                    const b = {
                         id: "skillsnetwork-authoring-extension:menu",
                         autoStart: !0,
-                        requires: [a.IMainMenu, i.INotebookTracker, r.IDocumentManager],
-                        activate: async (t, e, n, o) => {
+                        requires: [a.IMainMenu, s.INotebookTracker, r.IDocumentManager],
+                        activate: async (t, e, o, n) => {
                             if (console.log("Activated skillsnetwork-authoring-extension menu plugin!"), "learn" == await (0, u.IK)()) return;
                             const a = "edit-lab-from-token";
                             t.commands.addCommand(a, {
                                 label: "Edit a Lab",
                                 execute: () => {
-                                    h(n, o)
+                                    h(o, n)
                                 }
                             });
                             const {
-                                commands: i
+                                commands: s
                             } = t, r = new l.Menu({
-                                commands: i
+                                commands: s
                             });
                             r.title.label = "Skills Network", e.addMenu(r, {
                                 rank: 80
                             }), r.addItem({
                                 command: a,
                                 args: {}
                             });
                             const h = (t, e) => {
-                                let n = document.createElement("div"),
-                                    o = document.createElement("label");
-                                o.textContent = "Enter your authorization token: ";
+                                let o = document.createElement("div"),
+                                    n = document.createElement("label");
+                                n.textContent = "Enter your authorization token: ";
                                 let a = document.createElement("input");
-                                a.className = "jp-mod-styled", n.appendChild(o), n.appendChild(a), (0, s.showDialog)({
+                                a.className = "jp-mod-styled", o.appendChild(n), o.appendChild(a), (0, i.showDialog)({
                                     title: "Edit a Lab",
                                     body: new l.Widget({
-                                        node: n
+                                        node: o
                                     }),
-                                    buttons: [s.Dialog.cancelButton(), s.Dialog.okButton()]
+                                    buttons: [i.Dialog.cancelButton(), i.Dialog.okButton()]
                                 }).then((async t => {
                                     if (t.button.accept) {
                                         (0, c.Up)("Loading up your lab...");
                                         const t = a.value;
                                         await (0, d._Y)(t, e)
                                     }
                                 })).catch((t => {
-                                    s.Dialog.flush(), (0, c.YZ)(), console.log(t)
+                                    i.Dialog.flush(), (0, c.YZ)(), console.log(t)
                                 }))
                             }
                         }
                     };
-                    o()
+                    n()
                 } catch (t) {
-                    o(t)
+                    n(t)
                 }
             }))
         },
-        5449: (t, e, n) => {
-            n.a(t, (async (t, o) => {
+        5449: (t, e, o) => {
+            o.a(t, (async (t, n) => {
                 try {
-                    n.d(e, {
+                    o.d(e, {
                         E: () => d
                     });
-                    var a = n(1431),
-                        l = n(2884),
-                        s = n(405),
-                        i = t([s]);
-                    s = (i.then ? (await i)() : i)[0];
+                    var a = o(8832),
+                        l = o(3033),
+                        i = o(3619),
+                        s = t([i]);
+                    i = (s.then ? (await s)() : s)[0];
                     var r, c = function(t, e) {
                         if (!e.has(t)) throw new TypeError("attempted to get private field on non-instance");
                         return e.get(t)
                     };
                     class u extends a.Widget {
                         constructor(t) {
                             const e = document.createElement("iframe");
-                            e.src = `${s.CC}?atlas_token=${s.OH.TOKENS.get(t)}`, e.setAttribute("frameborder", "0"), e.setAttribute("allow", "clipboard-read; clipboard-write"), e.classList.add("sn-file-library-frame"), super({
+                            e.src = `${i.CC}?atlas_token=${i.OH.TOKENS.get(t)}`, e.setAttribute("frameborder", "0"), e.setAttribute("allow", "clipboard-read; clipboard-write"), e.classList.add("sn-file-library-frame"), super({
                                 node: e
                             })
                         }
                     }
                     class d {
                         constructor(t) {
                             r.set(this, void 0),
-                                function(t, e, n) {
+                                function(t, e, o) {
                                     if (!e.has(t)) throw new TypeError("attempted to set private field on non-instance");
-                                    e.set(t, n)
+                                    e.set(t, o)
                                 }(this, r, t)
                         }
                         launch() {
                             const t = new l.Dialog({
                                     title: "Skills Network File Library",
                                     body: new u(c(this, r)),
                                     hasClose: !0,
                                     buttons: []
                                 }),
                                 e = t.node.querySelector(".jp-Dialog-content");
                             e && e.classList.add("sn-file-library-dialog"), t.launch()
                         }
                     }
-                    r = new WeakMap, o()
+                    r = new WeakMap, n()
                 } catch (t) {
-                    o(t)
+                    n(t)
                 }
             }))
         },
-        8623: (t, e, n) => {
-            n.a(t, (async (t, o) => {
+        8623: (t, e, o) => {
+            o.a(t, (async (t, n) => {
                 try {
-                    n.d(e, {
+                    o.d(e, {
                         _Y: () => u,
                         nu: () => c
                     });
-                    var a = n(5679),
-                        l = n(405),
-                        s = n(3311),
-                        i = t([s, l]);
-                    [s, l] = i.then ? (await i)() : i;
+                    var a = o(1123),
+                        l = o(3619),
+                        i = o(3311),
+                        s = t([i, l]);
+                    [i, l] = s.then ? (await s)() : s;
                     const r = t => ({
                             cell_type: t.model.type,
                             id: t.model.id,
                             metadata: {},
                             outputs: [],
                             source: [t.model.value.text]
                         }),
                         c = (t, e) => {
-                            const n = [];
+                            const o = [];
                             t.content.widgets.forEach((t => {
                                 const e = r(t);
-                                n.push(e)
+                                o.push(e)
                             }));
-                            const o = e.model.metadata.toJSON(),
+                            const n = e.model.metadata.toJSON(),
                                 a = e.model.nbformat,
                                 l = e.model.nbformatMinor,
-                                s = {
-                                    cells: n,
-                                    metadata: o,
+                                i = {
+                                    cells: o,
+                                    metadata: n,
                                     nbformat: a,
                                     nbformat_minor: l
                                 };
-                            return JSON.stringify(s, null, 2)
+                            return JSON.stringify(i, null, 2)
                         },
                         u = async (t, e) => {
                             let {
-                                instructions_file_path: n,
-                                body: o
-                            } = await (0, s.B4)((0, s.SJ)(t));
-                            const a = h(n);
+                                instructions_file_path: o,
+                                body: n
+                            } = await (0, i.B4)((0, i.SJ)(t));
+                            const a = h(o);
                             l.OH.SHOW_PUBLISH_BUTTON_FOR = a;
-                            const i = e.createNew(a, "notebook", {
+                            const s = e.createNew(a, "notebook", {
                                 name: l.OH.PY_KERNEL_NAME
                             });
-                            if (l.OH.SHOW_PUBLISH_BUTTON_FOR = void 0, l.OH.TOKENS.set(i.id, t), void 0 === i) throw Error("Error loading lab");
-                            return d(i, JSON.parse(o)), i
-                        }, d = (t, e, n) => {
-                            const o = new a.NotebookModel;
-                            "local" !== n && o.fromJSON(e), t.content.model = o
+                            if (l.OH.SHOW_PUBLISH_BUTTON_FOR = void 0, l.OH.TOKENS.set(s.id, t), void 0 === s) throw Error("Error loading lab");
+                            return d(s, JSON.parse(n)), s
+                        }, d = (t, e, o) => {
+                            const n = new a.NotebookModel;
+                            "local" !== o && n.fromJSON(e), t.content.model = n
                         }, h = t => (null != t ? t : l.OH.DEFAULT_LAB_NAME).replace(/^.*[\\\/]/, "");
-                    o()
+                    n()
                 } catch (t) {
-                    o(t)
+                    n(t)
                 }
             }))
         }
     }
 ]);
```

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.b585f71a139b6c522bd1.js` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.1ebb17cfc896e2585599.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, c, d, p, h, v, b, m, g, y, w, k, _ = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b, m, g, y, w, k, _ = {
             5367: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(1568))),
                         "./extension": () => t.e(568).then((() => () => t(1568))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -37,20 +37,20 @@
         return _[e](t, t.exports, x), t.exports
     }
     x.m = _, x.c = S, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
         e && !e.d && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
     }, x.a = (o, a, i) => {
         var u;
         i && ((u = []).d = 1);
-        var l, s, f, c = new Set,
-            d = o.exports,
-            p = new Promise(((e, r) => {
+        var l, s, f, d = new Set,
+            p = o.exports,
+            c = new Promise(((e, r) => {
                 f = r, s = e
             }));
-        p[r] = d, p[e] = e => (u && e(u), c.forEach(e), p.catch((e => {}))), o.exports = p, a((o => {
+        c[r] = p, c[e] = e => (u && e(u), d.forEach(e), c.catch((e => {}))), o.exports = c, a((o => {
             var a;
             l = (o => o.map((o => {
                 if (null !== o && "object" == typeof o) {
                     if (o[e]) return o;
                     if (o.then) {
                         var a = [];
                         a.d = 0, o.then((e => {
@@ -67,35 +67,35 @@
             })))(o);
             var i = () => l.map((e => {
                     if (e[t]) throw e[t];
                     return e[r]
                 })),
                 s = new Promise((r => {
                     (a = () => r(i)).r = 0;
-                    var t = e => e !== u && !c.has(e) && (c.add(e), e && !e.d && (a.r++, e.push(a)));
+                    var t = e => e !== u && !d.has(e) && (d.add(e), e && !e.d && (a.r++, e.push(a)));
                     l.map((r => r[e](t)))
                 }));
             return a.r ? s : i()
-        }), (e => (e ? f(p[t] = e) : s(d), n(u)))), u && (u.d = 0)
+        }), (e => (e ? f(c[t] = e) : s(p), n(u)))), u && (u.d = 0)
     }, x.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return x.d(r, {
             a: r
         }), r
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
-        568: "ce87b2f96464ec26573e",
+        568: "d23144daea3f495050cb",
         669: "d32869c9490cd02b1382",
         747: "1af575e10eb228bf3434"
     } [e] + ".js?v=" + {
-        568: "ce87b2f96464ec26573e",
+        568: "d23144daea3f495050cb",
         669: "d32869c9490cd02b1382",
         747: "1af575e10eb228bf3434"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -110,24 +110,24 @@
                     var f = l[s];
                     if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == a + t) {
                         i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + t), i.src = e), o[e] = [r];
-            var c = (r, t) => {
-                    i.onerror = i.onload = null, clearTimeout(d);
+            var d = (r, t) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var n = o[e];
                     if (delete o[e], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(t))), r) return r(t)
                 },
-                d = setTimeout(c.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -149,15 +149,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "0.21.4", (() => x.e(669).then((() => () => x(9669))))), u("skillsnetwork-authoring-extension", "0.5.5-rc1", (() => x.e(568).then((() => () => x(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "0.21.4", (() => x.e(669).then((() => () => x(9669))))), u("skillsnetwork-authoring-extension", "0.5.6-rc1", (() => x.e(568).then((() => () => x(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -206,72 +206,72 @@
     }, s = (e, r) => {
         if (0 in e) {
             r = i(r);
             var t = e[0],
                 n = t < 0;
             n && (t = -t - 1);
             for (var o = 0, a = 1, u = !0;; a++, o++) {
-                var l, f, c = a < e.length ? (typeof e[a])[0] : "";
-                if (o >= r.length || "o" == (f = (typeof(l = r[o]))[0])) return !u || ("u" == c ? a > t && !n : "" == c != n);
+                var l, f, d = a < e.length ? (typeof e[a])[0] : "";
+                if (o >= r.length || "o" == (f = (typeof(l = r[o]))[0])) return !u || ("u" == d ? a > t && !n : "" == d != n);
                 if ("u" == f) {
-                    if (!u || "u" != c) return !1
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (c == f)
+                    if (d == f)
                         if (a <= t) {
                             if (l != e[a]) return !1
                         } else {
                             if (n ? l > e[a] : l < e[a]) return !1;
                             l != e[a] && (u = !1)
                         }
-                else if ("s" != c && "n" != c) {
+                else if ("s" != d && "n" != d) {
                     if (n || a <= t) return !1;
                     u = !1, a--
                 } else {
-                    if (a <= t || f < c != n) return !1;
+                    if (a <= t || f < d != n) return !1;
                     u = !1
-                } else "s" != c && "n" != c && (u = !1, a--)
+                } else "s" != d && "n" != d && (u = !1, a--)
             }
         }
-        var d = [],
-            p = d.pop.bind(d);
+        var p = [],
+            c = p.pop.bind(p);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
-            d.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? s(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? s(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, f = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, c = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && u(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", p = (e, r, t, n) => {
-        var o = c(e, t);
-        return s(n, o) || "undefined" != typeof console && console.warn && console.warn(d(e, t, o, n)), v(e[t][o])
+    }, p = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", c = (e, r, t, n) => {
+        var o = d(e, t);
+        return s(n, o) || "undefined" != typeof console && console.warn && console.warn(p(e, t, o, n)), v(e[t][o])
     }, h = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !s(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
     }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, n, o) {
         var a = x.I(r);
         return a && a.then ? a.then(e.bind(e, r, x.S[r], t, n, o)) : e(r, x.S[r], t, n, o)
-    })(((e, r, t, n) => (f(e, t), p(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (f(e, t), c(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
         var a = r && x.o(r, t) && h(r, t, n);
         return a ? v(a) : o()
     })), y = {}, w = {
-        1431: () => m("default", "@lumino/widgets", [1, 1, 37, 1]),
-        2884: () => m("default", "@jupyterlab/apputils", [1, 3, 6, 2]),
-        3619: () => m("default", "@jupyterlab/docmanager", [1, 3, 6, 2]),
-        5613: () => m("default", "@jupyterlab/services", [1, 6, 6, 2]),
-        5679: () => m("default", "@jupyterlab/notebook", [1, 3, 6, 2]),
+        1123: () => m("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        3033: () => m("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        5344: () => m("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
         5923: () => m("default", "@lumino/disposable", [1, 1, 10, 0]),
-        9448: () => m("default", "@jupyterlab/mainmenu", [1, 3, 6, 2]),
+        7986: () => m("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
+        8820: () => m("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        8832: () => m("default", "@lumino/widgets", [1, 1, 37, 2]),
         9581: () => g("default", "axios", [2, 0, 21, 2], (() => x.e(669).then((() => () => x(9669)))))
     }, k = {
-        568: [1431, 2884, 3619, 5613, 5679, 5923, 9448, 9581]
+        568: [1123, 3033, 5344, 5923, 7986, 8820, 8832, 9581]
     }, x.f.consumes = (e, r) => {
         x.o(k, e) && k[e].forEach((e => {
             if (x.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, x.m[e] = t => {
                         delete x.c[e], t.exports = r()
                     }
```

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.5rc1
+Version: 0.5.6rc1
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt` & `skillsnetwork-authoring-extension-0.5.6rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 yarn.lock
 jupyter-config/nb-config/skillsnetwork_authoring_extension.json
 jupyter-config/server-config/skillsnetwork_authoring_extension.json
 skillsnetwork-authoring-extension/__init__.py
 skillsnetwork-authoring-extension/_version.py
 skillsnetwork-authoring-extension/handlers.py
 skillsnetwork-authoring-extension/labextension/package.json
-skillsnetwork-authoring-extension/labextension/static/568.ce87b2f96464ec26573e.js
+skillsnetwork-authoring-extension/labextension/static/568.d23144daea3f495050cb.js
 skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
 skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
-skillsnetwork-authoring-extension/labextension/static/remoteEntry.b585f71a139b6c522bd1.js
+skillsnetwork-authoring-extension/labextension/static/remoteEntry.1ebb17cfc896e2585599.js
 skillsnetwork-authoring-extension/labextension/static/style.js
 skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
 skillsnetwork_authoring_extension.egg-info/PKG-INFO
 skillsnetwork_authoring_extension.egg-info/SOURCES.txt
 skillsnetwork_authoring_extension.egg-info/dependency_links.txt
 skillsnetwork_authoring_extension.egg-info/not-zip-safe
 skillsnetwork_authoring_extension.egg-info/requires.txt
```

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/src/button/index.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/button/index.ts`

 * *Files 11% similar despite different names*

```diff
@@ -66,31 +66,56 @@
           console.log('No atlas token found for id', panel.id);
           return;
         }
 
         postLabModel(axiosHandler(token), file);
       };
 
+      const download = async () => {
+        const file = await getFileContents(panel, context);
+        const blob = new Blob([file], { type: 'application/x-ipynb+json' });
+        const url = URL.createObjectURL(blob);
+
+        const link = document.createElement('a');
+        link.setAttribute('download', context.path);
+        link.setAttribute('href', url);
+
+        document.body.appendChild(link);
+        link.click();
+
+        document.body.removeChild(link);
+        URL.revokeObjectURL(url);
+      };
+
+      const downloadButton = new ToolbarButton({
+        className: 'download-lab-button',
+        label: 'Download',
+        onClick: download,
+        tooltip: 'Download Lab'
+      });
+
       const publishButton = new ToolbarButton({
         className: 'publish-lab-button',
         label: 'Publish on SN',
         onClick: start,
         tooltip: 'Publish Lab'
       });
 
       const snFileLibraryButton = new ToolbarButton({
         className: 'sn-file-library-button',
         label: 'SN File Library',
         onClick: () =>  (new SkillsNetworkFileLibrary(panel.id)).launch(),
         tooltip: 'Skills Network File Library'
       });
 
+      panel.toolbar.insertItem(8, 'download', downloadButton);
       panel.toolbar.insertItem(9, 'sn-file-library', snFileLibraryButton);
       panel.toolbar.insertItem(10, 'publish', publishButton);
       return new DisposableDelegate(() => {
+        downloadButton.dispose();
         publishButton.dispose();
         snFileLibraryButton.dispose();
       });
     }
   }
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/src/button/sample.json` & `skillsnetwork-authoring-extension-0.5.6rc1/src/button/sample.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/src/config.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/src/dialog.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/src/handler.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/src/menu/index.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/menu/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/src/sn-file-library.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/sn-file-library.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/src/tools.ts` & `skillsnetwork-authoring-extension-0.5.6rc1/src/tools.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/tsconfig.json` & `skillsnetwork-authoring-extension-0.5.6rc1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.5rc1/yarn.lock` & `skillsnetwork-authoring-extension-0.5.6rc1/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
   version "7.12.11"
   resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.12.11.tgz#f4ad435aa263db935b8f10f2c552d23fb716a63f"
   integrity sha512-Zt1yodBx1UcyiePMSkWnU4hPqhwq7hGi2nFL1LeA3EUl+q2LQx16MISgJ0+z7dnmgvP9QtIleuETGOiOH1RcIw==
   dependencies:
     "@babel/highlight" "^7.10.4"
 
 "@babel/code-frame@^7.0.0":
-  version "7.18.6"
-  resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.18.6.tgz#3b25d38c89600baa2dcc219edfa88a74eb2c427a"
-  integrity sha512-TDCmlK5eOvH+eH7cdAFlNXeVJqWIQ7gW9tY1GJIpUtFb6CmjVyq2VM3u71bOyR8CRihcCgMUYoDNyLXao3+70Q==
+  version "7.21.4"
+  resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.21.4.tgz#d0fa9e4413aca81f2b23b9442797bda1826edb39"
+  integrity sha512-LYvhNKfwWSPpocw8GI7gpK2nq3HSDuEPC/uSYaALSJu9xjsalaaYFOq0Pwt5KmVqwEbZlDu81aLXwBOmD/Fv9g==
   dependencies:
     "@babel/highlight" "^7.18.6"
 
 "@babel/helper-validator-identifier@^7.18.6":
   version "7.19.1"
   resolved "https://registry.yarnpkg.com/@babel/helper-validator-identifier/-/helper-validator-identifier-7.19.1.tgz#7eea834cf32901ffdc1a7ee555e2f9c27e249ca2"
   integrity sha512-awrNfaMtnHUr653GgGEs++LlAvW6w+DcPrOliSMXWCKo597CwL5Acf/wWdNkf/tfEQE3mjkeD1YOVZOUV/od1w==
@@ -131,17 +131,17 @@
   resolved "https://registry.yarnpkg.com/@hypnosphi/create-react-context/-/create-react-context-0.3.1.tgz#f8bfebdc7665f5d426cba3753e0e9c7d3154d7c6"
   integrity sha512-V1klUed202XahrWJLLOT3EXNeCpFHCcJntdFGI15ntCwau+jfT386w7OFTMaCqOgXUH1fa0w/I1oZs+i/Rfr0A==
   dependencies:
     gud "^1.0.0"
     warning "^4.0.3"
 
 "@jridgewell/gen-mapping@^0.3.0":
-  version "0.3.2"
-  resolved "https://registry.yarnpkg.com/@jridgewell/gen-mapping/-/gen-mapping-0.3.2.tgz#c1aedc61e853f2bb9f5dfe6d4442d3b565b253b9"
-  integrity sha512-mh65xKQAzI6iBcFzwv28KVWSmCkdRBWoOh+bYQGW3+6OZvbbN3TqMGo5hqYxQniRcH9F2VZIoJCm4pa3BPDK/A==
+  version "0.3.3"
+  resolved "https://registry.yarnpkg.com/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz#7e02e6eb5df901aaedb08514203b096614024098"
+  integrity sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==
   dependencies:
     "@jridgewell/set-array" "^1.0.1"
     "@jridgewell/sourcemap-codec" "^1.4.10"
     "@jridgewell/trace-mapping" "^0.3.9"
 
 "@jridgewell/resolve-uri@3.1.0":
   version "3.1.0"
@@ -150,135 +150,140 @@
 
 "@jridgewell/set-array@^1.0.1":
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/@jridgewell/set-array/-/set-array-1.1.2.tgz#7c6cf998d6d20b914c0a55a91ae928ff25965e72"
   integrity sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==
 
 "@jridgewell/source-map@^0.3.2":
-  version "0.3.2"
-  resolved "https://registry.yarnpkg.com/@jridgewell/source-map/-/source-map-0.3.2.tgz#f45351aaed4527a298512ec72f81040c998580fb"
-  integrity sha512-m7O9o2uR8k2ObDysZYzdfhb08VuEml5oWGiosa1VdaPZ/A6QyPkAJuwN0Q1lhULOf6B7MtQmHENS743hWtCrgw==
+  version "0.3.3"
+  resolved "https://registry.yarnpkg.com/@jridgewell/source-map/-/source-map-0.3.3.tgz#8108265659d4c33e72ffe14e33d6cc5eb59f2fda"
+  integrity sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==
   dependencies:
     "@jridgewell/gen-mapping" "^0.3.0"
     "@jridgewell/trace-mapping" "^0.3.9"
 
-"@jridgewell/sourcemap-codec@1.4.14", "@jridgewell/sourcemap-codec@^1.4.10":
+"@jridgewell/sourcemap-codec@1.4.14":
   version "1.4.14"
   resolved "https://registry.yarnpkg.com/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz#add4c98d341472a289190b424efbdb096991bb24"
   integrity sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==
 
+"@jridgewell/sourcemap-codec@^1.4.10":
+  version "1.4.15"
+  resolved "https://registry.yarnpkg.com/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.15.tgz#d7c6e6755c78567a951e04ab52ef0fd26de59f32"
+  integrity sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==
+
 "@jridgewell/trace-mapping@^0.3.17", "@jridgewell/trace-mapping@^0.3.9":
-  version "0.3.17"
-  resolved "https://registry.yarnpkg.com/@jridgewell/trace-mapping/-/trace-mapping-0.3.17.tgz#793041277af9073b0951a7fe0f0d8c4c98c36985"
-  integrity sha512-MCNzAp77qzKca9+W/+I0+sEpaUnZoeasnghNeVc41VZCEKaCH73Vq3BZZ/SzWIgrqE4H4ceI+p+b6C0mHf9T4g==
+  version "0.3.18"
+  resolved "https://registry.yarnpkg.com/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz#25783b2086daf6ff1dcb53c9249ae480e4dd4cd6"
+  integrity sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==
   dependencies:
     "@jridgewell/resolve-uri" "3.1.0"
     "@jridgewell/sourcemap-codec" "1.4.14"
 
 "@juggle/resize-observer@^3.3.1":
   version "3.4.0"
   resolved "https://registry.yarnpkg.com/@juggle/resize-observer/-/resize-observer-3.4.0.tgz#08d6c5e20cf7e4cc02fd181c4b0c225cd31dbb60"
   integrity sha512-dfLbk+PwWvFzSxwk3n5ySL0hfBog779o8h68wK/7/APo/7cgyWp5jcXockbxdk5kFRkbeXWm4Fbi9FrdN381sA==
 
 "@jupyter/ydoc@~0.2.3":
-  version "0.2.3"
-  resolved "https://registry.yarnpkg.com/@jupyter/ydoc/-/ydoc-0.2.3.tgz#468a88d0250c5d59800a5cc15a33df211b4b2141"
-  integrity sha512-mwmlzOYXr4StXL1ijrSkt6+Bu4cF5nZQAep2zULa5IDe/PVDBqDtMrLqZyKQOgB3IT/sLJidU1P3wTdb8bwmww==
+  version "0.2.4"
+  resolved "https://registry.yarnpkg.com/@jupyter/ydoc/-/ydoc-0.2.4.tgz#bc312f171777b58e286aadca62dadeca3a894dd1"
+  integrity sha512-QACcB4bF+Ew4UJmJP+3OyiyQm3vwRYF6iZCQK9q0nE2U5uAosQkfLyT6Bx71jPUXe4G9lEF6m9fjpZvSUX7Lyw==
   dependencies:
     "@jupyterlab/nbformat" "^3.0.0 || ^4.0.0-alpha.15"
     "@lumino/coreutils" "^1.11.0 || ^2.0.0-alpha.6"
     "@lumino/disposable" "^1.10.0 || ^2.0.0-alpha.6"
     "@lumino/signaling" "^1.10.0 || ^2.0.0-alpha.6"
     y-protocols "^1.0.5"
     yjs "^13.5.40"
 
 "@jupyterlab/application@^3.3.0":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.6.2.tgz#2920f2455484eea9a558956ce27640d18b901a51"
-  integrity sha512-yweyVTCQHfpvpxZmuBxLuGfxw30AtS4JrQGCh0P34taAbJfaYwQvzMEdK9fjvzbg8QDzIvp2lhsZZjQBjKdRzw==
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.6.3.tgz#7e199f77a4536bc7429fbecf9ba1850f51d9de52"
+  integrity sha512-G0tR6sUSCuHB8vGQnaB5lfihKNJVHtqYNoMlsZYF9rYpZEhW1TRD4uE5rg4RfDDR+GghjckQlP3rRNB2Vn4tMA==
   dependencies:
     "@fortawesome/fontawesome-free" "^5.12.0"
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/docregistry" "^3.6.2"
-    "@jupyterlab/rendermime" "^3.6.2"
-    "@jupyterlab/rendermime-interfaces" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/statedb" "^3.6.2"
-    "@jupyterlab/translation" "^3.6.2"
-    "@jupyterlab/ui-components" "^3.6.2"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
-    "@lumino/application" "^1.31.3"
+    "@lumino/application" "^1.31.4"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/apputils@^3.3.0", "@jupyterlab/apputils@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.6.2.tgz#743d46f9a002ff70cc8e487bc3b4b0375574010f"
-  integrity sha512-H0oYfIyZSI4QwZKq4X1/weoSWhKbNBKY/ikqQPrG/6KlRYhVqGtxxpRvrHVhhIa8TWQlJxVaXHoW3sbahzok0g==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/settingregistry" "^3.6.2"
-    "@jupyterlab/statedb" "^3.6.2"
-    "@jupyterlab/translation" "^3.6.2"
-    "@jupyterlab/ui-components" "^3.6.2"
+"@jupyterlab/apputils@^3.3.0", "@jupyterlab/apputils@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/apputils/-/apputils-3.6.3.tgz#bc37683142b281e21d22a2f4698634563658298e"
+  integrity sha512-um2Aaa5fOUwHFpAqKTDA+MFpnAldzOILIi5QsKOWRxiJA2W8x+hlg5HvHbq+eSWuWEU3ah15M7htzBcL3g9d4Q==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/settingregistry" "^3.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     "@types/react" "^17.0.0"
     react "^17.0.1"
     react-dom "^17.0.1"
     sanitize-html "~2.7.3"
     url "^0.11.0"
 
-"@jupyterlab/attachments@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/attachments/-/attachments-3.6.2.tgz#b9b59efe25dc043871e4d2110b6ed2847c9cc495"
-  integrity sha512-7gQPjD14DpSG6Thw6Rsw6KGWtjkqpoGQdpJcf2622KnF5p1/5JLzIqHt/ioMiDRWs3ETmKLtGj1VeznNflXs3w==
-  dependencies:
-    "@jupyterlab/nbformat" "^3.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/rendermime" "^3.6.2"
-    "@jupyterlab/rendermime-interfaces" "^3.6.2"
+"@jupyterlab/attachments@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/attachments/-/attachments-3.6.3.tgz#f2e52c3518d3f84cb7a7cc7c8a113f49dfdde4f1"
+  integrity sha512-ZYDJjcoExmojsGkX5f1WVFfW39XJcb7CtfzFcNz3AbytebRK13S1xqCRlef/TFW+XT6BG7hjMSJlpW3GdkCV1Q==
+  dependencies:
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
 "@jupyterlab/builder@^3.3.0":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.6.2.tgz#910727b6daa881b1a9cc563362c973f5bd91e142"
-  integrity sha512-xn6zej5slJLoB6bldq7F+F2FAue5mQQ9djVtmcLuLxyhR8lPSaDqVkfCnHp62XlFxwOFm4YIMCV4ip6W8ug/Fw==
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.6.3.tgz#a4b22efe34e9598b84122ff10509d3d890017b6a"
+  integrity sha512-oY1a/r75RMoPzhSmuVu+DfjL0cKk1ceHTniZsM2wPuhjjyoF875u6CDzArJatpOOuTgLm7CY5OcU3LCIK1OAgg==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
-    "@lumino/application" "^1.31.3"
+    "@lumino/application" "^1.31.4"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     ajv "^6.12.3"
     commander "~6.0.0"
     css-loader "^5.0.1"
     duplicate-package-checker-webpack-plugin "^3.0.0"
     file-loader "~6.0.0"
     fs-extra "^9.0.1"
     glob "~7.1.6"
@@ -295,386 +300,386 @@
     to-string-loader "^1.1.6"
     url-loader "~4.1.0"
     webpack "^5.41.1"
     webpack-cli "^4.1.0"
     webpack-merge "^5.1.2"
     worker-loader "^3.0.2"
 
-"@jupyterlab/cells@^3.3.3", "@jupyterlab/cells@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/cells/-/cells-3.6.2.tgz#d48b03cb17a59d4a41b6492d83c5131db30984fe"
-  integrity sha512-bs+TMCEpV4HtlT2BEcxD9IA+IKM8Tefo9DXMoHO8L7uX6k4Je54imJRuQCI9K9cPTw06GIV8YRkAJw+kjwtePA==
+"@jupyterlab/cells@^3.3.3", "@jupyterlab/cells@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/cells/-/cells-3.6.3.tgz#ac8191f99923a004211725435d25280347794cff"
+  integrity sha512-o3Uydof6bZ6HGSRgSm6isuAhaqYVmv+ozsmADYNmIGbwwwC+eb391Cv+rC3kuPZX/+2UhhO6s7fqFxW8aHUDkg==
   dependencies:
     "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/attachments" "^3.6.2"
-    "@jupyterlab/codeeditor" "^3.6.2"
-    "@jupyterlab/codemirror" "^3.6.2"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/filebrowser" "^3.6.2"
-    "@jupyterlab/nbformat" "^3.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/outputarea" "^3.6.2"
-    "@jupyterlab/rendermime" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/ui-components" "^3.6.2"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/attachments" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/codemirror" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/filebrowser" "^3.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/outputarea" "^3.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     marked "^4.0.17"
     react "^17.0.1"
 
-"@jupyterlab/codeeditor@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.6.2.tgz#f9c02b78c3e30e4a54e148749f797b149b09c880"
-  integrity sha512-lLk3adJSx5XHuS1x8ZHAluZU98T/TsZEHkGhwnlWBoXooLnukieS3azAXWhjXaeM6RAXpd7tlDwq+kQLESoz3g==
+"@jupyterlab/codeeditor@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codeeditor/-/codeeditor-3.6.3.tgz#a889c1821001888af7b60f66b1ee91e15797c0bb"
+  integrity sha512-SnVo5KDhyRkK/o1SDRX9nehLEAMaOBFf+GUx2jeXBTfr6wTKcwDBnJAUwlOfncwRlMV79aUIqTIcS861FSXDyA==
   dependencies:
     "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/nbformat" "^3.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/translation" "^3.6.2"
-    "@jupyterlab/ui-components" "^3.6.2"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/codemirror@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.6.2.tgz#9cdded7a86c56785d25128878243d1c9aa08081a"
-  integrity sha512-qCPKmtR2h8trPx/8HI8Mopwg7ZSNnyZqaMVy+M9YBdqiD+42iAHtnuzR2Q9lqlU0yxDBnukmlUeABh69voNaYg==
+"@jupyterlab/codemirror@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/codemirror/-/codemirror-3.6.3.tgz#7cb19faae58d4fc26bc37064f029c4b17098c20a"
+  integrity sha512-VU5bInzSqsyPGZkEd/w6HtJ9PSw7U5twoyrQSpSM+E2SEYWskaBZOHJf8XNunVoRRKwSvDLyxSs07Ot6zUlA0w==
   dependencies:
     "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/codeeditor" "^3.6.2"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/nbformat" "^3.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/statusbar" "^3.6.2"
-    "@jupyterlab/translation" "^3.6.2"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     codemirror "~5.61.0"
     react "^17.0.1"
     y-codemirror "^3.0.1"
 
-"@jupyterlab/coreutils@^5.6.2":
-  version "5.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.2.tgz#3c01491037e7a8eadf3b52176a772e856c9681ef"
-  integrity sha512-Iy0+A4TCFbcW7IGpPWK1bk7yB/FzFLGLGSreMlQ/jlyU3Y/8ik9Ui6ZpPXkLUW0lXj7zmWhQu6aq2O4gPbkL3A==
+"@jupyterlab/coreutils@^5.6.3":
+  version "5.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.3.tgz#3b0b5d481b14596158b560336833c89be509e84e"
+  integrity sha512-jRVTpwGzP9wBNYuaZTip89FS1qbeSYrEO2qdNVdW2rs0mQHcIlu3Fkv5muMFmKYGi0XHhG3UhZiWQ7qiPw2svQ==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     minimist "~1.2.0"
     moment "^2.24.0"
     path-browserify "^1.0.0"
     url-parse "~1.5.1"
 
-"@jupyterlab/docmanager@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.6.2.tgz#690f3d5c23b659f63e3239a32a64e6e9f8130926"
-  integrity sha512-BrN9HIURZ3iuzHq0p3nTTQThRREx2gAAsuYspq/HhVGdEvyOpdByMlPUbOgUrf/ytok9Tyo14gJBfgXAZ7yUFA==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/docprovider" "^3.6.2"
-    "@jupyterlab/docregistry" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/statusbar" "^3.6.2"
-    "@jupyterlab/translation" "^3.6.2"
+"@jupyterlab/docmanager@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docmanager/-/docmanager-3.6.3.tgz#df2c5b45c5e9b38e2a48eb703ff5e3a9b4b7860c"
+  integrity sha512-4d5zGE3SGbg58wsFJtyskUxK7dEvl8d5Wh90hTlmsFNmr+nh5duTWcqTQ/a+d76YxYbGhH5vqOsNm5ORZq4Umw==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docprovider" "^3.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/docprovider@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.6.2.tgz#64fe1651b8929aa5dacb4be4ad1e8ebc6c621997"
-  integrity sha512-szjBu/k33oX6rdu6qvEAIzzqrRhGleJ/6qpOaVwguTY25HmmVWFwJAFhANiZQdt+u5LOTXGoS2hz09yUWjm52g==
+"@jupyterlab/docprovider@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docprovider/-/docprovider-3.6.3.tgz#90fbf07214b6c3e98055787fc351a68e9d83470c"
+  integrity sha512-M5IoyykDpWnUFNePHz3+fi/RNvV92UNbQGfAvsaCMSn+fl48rD4rHB9EZGceOisb3m1U+E4SntKYI3pl49yUEg==
   dependencies:
     "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/translation" "^3.6.2"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     y-protocols "^1.0.5"
     y-websocket "^1.4.6"
 
-"@jupyterlab/docregistry@^3.3.0", "@jupyterlab/docregistry@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.6.2.tgz#b7bbd6c5e275bf0107245a5cc0d795619bcbc756"
-  integrity sha512-f1qr72AfIhi2TnI+JkAou6SG3fnHUtyinq3WrWLN9C85kmKua4hLkVM5NaECDJROOFQ/jO+2Yn24eH2tHBhSkw==
+"@jupyterlab/docregistry@^3.3.0", "@jupyterlab/docregistry@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/docregistry/-/docregistry-3.6.3.tgz#4a03fbb704449bda7a94df7a4bd63078c11aef58"
+  integrity sha512-unDMrtCSGKPqX9uvYCkI7zGTvskuC9odAPIHPsYSVMcHL/o5M7lQkHmRZCoSIezfe5OvPGXbYT2boQrBKXqCFw==
   dependencies:
     "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/codeeditor" "^3.6.2"
-    "@jupyterlab/codemirror" "^3.6.2"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/docprovider" "^3.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/rendermime" "^3.6.2"
-    "@jupyterlab/rendermime-interfaces" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/translation" "^3.6.2"
-    "@jupyterlab/ui-components" "^3.6.2"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/codemirror" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docprovider" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/filebrowser@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/filebrowser/-/filebrowser-3.6.2.tgz#b9b66948feb4568ed60b384c0851393d154d301d"
-  integrity sha512-/s+p+Wk/RerlSKfnTbBf2SUlOgMo/cf7i9SWMB12gJxjJyK1E5ja1eNn7cdNORukjCG5mLPFK5+NR/aAIRVxsg==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/docmanager" "^3.6.2"
-    "@jupyterlab/docregistry" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/statedb" "^3.6.2"
-    "@jupyterlab/statusbar" "^3.6.2"
-    "@jupyterlab/translation" "^3.6.2"
-    "@jupyterlab/ui-components" "^3.6.2"
+"@jupyterlab/filebrowser@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/filebrowser/-/filebrowser-3.6.3.tgz#169b880e19a8686f9a669a750027c2817b4b6cef"
+  integrity sha512-Qu+Mtx3d0QY7qCMIxg5nQtkQYh+kZ2kGO7tgS+yfKjo0cluPsxo+Zr56KtJU6zyDYjylVCtLYIK2RflwRKhdng==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docmanager" "^3.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
 "@jupyterlab/mainmenu@^3.4.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.6.2.tgz#30d8a59fd716d8f6ee5e3712f883a56392e0a232"
-  integrity sha512-pnMLAQookw5GOPpD7cgu0HuDIZirJ62xuHAkxOS1o++BkoE7VYZlrNCFz+jzlRoXiwbf+bKPw5WU0/xHcpvwqA==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/translation" "^3.6.2"
-    "@jupyterlab/ui-components" "^3.6.2"
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.6.3.tgz#5d322db9b8d742b7042109ab7e8c733696ae38fc"
+  integrity sha512-ohZzHDeReKX3zbLz2bUsYRSdkX6bVhNoCer3Rat8gjfb8vr/bqK9ReAvvoA4rRqm0mrfqwotpZSzbE4+y5KqZA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15", "@jupyterlab/nbformat@^3.3.3", "@jupyterlab/nbformat@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.2.tgz#fc51917e04c2671c8929d38980795a4928f14282"
-  integrity sha512-I4B4jo5Vnlfr94Nzc82wt8OYYeGvNAp6NPRjUWuUDdoUDKE6V2Wz+N3HCf9atLBy0Ervc8rrDqpE18eJLUCUGg==
+"@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15", "@jupyterlab/nbformat@^3.3.3", "@jupyterlab/nbformat@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.3.tgz#8520338e3679cbe8ce2ea8eb5a9b816f8b774ad3"
+  integrity sha512-0qJLa4dtOmu9EmHFeM7gaZi4qheovIPc9ZrgGGRuG0obajs4YYlvh4MQvCSgpVhme4AuBfGlcfzhlx+Gbzr5Xw==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
 
 "@jupyterlab/notebook@^3.3.0":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/notebook/-/notebook-3.6.2.tgz#df741fb4b3955131e6c811a3fe753311169db0b8"
-  integrity sha512-ArX5pm4cGyAcMWWLT8PYylFAqrF/rVY8+Rovk/maRydteTQ36fMZLgKnW5v+k1g8wQVeAcxM4G4gYnRQ8BkHng==
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/notebook/-/notebook-3.6.3.tgz#1584be72184d67d59291e2b22f55bc257afde436"
+  integrity sha512-id1KD5/9IDPr/IZFCl/YX4Vc+Q198LZshhFNEcVJZcRdjD7Vh+LGvWcLOh80OAv86J4XSTTAsp3gHPr4iSwPDg==
   dependencies:
     "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/cells" "^3.6.2"
-    "@jupyterlab/codeeditor" "^3.6.2"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/docregistry" "^3.6.2"
-    "@jupyterlab/nbformat" "^3.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/rendermime" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/settingregistry" "^3.6.2"
-    "@jupyterlab/statusbar" "^3.6.2"
-    "@jupyterlab/translation" "^3.6.2"
-    "@jupyterlab/ui-components" "^3.6.2"
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/cells" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/docregistry" "^3.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/settingregistry" "^3.6.3"
+    "@jupyterlab/statusbar" "^3.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/domutils" "^1.8.0"
     "@lumino/dragdrop" "^1.13.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/observables@^4.6.2":
-  version "4.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.2.tgz#b12ad9938bb337c2fa34bc4adacb7600210930ba"
-  integrity sha512-MEymiTUzmBGfqw4Jd+NhemYNcbX2Wv38G63Oy4rFW+MEZIX/3Rwf2KigVhrq80dfxHV3/BRXcAj0bVY+pboswg==
+"@jupyterlab/observables@^4.6.3":
+  version "4.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.3.tgz#49a9ca49fbda7428abbd1bfb8a4006ecd406c18d"
+  integrity sha512-CvQoL+9WHXOy/CXp/PQLi4c5iZVJ4psz11+GrycDDinX1AdVQ8a43OLTC0gxWl3Tk2C8ZvAi1sgn4FS68E1ACQ==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/outputarea@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.6.2.tgz#5f21aedbcb78100444dfdcc79ac74ffcde169784"
-  integrity sha512-yPq4zRnbT9OMRHSwI1flGCSswmIJXZq6vnWdEVpCm20GJZ5xYI51XijXxgbrmhkFh13UCKRlu/TLr6tmSaWI7A==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/nbformat" "^3.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/rendermime" "^3.6.2"
-    "@jupyterlab/rendermime-interfaces" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
+"@jupyterlab/outputarea@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/outputarea/-/outputarea-3.6.3.tgz#acf7a604eb352109d096d2a9fdd1fbbddbf80af1"
+  integrity sha512-SSmkDWS8MhdXl7+rQoLu/5wJBKTq1YEkxlQcKh1Z0VN4VjYDCA/bKFGjOmKN7wMmoVP/zRmWvUwl/DLJCHx/Tw==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime" "^3.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     resize-observer-polyfill "^1.5.1"
 
-"@jupyterlab/rendermime-interfaces@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.6.2.tgz#7844a3e23c3af12fb5a83c3e6bbe0951e861d0da"
-  integrity sha512-vWpAd7+KriSkzamcbP3IjJmt1dj1oMcbZMM7cgqfh+czzwDTakZZDareqw36tBDaqPQuCpcbpsCxDjEAci+uRw==
+"@jupyterlab/rendermime-interfaces@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.6.3.tgz#80009705d5ded65a4b27c4b826b295f40f126902"
+  integrity sha512-VHZVnqB0K1nmoQMOhFGHwvSYMQmxqcOC3wWDRFeUOv8S+tejTYfbrKXPOZJvhdGB52Jn8XNIesXOuNpLhl4HmQ==
   dependencies:
-    "@jupyterlab/translation" "^3.6.2"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
 
-"@jupyterlab/rendermime@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.2.tgz#28663ae8749055cc1f75d3a7e51f79c1df444b5f"
-  integrity sha512-MeUxOioXMESN4iA1uVIWSV+INjTz50CNq7W7IP3SNOWd/GM3ieLXCKtewG3HuMJPFbH0ifB0IfD5+MEP1z51cA==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/codemirror" "^3.6.2"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/nbformat" "^3.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/rendermime-interfaces" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/translation" "^3.6.2"
+"@jupyterlab/rendermime@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.3.tgz#48d83c70493b0356d4dac6d89a863d8a5a84f68e"
+  integrity sha512-w3e38OddJin9fbfe7EWsKiiup/0ayvHPrAsacde8PqGLvi/sLeAXT98PqihsKt8EAlOgXSkSO0Ivjbd0JzgGgA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codemirror" "^3.6.3"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/rendermime-interfaces" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     lodash.escape "^4.0.1"
     marked "^4.0.17"
 
-"@jupyterlab/services@^6.4.3", "@jupyterlab/services@^6.6.2":
-  version "6.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.2.tgz#81d75113e436bd5d63b0e7784f1ac465775c6d18"
-  integrity sha512-yuI4C2ZPFrJ5h4DzM6t2ue255gkpAbNFtDlUDCcaJv3dfuaAJdsU9uhkfcfTEMdr0thMXCUpb/svr3QHDabe3w==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/nbformat" "^3.6.2"
-    "@jupyterlab/observables" "^4.6.2"
-    "@jupyterlab/settingregistry" "^3.6.2"
-    "@jupyterlab/statedb" "^3.6.2"
+"@jupyterlab/services@^6.4.3", "@jupyterlab/services@^6.6.3":
+  version "6.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.3.tgz#303938e5dc5aebce7a86324a64ed89c25c61c9e7"
+  integrity sha512-BxEOMRl9X18T5wY7iV6ZJhARnibFghpD3OruqeSbnGdbRv6XJi8prsRbCQQ6Mf9agvf81B20KmDvYKikPHC0xQ==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/nbformat" "^3.6.3"
+    "@jupyterlab/observables" "^4.6.3"
+    "@jupyterlab/settingregistry" "^3.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     node-fetch "^2.6.0"
     ws "^7.4.6"
 
-"@jupyterlab/settingregistry@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.2.tgz#1a98315dafa80b8b0166ed36d9e4cbba0af054a6"
-  integrity sha512-kAOzuuZOXQWs7UxyvgsK6rDwRLF26HiCpUdjbEQwobmQUVysXB+t6YRG2wYTuz3cMVlWn52gj3Nvi81P+7xPdA==
+"@jupyterlab/settingregistry@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.3.tgz#642f8b6449d626821ef13a7e778ae716fa8331c9"
+  integrity sha512-pnzIge0ZC8V63R97HiNroJ0eaPM0DN6x65SStyLuv/K8Qez4XqpOdc0Wfell5ri5mxMvm1qKekuFeTikqSXQKQ==
   dependencies:
-    "@jupyterlab/statedb" "^3.6.2"
+    "@jupyterlab/statedb" "^3.6.3"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     ajv "^6.12.3"
     json5 "^2.1.1"
 
-"@jupyterlab/statedb@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.2.tgz#ac70d7e11da3ea7215d08496258a073f8b7aefdb"
-  integrity sha512-xJ30zIuUHHU2UFULCI6VvWHwZrtN1cib/+o7V/REnPWWWqWEmn7TTi3lyzRg8zPtaKcUkVjtKv85QRnxZF3Pug==
+"@jupyterlab/statedb@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.3.tgz#6ba2166af9232c9a185cf0077cf1272f24cc9a69"
+  integrity sha512-A36L+0NN8f0WOES2GdtZjp9uFuC7IBjhKiO/RlKRX5AFjNxoJ9oO3PZtoxJQYPnGBljMqVdRa+m9aYEfvKhYyQ==
   dependencies:
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/statusbar@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.6.2.tgz#5a8f65e53da6e89c279119af5f93d3fe688872c6"
-  integrity sha512-lXlaVi9CvPs9+6viwQ9HEMET38Je5vtMyf8PqZVbE75NAdZoyU/635NOpP3dd/cuUk+VTSzOomocRCWtdtaDVQ==
-  dependencies:
-    "@jupyterlab/apputils" "^3.6.2"
-    "@jupyterlab/codeeditor" "^3.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/translation" "^3.6.2"
-    "@jupyterlab/ui-components" "^3.6.2"
+"@jupyterlab/statusbar@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statusbar/-/statusbar-3.6.3.tgz#29c24427a2d6b205349b94583de0ccb8b9435d88"
+  integrity sha512-m59NLR0Zghm53PU6hDzRF4XVORnJx/YRx0svcjj/TGLk8LSffpQbUDBy24dl3tOuChk4D5cCdgeDH1X30TzCaA==
+  dependencies:
+    "@jupyterlab/apputils" "^3.6.3"
+    "@jupyterlab/codeeditor" "^3.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/translation" "^3.6.3"
+    "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     csstype "~3.0.3"
     react "^17.0.1"
     typestyle "^2.0.4"
 
-"@jupyterlab/translation@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.6.2.tgz#f10a2c61e1515466290c0cfe655d96a65589e7ae"
-  integrity sha512-hAV/2tfCwYcIld4B//L1t7inkWOPmg9VYTqBau2kSz7Lz62924RU+caEpDwiVHXWedn396kt7ugEotWg7FO22w==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/services" "^6.6.2"
-    "@jupyterlab/statedb" "^3.6.2"
+"@jupyterlab/translation@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/translation/-/translation-3.6.3.tgz#3fd95f726316762bc1799a7b7be0243d5465932a"
+  integrity sha512-m+wwBv/hiN5Y6Sb7Ij150ZhPXZdhN5wI8CT3afnzARwKr2Aww5AIURO3upmMwnKaPVQTrWqsS3+7bZS/21JuJA==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/services" "^6.6.3"
+    "@jupyterlab/statedb" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/ui-components@^3.6.2":
-  version "3.6.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.6.2.tgz#8d4c95153ae082b001349d0c57f5f6fa40009d28"
-  integrity sha512-itOGQDyNVl9kqDxRAAH8Z6BJoc2x4jqfLRdia7eWwHAed+1dtSkf0VedEEHyjgAglv17Yvbg9xwWxLeQ5EJlBw==
+"@jupyterlab/ui-components@^3.6.3":
+  version "3.6.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/ui-components/-/ui-components-3.6.3.tgz#36555036b383c5d80346f409a7a168d13c9d8c85"
+  integrity sha512-XzseUo2IXclPlYcGxCIz8evjWF+dCBMmbJlvoE5OF29BYBvI5N/DUaTem8bHN5kmQwHIXX6BImHu7rbC9Xjl6w==
   dependencies:
     "@blueprintjs/core" "^3.36.0"
     "@blueprintjs/select" "^3.15.0"
-    "@jupyterlab/coreutils" "^5.6.2"
-    "@jupyterlab/translation" "^3.6.2"
+    "@jupyterlab/coreutils" "^5.6.3"
+    "@jupyterlab/translation" "^3.6.3"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.1"
+    "@lumino/widgets" "^1.37.2"
     "@rjsf/core" "^3.1.0"
     react "^17.0.1"
     react-dom "^17.0.1"
     typestyle "^2.0.4"
 
 "@lumino/algorithm@^1.9.0", "@lumino/algorithm@^1.9.2":
   version "1.9.2"
@@ -682,15 +687,15 @@
   integrity sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==
 
 "@lumino/algorithm@^2.0.0":
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-2.0.0.tgz#f36e4b6bf6d2b9bde66dc3162afc9a0d2ef47530"
   integrity sha512-SwM/8U1zlMWMJj00wTCThdTUit9zap2Xghuo4uUxvZ+mfog5b1UIk2j1dP8TPpzEXHCDPEb85s2/ERo1tee3Dw==
 
-"@lumino/application@^1.31.3":
+"@lumino/application@^1.31.4":
   version "1.31.4"
   resolved "https://registry.yarnpkg.com/@lumino/application/-/application-1.31.4.tgz#b804fcc46fb77deb41aee94c48bea990f735d6b9"
   integrity sha512-dOSsDJ1tXOxC3fnSHvtDQK5RcICLEVPtO19HeCGwurb5W2ZZ55SZT2b5jZu6V/v8lGdtkNbr1RJltRpJRSRb/A==
   dependencies:
     "@lumino/commands" "^1.21.1"
     "@lumino/coreutils" "^1.12.1"
     "@lumino/widgets" "^1.37.2"
@@ -716,33 +721,33 @@
     "@lumino/virtualdom" "^1.14.3"
 
 "@lumino/coreutils@^1.11.0", "@lumino/coreutils@^1.12.1":
   version "1.12.1"
   resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-1.12.1.tgz#79860c9937483ddf6cda87f6c2b9da8eb1a5d768"
   integrity sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==
 
-"@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^2.0.0":
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.0.0.tgz#f7a82e616156bda83197ee4e176810af6799a27b"
-  integrity sha512-eMPssdjM/qYsX7AwX4gWI07ijzxDFyM7i8dT35YY7P6r0OeqIzmVruu/3RJhHfKoVJ/fINlS9B8EsOC81GMIGA==
+"@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^2.1.0":
+  version "2.1.0"
+  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.1.0.tgz#291ed11a1bd143bfd5a2f2638cfb27aefd1bd9ba"
+  integrity sha512-1pF3gaTxZY6P+Tixs2rd1aj5HgFOdH3RNupgsMaq0sFmxuvuSxaYhiK5/LB9evDN8a6HqHFeS6wVhVajSOJfDQ==
 
 "@lumino/disposable@^1.10.0", "@lumino/disposable@^1.10.4", "@lumino/disposable@^1.4.3":
   version "1.10.4"
   resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-1.10.4.tgz#73b452044fecf988d7fa73fac9451b1a7f987323"
   integrity sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/signaling" "^1.11.1"
 
 "@lumino/disposable@^1.10.0 || ^2.0.0-alpha.6":
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-2.0.0.tgz#6ad4927aaee03b8c55b870a8466fca5b759d5a1e"
-  integrity sha512-2PcwxbKU1xYd02wWCsk5F/Ufh/tbNAMb+zXJEOGcRPrgOihkIz3FEDtbhOVGuGw8FtYlisKIs1m+pq37LUHL6A==
+  version "2.1.0"
+  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-2.1.0.tgz#54dfd2e8f361570b08751784b80751056816c66f"
+  integrity sha512-BFSNoNKxdX/qpN8cvL+5/I3MErzBUZYlqLuURSp4aTnqkVg4fYVOUo3E8fD/V9zQRu9pX0WzgTl8H0w0uVK6Gg==
   dependencies:
-    "@lumino/signaling" "^2.0.0"
+    "@lumino/signaling" "^2.1.0"
 
 "@lumino/domutils@^1.8.0", "@lumino/domutils@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/domutils/-/domutils-1.8.2.tgz#d15cdbae12bea52852bbc13c4629360f9f05b7f5"
   integrity sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==
 
 "@lumino/dragdrop@^1.13.0", "@lumino/dragdrop@^1.14.5":
@@ -784,30 +789,30 @@
   version "1.11.1"
   resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-1.11.1.tgz#438f447a1b644fd286549804f9851b5aec9679a2"
   integrity sha512-YCUmgw08VoyMN5KxzqPO3KMx+cwdPv28tAN06C0K7Q/dQf+oufb1XocuhZb5selTrTmmuXeizaYxgLIQGdS1fA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/properties" "^1.8.2"
 
-"@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^2.0.0":
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-2.0.0.tgz#56ad85d966719adde7532c2888f3c73562de5c86"
-  integrity sha512-v5VRG4asmrVV5yy9rrpZgS5s9djkLbnmI60dVFXIbMWKyNUziVaUB9SkMzsCOOF6b9IKxXVdrMxjcieX7F9qfA==
+"@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^2.1.0":
+  version "2.1.0"
+  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-2.1.0.tgz#82bddad7e074e757b5c9b5e0822278115f81beec"
+  integrity sha512-Vk2qPmuYn7TdEiqn/bmIrLNBaLmcuB09s+cI8FOxyEZvuW92fGP5P5H2C0rgqy9OT1mvZqobhkEvcCav8HdxxA==
   dependencies:
     "@lumino/algorithm" "^2.0.0"
-    "@lumino/coreutils" "^2.0.0"
+    "@lumino/coreutils" "^2.1.0"
 
 "@lumino/virtualdom@^1.14.0", "@lumino/virtualdom@^1.14.3":
   version "1.14.3"
   resolved "https://registry.yarnpkg.com/@lumino/virtualdom/-/virtualdom-1.14.3.tgz#e490c36ff506d877cf45771d6968e3e26a8919fd"
   integrity sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
 
-"@lumino/widgets@^1.37.1", "@lumino/widgets@^1.37.2":
+"@lumino/widgets@^1.37.2":
   version "1.37.2"
   resolved "https://registry.yarnpkg.com/@lumino/widgets/-/widgets-1.37.2.tgz#b408fae221ecec2f1b028607782fbe1e82588bce"
   integrity sha512-NHKu1NBDo6ETBDoNrqSkornfUCwc8EFFzw6+LWBfYVxn2PIwciq2SdiJGEyNqL+0h/A9eVKb5ui5z4cwpRekmQ==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/commands" "^1.21.1"
     "@lumino/coreutils" "^1.12.1"
@@ -889,23 +894,18 @@
   version "8.37.0"
   resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.37.0.tgz#29cebc6c2a3ac7fea7113207bf5a828fdf4d7ef1"
   integrity sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ==
   dependencies:
     "@types/estree" "*"
     "@types/json-schema" "*"
 
-"@types/estree@*":
-  version "1.0.0"
-  resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.0.tgz#5fb2e536c1ae9bf35366eed879e827fa59ca41c2"
-  integrity sha512-WulqXMDUTYAXCjZnk6JtIHPigp55cVtDgDrO2gHRwhyJto21+1zbVCtOYB2L1F9w4qCQ0rOGWBnBe0FNTiEJIQ==
-
-"@types/estree@^0.0.51":
-  version "0.0.51"
-  resolved "https://registry.yarnpkg.com/@types/estree/-/estree-0.0.51.tgz#cfd70924a25a3fd32b218e5e420e6897e1ac4f40"
-  integrity sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==
+"@types/estree@*", "@types/estree@^1.0.0":
+  version "1.0.1"
+  resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.1.tgz#aa22750962f3bf0e79d753d3cc067f010c95f194"
+  integrity sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==
 
 "@types/json-schema@*", "@types/json-schema@^7.0.5", "@types/json-schema@^7.0.7", "@types/json-schema@^7.0.8":
   version "7.0.11"
   resolved "https://registry.yarnpkg.com/@types/json-schema/-/json-schema-7.0.11.tgz#d421b6c527a3037f7c84433fd2c4229e016863d3"
   integrity sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==
 
 "@types/minimist@^1.2.0":
@@ -935,17 +935,17 @@
 
 "@types/prop-types@*":
   version "15.7.5"
   resolved "https://registry.yarnpkg.com/@types/prop-types/-/prop-types-15.7.5.tgz#5f19d2b85a98e9558036f6a3cacc8819420f05cf"
   integrity sha512-JCB8C6SnDoQf0cNycqd/35A7MjcnK+ZTqE7judS6o7utxUCg6imJg3QK2qzHKszlTjcj2cn+NwMB2i96ubpj7w==
 
 "@types/react@^17.0.0":
-  version "17.0.55"
-  resolved "https://registry.yarnpkg.com/@types/react/-/react-17.0.55.tgz#f94eac1a37929cd86d1cc084c239c08dcfd10e5f"
-  integrity sha512-kBcAhmT8RivFDYxHdy8QfPKu+WyfiiGjdPb9pIRtd6tj05j0zRHq5DBGW5Ogxv5cwSKd93BVgUk/HZ4I9p3zNg==
+  version "17.0.58"
+  resolved "https://registry.yarnpkg.com/@types/react/-/react-17.0.58.tgz#c8bbc82114e5c29001548ebe8ed6c4ba4d3c9fb0"
+  integrity sha512-c1GzVY97P0fGxwGxhYq989j4XwlcHQoto6wQISOC2v6wm3h0PORRWJFHlkRjfGsiG3y1609WdQ+J+tKxvrEd6A==
   dependencies:
     "@types/prop-types" "*"
     "@types/scheduler" "*"
     csstype "^3.0.2"
 
 "@types/scheduler@*":
   version "0.16.3"
@@ -1461,17 +1461,17 @@
 
 camelcase@^5.3.1:
   version "5.3.1"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-5.3.1.tgz#e3c9b31569e106811df242f715725a1f4c494320"
   integrity sha512-L28STB170nwWS63UjtlEOE3dldQApaJXZkOI1uMFfzf3rRuPegHaHesyee+YxQ+W6SvRDQV6UrdOdRiR153wJg==
 
 caniuse-lite@^1.0.30001449:
-  version "1.0.30001473"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001473.tgz#3859898b3cab65fc8905bb923df36ad35058153c"
-  integrity sha512-ewDad7+D2vlyy+E4UJuVfiBsU69IL+8oVmTuZnH5Q6CIUbxNfI50uVpRHbUPDD6SUaN2o0Lh4DhTrvLG/Tn1yg==
+  version "1.0.30001480"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001480.tgz#9bbd35ee44c2480a1e3a3b9f4496f5066817164a"
+  integrity sha512-q7cpoPPvZYgtyC4VaBSN0Bt+PJ4c4EYRf0DrduInOz2SkFpHD5p3LnvEpqBp7UnJn+8x1Ogl1s38saUxe+ihQQ==
 
 chalk@^2.0.0, chalk@^2.3.0, chalk@^2.4.1:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
@@ -1546,17 +1546,17 @@
 
 colord@^2.9.3:
   version "2.9.3"
   resolved "https://registry.yarnpkg.com/colord/-/colord-2.9.3.tgz#4f8ce919de456f1d5c1c368c307fe20f3e59fb43"
   integrity sha512-jeC1axXpnb0/2nn/Y1LPuLdgXBLH7aDcHu4KEKfqw3CUhX7ZpfBSlPKyqXE6btIgEzfWtrX3/tyBCaCvXvMkOw==
 
 colorette@^2.0.14:
-  version "2.0.19"
-  resolved "https://registry.yarnpkg.com/colorette/-/colorette-2.0.19.tgz#cdf044f47ad41a0f4b56b3a0d5b4e6e1a2d5a798"
-  integrity sha512-3tlv/dIP7FWvj3BsbHrGLJ6l/oKh1O3TcgBqMn+yyCagOxc23fyzDS6HypQbgxWbkpDnf52p1LuR4eWDQ/K9WQ==
+  version "2.0.20"
+  resolved "https://registry.yarnpkg.com/colorette/-/colorette-2.0.20.tgz#9eb793e6833067f7235902fcd3b09917a000a95a"
+  integrity sha512-IfEDxwoWIjkeXL1eXcDiow4UbKjhLdq6/EuSVR9GMN7KVH3r9gQ83e73hsz1Nd1T3ijd5xv1wcWRYO+D6kCI2w==
 
 commander@^2.20.0:
   version "2.20.3"
   resolved "https://registry.yarnpkg.com/commander/-/commander-2.20.3.tgz#fd485e84c03eb4881c20722ba48035e8531aeb33"
   integrity sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==
 
 commander@^7.0.0:
@@ -1595,17 +1595,17 @@
 
 concat-map@0.0.1:
   version "0.0.1"
   resolved "https://registry.yarnpkg.com/concat-map/-/concat-map-0.0.1.tgz#d8a96bd77fd68df7793a73036a3ba0d5405d477b"
   integrity sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==
 
 core-js-pure@^3.6.5:
-  version "3.29.1"
-  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.29.1.tgz#1be6ca2b8772f6b4df7fc4621743286e676c6162"
-  integrity sha512-4En6zYVi0i0XlXHVz/bi6l1XDjCqkKRq765NXuX+SnaIatlE96Odt5lMLjdxUiNI1v9OXI5DSLWYPlmTfkTktg==
+  version "3.30.1"
+  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.30.1.tgz#7d93dc89e7d47b8ef05d7e79f507b0e99ea77eec"
+  integrity sha512-nXBEVpmUnNRhz83cHd9JRQC52cTMcuXAmR56+9dSMpRdpeA4I1PX6yjmhd71Eyc/wXNsdBdUDIj1QTIeZpU5Tg==
 
 cosmiconfig@^7.1.0:
   version "7.1.0"
   resolved "https://registry.yarnpkg.com/cosmiconfig/-/cosmiconfig-7.1.0.tgz#1443b9afa596b670082ea46cbd8f6a62b84635f6"
   integrity sha512-AdmX6xUzdNASswsFtmwSt7Vj8po9IuqXm0UXz7QKPuEUmPB4XyjGfaAr2PSuELMwkRMVH1EpIkX5bTZGRB3eCA==
   dependencies:
     "@types/parse-json" "^4.0.0"
@@ -1662,17 +1662,17 @@
 
 csstype@3.0.10:
   version "3.0.10"
   resolved "https://registry.yarnpkg.com/csstype/-/csstype-3.0.10.tgz#2ad3a7bed70f35b965707c092e5f30b327c290e5"
   integrity sha512-2u44ZG2OcNUO9HDp/Jl8C07x6pU/eTR3ncV91SiK3dhG9TWvRVsCoJw14Ckx5DgWkzGA3waZWO3d7pgqpUI/XA==
 
 csstype@^3.0.2:
-  version "3.1.1"
-  resolved "https://registry.yarnpkg.com/csstype/-/csstype-3.1.1.tgz#841b532c45c758ee546a11d5bd7b7b473c8c30b9"
-  integrity sha512-DJR/VvkAvSZW9bTouZue2sSxDwdTN92uHjqeKVm+0dAqdfNykRzQ95tay8aXMBAAPpUiq4Qcug2L7neoRh2Egw==
+  version "3.1.2"
+  resolved "https://registry.yarnpkg.com/csstype/-/csstype-3.1.2.tgz#1d4bf9d572f11c14031f0436e1c10bc1f571f50b"
+  integrity sha512-I7K1Uu0MBPzaFKg4nI5Q7Vs2t+3gWWW648spaF+Rg7pI9ds18Ugn+lvg4SHczUdKlHI5LWBXyqfS8+DufyBsgQ==
 
 csstype@~3.0.3:
   version "3.0.11"
   resolved "https://registry.yarnpkg.com/csstype/-/csstype-3.0.11.tgz#d66700c5eacfac1940deb4e3ee5642792d85cd33"
   integrity sha512-sa6P2wJ+CAbgyy4KFssIb/JNMLxFvKF1pCYCSXS8ZMuqZnMsrxqI2E5sPyoTpxoPU/gVZMzr2zjOfg8GIZOMsw==
 
 data-urls@^2.0.0:
@@ -1730,15 +1730,15 @@
   version "5.3.0"
   resolved "https://registry.yarnpkg.com/deferred-leveldown/-/deferred-leveldown-5.3.0.tgz#27a997ad95408b61161aa69bd489b86c71b78058"
   integrity sha512-a59VOT+oDy7vtAbLRCZwWgxu2BaCfd5Hk7wxJd48ei7I+nsg8Orlb9CLG0PMZienk9BSUKgeAqkO2+Lw+1+Ukw==
   dependencies:
     abstract-leveldown "~6.2.1"
     inherits "^2.0.3"
 
-define-properties@^1.1.3, define-properties@^1.1.4:
+define-properties@^1.1.3, define-properties@^1.1.4, define-properties@^1.2.0:
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/define-properties/-/define-properties-1.2.0.tgz#52988570670c9eacedd8064f4a990f2405849bd5"
   integrity sha512-xvqAVKGfT1+UAvPwKTVw/njhdQ8ZhXK4lI0bCIuCMrp2up9nPnaDftrLtmpTazqd1o+UY4zgzU+avtMbDP+ldA==
   dependencies:
     has-property-descriptors "^1.0.0"
     object-keys "^1.1.1"
 
@@ -1805,17 +1805,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.284:
-  version "1.4.347"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.347.tgz#4b72564912c3456c6704d4250918aa6a105d5dc3"
-  integrity sha512-LNi3+/9nV0vT6Bz1OsSoZ/w7IgNuWdefZ7mjKNjZxyRlI/ag6uMXxsxAy5Etvuixq3Q26exw2fc4bNYvYQqXSw==
+  version "1.4.368"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.368.tgz#75901f97d3e23da2e66feb1e61fbb8e70ac96430"
+  integrity sha512-e2aeCAixCj9M7nJxdB/wDjO6mbYX+lJJxSJCXDzlr5YPGYVofuJwGN9nKg2o6wWInjX6XmxRinn3AeJMK81ltw==
 
 emoji-regex@^8.0.0:
   version "8.0.0"
   resolved "https://registry.yarnpkg.com/emoji-regex/-/emoji-regex-8.0.0.tgz#e818fd69ce5ccfcb404594f842963bf53164cc37"
   integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
 
 emojis-list@^3.0.0:
@@ -1908,18 +1908,18 @@
     string.prototype.trim "^1.2.7"
     string.prototype.trimend "^1.0.6"
     string.prototype.trimstart "^1.0.6"
     typed-array-length "^1.0.4"
     unbox-primitive "^1.0.2"
     which-typed-array "^1.1.9"
 
-es-module-lexer@^0.9.0:
-  version "0.9.3"
-  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-0.9.3.tgz#6f13db00cc38417137daf74366f535c8eb438f19"
-  integrity sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==
+es-module-lexer@^1.2.1:
+  version "1.2.1"
+  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-1.2.1.tgz#ba303831f63e6a394983fde2f97ad77b22324527"
+  integrity sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==
 
 es-set-tostringtag@^2.0.1:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/es-set-tostringtag/-/es-set-tostringtag-2.0.1.tgz#338d502f6f674301d710b80c8592de8a15f09cd8"
   integrity sha512-g3OMbtlwY3QewlqAiMLI47KywjWZoEytKr8pf6iTC8uJq5bIAH52Z9pnQ8pVL6whrCto53JZDuUIsifGeLorTg==
   dependencies:
     get-intrinsic "^1.1.3"
@@ -2245,15 +2245,15 @@
     functions-have-names "^1.2.2"
 
 functional-red-black-tree@^1.0.1:
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/functional-red-black-tree/-/functional-red-black-tree-1.0.1.tgz#1b0ab3bd553b2a0d6399d29c0e3ea0b252078327"
   integrity sha512-dsKNQNdj6xA3T+QlADDA7mOSlX0qiMINjn0cgr+eGHGsbSHzTabcIogz2+p/iqP1Xs6EP/sS2SbqH+brGTbq0g==
 
-functions-have-names@^1.2.2:
+functions-have-names@^1.2.2, functions-have-names@^1.2.3:
   version "1.2.3"
   resolved "https://registry.yarnpkg.com/functions-have-names/-/functions-have-names-1.2.3.tgz#0404fe4ee2ba2f607f0e0ec3c80bae994133b834"
   integrity sha512-xckBUXyTIqT97tq2x2AMb+g163b5JFysYk0x4qxNFwbfQkmNZoiRHb6sPzI9/QV33WeuvVYBUIiD4NzNIyqaRQ==
 
 get-intrinsic@^1.0.2, get-intrinsic@^1.1.1, get-intrinsic@^1.1.3, get-intrinsic@^1.2.0:
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/get-intrinsic/-/get-intrinsic-1.2.0.tgz#7ad1dc0535f3a2904bba075772763e5051f6d05f"
@@ -2436,17 +2436,17 @@
   version "4.1.0"
   resolved "https://registry.yarnpkg.com/hosted-git-info/-/hosted-git-info-4.1.0.tgz#827b82867e9ff1c8d0c4d9d53880397d2c86d224"
   integrity sha512-kyCuEOWjJqZuDbRHzL8V93NzQhwIB71oFWSyzVo+KPZI+pnQPPxucdkrOZvkLRnrf5URsQM+IJ09Dw29cRALIA==
   dependencies:
     lru-cache "^6.0.0"
 
 html-tags@^3.2.0:
-  version "3.2.0"
-  resolved "https://registry.yarnpkg.com/html-tags/-/html-tags-3.2.0.tgz#dbb3518d20b726524e4dd43de397eb0a95726961"
-  integrity sha512-vy7ClnArOZwCnqZgvv+ddgHgJiAFXe3Ge9ML5/mBctVJoUoYPCdxVucOywjDARn6CVoh3dRSFdPHy2sX80L0Wg==
+  version "3.3.1"
+  resolved "https://registry.yarnpkg.com/html-tags/-/html-tags-3.3.1.tgz#a04026a18c882e4bba8a01a3d39cfe465d40b5ce"
+  integrity sha512-ztqyC3kLto0e9WbNp0aeP+M3kTt+nbaIveGmUxAtZa+8iFgKLUOD4YKM5j+f3QD89bra7UeumolZHKuOXnTmeQ==
 
 htmlparser2@^6.0.0:
   version "6.1.0"
   resolved "https://registry.yarnpkg.com/htmlparser2/-/htmlparser2-6.1.0.tgz#c4d762b6c3371a05dbe65e94ae43a9f845fb8fb7"
   integrity sha512-gyyPk6rgonLFEDGoeRgQNaEUvdJ4ktTmmUh/h2t7s+M8oPpIPxgNACWa+6ESR57kXstwqPiCut0V8NRpcwgU7A==
   dependencies:
     domelementtype "^2.0.1"
@@ -2592,18 +2592,18 @@
     has-tostringtag "^1.0.0"
 
 is-callable@^1.1.3, is-callable@^1.1.4, is-callable@^1.2.7:
   version "1.2.7"
   resolved "https://registry.yarnpkg.com/is-callable/-/is-callable-1.2.7.tgz#3bc2a85ea742d9e36205dcacdd72ca1fdc51b055"
   integrity sha512-1BC0BVFhS/p0qtw6enp8e+8OD0UrK0oFLztSjNzhcKA3WDuJxxAPXzPuPtKkjEY9UUoEWlX/8fgKeu2S8i9JTA==
 
-is-core-module@^2.5.0, is-core-module@^2.9.0:
-  version "2.11.0"
-  resolved "https://registry.yarnpkg.com/is-core-module/-/is-core-module-2.11.0.tgz#ad4cb3e3863e814523c96f3f58d26cc570ff0144"
-  integrity sha512-RRjxlvLDkD1YJwDbroBHMb+cukurkDWNyHx7D3oNB5x9rb5ogcksMC5wHCadcXoo67gVr/+3GFySh3134zi6rw==
+is-core-module@^2.11.0, is-core-module@^2.5.0:
+  version "2.12.0"
+  resolved "https://registry.yarnpkg.com/is-core-module/-/is-core-module-2.12.0.tgz#36ad62f6f73c8253fd6472517a12483cf03e7ec4"
+  integrity sha512-RECHCBCd/viahWmwj6enj19sKbHfJrddi/6cBDsNTKbNq0f7VeaUkBo60BqzvPqo/W54ChS62Z5qyun7cfOMqQ==
   dependencies:
     has "^1.0.3"
 
 is-date-object@^1.0.1:
   version "1.0.5"
   resolved "https://registry.yarnpkg.com/is-date-object/-/is-date-object-1.0.5.tgz#0841d5536e724c25597bf6ea62e1bd38298df31f"
   integrity sha512-9YQaSxsAiSwcvS33MBk3wTCVnWK+HhF8VZR2jRxehM16QcVOdHqPn4VPHmRK4lSr38n9JriurInLcP90xsYNfQ==
@@ -3165,17 +3165,17 @@
   version "3.3.6"
   resolved "https://registry.yarnpkg.com/minipass/-/minipass-3.3.6.tgz#7bba384db3a1520d18c9c0e5251c3444e95dd94a"
   integrity sha512-DxiNidxSEK+tHG6zOIklvNOwm3hvCrbUrdtzY74U6HKTJxvIDfOUL5W5P2Ghd3DTkhhKPYGqeNUIh5qcM4YBfw==
   dependencies:
     yallist "^4.0.0"
 
 minipass@^4.0.0:
-  version "4.2.5"
-  resolved "https://registry.yarnpkg.com/minipass/-/minipass-4.2.5.tgz#9e0e5256f1e3513f8c34691dd68549e85b2c8ceb"
-  integrity sha512-+yQl7SX3bIT83Lhb4BVorMAHVuqsskxRdlmO9kTpyukp8vsm2Sn/fUOV9xlnG8/a5JsypJzap21lz/y3FBMJ8Q==
+  version "4.2.8"
+  resolved "https://registry.yarnpkg.com/minipass/-/minipass-4.2.8.tgz#f0010f64393ecfc1d1ccb5f582bcaf45f48e1a3a"
+  integrity sha512-fNzuVyifolSLFL4NzpF+wEF4qrgqaaKX0haXPQEdQ7NKAN+WecoKMHV09YcuL/DHxrUsYQOK3MiuDf7Ip2OXfQ==
 
 minizlib@^2.1.1:
   version "2.1.2"
   resolved "https://registry.yarnpkg.com/minizlib/-/minizlib-2.1.2.tgz#e90d3466ba209b932451508a11ce3d3632145931"
   integrity sha512-bAxsR8BVfj60DWXHE3u30oHzfl4G7khkSuPW+qvpd7jFRHm7dLxOjUk1EHACJ/hxLY8phGJ0YhYHZo7jil7Qdg==
   dependencies:
     minipass "^3.0.0"
@@ -3192,15 +3192,15 @@
   integrity sha512-5LC9SOxjSc2HF6vO2CyuTDNivEdoz2IvyJJGj6X8DJ0eFyfszE0QiEd+iXmBvUP3WHxSjFH/vIsA0EN00cgr8w==
 
 ms@2.1.2:
   version "2.1.2"
   resolved "https://registry.yarnpkg.com/ms/-/ms-2.1.2.tgz#d09d1f357b443f493382a8eb3ccd183872ae6009"
   integrity sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==
 
-nanoid@^3.1.23, nanoid@^3.3.4:
+nanoid@^3.1.23, nanoid@^3.3.6:
   version "3.3.6"
   resolved "https://registry.yarnpkg.com/nanoid/-/nanoid-3.3.6.tgz#443380c856d6e9f9824267d960b4236ad583ea4c"
   integrity sha512-BGcqMMJuToF7i1rt+2PWSNVnWIkGCU78jBG3RxO/bZlnZPK2Cmi2QaffxGO/2RvWi9sL+FAiRiXMgsyxQ1DIDA==
 
 napi-macros@~2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/napi-macros/-/napi-macros-2.0.0.tgz#2b6bae421e7b96eb687aa6c77a7858640670001b"
@@ -3525,19 +3525,19 @@
 
 postcss-value-parser@^4.1.0, postcss-value-parser@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz#723c09920836ba6d3e5af019f92bc0971c02e514"
   integrity sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==
 
 postcss@^8.2.15, postcss@^8.3.11, postcss@^8.4.19:
-  version "8.4.21"
-  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.21.tgz#c639b719a57efc3187b13a1d765675485f4134f4"
-  integrity sha512-tP7u/Sn/dVxK2NnruI4H9BG+x+Wxz6oeZ1cJ8P6G/PZY0IKk4k/63TDsQf2kQq3+qoJeLm2kIBUNlZe3zgb4Zg==
+  version "8.4.22"
+  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.22.tgz#c29e6776b60ab3af602d4b513d5bd2ff9aa85dc1"
+  integrity sha512-XseknLAfRHzVWjCEtdviapiBtfLdgyzExD50Rg2ePaucEesyh8Wv4VPdW0nbyDa1ydbrAxV19jvMT4+LFmcNUA==
   dependencies:
-    nanoid "^3.3.4"
+    nanoid "^3.3.6"
     picocolors "^1.0.0"
     source-map-js "^1.0.2"
 
 prelude-ls@^1.2.1:
   version "1.2.1"
   resolved "https://registry.yarnpkg.com/prelude-ls/-/prelude-ls-1.2.1.tgz#debc6489d7a6e6b0e7611888cec880337d316396"
   integrity sha512-vkcDPrRZo1QZLbn5RLGPpg/WmIQ65qoWWhcGKf/b5eplkkarX0m9z8ppCat4mlOqUsWpyNuYgO3VRyrYHSzX5g==
@@ -3732,21 +3732,21 @@
 
 regenerator-runtime@^0.13.11:
   version "0.13.11"
   resolved "https://registry.yarnpkg.com/regenerator-runtime/-/regenerator-runtime-0.13.11.tgz#f6dca3e7ceec20590d07ada785636a90cdca17f9"
   integrity sha512-kY1AZVr2Ra+t+piVaJ4gxaFaReZVH40AKNo7UCX6W+dEwBo/2oZJzqfuN1qLq1oL45o56cPaTXELwrTh8Fpggg==
 
 regexp.prototype.flags@^1.2.0, regexp.prototype.flags@^1.4.3:
-  version "1.4.3"
-  resolved "https://registry.yarnpkg.com/regexp.prototype.flags/-/regexp.prototype.flags-1.4.3.tgz#87cab30f80f66660181a3bb7bf5981a872b367ac"
-  integrity sha512-fjggEOO3slI6Wvgjwflkc4NFRCTZAu5CnNfBd5qOMYhWdn67nJBBu34/TkD++eeFmd8C9r9jfXJ27+nSiRkSUA==
+  version "1.5.0"
+  resolved "https://registry.yarnpkg.com/regexp.prototype.flags/-/regexp.prototype.flags-1.5.0.tgz#fe7ce25e7e4cca8db37b6634c8a2c7009199b9cb"
+  integrity sha512-0SutC3pNudRKgquxGoRGIz946MZVHqbNfPjBdxeOhBrdgDKlRoXmYLQN9xRbrR09ZXWeGAdPuif7egofn6v5LA==
   dependencies:
     call-bind "^1.0.2"
-    define-properties "^1.1.3"
-    functions-have-names "^1.2.2"
+    define-properties "^1.2.0"
+    functions-have-names "^1.2.3"
 
 regexpp@^3.1.0:
   version "3.2.0"
   resolved "https://registry.yarnpkg.com/regexpp/-/regexpp-3.2.0.tgz#0425a2768d8f23bad70ca4b90461fa2f1213e1b2"
   integrity sha512-pq2bWo9mVD43nbts2wGv17XLiNLya+GklZ8kaDLV2Z08gDCsGpnKn9BFMepvWuHCbyVvY7J5o5+BVvoQbmlJLg==
 
 require-from-string@^2.0.2:
@@ -3778,19 +3778,19 @@
 
 resolve-from@^5.0.0:
   version "5.0.0"
   resolved "https://registry.yarnpkg.com/resolve-from/-/resolve-from-5.0.0.tgz#c35225843df8f776df21c57557bc087e9dfdfc69"
   integrity sha512-qYg9KP24dD5qka9J47d0aVky0N+b4fTU89LN9iDnjB5waksiC49rvMB0PrUJQGoTmH50XPiqOvAjDfaijGxYZw==
 
 resolve@^1.10.0, resolve@^1.9.0:
-  version "1.22.1"
-  resolved "https://registry.yarnpkg.com/resolve/-/resolve-1.22.1.tgz#27cb2ebb53f91abb49470a928bba7558066ac177"
-  integrity sha512-nBpuuYuY5jFsli/JIs1oldw6fOQCBioohqWZg/2hiaOybXOft4lonv85uDOKXdf8rhyK159cxU5cDcK/NKk8zw==
+  version "1.22.2"
+  resolved "https://registry.yarnpkg.com/resolve/-/resolve-1.22.2.tgz#0ed0943d4e301867955766c9f3e1ae6d01c6845f"
+  integrity sha512-Sb+mjNHOULsBv818T40qSPeRiuWLyaGMa5ewydRLFimneixmVy2zdivRl+AF6jaYPC8ERxGDmFSiqui6SfPd+g==
   dependencies:
-    is-core-module "^2.9.0"
+    is-core-module "^2.11.0"
     path-parse "^1.0.7"
     supports-preserve-symlinks-flag "^1.0.0"
 
 reusify@^1.0.4:
   version "1.0.4"
   resolved "https://registry.yarnpkg.com/reusify/-/reusify-1.0.4.tgz#90da382b1e126efc02146e90845a88db12925d76"
   integrity sha512-U9nH88a3fc/ekCF1l0/UP1IosiuIjyTh7hBvXVMHYgVcfGvt897Xguj2UOLDeI5BG2m7/uwyaLVT6fbtCwTyzw==
@@ -3854,17 +3854,17 @@
   integrity sha512-SHiNtMOUGWBQJwzISiVYKu82GiV4QYGePp3odlY1tuKO7gPtphAT5R/py0fA6xtbgLL/RvtJZnU9b8s0F1q0Xg==
   dependencies:
     "@types/json-schema" "^7.0.5"
     ajv "^6.12.4"
     ajv-keywords "^3.5.2"
 
 schema-utils@^3.0.0, schema-utils@^3.1.0, schema-utils@^3.1.1:
-  version "3.1.1"
-  resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-3.1.1.tgz#bc74c4b6b6995c1d88f76a8b77bea7219e0c8281"
-  integrity sha512-Y5PQxS4ITlC+EahLuXaY86TXfR7Dc5lw294alXOq86JAHCihAIZfqv8nNCWvaEJvaC51uN9hbLGeV0cFBdH+Fw==
+  version "3.1.2"
+  resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-3.1.2.tgz#36c10abca6f7577aeae136c804b0c741edeadc99"
+  integrity sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==
   dependencies:
     "@types/json-schema" "^7.0.8"
     ajv "^6.12.5"
     ajv-keywords "^3.5.2"
 
 "semver@2 || 3 || 4 || 5", semver@^5.4.1, semver@^5.5.0:
   version "5.7.1"
@@ -3873,17 +3873,17 @@
 
 semver@^6.0.0:
   version "6.3.0"
   resolved "https://registry.yarnpkg.com/semver/-/semver-6.3.0.tgz#ee0a64c8af5e8ceea67687b133761e1becbd1d3d"
   integrity sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==
 
 semver@^7.2.1, semver@^7.3.4, semver@^7.3.5:
-  version "7.3.8"
-  resolved "https://registry.yarnpkg.com/semver/-/semver-7.3.8.tgz#07a78feafb3f7b32347d725e33de7e2a2df67798"
-  integrity sha512-NB1ctGL5rlHrPJtFDVIVzTyQylMLu9N9VICA6HSFJo8MCGVTMW6gfpicwKmmK/dAjTOrqu5l63JJOpDSrAis3A==
+  version "7.5.0"
+  resolved "https://registry.yarnpkg.com/semver/-/semver-7.5.0.tgz#ed8c5dc8efb6c629c88b23d41dc9bf40c1d96cd0"
+  integrity sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==
   dependencies:
     lru-cache "^6.0.0"
 
 serialize-javascript@^5.0.1:
   version "5.0.1"
   resolved "https://registry.yarnpkg.com/serialize-javascript/-/serialize-javascript-5.0.1.tgz#7886ec848049a462467a97d3d918ebb2aaf934f4"
   integrity sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==
@@ -3925,17 +3925,17 @@
 
 shebang-regex@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/shebang-regex/-/shebang-regex-3.0.0.tgz#ae16f1644d873ecad843b0307b143362d4c42172"
   integrity sha512-7++dFhtcx3353uBaq8DDR4NuxBetBzC7ZQOhmTQInHEd6bSrXdiEyzCvG07Z44UYdLShWUyXt5M/yhz8ekcb1A==
 
 shell-quote@^1.6.1:
-  version "1.8.0"
-  resolved "https://registry.yarnpkg.com/shell-quote/-/shell-quote-1.8.0.tgz#20d078d0eaf71d54f43bd2ba14a1b5b9bfa5c8ba"
-  integrity sha512-QHsz8GgQIGKlRi24yFc6a6lN69Idnx634w49ay6+jA5yFh7a1UY+4Rp6HPx/L/1zcEDPEij8cIsiqR6bQsE5VQ==
+  version "1.8.1"
+  resolved "https://registry.yarnpkg.com/shell-quote/-/shell-quote-1.8.1.tgz#6dbf4db75515ad5bac63b4f1894c3a154c766680"
+  integrity sha512-6j1W9l1iAs/4xYBI1SYOVZyFcCis9b4KCLQ8fgAGG07QvzaRLVVRQvAy85yNmmZSjYjg4MWh4gNvlPujU/5LpA==
 
 side-channel@^1.0.4:
   version "1.0.4"
   resolved "https://registry.yarnpkg.com/side-channel/-/side-channel-1.0.4.tgz#efce5c8fdc104ee751b25c58d4290011fa5ea2cf"
   integrity sha512-q5XPytqFEIKHkGdiMIrY10mvLRvnQh42/+GoBlFW3b2LXLE2xxJpZFdm94we0BaoV3RwJyGqg5wS7epxTv0Zvw==
   dependencies:
     call-bind "^1.0.0"
@@ -4276,29 +4276,29 @@
     p-limit "^3.0.2"
     schema-utils "^3.0.0"
     serialize-javascript "^5.0.1"
     source-map "^0.6.1"
     terser "^5.3.4"
     webpack-sources "^1.4.3"
 
-terser-webpack-plugin@^5.1.3:
+terser-webpack-plugin@^5.3.7:
   version "5.3.7"
   resolved "https://registry.yarnpkg.com/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz#ef760632d24991760f339fe9290deb936ad1ffc7"
   integrity sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==
   dependencies:
     "@jridgewell/trace-mapping" "^0.3.17"
     jest-worker "^27.4.5"
     schema-utils "^3.1.1"
     serialize-javascript "^6.0.1"
     terser "^5.16.5"
 
 terser@^5.16.5, terser@^5.3.4:
-  version "5.16.8"
-  resolved "https://registry.yarnpkg.com/terser/-/terser-5.16.8.tgz#ccde583dabe71df3f4ed02b65eb6532e0fae15d5"
-  integrity sha512-QI5g1E/ef7d+PsDifb+a6nnVgC4F22Bg6T0xrBrz6iloVB4PUkkunp6V8nzoOOZJIzjWVdAGqCdlKlhLq/TbIA==
+  version "5.17.1"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-5.17.1.tgz#948f10830454761e2eeedc6debe45c532c83fd69"
+  integrity sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==
   dependencies:
     "@jridgewell/source-map" "^0.3.2"
     acorn "^8.5.0"
     commander "^2.20.0"
     source-map-support "~0.5.20"
 
 text-table@^0.2.0:
@@ -4434,17 +4434,17 @@
 
 universalify@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/universalify/-/universalify-2.0.0.tgz#75a4984efedc4b08975c5aeb73f530d02df25717"
   integrity sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==
 
 update-browserslist-db@^1.0.10:
-  version "1.0.10"
-  resolved "https://registry.yarnpkg.com/update-browserslist-db/-/update-browserslist-db-1.0.10.tgz#0f54b876545726f17d00cd9a2561e6dade943ff3"
-  integrity sha512-OztqDenkfFkbSG+tRxBeAnCVPckDBcvibKd35yDONx6OU8N7sqgwc7rCbkJ/WcYtVRZ4ba68d6byhC21GFh7sQ==
+  version "1.0.11"
+  resolved "https://registry.yarnpkg.com/update-browserslist-db/-/update-browserslist-db-1.0.11.tgz#9a2a641ad2907ae7b3616506f4b977851db5b940"
+  integrity sha512-dCwEFf0/oT85M1fHBg4F0jtLwJrutGoHSQXCh7u4o2t1drG+c0a9Flnqww6XUKSfQMPpJBRjU8d4RXB09qtvaA==
   dependencies:
     escalade "^3.1.1"
     picocolors "^1.0.0"
 
 uri-js@^4.2.2:
   version "4.4.1"
   resolved "https://registry.yarnpkg.com/uri-js/-/uri-js-4.4.1.tgz#9b1a52595225859e55f669d928f88c6c57f2a77e"
@@ -4586,40 +4586,40 @@
 
 webpack-sources@^3.2.3:
   version "3.2.3"
   resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-3.2.3.tgz#2d4daab8451fd4b240cc27055ff6a0c2ccea0cde"
   integrity sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==
 
 webpack@^5.41.1:
-  version "5.77.0"
-  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.77.0.tgz#dea3ad16d7ea6b84aa55fa42f4eac9f30e7eb9b4"
-  integrity sha512-sbGNjBr5Ya5ss91yzjeJTLKyfiwo5C628AFjEa6WSXcZa4E+F57om3Cc8xLb1Jh0b243AWuSYRf3dn7HVeFQ9Q==
+  version "5.79.0"
+  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.79.0.tgz#8552b5da5a26e4e25842c08a883e08fc7740547a"
+  integrity sha512-3mN4rR2Xq+INd6NnYuL9RC9GAmc1ROPKJoHhrZ4pAjdMFEkJJWrsPw8o2JjCIyQyTu7rTXYn4VG6OpyB3CobZg==
   dependencies:
     "@types/eslint-scope" "^3.7.3"
-    "@types/estree" "^0.0.51"
+    "@types/estree" "^1.0.0"
     "@webassemblyjs/ast" "1.11.1"
     "@webassemblyjs/wasm-edit" "1.11.1"
     "@webassemblyjs/wasm-parser" "1.11.1"
     acorn "^8.7.1"
     acorn-import-assertions "^1.7.6"
     browserslist "^4.14.5"
     chrome-trace-event "^1.0.2"
     enhanced-resolve "^5.10.0"
-    es-module-lexer "^0.9.0"
+    es-module-lexer "^1.2.1"
     eslint-scope "5.1.1"
     events "^3.2.0"
     glob-to-regexp "^0.4.1"
     graceful-fs "^4.2.9"
     json-parse-even-better-errors "^2.3.1"
     loader-runner "^4.2.0"
     mime-types "^2.1.27"
     neo-async "^2.6.2"
     schema-utils "^3.1.0"
     tapable "^2.1.1"
-    terser-webpack-plugin "^5.1.3"
+    terser-webpack-plugin "^5.3.7"
     watchpack "^2.4.0"
     webpack-sources "^3.2.3"
 
 whatwg-mimetype@^2.3.0:
   version "2.3.0"
   resolved "https://registry.yarnpkg.com/whatwg-mimetype/-/whatwg-mimetype-2.3.0.tgz#3d4b1e0312d2079879f826aff18dbeeca5960fbf"
   integrity sha512-M4yMwr6mAnQz76TbJm914+gPpB/nCwvZbJU28cUD6dR004SAxDLOOSUaB1JDRqLtaOV/vi0IC5lEAGFgrjGv/g==
@@ -4772,17 +4772,17 @@
 
 yargs-parser@^20.2.3:
   version "20.2.9"
   resolved "https://registry.yarnpkg.com/yargs-parser/-/yargs-parser-20.2.9.tgz#2eb7dc3b0289718fc295f362753845c41a0c94ee"
   integrity sha512-y11nGElTIV+CT3Zv9t7VKl+Q3hTQoT9a1Qzezhhl6Rp21gJ/IVTW7Z3y9EWXhuUBC2Shnf+DX0antecpAwSP8w==
 
 yjs@^13.5.40:
-  version "13.5.51"
-  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.5.51.tgz#afd5a26a230498c3b4bf8fee9c8dbeea71ef7e5c"
-  integrity sha512-F1Nb3z3TdandD80IAeQqgqy/2n9AhDLcXoBhZvCUX1dNVe0ef7fIwi6MjSYaGAYF2Ev8VcLcsGnmuGGOl7AWbw==
+  version "13.5.53"
+  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.5.53.tgz#6531378981b89cfadd107145f7fb9f65f708a01f"
+  integrity sha512-B4UUycEK8BcYf195HL4LN4Az4Sg2+QzTHnabFHjQwLvGn96v/G+4CS52xNZk/0QWNXhLRCb+2GK3JmcX5fiCEQ==
   dependencies:
     lib0 "^0.2.72"
 
 yocto-queue@^0.1.0:
   version "0.1.0"
   resolved "https://registry.yarnpkg.com/yocto-queue/-/yocto-queue-0.1.0.tgz#0294eb3dee05028d31ee1a5fa2c556a6aaf10a1b"
   integrity sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==
```

