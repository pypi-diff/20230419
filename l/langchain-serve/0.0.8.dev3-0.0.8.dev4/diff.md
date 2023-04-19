# Comparing `tmp/langchain-serve-0.0.8.dev3.tar.gz` & `tmp/langchain-serve-0.0.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-serve-0.0.8.dev3.tar", last modified: Wed Apr 19 02:08:31 2023, max compression
+gzip compressed data, was "langchain-serve-0.0.8.dev4.tar", last modified: Wed Apr 19 02:09:39 2023, max compression
```

## Comparing `langchain-serve-0.0.8.dev3.tar` & `langchain-serve-0.0.8.dev4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.799896 langchain-serve-0.0.8.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-19 02:08:31.799896 langchain-serve-0.0.8.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25905 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.795896 langchain-serve-0.0.8.dev3/langchain_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-19 02:08:31.000000 langchain-serve-0.0.8.dev3/langchain_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-19 02:08:31.000000 langchain-serve-0.0.8.dev3/langchain_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:08:31.000000 langchain-serve-0.0.8.dev3/langchain_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-19 02:08:31.000000 langchain-serve-0.0.8.dev3/langchain_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:08:31.000000 langchain-serve-0.0.8.dev3/langchain_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 02:08:31.000000 langchain-serve-0.0.8.dev3/langchain_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 02:08:31.000000 langchain-serve-0.0.8.dev3/langchain_serve.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.795896 langchain-serve-0.0.8.dev3/lcserve/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 02:08:31.000000 langchain-serve-0.0.8.dev3/lcserve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/agent-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.795896 langchain-serve-0.0.8.dev3/lcserve/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.795896 langchain-serve-0.0.8.dev3/lcserve/apps/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/apps/babyagi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/apps/babyagi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/apps/babyagi/babyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/apps/babyagi/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.799896 langchain-serve-0.0.8.dev3/lcserve/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/agentexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.799896 langchain-serve-0.0.8.dev3/lcserve/backend/playground/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/playground/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/playground/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.799896 langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/langchain_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/customgateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/customgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/flow.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.795896 langchain-serve-0.0.8.dev3/lcserve/playground/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:08:31.799896 langchain-serve-0.0.8.dev3/lcserve/playground/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/playground/babyagi/playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/playground/babyagi/user_input.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/playgroundgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/servinggateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/lcserve/servinggateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 02:08:31.799896 langchain-serve-0.0.8.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-19 02:08:27.000000 langchain-serve-0.0.8.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.442920 langchain-serve-0.0.8.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-19 02:09:39.442920 langchain-serve-0.0.8.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25905 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.438919 langchain-serve-0.0.8.dev4/langchain_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-19 02:09:39.000000 langchain-serve-0.0.8.dev4/langchain_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-19 02:09:39.000000 langchain-serve-0.0.8.dev4/langchain_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:09:39.000000 langchain-serve-0.0.8.dev4/langchain_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-19 02:09:39.000000 langchain-serve-0.0.8.dev4/langchain_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:09:39.000000 langchain-serve-0.0.8.dev4/langchain_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 02:09:39.000000 langchain-serve-0.0.8.dev4/langchain_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 02:09:39.000000 langchain-serve-0.0.8.dev4/langchain_serve.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.438919 langchain-serve-0.0.8.dev4/lcserve/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 02:09:39.000000 langchain-serve-0.0.8.dev4/lcserve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/agent-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.434919 langchain-serve-0.0.8.dev4/lcserve/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.438919 langchain-serve-0.0.8.dev4/lcserve/apps/babyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/apps/babyagi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/apps/babyagi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/apps/babyagi/babyagi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/apps/babyagi/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.438919 langchain-serve-0.0.8.dev4/lcserve/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/agentexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.438919 langchain-serve-0.0.8.dev4/lcserve/backend/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/playground/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/playground/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.438919 langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/langchain_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/customgateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/customgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/flow.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.438919 langchain-serve-0.0.8.dev4/lcserve/playground/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:09:39.438919 langchain-serve-0.0.8.dev4/lcserve/playground/babyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/playground/babyagi/playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/playground/babyagi/user_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/playgroundgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/servinggateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/lcserve/servinggateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 02:09:39.442920 langchain-serve-0.0.8.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-19 02:09:35.000000 langchain-serve-0.0.8.dev4/setup.py
```

### Comparing `langchain-serve-0.0.8.dev3/LICENSE` & `langchain-serve-0.0.8.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/PKG-INFO` & `langchain-serve-0.0.8.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-serve
-Version: 0.0.8.dev3
+Version: 0.0.8.dev4
 Summary: Langchain Serve - serve your langchain apps on Jina AI Cloud.
 Home-page: https://github.com/jina-ai/langchain-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/langchain-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

### Comparing `langchain-serve-0.0.8.dev3/README.md` & `langchain-serve-0.0.8.dev4/README.md`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/langchain_serve.egg-info/PKG-INFO` & `langchain-serve-0.0.8.dev4/langchain_serve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-serve
-Version: 0.0.8.dev3
+Version: 0.0.8.dev4
 Summary: Langchain Serve - serve your langchain apps on Jina AI Cloud.
 Home-page: https://github.com/jina-ai/langchain-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/langchain-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

### Comparing `langchain-serve-0.0.8.dev3/langchain_serve.egg-info/SOURCES.txt` & `langchain-serve-0.0.8.dev4/langchain_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/__main__.py` & `langchain-serve-0.0.8.dev4/lcserve/__main__.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/apps/babyagi/app.py` & `langchain-serve-0.0.8.dev4/lcserve/apps/babyagi/app.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/apps/babyagi/babyagi.py` & `langchain-serve-0.0.8.dev4/lcserve/apps/babyagi/babyagi.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/backend/agentexecutor.py` & `langchain-serve-0.0.8.dev4/lcserve/backend/agentexecutor.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/backend/decorators.py` & `langchain-serve-0.0.8.dev4/lcserve/backend/decorators.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/backend/gateway.py` & `langchain-serve-0.0.8.dev4/lcserve/backend/gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/backend/nginx.conf` & `langchain-serve-0.0.8.dev4/lcserve/backend/nginx.conf`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/backend/playground/app.py` & `langchain-serve-0.0.8.dev4/lcserve/backend/playground/app.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/helper.py` & `langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/helper.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/langchain_helper.py` & `langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/langchain_helper.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/talk.py` & `langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/talk.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/backend/playground/utils/tools.py` & `langchain-serve-0.0.8.dev4/lcserve/backend/playground/utils/tools.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/customgateway.Dockerfile` & `langchain-serve-0.0.8.dev4/lcserve/customgateway.Dockerfile`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/flow.py` & `langchain-serve-0.0.8.dev4/lcserve/flow.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/flow.yml` & `langchain-serve-0.0.8.dev4/lcserve/flow.yml`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/playground/babyagi/playground.py` & `langchain-serve-0.0.8.dev4/lcserve/playground/babyagi/playground.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/lcserve/playground/babyagi/user_input.py` & `langchain-serve-0.0.8.dev4/lcserve/playground/babyagi/user_input.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.8.dev3/setup.py` & `langchain-serve-0.0.8.dev4/setup.py`

 * *Files identical despite different names*

