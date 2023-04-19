# Comparing `tmp/frz-jupyterlab-variableinspector-0.1.3.tar.gz` & `tmp/frz-jupyterlab-variableinspector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frz-jupyterlab-variableinspector-0.1.3.tar", last modified: Wed Jun  8 08:06:54 2022, max compression
+gzip compressed data, was "frz-jupyterlab-variableinspector-0.1.4.tar", last modified: Wed Apr 19 15:25:45 2023, max compression
```

## Comparing `frz-jupyterlab-variableinspector-0.1.3.tar` & `frz-jupyterlab-variableinspector-0.1.4.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 zfr       (1000) zfr       (1000)        0 2022-06-08 08:06:54.390399 frz-jupyterlab-variableinspector-0.1.3/
--rw-r--r--   0 zfr       (1000) zfr       (1000)       86 2022-06-07 12:16:46.000000 frz-jupyterlab-variableinspector-0.1.3/CHANGELOG.md
--rw-r--r--   0 zfr       (1000) zfr       (1000)     1520 2022-06-07 12:16:46.000000 frz-jupyterlab-variableinspector-0.1.3/LICENSE
--rw-r--r--   0 zfr       (1000) zfr       (1000)      426 2022-06-07 13:45:43.000000 frz-jupyterlab-variableinspector-0.1.3/MANIFEST.in
--rw-r--r--   0 zfr       (1000) zfr       (1000)     3707 2022-06-08 08:06:54.390399 frz-jupyterlab-variableinspector-0.1.3/PKG-INFO
--rw-r--r--   0 zfr       (1000) zfr       (1000)     2625 2022-06-08 07:57:23.000000 frz-jupyterlab-variableinspector-0.1.3/README.md
--rw-r--r--   0 zfr       (1000) zfr       (1000)     1914 2022-06-07 13:45:43.000000 frz-jupyterlab-variableinspector-0.1.3/RELEASE.md
-drwxr-xr-x   0 zfr       (1000) zfr       (1000)        0 2022-06-08 08:06:54.390399 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/
--rw-r--r--   0 zfr       (1000) zfr       (1000)      321 2022-06-06 19:38:26.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/__init__.py
--rw-r--r--   0 zfr       (1000) zfr       (1000)      625 2022-06-06 19:38:26.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/_version.py
-drwxr-xr-x   0 zfr       (1000) zfr       (1000)        0 2022-06-08 08:06:54.390399 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/
--rw-r--r--   0 zfr       (1000) zfr       (1000)    20054 2022-06-08 08:00:19.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/build_log.json
--rw-r--r--   0 zfr       (1000) zfr       (1000)     3830 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/package.json
-drwxr-xr-x   0 zfr       (1000) zfr       (1000)        0 2022-06-08 08:06:54.390399 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/
--rw-r--r--   0 zfr       (1000) zfr       (1000)    63230 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/lib_index_js.d8a6a68cd2c54907e293.js
--rw-r--r--   0 zfr       (1000) zfr       (1000)    60008 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/lib_index_js.d8a6a68cd2c54907e293.js.map
--rw-r--r--   0 zfr       (1000) zfr       (1000)    33093 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/remoteEntry.01eb97769bed74d9aebb.js
--rw-r--r--   0 zfr       (1000) zfr       (1000)    32314 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/remoteEntry.01eb97769bed74d9aebb.js.map
--rw-r--r--   0 zfr       (1000) zfr       (1000)      184 2022-06-08 08:00:19.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/style.js
--rw-r--r--   0 zfr       (1000) zfr       (1000)     4654 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js
--rw-r--r--   0 zfr       (1000) zfr       (1000)     1866 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js.map
--rw-r--r--   0 zfr       (1000) zfr       (1000)    12112 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js
--rw-r--r--   0 zfr       (1000) zfr       (1000)    13871 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js.map
--rw-r--r--   0 zfr       (1000) zfr       (1000)   431248 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js
--rw-r--r--   0 zfr       (1000) zfr       (1000)   498241 2022-06-08 08:00:20.000000 frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js.map
-drwxr-xr-x   0 zfr       (1000) zfr       (1000)        0 2022-06-08 08:06:54.390399 frz-jupyterlab-variableinspector-0.1.3/frz_jupyterlab_variableinspector.egg-info/
--rw-r--r--   0 zfr       (1000) zfr       (1000)     3707 2022-06-08 08:06:53.000000 frz-jupyterlab-variableinspector-0.1.3/frz_jupyterlab_variableinspector.egg-info/PKG-INFO
--rw-r--r--   0 zfr       (1000) zfr       (1000)     2026 2022-06-08 08:06:54.000000 frz-jupyterlab-variableinspector-0.1.3/frz_jupyterlab_variableinspector.egg-info/SOURCES.txt
--rw-r--r--   0 zfr       (1000) zfr       (1000)        1 2022-06-08 08:06:53.000000 frz-jupyterlab-variableinspector-0.1.3/frz_jupyterlab_variableinspector.egg-info/dependency_links.txt
--rw-r--r--   0 zfr       (1000) zfr       (1000)        1 2022-06-07 13:51:27.000000 frz-jupyterlab-variableinspector-0.1.3/frz_jupyterlab_variableinspector.egg-info/not-zip-safe
--rw-r--r--   0 zfr       (1000) zfr       (1000)       33 2022-06-08 08:06:54.000000 frz-jupyterlab-variableinspector-0.1.3/frz_jupyterlab_variableinspector.egg-info/top_level.txt
--rw-r--r--   0 zfr       (1000) zfr       (1000)      225 2022-06-07 13:45:43.000000 frz-jupyterlab-variableinspector-0.1.3/install.json
--rw-r--r--   0 zfr       (1000) zfr       (1000)     3689 2022-06-08 07:42:14.000000 frz-jupyterlab-variableinspector-0.1.3/package.json
--rw-r--r--   0 zfr       (1000) zfr       (1000)      663 2022-06-07 13:45:43.000000 frz-jupyterlab-variableinspector-0.1.3/pyproject.toml
--rw-r--r--   0 zfr       (1000) zfr       (1000)       38 2022-06-08 08:06:54.390399 frz-jupyterlab-variableinspector-0.1.3/setup.cfg
--rw-r--r--   0 zfr       (1000) zfr       (1000)     2896 2022-06-07 13:45:43.000000 frz-jupyterlab-variableinspector-0.1.3/setup.py
-drwxr-xr-x   0 zfr       (1000) zfr       (1000)        0 2022-06-08 08:06:54.390399 frz-jupyterlab-variableinspector-0.1.3/src/
--rw-r--r--   0 zfr       (1000) zfr       (1000)     1751 2022-06-07 11:55:49.000000 frz-jupyterlab-variableinspector-0.1.3/src/LICENCE.md
--rw-r--r--   0 zfr       (1000) zfr       (1000)    12890 2022-06-07 12:19:37.000000 frz-jupyterlab-variableinspector-0.1.3/src/handler.ts
--rw-r--r--   0 zfr       (1000) zfr       (1000)    10138 2022-06-07 13:44:31.000000 frz-jupyterlab-variableinspector-0.1.3/src/index.ts
--rw-r--r--   0 zfr       (1000) zfr       (1000)    13101 2022-06-08 08:00:08.000000 frz-jupyterlab-variableinspector-0.1.3/src/inspectorscripts.ts
--rw-r--r--   0 zfr       (1000) zfr       (1000)     2872 2022-06-07 11:55:49.000000 frz-jupyterlab-variableinspector-0.1.3/src/kernelconnector.ts
--rw-r--r--   0 zfr       (1000) zfr       (1000)     2384 2022-06-07 11:55:49.000000 frz-jupyterlab-variableinspector-0.1.3/src/manager.ts
--rw-r--r--   0 zfr       (1000) zfr       (1000)     9177 2022-06-07 13:25:17.000000 frz-jupyterlab-variableinspector-0.1.3/src/variableinspector.ts
-drwxr-xr-x   0 zfr       (1000) zfr       (1000)        0 2022-06-08 08:06:54.390399 frz-jupyterlab-variableinspector-0.1.3/style/
--rw-r--r--   0 zfr       (1000) zfr       (1000)      138 2022-06-07 12:16:46.000000 frz-jupyterlab-variableinspector-0.1.3/style/base.css
--rw-r--r--   0 zfr       (1000) zfr       (1000)     1400 2022-06-07 12:35:29.000000 frz-jupyterlab-variableinspector-0.1.3/style/index.css
--rw-r--r--   0 zfr       (1000) zfr       (1000)       21 2022-06-07 12:16:46.000000 frz-jupyterlab-variableinspector-0.1.3/style/index.js
--rw-r--r--   0 zfr       (1000) zfr       (1000)      555 2022-06-07 12:32:17.000000 frz-jupyterlab-variableinspector-0.1.3/tsconfig.json
+drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-04-19 15:25:45.577081 frz-jupyterlab-variableinspector-0.1.4/
+-rw-rw-r--   0 frz       (1000) frz       (1000)       86 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/CHANGELOG.md
+-rw-rw-r--   0 frz       (1000) frz       (1000)     1520 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/LICENSE
+-rw-rw-r--   0 frz       (1000) frz       (1000)      426 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/MANIFEST.in
+-rw-rw-r--   0 frz       (1000) frz       (1000)     3707 2023-04-19 15:25:45.577081 frz-jupyterlab-variableinspector-0.1.4/PKG-INFO
+-rw-rw-r--   0 frz       (1000) frz       (1000)     2625 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/README.md
+-rw-rw-r--   0 frz       (1000) frz       (1000)     1914 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/RELEASE.md
+drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-04-19 15:25:45.567081 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/
+-rw-r--r--   0 frz       (1000) frz       (1000)      340 2023-04-19 13:56:44.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/__init__.py
+-rw-r--r--   0 frz       (1000) frz       (1000)      648 2023-04-19 13:56:44.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/_version.py
+drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-04-19 15:25:45.567081 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/
+-rw-rw-r--   0 frz       (1000) frz       (1000)    21296 2023-04-19 15:15:40.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/build_log.json
+-rw-rw-r--   0 frz       (1000) frz       (1000)     3830 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/package.json
+drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-04-19 15:25:45.567081 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/
+-rw-rw-r--   0 frz       (1000) frz       (1000)    63178 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/lib_index_js.92aa6d645091a304c589.js
+-rw-rw-r--   0 frz       (1000) frz       (1000)    59950 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/lib_index_js.92aa6d645091a304c589.js.map
+-rw-rw-r--   0 frz       (1000) frz       (1000)    33092 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/remoteEntry.c589841968c12546b849.js
+-rw-rw-r--   0 frz       (1000) frz       (1000)    32313 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/remoteEntry.c589841968c12546b849.js.map
+-rw-rw-r--   0 frz       (1000) frz       (1000)      184 2023-04-19 15:15:40.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/style.js
+-rw-rw-r--   0 frz       (1000) frz       (1000)     4654 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js
+-rw-rw-r--   0 frz       (1000) frz       (1000)     1866 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js.map
+-rw-rw-r--   0 frz       (1000) frz       (1000)    12112 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js
+-rw-rw-r--   0 frz       (1000) frz       (1000)    13871 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js.map
+-rw-rw-r--   0 frz       (1000) frz       (1000)   431248 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js
+-rw-rw-r--   0 frz       (1000) frz       (1000)   498241 2023-04-19 15:15:41.000000 frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js.map
+drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-04-19 15:25:45.577081 frz-jupyterlab-variableinspector-0.1.4/frz_jupyterlab_variableinspector.egg-info/
+-rw-rw-r--   0 frz       (1000) frz       (1000)     3707 2023-04-19 15:25:45.000000 frz-jupyterlab-variableinspector-0.1.4/frz_jupyterlab_variableinspector.egg-info/PKG-INFO
+-rw-rw-r--   0 frz       (1000) frz       (1000)     2036 2023-04-19 15:25:45.000000 frz-jupyterlab-variableinspector-0.1.4/frz_jupyterlab_variableinspector.egg-info/SOURCES.txt
+-rw-rw-r--   0 frz       (1000) frz       (1000)        1 2023-04-19 15:25:45.000000 frz-jupyterlab-variableinspector-0.1.4/frz_jupyterlab_variableinspector.egg-info/dependency_links.txt
+-rw-rw-r--   0 frz       (1000) frz       (1000)        1 2023-04-19 13:58:31.000000 frz-jupyterlab-variableinspector-0.1.4/frz_jupyterlab_variableinspector.egg-info/not-zip-safe
+-rw-rw-r--   0 frz       (1000) frz       (1000)       33 2023-04-19 15:25:45.000000 frz-jupyterlab-variableinspector-0.1.4/frz_jupyterlab_variableinspector.egg-info/top_level.txt
+-rw-rw-r--   0 frz       (1000) frz       (1000)      225 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/install.json
+-rw-rw-r--   0 frz       (1000) frz       (1000)     3689 2023-04-19 12:01:29.000000 frz-jupyterlab-variableinspector-0.1.4/package.json
+-rw-rw-r--   0 frz       (1000) frz       (1000)      663 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/pyproject.toml
+-rw-rw-r--   0 frz       (1000) frz       (1000)       38 2023-04-19 15:25:45.577081 frz-jupyterlab-variableinspector-0.1.4/setup.cfg
+-rw-rw-r--   0 frz       (1000) frz       (1000)     2896 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/setup.py
+drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-04-19 15:25:45.577081 frz-jupyterlab-variableinspector-0.1.4/src/
+-rw-rw-r--   0 frz       (1000) frz       (1000)     1751 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/src/LICENCE.md
+-rw-rw-r--   0 frz       (1000) frz       (1000)    12890 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/src/handler.ts
+-rw-rw-r--   0 frz       (1000) frz       (1000)    10138 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/src/index.ts
+-rw-rw-r--   0 frz       (1000) frz       (1000)    13049 2023-04-19 15:15:09.000000 frz-jupyterlab-variableinspector-0.1.4/src/inspectorscripts.ts
+-rw-rw-r--   0 frz       (1000) frz       (1000)     2872 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/src/kernelconnector.ts
+-rw-rw-r--   0 frz       (1000) frz       (1000)     2384 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/src/manager.ts
+-rw-rw-r--   0 frz       (1000) frz       (1000)     9177 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/src/variableinspector.ts
+drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-04-19 15:25:45.577081 frz-jupyterlab-variableinspector-0.1.4/style/
+-rw-rw-r--   0 frz       (1000) frz       (1000)      138 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/style/base.css
+-rw-rw-r--   0 frz       (1000) frz       (1000)     1400 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/style/index.css
+-rw-rw-r--   0 frz       (1000) frz       (1000)       21 2023-04-18 15:38:52.000000 frz-jupyterlab-variableinspector-0.1.4/style/index.js
+-rw-r--r--   0 frz       (1000) frz       (1000)      579 2023-04-19 14:46:27.000000 frz-jupyterlab-variableinspector-0.1.4/tsconfig.json
+-rw-rw-r--   0 frz       (1000) frz       (1000)   262294 2023-04-19 14:40:05.000000 frz-jupyterlab-variableinspector-0.1.4/yarn.lock
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/LICENSE` & `frz-jupyterlab-variableinspector-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/PKG-INFO` & `frz-jupyterlab-variableinspector-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frz-jupyterlab-variableinspector
-Version: 0.1.3
+Version: 0.1.4
 Summary: Customized Variable Inspector extension for JupyterLab.
 Home-page: https://github.com/zhangfeiran/jupyterlab-variableInspector
 Author: Feiran Zhang
 Author-email: feiranzhang@outlook.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/README.md` & `frz-jupyterlab-variableinspector-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/RELEASE.md` & `frz-jupyterlab-variableinspector-0.1.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/_version.py` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/_version.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import json
-from pathlib import Path
-
-__all__ = ["__version__"]
-
-def _fetchVersion():
-    HERE = Path(__file__).parent.resolve()
-
-    for settings in HERE.rglob("package.json"): 
-        try:
-            with settings.open() as f:
-                version = json.load(f)["version"]
-                return (
-                    version.replace("-alpha.", "a")
-                    .replace("-beta.", "b")
-                    .replace("-rc.", "rc")
-                )
-        except FileNotFoundError:
-            pass
-
-    raise FileNotFoundError(f"Could not find package.json under dir {HERE!s}")
-
-__version__ = _fetchVersion()
+import json
+from pathlib import Path
+
+__all__ = ["__version__"]
+
+def _fetchVersion():
+    HERE = Path(__file__).parent.resolve()
+
+    for settings in HERE.rglob("package.json"): 
+        try:
+            with settings.open() as f:
+                version = json.load(f)["version"]
+                return (
+                    version.replace("-alpha.", "a")
+                    .replace("-beta.", "b")
+                    .replace("-rc.", "rc")
+                )
+        except FileNotFoundError:
+            pass
+
+    raise FileNotFoundError(f"Could not find package.json under dir {HERE!s}")
+
+__version__ = _fetchVersion()
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/build_log.json` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/build_log.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9820120452310719%*

 * *Differences: {'0': "{'resolve': {'alias': {'@phosphor/algorithm$': "*

 * *      "'/home/frz/jupyterlab-variableInspector/node_modules/@lumino/algorithm/dist/index.js', "*

 * *      "'@phosphor/application$': "*

 * *      "'/home/frz/jupyterlab-variableInspector/node_modules/@lumino/application/dist/index.js', "*

 * *      "'@phosphor/commands$': "*

 * *      "'/home/frz/jupyterlab-variableInspector/node_modules/@lumino/commands/dist/index.js', "*

 * *      "'@phosphor/coreutils$': "*

 * *      "'/home/frz/jupyterlab-variableInspector/node_modules/@lumino […]*

```diff
@@ -84,525 +84,568 @@
                     "use": "file-loader"
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
             "hashFunction": "sha256",
-            "path": "/home/zfr/frz-jupyterlab-variableinspector/frz-jupyterlab-variableinspector/labextension/static",
+            "path": "/home/frz/jupyterlab-variableInspector/frz-jupyterlab-variableinspector/labextension/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
             },
             {
                 "_options": {
                     "exposes": {
-                        "./extension": "/home/zfr/frz-jupyterlab-variableinspector/lib/index.js",
-                        "./index": "/home/zfr/frz-jupyterlab-variableinspector/lib/index.js",
-                        "./style": "/home/zfr/frz-jupyterlab-variableinspector/style/index.js"
+                        "./extension": "/home/frz/jupyterlab-variableInspector/lib/index.js",
+                        "./index": "/home/frz/jupyterlab-variableInspector/lib/index.js",
+                        "./style": "/home/frz/jupyterlab-variableInspector/style/index.js"
                     },
                     "filename": "remoteEntry.[contenthash].js",
                     "library": {
                         "name": [
                             "_JUPYTERLAB",
                             "@feiranzhang/jupyterlab-variableinspector"
                         ],
                         "type": "var"
                     },
                     "name": "@feiranzhang/jupyterlab-variableinspector",
                     "shared": {
                         "@feiranzhang/jupyterlab-variableinspector": {
-                            "import": "/home/zfr/frz-jupyterlab-variableinspector/lib/index.js",
+                            "import": "/home/frz/jupyterlab-variableInspector/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.3"
+                            "version": "0.1.4"
+                        },
+                        "@jupyter/ydoc": {
+                            "import": false,
+                            "requiredVersion": "^0.2.3",
+                            "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.0.13",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.0.10",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.0.12"
+                            "requiredVersion": "^3.6.3"
+                        },
+                        "@jupyterlab/cell-toolbar": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3",
+                            "singleton": true
+                        },
+                        "@jupyterlab/cell-toolbar-extension": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.0.10",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.0.10",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
+                        },
+                        "@jupyterlab/collaboration": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3",
+                            "singleton": true
+                        },
+                        "@jupyterlab/collaboration-extension": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.0.10",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.0.12",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.0.7",
+                            "requiredVersion": "^5.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.0.14",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.14"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.0.13",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
+                        },
+                        "@jupyterlab/docprovider": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3",
+                            "singleton": true
+                        },
+                        "@jupyterlab/docprovider-extension": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.0.13",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.0.14",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.14"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.0.13",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.0.13",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.0.13",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.0.12",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.12"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.10"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.0.10",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.0.12",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.0.10",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.0.13",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mathjax2": {
                             "import": false,
-                            "requiredVersion": "^3.0.10"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mathjax2-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.0.17"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.0.7"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.0.13",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.0.7"
+                            "requiredVersion": "^4.6.3"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.0.12"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.10"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.0.12",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.0.10",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.0.10"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.0.10",
+                            "requiredVersion": "^6.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.0.12",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.0.7",
+                            "requiredVersion": "^3.6.3",
+                            "singleton": true
+                        },
+                        "@jupyterlab/shared-models": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.0.7",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.0.10",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.0.11",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.14"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.0.14"
+                            "requiredVersion": "^5.6.3",
+                            "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.0.14"
+                            "requiredVersion": "^5.6.3"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.0.12",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.0.10",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.0.8",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vdom": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vdom-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.13"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.0.10"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@lumino/algorithm": {
                             "import": false,
-                            "requiredVersion": "^1.3.3",
+                            "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
                             "import": false,
-                            "requiredVersion": "^1.13.1",
+                            "requiredVersion": "^1.31.4",
                             "singleton": true
                         },
                         "@lumino/commands": {
                             "import": false,
-                            "requiredVersion": "^1.12.0",
+                            "requiredVersion": "^1.19.0",
                             "singleton": true
                         },
                         "@lumino/coreutils": {
                             "import": false,
-                            "requiredVersion": "^1.5.3",
+                            "requiredVersion": "^1.11.0",
                             "singleton": true
                         },
                         "@lumino/datagrid": {},
                         "@lumino/disposable": {
                             "import": false,
-                            "requiredVersion": "^1.4.3",
+                            "requiredVersion": "^1.10.0",
                             "singleton": true
                         },
                         "@lumino/domutils": {
                             "import": false,
-                            "requiredVersion": "^1.2.3",
+                            "requiredVersion": "^1.8.0",
                             "singleton": true
                         },
                         "@lumino/dragdrop": {
                             "import": false,
-                            "requiredVersion": "^1.7.1",
+                            "requiredVersion": "^1.13.0",
                             "singleton": true
                         },
                         "@lumino/messaging": {
                             "import": false,
-                            "requiredVersion": "^1.4.3",
+                            "requiredVersion": "^1.10.0",
                             "singleton": true
                         },
                         "@lumino/properties": {
                             "import": false,
-                            "requiredVersion": "^1.2.3",
+                            "requiredVersion": "^1.8.0",
                             "singleton": true
                         },
                         "@lumino/signaling": {
                             "import": false,
-                            "requiredVersion": "^1.4.3",
+                            "requiredVersion": "^1.10.0",
                             "singleton": true
                         },
                         "@lumino/virtualdom": {
                             "import": false,
-                            "requiredVersion": "^1.8.0",
+                            "requiredVersion": "^1.14.0",
                             "singleton": true
                         },
                         "@lumino/widgets": {
                             "import": false,
-                            "requiredVersion": "^1.16.1",
+                            "requiredVersion": "^1.37.2",
                             "singleton": true
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
+                        },
+                        "yjs": {
+                            "import": false,
+                            "requiredVersion": "^13.5.17",
+                            "singleton": true
                         }
                     }
                 }
             },
             {}
         ],
         "resolve": {
             "alias": {
-                "@phosphor/algorithm$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/algorithm/dist/index.js",
-                "@phosphor/application$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/application/dist/index.js",
-                "@phosphor/commands$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/commands/dist/index.js",
-                "@phosphor/coreutils$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/coreutils/dist/index.node.js",
-                "@phosphor/disposable$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/disposable/dist/index.js",
-                "@phosphor/domutils$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/domutils/dist/index.js",
-                "@phosphor/dragdrop$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/dragdrop/dist/index.js",
-                "@phosphor/dragdrop/style": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/widgets/style",
-                "@phosphor/messaging$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/messaging/dist/index.js",
-                "@phosphor/properties$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/properties/dist/index.js",
-                "@phosphor/signaling": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/signaling/dist/index.js",
-                "@phosphor/virtualdom$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/virtualdom/dist/index.js",
-                "@phosphor/widgets$": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/widgets/dist/index.js",
-                "@phosphor/widgets/style": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/@lumino/widgets/style"
+                "@phosphor/algorithm$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/algorithm/dist/index.js",
+                "@phosphor/application$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/application/dist/index.js",
+                "@phosphor/commands$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/commands/dist/index.js",
+                "@phosphor/coreutils$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/coreutils/dist/index.node.js",
+                "@phosphor/disposable$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/disposable/dist/index.js",
+                "@phosphor/domutils$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/domutils/dist/index.js",
+                "@phosphor/dragdrop$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/dragdrop/dist/index.js",
+                "@phosphor/dragdrop/style": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/widgets/style",
+                "@phosphor/messaging$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/messaging/dist/index.js",
+                "@phosphor/properties$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/properties/dist/index.js",
+                "@phosphor/signaling": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/signaling/dist/index.js",
+                "@phosphor/virtualdom$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/virtualdom/dist/index.js",
+                "@phosphor/widgets$": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/widgets/dist/index.js",
+                "@phosphor/widgets/style": "/home/frz/jupyterlab-variableInspector/node_modules/@lumino/widgets/style"
             },
             "fallback": {
                 "buffer": false,
-                "path": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/path-browserify/index.js",
-                "process": "/home/zfr/frz-jupyterlab-variableinspector/node_modules/process/browser.js",
+                "path": "/home/frz/jupyterlab-variableInspector/node_modules/path-browserify/index.js",
+                "process": "/home/frz/jupyterlab-variableInspector/node_modules/process/browser.js",
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
             "poll": 500
         }
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/package.json` & `frz-jupyterlab-variableinspector-0.1.4/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9682539682539681%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.1.4'"}*

```diff
@@ -48,19 +48,14 @@
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.01eb97769bed74d9aebb.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "frz-jupyterlab-variableinspector/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension",
@@ -104,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.4"
 }
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/lib_index_js.d8a6a68cd2c54907e293.js` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/lib_index_js.92aa6d645091a304c589.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -892,28 +892,29 @@
 
 def _jupyterlab_variableinspector_deletevariable(x):
     exec("del %s" % x, globals())
 `;
                 Languages.r_script = `
 library(repr)
 
-.Last.value = 'wtf'
+.Last.value = ''
 
 .ls.objects = function (pos = 1, pattern, order.by, decreasing = FALSE, head = FALSE, n = 5) 
 {
-    napply <- function(names, fn) sapply(names, function(x) fn(get(x, 
-        pos = pos)))
+    napply <- function(names, fn) sapply(names, function(x) fn(get(x, pos = pos)))
     names <- ls(pos = pos, pattern = pattern)
-    
-    if (class(base::.Last.value) != 'json') .Last.value <<- base::.Last.value
-    names = c('.Last.value',names)
+
+    .Last.value <<- base::.Last.value
 
     if (length(names) == 0) {
         return(jsonlite::toJSON(data.frame()))
     }
+
+    names = c('.Last.value',names)
+
     obj.class <- napply(names, function(x) paste(as.character(class(x)),collapse=rawToChar(as.raw(c(92,110)))))
     obj.mode <- napply(names, mode)
     obj.type <- ifelse(is.na(obj.class), obj.mode, obj.class)
     
     obj.dim <- t(napply(names, function(x) as.numeric(dim(x))[1:2]))
     has_no_dim <- is.na(obj.dim)[1:length(names)]                        
     obj.dim[has_no_dim, 1] <- napply(names, length)[has_no_dim]
@@ -950,15 +951,15 @@
     names(out) <- c("varType", "varSize", "Rows", "Columns")
     out$varShape <- paste(out$Rows, " x ", out$Columns)
     out$varContent <- obj.content
     out$isMatrix <- FALSE
     out$varName <- row.names(out)
     out <- out[, !(names(out) %in% c("Rows", "Columns"))]
     rownames(out) <- NULL
-    print(out)
+    # print(out)
     if (!missing(order.by)) 
         out <- out[order(out[[order.by]], decreasing = decreasing), 
             ]
     if (head) 
         out <- head(out, n)
     jsonlite::toJSON(out)
 }
@@ -1569,8 +1570,8 @@
                 const __WEBPACK_DEFAULT_EXPORT__ = (_node_modules_css_loader_dist_cjs_js_index_css__WEBPACK_IMPORTED_MODULE_1__["default"].locals || {});
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.d8a6a68cd2c54907e293.js.map
+//# sourceMappingURL=lib_index_js.92aa6d645091a304c589.js.map
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/lib_index_js.d8a6a68cd2c54907e293.js.map` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/lib_index_js.92aa6d645091a304c589.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8428571428571429%*

 * *Differences: {"'file'": "'lib_index_js.92aa6d645091a304c589.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;AAA2C;AACE;AAC7C;AACA;AACA;AACO;AACP;AACA,6BAA6B,qDAAM;AACnC,8BAA8B,qDAAM;AACpC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,+BAA+B;AAC1E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,6CAA6C;AACxF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "lib_index_js.d8a6a68cd2c54907e293.js",
-    "mappings": ";;;;;;;;;;;;;;;;;;AAA2C;AACE;AAC7C;AACA;AACA;AACO;AACP;AACA,6BAA6B,qDAAM;AACnC,8BAA8B,qDAAM;AACpC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,+BAA+B;AAC1E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,6CAA6C;AACxF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8CAA8C,uDAAS;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,+DAAgB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA,6BAA6B,qDAAM;AACnC,8BAA8B,qDAAM;AACpC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,+DAAgB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AClR8D;AACV;AACgB;AACY;AACjC;AACuB;AACA;AAChB;AACE;AACH;AACrD;AACA;AACA;AACA,CAAC,gCAAgC;AACjC;AACA;AACA;AACA;AACA;AACA,eAAe,iEAAe,EAAE,oEAAe,EAAE,8DAAS;AAC1D,cAAc,+DAAyB;AACvC;AACA;AACA,4BAA4B,8DAAwB;AACpD;AACA;AACA;AACA;AACA,4BAA4B,+DAAa,GAAG,WAAW;AACvD;AACA;AACA;AACA;AACA,8BAA8B,sEAAsB;AACpD;AACA;AACA,+BAA+B,+DAAQ;AACvC;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT,0BAA0B,mBAAmB;AAC7C;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,+DAAyB,EAAE,gEAAe,EAAE,8DAAS;AACpE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA,0CAA0C,6DAAe,GAAG,SAAS;AACrE;AACA;AACA,mCAAmC,kEAAmB;AACtD,yBAAyB;AACzB,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4CAA4C,+DAAyB;AACrE;AACA;AACA;AACA;AACA,yBAAyB;AACzB;AACA;AACA,yBAAyB;AACzB,qBAAqB;AACrB;AACA;AACA;AACA,4CAA4C,kDAAY;AACxD;AACA;AACA;AACA,yBAAyB;AACzB;AACA,qBAAqB;AACrB,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,+DAAyB,EAAE,kEAAgB,EAAE,8DAAS;AACrE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sCAAsC,6DAAe,GAAG,SAAS;AACjE;AACA;AACA;AACA,+BAA+B,kEAAmB;AAClD,qBAAqB;AACrB,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wCAAwC,+DAAyB;AACjE;AACA;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB,iBAAiB;AACjB;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iEAAe,OAAO,EAAC;;;;;;;;;;;;;;;AC7PhB;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;;;AAGA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;;AAEA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oCAAoC,oCAAoC;AACxE;AACA;AACA,aAAa;AACb;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;;;;;;;;;;;;;;;;;AC3W2C;AAC3C;AACA;AACA;AACO;AACP;AACA,oCAAoC,qDAAM;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;AC9D0C;AACnC,sCAAsC,oDAAK;AAClD;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;ACnE+E;AACrC;AACD;AACG;AACsB;AACtC;AAC5B;AACA;AACA;AACA;AACA;AACA;AACA;AACO,+BAA+B,oDAAK;AAC3C;AACA;AACA;AACO,qCAAqC,mDAAM;AAClD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,qBAAqB;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wBAAwB,wEAAiB;AACzC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,yEAAkB;AAC9C;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,mEAAe,GAAG,eAAe;AACnE,mCAAmC,wEAAoB,GAAG,mBAAmB;AAC7E;AACA,gBAAgB,0DAAa;AAC7B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,6BAA6B,sDAAQ;AACrC;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA,mCAAmC,qBAAqB;AACxD;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB,kBAAkB;AAClB,kBAAkB;AAClB,oBAAoB;AACpB,mBAAmB;AACnB,oBAAoB;AACpB,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC,0BAA0B;;;;;;;;;;;;;;;;;;;ACxM3B;AACsH;AAC7B;AACzF,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F;AACA,gMAAgM,oFAAoF,2LAA2L;AAC/c;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;;;ACPvC;AACsH;AAC7B;AACW;AACpG,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F,0BAA0B,qFAAiC;AAC3D;AACA,8DAA8D,6BAA6B,qBAAqB,yCAAyC,KAAK,gCAAgC,gCAAgC,mBAAmB,kBAAkB,2CAA2C,KAAK,oEAAoE,wBAAwB,4CAA4C,mBAAmB,KAAK,mDAAmD,gDAAgD,KAAK,2CAA2C,gDAAgD,KAAK,sCAAsC,yCAAyC,yBAAyB,gDAAgD,sCAAsC,uBAAuB,0BAA0B,gCAAgC,KAAK,gCAAgC,yCAAyC,2CAA2C,uBAAuB,yBAAyB,KAAK,uCAAuC,yBAAyB,iBAAiB,KAAK,2CAA2C,6BAA6B,gDAAgD,KAAK,sCAAsC,yBAAyB,iBAAiB,KAAK,0CAA0C,uBAAuB,KAAK,WAAW,8EAA8E,KAAK,YAAY,WAAW,YAAY,OAAO,KAAK,YAAY,WAAW,UAAU,YAAY,OAAO,MAAM,YAAY,aAAa,WAAW,MAAM,KAAK,YAAY,OAAO,KAAK,YAAY,OAAO,KAAK,YAAY,aAAa,aAAa,aAAa,aAAa,aAAa,aAAa,OAAO,KAAK,YAAY,aAAa,aAAa,aAAa,OAAO,KAAK,YAAY,WAAW,MAAM,KAAK,YAAY,aAAa,OAAO,KAAK,YAAY,WAAW,OAAO,KAAK,YAAY,oDAAoD,sBAAsB,6BAA6B,qBAAqB,yCAAyC,KAAK,gCAAgC,gCAAgC,mBAAmB,kBAAkB,2CAA2C,KAAK,oEAAoE,wBAAwB,4CAA4C,mBAAmB,KAAK,mDAAmD,gDAAgD,KAAK,2CAA2C,gDAAgD,KAAK,sCAAsC,yCAAyC,yBAAyB,gDAAgD,sCAAsC,uBAAuB,0BAA0B,gCAAgC,KAAK,gCAAgC,yCAAyC,2CAA2C,uBAAuB,yBAAyB,KAAK,uCAAuC,yBAAyB,iBAAiB,KAAK,2CAA2C,6BAA6B,gDAAgD,KAAK,sCAAsC,yBAAyB,iBAAiB,KAAK,0CAA0C,uBAAuB,KAAK,uBAAuB;AACh/G;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;ACTkD;AACzF,YAAuF;;AAEvF;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,sFAAO;;;;AAIxB,iEAAe,6FAAc,MAAM",
+    "file": "lib_index_js.92aa6d645091a304c589.js",
+    "mappings": ";;;;;;;;;;;;;;;;;;AAA2C;AACE;AAC7C;AACA;AACA;AACO;AACP;AACA,6BAA6B,qDAAM;AACnC,8BAA8B,qDAAM;AACpC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,+BAA+B;AAC1E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,6CAA6C;AACxF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8CAA8C,uDAAS;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,+DAAgB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA,6BAA6B,qDAAM;AACnC,8BAA8B,qDAAM;AACpC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,+DAAgB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AClR8D;AACV;AACgB;AACY;AACjC;AACuB;AACA;AAChB;AACE;AACH;AACrD;AACA;AACA;AACA,CAAC,gCAAgC;AACjC;AACA;AACA;AACA;AACA;AACA,eAAe,iEAAe,EAAE,oEAAe,EAAE,8DAAS;AAC1D,cAAc,+DAAyB;AACvC;AACA;AACA,4BAA4B,8DAAwB;AACpD;AACA;AACA;AACA;AACA,4BAA4B,+DAAa,GAAG,WAAW;AACvD;AACA;AACA;AACA;AACA,8BAA8B,sEAAsB;AACpD;AACA;AACA,+BAA+B,+DAAQ;AACvC;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT,0BAA0B,mBAAmB;AAC7C;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,+DAAyB,EAAE,gEAAe,EAAE,8DAAS;AACpE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA,0CAA0C,6DAAe,GAAG,SAAS;AACrE;AACA;AACA,mCAAmC,kEAAmB;AACtD,yBAAyB;AACzB,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4CAA4C,+DAAyB;AACrE;AACA;AACA;AACA;AACA,yBAAyB;AACzB;AACA;AACA,yBAAyB;AACzB,qBAAqB;AACrB;AACA;AACA;AACA,4CAA4C,kDAAY;AACxD;AACA;AACA;AACA,yBAAyB;AACzB;AACA,qBAAqB;AACrB,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,+DAAyB,EAAE,kEAAgB,EAAE,8DAAS;AACrE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sCAAsC,6DAAe,GAAG,SAAS;AACjE;AACA;AACA;AACA,+BAA+B,kEAAmB;AAClD,qBAAqB;AACrB,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wCAAwC,+DAAyB;AACjE;AACA;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB,iBAAiB;AACjB;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iEAAe,OAAO,EAAC;;;;;;;;;;;;;;;AC7PhB;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;AAGA;AACA;;;AAGA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;;AAEA;;AAEA;AACA;AACA;AACA;;AAEA;;AAEA;AACA;AACA;;AAEA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oCAAoC,oCAAoC;AACxE;AACA;AACA,aAAa;AACb;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;;;;;;;;;;;;;;;;;AC5W2C;AAC3C;AACA;AACA;AACO;AACP;AACA,oCAAoC,qDAAM;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;AC9D0C;AACnC,sCAAsC,oDAAK;AAClD;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;ACnE+E;AACrC;AACD;AACG;AACsB;AACtC;AAC5B;AACA;AACA;AACA;AACA;AACA;AACA;AACO,+BAA+B,oDAAK;AAC3C;AACA;AACA;AACO,qCAAqC,mDAAM;AAClD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,qBAAqB;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wBAAwB,wEAAiB;AACzC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,yEAAkB;AAC9C;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,mEAAe,GAAG,eAAe;AACnE,mCAAmC,wEAAoB,GAAG,mBAAmB;AAC7E;AACA,gBAAgB,0DAAa;AAC7B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,6BAA6B,sDAAQ;AACrC;AACA;AACA;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA,mCAAmC,qBAAqB;AACxD;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB;AACnB,kBAAkB;AAClB,kBAAkB;AAClB,oBAAoB;AACpB,mBAAmB;AACnB,oBAAoB;AACpB,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC,0BAA0B;;;;;;;;;;;;;;;;;;;ACxM3B;AACsH;AAC7B;AACzF,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F;AACA,gMAAgM,oFAAoF,2LAA2L;AAC/c;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;;;ACPvC;AACsH;AAC7B;AACW;AACpG,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F,0BAA0B,qFAAiC;AAC3D;AACA,8DAA8D,6BAA6B,qBAAqB,yCAAyC,KAAK,gCAAgC,gCAAgC,mBAAmB,kBAAkB,2CAA2C,KAAK,oEAAoE,wBAAwB,4CAA4C,mBAAmB,KAAK,mDAAmD,gDAAgD,KAAK,2CAA2C,gDAAgD,KAAK,sCAAsC,yCAAyC,yBAAyB,gDAAgD,sCAAsC,uBAAuB,0BAA0B,gCAAgC,KAAK,gCAAgC,yCAAyC,2CAA2C,uBAAuB,yBAAyB,KAAK,uCAAuC,yBAAyB,iBAAiB,KAAK,2CAA2C,6BAA6B,gDAAgD,KAAK,sCAAsC,yBAAyB,iBAAiB,KAAK,0CAA0C,uBAAuB,KAAK,WAAW,8EAA8E,KAAK,YAAY,WAAW,YAAY,OAAO,KAAK,YAAY,WAAW,UAAU,YAAY,OAAO,MAAM,YAAY,aAAa,WAAW,MAAM,KAAK,YAAY,OAAO,KAAK,YAAY,OAAO,KAAK,YAAY,aAAa,aAAa,aAAa,aAAa,aAAa,aAAa,OAAO,KAAK,YAAY,aAAa,aAAa,aAAa,OAAO,KAAK,YAAY,WAAW,MAAM,KAAK,YAAY,aAAa,OAAO,KAAK,YAAY,WAAW,OAAO,KAAK,YAAY,oDAAoD,sBAAsB,6BAA6B,qBAAqB,yCAAyC,KAAK,gCAAgC,gCAAgC,mBAAmB,kBAAkB,2CAA2C,KAAK,oEAAoE,wBAAwB,4CAA4C,mBAAmB,KAAK,mDAAmD,gDAAgD,KAAK,2CAA2C,gDAAgD,KAAK,sCAAsC,yCAAyC,yBAAyB,gDAAgD,sCAAsC,uBAAuB,0BAA0B,gCAAgC,KAAK,gCAAgC,yCAAyC,2CAA2C,uBAAuB,yBAAyB,KAAK,uCAAuC,yBAAyB,iBAAiB,KAAK,2CAA2C,6BAA6B,gDAAgD,KAAK,sCAAsC,yBAAyB,iBAAiB,KAAK,0CAA0C,uBAAuB,KAAK,uBAAuB;AACh/G;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;ACTkD;AACzF,YAAuF;;AAEvF;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,sFAAO;;;;AAIxB,iEAAe,6FAAc,MAAM",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@feiranzhang/jupyterlab-variableinspector/./lib/handler.js",
         "webpack://@feiranzhang/jupyterlab-variableinspector/./lib/index.js",
         "webpack://@feiranzhang/jupyterlab-variableinspector/./lib/inspectorscripts.js",
         "webpack://@feiranzhang/jupyterlab-variableinspector/./lib/kernelconnector.js",
@@ -13,15 +13,15 @@
         "webpack://@feiranzhang/jupyterlab-variableinspector/./style/base.css",
         "webpack://@feiranzhang/jupyterlab-variableinspector/./style/index.css",
         "webpack://@feiranzhang/jupyterlab-variableinspector/./style/index.css?0140"
     ],
     "sourcesContent": [
         "import { Signal } from '@lumino/signaling';\nimport { JSONModel } from '@lumino/datagrid';\n/**\n * An object that handles code inspection.\n */\nexport class VariableInspectionHandler {\n    constructor(options) {\n        this._disposed = new Signal(this);\n        this._inspected = new Signal(this);\n        this._isDisposed = false;\n        /*\n         * Handle query response. Emit new signal containing the IVariableInspector.IInspectorUpdate object.\n         * (TODO: query resp. could be forwarded to panel directly)\n         */\n        this._handleQueryResponse = (response) => {\n            const msgType = response.header.msg_type;\n            switch (msgType) {\n                case 'execute_result': {\n                    const payload = response.content;\n                    let content = payload.data['text/plain'];\n                    if (content.slice(0, 1) === \"'\" || content.slice(0, 1) === '\"') {\n                        content = content.slice(1, -1);\n                        content = content.replace(/\\\\\"/g, '\"').replace(/\\\\'/g, \"'\");\n                    }\n                    const update = JSON.parse(content);\n                    const title = {\n                        contextName: '',\n                        kernelName: this._connector.kernelName || '',\n                    };\n                    this._inspected.emit({ title: title, payload: update });\n                    break;\n                }\n                case 'display_data': {\n                    const payloadDisplay = response.content;\n                    let contentDisplay = payloadDisplay.data['text/plain'];\n                    if (contentDisplay.slice(0, 1) === \"'\" ||\n                        contentDisplay.slice(0, 1) === '\"') {\n                        contentDisplay = contentDisplay.slice(1, -1);\n                        contentDisplay = contentDisplay\n                            .replace(/\\\\\"/g, '\"')\n                            .replace(/\\\\'/g, \"'\");\n                    }\n                    const updateDisplay = JSON.parse(contentDisplay);\n                    const titleDisplay = {\n                        contextName: '',\n                        kernelName: this._connector.kernelName || '',\n                    };\n                    this._inspected.emit({ title: titleDisplay, payload: updateDisplay });\n                    break;\n                }\n                default:\n                    break;\n            }\n        };\n        /*\n         * Invokes a inspection if the signal emitted from specified session is an 'execute_input' msg.\n         */\n        this._queryCall = (sess, msg) => {\n            const msgType = msg.header.msg_type;\n            switch (msgType) {\n                case 'execute_input': {\n                    const code = msg.content.code;\n                    if (!(code === this._queryCommand) &&\n                        !(code === this._matrixQueryCommand) &&\n                        !code.startsWith(this._widgetQueryCommand)) {\n                        this.performInspection();\n                    }\n                    break;\n                }\n                default:\n                    break;\n            }\n        };\n        this._id = options.id;\n        this._connector = options.connector;\n        this._rendermime = options.rendermime;\n        this._queryCommand = options.queryCommand;\n        this._matrixQueryCommand = options.matrixQueryCommand;\n        this._widgetQueryCommand = options.widgetQueryCommand;\n        this._deleteCommand = options.deleteCommand;\n        this._initScript = options.initScript;\n        this._ready = this._connector.ready.then(() => {\n            this._initOnKernel().then((msg) => {\n                this._connector.iopubMessage.connect(this._queryCall);\n                return;\n            });\n        });\n        this._connector.kernelRestarted.connect((sender, kernelReady) => {\n            const title = {\n                contextName: '<b>Restarting kernel...</b> ',\n            };\n            this._inspected.emit({\n                title: title,\n                payload: [],\n            });\n            this._ready = kernelReady.then(() => {\n                this._initOnKernel().then((msg) => {\n                    this._connector.iopubMessage.connect(this._queryCall);\n                    this.performInspection();\n                });\n            });\n        });\n    }\n    get id() {\n        return this._id;\n    }\n    get rendermime() {\n        return this._rendermime;\n    }\n    /**\n     * A signal emitted when the handler is disposed.\n     */\n    get disposed() {\n        return this._disposed;\n    }\n    get isDisposed() {\n        return this._isDisposed;\n    }\n    get ready() {\n        return this._ready;\n    }\n    /**\n     * A signal emitted when an inspector value is generated.\n     */\n    get inspected() {\n        return this._inspected;\n    }\n    /**\n     * Performs an inspection by sending an execute request with the query command to the kernel.\n     */\n    performInspection() {\n        const content = {\n            code: this._queryCommand,\n            stop_on_error: false,\n            store_history: false,\n        };\n        this._connector.fetch(content, this._handleQueryResponse);\n    }\n    /**\n     * Performs an inspection of a Jupyter Widget\n     */\n    performWidgetInspection(varName) {\n        const request = {\n            code: this._widgetQueryCommand + '(' + varName + ')',\n            stop_on_error: false,\n            store_history: false,\n        };\n        return this._connector.execute(request);\n    }\n    /**\n     * Performs an inspection of the specified matrix.\n     */\n    performMatrixInspection(varName, maxRows = 100000) {\n        const request = {\n            code: this._matrixQueryCommand + '(' + varName + ', ' + maxRows + ')',\n            stop_on_error: false,\n            store_history: false,\n        };\n        const con = this._connector;\n        return new Promise((resolve, reject) => {\n            con.fetch(request, (response) => {\n                const msgType = response.header.msg_type;\n                switch (msgType) {\n                    case 'execute_result': {\n                        const payload = response.content;\n                        let content = payload.data['text/plain'];\n                        content = content.replace(/^'|'$/g, '');\n                        content = content.replace(/\\\\\"/g, '\"');\n                        content = content.replace(/\\\\'/g, \"\\\\\\\\'\");\n                        const modelOptions = JSON.parse(content);\n                        const jsonModel = new JSONModel(modelOptions);\n                        resolve(jsonModel);\n                        break;\n                    }\n                    case 'error':\n                        console.log(response);\n                        reject(\"Kernel error on 'matrixQuery' call!\");\n                        break;\n                    default:\n                        break;\n                }\n            });\n        });\n    }\n    /**\n     * Send a kernel request to delete a variable from the global environment\n     */\n    performDelete(varName) {\n        const content = {\n            code: this._deleteCommand + \"('\" + varName + \"')\",\n            stop_on_error: false,\n            store_history: false,\n        };\n        this._connector.fetch(content, this._handleQueryResponse);\n    }\n    /*\n     * Disposes the kernel connector.\n     */\n    dispose() {\n        if (this.isDisposed) {\n            return;\n        }\n        this._isDisposed = true;\n        this._disposed.emit(void 0);\n        Signal.clearData(this);\n    }\n    /**\n     * Initializes the kernel by running the set up script located at _initScriptPath.\n     */\n    _initOnKernel() {\n        const content = {\n            code: this._initScript,\n            stop_on_error: false,\n            silent: true,\n        };\n        return this._connector.fetch(content, () => {\n            //no op\n        });\n    }\n}\nexport class DummyHandler {\n    constructor(connector) {\n        this._isDisposed = false;\n        this._disposed = new Signal(this);\n        this._inspected = new Signal(this);\n        this._rendermime = null;\n        this._connector = connector;\n    }\n    get disposed() {\n        return this._disposed;\n    }\n    get isDisposed() {\n        return this._isDisposed;\n    }\n    get inspected() {\n        return this._inspected;\n    }\n    get rendermime() {\n        return this._rendermime;\n    }\n    dispose() {\n        if (this.isDisposed) {\n            return;\n        }\n        this._isDisposed = true;\n        this._disposed.emit(void 0);\n        Signal.clearData(this);\n    }\n    performInspection() {\n        const title = {\n            contextName: '. <b>Language currently not supported.</b> ',\n            kernelName: this._connector.kernelName || '',\n        };\n        this._inspected.emit({\n            title: title,\n            payload: [],\n        });\n    }\n    performMatrixInspection(varName, maxRows) {\n        return new Promise((resolve, reject) => {\n            reject('Cannot inspect matrices w/ the DummyHandler!');\n        });\n    }\n    performWidgetInspection(varName) {\n        const request = {\n            code: '',\n            stop_on_error: false,\n            store_history: false,\n        };\n        return this._connector.execute(request);\n    }\n    performDelete(varName) {\n        //noop\n    }\n}\n",
         "import { VariableInspectorPanel, } from './variableinspector';\nimport { KernelConnector } from './kernelconnector';\nimport { VariableInspectionHandler, DummyHandler } from './handler';\nimport { VariableInspectorManager, IVariableInspectorManager } from './manager';\nimport { Languages } from './inspectorscripts';\nimport { ICommandPalette, WidgetTracker } from '@jupyterlab/apputils';\nimport { ILabShell, ILayoutRestorer, } from '@jupyterlab/application';\nimport { IConsoleTracker } from '@jupyterlab/console';\nimport { INotebookTracker } from '@jupyterlab/notebook';\nimport { listIcon } from '@jupyterlab/ui-components';\nvar CommandIDs;\n(function (CommandIDs) {\n    CommandIDs.open = 'variableinspector:open';\n})(CommandIDs || (CommandIDs = {}));\n/**\n * A service providing variable introspection.\n */\nconst variableinspector = {\n    id: 'jupyterlab_variableinspector',\n    requires: [ICommandPalette, ILayoutRestorer, ILabShell],\n    provides: IVariableInspectorManager,\n    autoStart: true,\n    activate: (app, palette, restorer, labShell) => {\n        const manager = new VariableInspectorManager();\n        const category = 'Variable Inspector';\n        const command = CommandIDs.open;\n        const label = 'Open Variable Inspector';\n        const namespace = 'variableinspector';\n        const tracker = new WidgetTracker({ namespace });\n        /**\n         * Create and track a new inspector.\n         */\n        function newPanel() {\n            const panel = new VariableInspectorPanel();\n            panel.id = 'jp-variableinspector';\n            panel.title.label = 'Variable Inspector';\n            panel.title.icon = listIcon;\n            panel.title.closable = true;\n            panel.disposed.connect(() => {\n                if (manager.panel === panel) {\n                    manager.panel = null;\n                }\n            });\n            //Track the inspector panel\n            tracker.add(panel);\n            return panel;\n        }\n        // Enable state restoration\n        restorer.restore(tracker, {\n            command,\n            args: () => null,\n            name: () => 'variableinspector',\n        });\n        // Add command to palette\n        app.commands.addCommand(command, {\n            label,\n            execute: () => {\n                if (!manager.panel || manager.panel.isDisposed) {\n                    manager.panel = newPanel();\n                }\n                if (!manager.panel.isAttached) {\n                    labShell.add(manager.panel, 'main');\n                }\n                if (manager.source) {\n                    manager.source.performInspection();\n                }\n                labShell.activateById(manager.panel.id);\n            },\n        });\n        palette.addItem({ command, category });\n        console.log('JupyterLab extension jupyterlab_variableinspector is activated!');\n        return manager;\n    },\n};\n/**\n * An extension that registers consoles for variable inspection.\n */\nconst consoles = {\n    id: 'jupyterlab-variableinspector:consoles',\n    requires: [IVariableInspectorManager, IConsoleTracker, ILabShell],\n    autoStart: true,\n    activate: (app, manager, consoles, labShell) => {\n        const handlers = {};\n        /**\n         * Subscribes to the creation of new consoles. If a new notebook is created, build a new handler for the consoles.\n         * Adds a promise for a instanced handler to the 'handlers' collection.\n         */\n        consoles.widgetAdded.connect((sender, consolePanel) => {\n            if (manager.hasHandler(consolePanel.sessionContext.path)) {\n                handlers[consolePanel.id] = new Promise((resolve, reject) => {\n                    resolve(manager.getHandler(consolePanel.sessionContext.path));\n                });\n            }\n            else {\n                handlers[consolePanel.id] = new Promise((resolve, reject) => {\n                    const session = consolePanel.sessionContext;\n                    // Create connector and init w script if it exists for kernel type.\n                    const connector = new KernelConnector({ session });\n                    const scripts = connector.ready.then(() => {\n                        return connector.kernelLanguage.then((lang) => {\n                            return Languages.getScript(lang);\n                        });\n                    });\n                    scripts.then((result) => {\n                        const initScript = result.initScript;\n                        const queryCommand = result.queryCommand;\n                        const matrixQueryCommand = result.matrixQueryCommand;\n                        const widgetQueryCommand = result.widgetQueryCommand;\n                        const deleteCommand = result.deleteCommand;\n                        const options = {\n                            queryCommand: queryCommand,\n                            matrixQueryCommand: matrixQueryCommand,\n                            widgetQueryCommand,\n                            deleteCommand: deleteCommand,\n                            connector: connector,\n                            initScript: initScript,\n                            id: session.path,\n                        };\n                        const handler = new VariableInspectionHandler(options);\n                        manager.addHandler(handler);\n                        consolePanel.disposed.connect(() => {\n                            delete handlers[consolePanel.id];\n                            handler.dispose();\n                        });\n                        handler.ready.then(() => {\n                            resolve(handler);\n                        });\n                    });\n                    //Otherwise log error message.\n                    scripts.catch((result) => {\n                        console.log(result);\n                        const handler = new DummyHandler(connector);\n                        consolePanel.disposed.connect(() => {\n                            delete handlers[consolePanel.id];\n                            handler.dispose();\n                        });\n                        resolve(handler);\n                    });\n                });\n            }\n        });\n        /**\n         * If focus window changes, checks whether new focus widget is a console.\n         * In that case, retrieves the handler associated to the console after it has been\n         * initialized and updates the manager with it.\n         */\n        labShell.currentChanged.connect((sender, args) => {\n            const widget = args.newValue;\n            if (!widget || !consoles.has(widget)) {\n                return;\n            }\n            const future = handlers[widget.id];\n            future.then((source) => {\n                if (source) {\n                    manager.source = source;\n                    manager.source.performInspection();\n                }\n            });\n        });\n        app.contextMenu.addItem({\n            command: CommandIDs.open,\n            selector: '.jp-CodeConsole',\n        });\n    },\n};\n/**\n * An extension that registers notebooks for variable inspection.\n */\nconst notebooks = {\n    id: 'jupyterlab-variableinspector:notebooks',\n    requires: [IVariableInspectorManager, INotebookTracker, ILabShell],\n    autoStart: true,\n    activate: (app, manager, notebooks, labShell) => {\n        const handlers = {};\n        /**\n         * Subscribes to the creation of new notebooks. If a new notebook is created, build a new handler for the notebook.\n         * Adds a promise for a instanced handler to the 'handlers' collection.\n         */\n        notebooks.widgetAdded.connect((sender, nbPanel) => {\n            //A promise that resolves after the initialization of the handler is done.\n            handlers[nbPanel.id] = new Promise((resolve, reject) => {\n                const session = nbPanel.sessionContext;\n                const connector = new KernelConnector({ session });\n                const rendermime = nbPanel.content.rendermime;\n                const scripts = connector.ready.then(() => {\n                    return connector.kernelLanguage.then((lang) => {\n                        return Languages.getScript(lang);\n                    });\n                });\n                scripts.then((result) => {\n                    const initScript = result.initScript;\n                    const queryCommand = result.queryCommand;\n                    const matrixQueryCommand = result.matrixQueryCommand;\n                    const widgetQueryCommand = result.widgetQueryCommand;\n                    const deleteCommand = result.deleteCommand;\n                    const options = {\n                        queryCommand: queryCommand,\n                        matrixQueryCommand: matrixQueryCommand,\n                        widgetQueryCommand,\n                        deleteCommand: deleteCommand,\n                        connector: connector,\n                        rendermime,\n                        initScript: initScript,\n                        id: session.path,\n                    };\n                    const handler = new VariableInspectionHandler(options);\n                    manager.addHandler(handler);\n                    nbPanel.disposed.connect(() => {\n                        delete handlers[nbPanel.id];\n                        handler.dispose();\n                    });\n                    handler.ready.then(() => {\n                        resolve(handler);\n                    });\n                });\n                //Otherwise log error message.\n                scripts.catch((result) => {\n                    reject(result);\n                });\n            });\n        });\n        /**\n         * If focus window changes, checks whether new focus widget is a notebook.\n         * In that case, retrieves the handler associated to the notebook after it has been\n         * initialized and updates the manager with it.\n         */\n        labShell.currentChanged.connect((sender, args) => {\n            const widget = args.newValue;\n            if (!widget || !notebooks.has(widget)) {\n                return;\n            }\n            const future = handlers[widget.id];\n            future.then((source) => {\n                if (source) {\n                    manager.source = source;\n                    manager.source.performInspection();\n                }\n            });\n        });\n        app.contextMenu.addItem({\n            command: CommandIDs.open,\n            selector: '.jp-Notebook',\n        });\n    },\n};\n/**\n * Export the plugins as default.\n */\nconst plugins = [\n    variableinspector,\n    consoles,\n    notebooks,\n];\nexport default plugins;\n",
-        "export class Languages {\n    static getScript(lang) {\n        return new Promise((resolve, reject) => {\n            if (lang in Languages.scripts) {\n                resolve(Languages.scripts[lang]);\n            }\n            else {\n                reject('Language ' + lang + ' not supported yet!');\n            }\n        });\n    }\n}\n/**\n * Init and query script for supported languages.\n */\nLanguages.py_script = `import json\nimport sys\nfrom IPython import get_ipython\nfrom IPython.core.magics.namespace import NamespaceMagics\n\n\n_jupyterlab_variableinspector_nms = NamespaceMagics()\n_jupyterlab_variableinspector_Jupyter = get_ipython()\n_jupyterlab_variableinspector_nms.shell = _jupyterlab_variableinspector_Jupyter.kernel.shell\n\n__np = None\n__pd = None\n__pyspark = None\n__tf = None\n__K = None\n__torch = None\n__ipywidgets = None\n\n\ndef _check_imported():\n    global __np, __pd, __pyspark, __tf, __K, __torch, __ipywidgets\n\n    if 'numpy' in sys.modules:\n        # don't really need the try\n        import numpy as __np\n\n    if 'pandas' in sys.modules:\n        import pandas as __pd\n\n    if 'pyspark' in sys.modules:\n        import pyspark as __pyspark\n\n    if 'tensorflow' in sys.modules or 'keras' in sys.modules:\n        import tensorflow as __tf\n\n        try:\n            import keras.backend as __K\n        except ImportError:\n            try:\n                import tensorflow.keras.backend as __K\n            except ImportError:\n                __K = None\n\n    if 'torch' in sys.modules:\n        import torch as __torch\n\n    if 'ipywidgets' in sys.modules:\n        import ipywidgets as __ipywidgets\n\n\ndef _jupyterlab_variableinspector_getsizeof(x):\n    if type(x).__name__ in ['ndarray', 'Series']:\n        return x.nbytes\n    elif __pyspark and isinstance(x, __pyspark.sql.DataFrame):\n        return \"?\"\n    elif __tf and isinstance(x, __tf.Variable):\n        return \"?\"\n    elif __torch and isinstance(x, __torch.Tensor):\n        return x.element_size() * x.nelement()\n    elif __pd and type(x).__name__ == 'DataFrame':\n        return x.memory_usage().sum()\n    else:\n        return sys.getsizeof(x)\n\n\ndef _jupyterlab_variableinspector_getshapeof(x):\n    if __pd and isinstance(x, __pd.DataFrame):\n        return \"%d rows x %d cols\" % x.shape\n    if __pd and isinstance(x, __pd.Series):\n        return \"%d rows\" % x.shape\n    if __np and isinstance(x, __np.ndarray):\n        shape = \" x \".join([str(i) for i in x.shape])\n        return \"%s\" % shape\n    if __pyspark and isinstance(x, __pyspark.sql.DataFrame):\n        return \"? rows x %d cols\" % len(x.columns)\n    if __tf and isinstance(x, __tf.Variable):\n        shape = \" x \".join([str(int(i)) for i in x.shape])\n        return \"%s\" % shape\n    if __tf and isinstance(x, __tf.Tensor):\n        shape = \" x \".join([str(int(i)) for i in x.shape])\n        return \"%s\" % shape\n    if __torch and isinstance(x, __torch.Tensor):\n        shape = \" x \".join([str(int(i)) for i in x.shape])\n        return \"%s\" % shape\n    if isinstance(x, list):\n        return \"%s\" % len(x)\n    if isinstance(x, dict):\n        return \"%s keys\" % len(x)\n    return ''\n\n\ndef _jupyterlab_variableinspector_getcontentof(x):\n    # returns content in a friendly way for python variables\n    # pandas and numpy\n    if __pd and isinstance(x, __pd.DataFrame):\n        colnames = ', '.join(x.columns.map(str))\n        content = \"Columns: %s\" % colnames\n    elif __pd and isinstance(x, __pd.Series):\n        content = str(x.values).replace(\" \", \", \")[1:-1]\n        content = content.replace(\"\\\\n\", \"\")\n    elif __np and isinstance(x, __np.ndarray):\n        content = x.__repr__()\n    elif __torch and isinstance(x, __torch.Tensor):\n        if x.nelement() < 1048576:\n            content = x.__repr__()\n        else:\n            content = 'too big'\n    else:\n        content = str(x)\n\n    if len(content) > 50:\n        return content[:50] + \" ...\"\n    else:\n        return content\n\n\ndef _jupyterlab_variableinspector_is_matrix(x):\n    # True if type(x).__name__ in [\"DataFrame\", \"ndarray\", \"Series\"] else False\n    if __pd and isinstance(x, __pd.DataFrame):\n        return True\n    if __pd and isinstance(x, __pd.Series):\n        return True\n    if __np and isinstance(x, __np.ndarray) and len(x.shape) <= 2:\n        return True\n    if __pyspark and isinstance(x, __pyspark.sql.DataFrame):\n        return True\n    if __tf and isinstance(x, __tf.Variable) and len(x.shape) <= 2:\n        return True\n    if __tf and isinstance(x, __tf.Tensor) and len(x.shape) <= 2:\n        return True\n    if __torch and isinstance(x, __torch.Tensor) and len(x.shape) <= 2:\n        return True\n    if isinstance(x, list):\n        return True\n    return False\n\n\ndef _jupyterlab_variableinspector_is_widget(x):\n    return __ipywidgets and issubclass(x, __ipywidgets.DOMWidget)\n\n\ndef _jupyterlab_variableinspector_dict_list():\n    _check_imported()\n    def keep_cond(v):\n        try:\n            obj = eval(v)\n            if isinstance(obj, (str, list, dict)):\n                return True\n            if __tf and isinstance(obj, __tf.Variable):\n                return True\n            if __torch and isinstance(obj, __torch.Tensor):\n                return True\n            if __pd and __pd is not None and (\n                isinstance(obj, __pd.core.frame.DataFrame)\n                or isinstance(obj, __pd.core.series.Series)):\n                return True\n            if v in ['__np', '__pd', '__pyspark', '__tf', '__K', '__torch', '__ipywidgets']:\n                return obj is not None\n            if str(obj)[0] == \"<\":\n                return False\n            if str(obj).startswith(\"_Feature\"):\n                # removes tf/keras objects\n                return False\n            return True\n        except:\n            return False\n    values = _jupyterlab_variableinspector_nms.who_ls()\n    if 'jlvi_brief' in values:\n        vardic = [\n            {\n                'varName': _v,\n                'varType': type(eval(_v)).__name__, \n                'varSize': '0', \n                'varShape': str(_jupyterlab_variableinspector_getshapeof(eval(_v))), \n                'varContent': '', \n                'isMatrix': False,\n                'isWidget': _jupyterlab_variableinspector_is_widget(type(eval(_v)))\n            }\n            for _v in values if keep_cond(_v)\n        ]\n    else:\n        vardic = [\n            {\n                'varName': _v,\n                'varType': type(eval(_v)).__name__, \n                'varSize': '0', \n                'varShape': str(_jupyterlab_variableinspector_getshapeof(eval(_v))), \n                'varContent': str(_jupyterlab_variableinspector_getcontentof(eval(_v))), \n                'isMatrix': False,\n                'isWidget': _jupyterlab_variableinspector_is_widget(type(eval(_v)))\n            }\n            for _v in values if keep_cond(_v)\n        ]\n    return json.dumps(vardic, ensure_ascii=False)\n\n\ndef _jupyterlab_variableinspector_getmatrixcontent(x, max_rows=10000):\n    # to do: add something to handle this in the future\n    threshold = max_rows\n\n    if __pd and __pyspark and isinstance(x, __pyspark.sql.DataFrame):\n        df = x.limit(threshold).toPandas()\n        return _jupyterlab_variableinspector_getmatrixcontent(df.copy())\n    elif __np and __pd and type(x).__name__ == \"DataFrame\":\n        if threshold is not None:\n            x = x.head(threshold)\n        x.columns = x.columns.map(str)\n        return x.to_json(orient=\"table\", default_handler=_jupyterlab_variableinspector_default, force_ascii=False)\n    elif __np and __pd and type(x).__name__ == \"Series\":\n        if threshold is not None:\n            x = x.head(threshold)\n        return x.to_json(orient=\"table\", default_handler=_jupyterlab_variableinspector_default, force_ascii=False)\n    elif __np and __pd and type(x).__name__ == \"ndarray\":\n        df = __pd.DataFrame(x)\n        return _jupyterlab_variableinspector_getmatrixcontent(df)\n    elif __tf and (isinstance(x, __tf.Variable) or isinstance(x, __tf.Tensor)):\n        df = __K.get_value(x)\n        return _jupyterlab_variableinspector_getmatrixcontent(df)\n    elif __torch and isinstance(x, __torch.Tensor):\n        df = x.cpu().numpy()\n        return _jupyterlab_variableinspector_getmatrixcontent(df)\n    elif isinstance(x, list):\n        s = __pd.Series(x)\n        return _jupyterlab_variableinspector_getmatrixcontent(s)\n\n\ndef _jupyterlab_variableinspector_displaywidget(widget):\n    display(widget)\n\n\ndef _jupyterlab_variableinspector_default(o):\n    if isinstance(o, __np.number): return int(o)  \n    raise TypeError\n\n\ndef _jupyterlab_variableinspector_deletevariable(x):\n    exec(\"del %s\" % x, globals())\n`;\nLanguages.r_script = `\nlibrary(repr)\n\n.Last.value = 'wtf'\n\n.ls.objects = function (pos = 1, pattern, order.by, decreasing = FALSE, head = FALSE, n = 5) \n{\n    napply <- function(names, fn) sapply(names, function(x) fn(get(x, \n        pos = pos)))\n    names <- ls(pos = pos, pattern = pattern)\n    \n    if (class(base::.Last.value) != 'json') .Last.value <<- base::.Last.value\n    names = c('.Last.value',names)\n\n    if (length(names) == 0) {\n        return(jsonlite::toJSON(data.frame()))\n    }\n    obj.class <- napply(names, function(x) paste(as.character(class(x)),collapse=rawToChar(as.raw(c(92,110)))))\n    obj.mode <- napply(names, mode)\n    obj.type <- ifelse(is.na(obj.class), obj.mode, obj.class)\n    \n    obj.dim <- t(napply(names, function(x) as.numeric(dim(x))[1:2]))\n    has_no_dim <- is.na(obj.dim)[1:length(names)]                        \n    obj.dim[has_no_dim, 1] <- napply(names, length)[has_no_dim]\n    \n    obj.size = rep(0,length(names))\n    \n    obj.content = rep(\"NA\", length(names))\n    if (!\"jlvi_brief\" %in% names) {\n        obj.content <- napply(names, function(x) {\n            a = capture.output(try({str(x, max.level = 1, list.len = 3)}))\n            b = lapply(a[1:min(length(a), 4)], function(x) {\n                paste(substring(x, 1, 30), ifelse(nchar(x) > 30, \"...\", \"\"))\n            })\n            paste(b, collapse = rawToChar(as.raw(c(92, 110))))\n        })\n    }\n    \n    is_function <- (obj.type == \"function\")\n    if (!\"jlvi_brief\" %in% names) {\n        obj.content[is_function] <- napply(names[is_function], function(x) {\n            a = strsplit(repr_text(x), rawToChar(as.raw(c(92, 110))))[[1]]\n            if (length(a) >= 4) \n                a[[4]] = \"...\"\n            b = lapply(a[1:min(length(a), 4)], function(x) {\n                paste(substring(x, 1, 30), ifelse(nchar(x) > 30, \"...\", \"\"))\n            })\n            paste(b, collapse = rawToChar(as.raw(c(92, 110))))\n        })\n    }\n    \n    obj.content <- unlist(obj.content, use.names = FALSE)\n    \n    out <- data.frame(obj.type, obj.size, obj.dim)\n    names(out) <- c(\"varType\", \"varSize\", \"Rows\", \"Columns\")\n    out$varShape <- paste(out$Rows, \" x \", out$Columns)\n    out$varContent <- obj.content\n    out$isMatrix <- FALSE\n    out$varName <- row.names(out)\n    out <- out[, !(names(out) %in% c(\"Rows\", \"Columns\"))]\n    rownames(out) <- NULL\n    print(out)\n    if (!missing(order.by)) \n        out <- out[order(out[[order.by]], decreasing = decreasing), \n            ]\n    if (head) \n        out <- head(out, n)\n    jsonlite::toJSON(out)\n}\n\n.deleteVariable <- function(x) {\n    remove(list=c(x), envir=.GlobalEnv)\n}\n      `;\nLanguages.scripts = {\n    python3: {\n        initScript: Languages.py_script,\n        queryCommand: '_jupyterlab_variableinspector_dict_list()',\n        matrixQueryCommand: '_jupyterlab_variableinspector_getmatrixcontent',\n        widgetQueryCommand: '_jupyterlab_variableinspector_displaywidget',\n        deleteCommand: '_jupyterlab_variableinspector_deletevariable',\n    },\n    python2: {\n        initScript: Languages.py_script,\n        queryCommand: '_jupyterlab_variableinspector_dict_list()',\n        matrixQueryCommand: '_jupyterlab_variableinspector_getmatrixcontent',\n        widgetQueryCommand: '_jupyterlab_variableinspector_displaywidget',\n        deleteCommand: '_jupyterlab_variableinspector_deletevariable',\n    },\n    python: {\n        initScript: Languages.py_script,\n        queryCommand: '_jupyterlab_variableinspector_dict_list()',\n        matrixQueryCommand: '_jupyterlab_variableinspector_getmatrixcontent',\n        widgetQueryCommand: '_jupyterlab_variableinspector_displaywidget',\n        deleteCommand: '_jupyterlab_variableinspector_deletevariable',\n    },\n    R: {\n        initScript: Languages.r_script,\n        queryCommand: '.ls.objects()',\n        matrixQueryCommand: '.ls.objects',\n        widgetQueryCommand: 'TODO',\n        deleteCommand: '.deleteVariable',\n    },\n    scala: {\n        initScript: '_root_.almond.api.JupyterAPIHolder.value.VariableInspector.init()',\n        queryCommand: '_root_.almond.api.JupyterAPIHolder.value.VariableInspector.dictList()',\n        matrixQueryCommand: '',\n        widgetQueryCommand: '',\n        deleteCommand: '',\n    },\n};\n",
+        "export class Languages {\n    static getScript(lang) {\n        return new Promise((resolve, reject) => {\n            if (lang in Languages.scripts) {\n                resolve(Languages.scripts[lang]);\n            }\n            else {\n                reject('Language ' + lang + ' not supported yet!');\n            }\n        });\n    }\n}\n/**\n * Init and query script for supported languages.\n */\nLanguages.py_script = `import json\nimport sys\nfrom IPython import get_ipython\nfrom IPython.core.magics.namespace import NamespaceMagics\n\n\n_jupyterlab_variableinspector_nms = NamespaceMagics()\n_jupyterlab_variableinspector_Jupyter = get_ipython()\n_jupyterlab_variableinspector_nms.shell = _jupyterlab_variableinspector_Jupyter.kernel.shell\n\n__np = None\n__pd = None\n__pyspark = None\n__tf = None\n__K = None\n__torch = None\n__ipywidgets = None\n\n\ndef _check_imported():\n    global __np, __pd, __pyspark, __tf, __K, __torch, __ipywidgets\n\n    if 'numpy' in sys.modules:\n        # don't really need the try\n        import numpy as __np\n\n    if 'pandas' in sys.modules:\n        import pandas as __pd\n\n    if 'pyspark' in sys.modules:\n        import pyspark as __pyspark\n\n    if 'tensorflow' in sys.modules or 'keras' in sys.modules:\n        import tensorflow as __tf\n\n        try:\n            import keras.backend as __K\n        except ImportError:\n            try:\n                import tensorflow.keras.backend as __K\n            except ImportError:\n                __K = None\n\n    if 'torch' in sys.modules:\n        import torch as __torch\n\n    if 'ipywidgets' in sys.modules:\n        import ipywidgets as __ipywidgets\n\n\ndef _jupyterlab_variableinspector_getsizeof(x):\n    if type(x).__name__ in ['ndarray', 'Series']:\n        return x.nbytes\n    elif __pyspark and isinstance(x, __pyspark.sql.DataFrame):\n        return \"?\"\n    elif __tf and isinstance(x, __tf.Variable):\n        return \"?\"\n    elif __torch and isinstance(x, __torch.Tensor):\n        return x.element_size() * x.nelement()\n    elif __pd and type(x).__name__ == 'DataFrame':\n        return x.memory_usage().sum()\n    else:\n        return sys.getsizeof(x)\n\n\ndef _jupyterlab_variableinspector_getshapeof(x):\n    if __pd and isinstance(x, __pd.DataFrame):\n        return \"%d rows x %d cols\" % x.shape\n    if __pd and isinstance(x, __pd.Series):\n        return \"%d rows\" % x.shape\n    if __np and isinstance(x, __np.ndarray):\n        shape = \" x \".join([str(i) for i in x.shape])\n        return \"%s\" % shape\n    if __pyspark and isinstance(x, __pyspark.sql.DataFrame):\n        return \"? rows x %d cols\" % len(x.columns)\n    if __tf and isinstance(x, __tf.Variable):\n        shape = \" x \".join([str(int(i)) for i in x.shape])\n        return \"%s\" % shape\n    if __tf and isinstance(x, __tf.Tensor):\n        shape = \" x \".join([str(int(i)) for i in x.shape])\n        return \"%s\" % shape\n    if __torch and isinstance(x, __torch.Tensor):\n        shape = \" x \".join([str(int(i)) for i in x.shape])\n        return \"%s\" % shape\n    if isinstance(x, list):\n        return \"%s\" % len(x)\n    if isinstance(x, dict):\n        return \"%s keys\" % len(x)\n    return ''\n\n\ndef _jupyterlab_variableinspector_getcontentof(x):\n    # returns content in a friendly way for python variables\n    # pandas and numpy\n    if __pd and isinstance(x, __pd.DataFrame):\n        colnames = ', '.join(x.columns.map(str))\n        content = \"Columns: %s\" % colnames\n    elif __pd and isinstance(x, __pd.Series):\n        content = str(x.values).replace(\" \", \", \")[1:-1]\n        content = content.replace(\"\\\\n\", \"\")\n    elif __np and isinstance(x, __np.ndarray):\n        content = x.__repr__()\n    elif __torch and isinstance(x, __torch.Tensor):\n        if x.nelement() < 1048576:\n            content = x.__repr__()\n        else:\n            content = 'too big'\n    else:\n        content = str(x)\n\n    if len(content) > 50:\n        return content[:50] + \" ...\"\n    else:\n        return content\n\n\ndef _jupyterlab_variableinspector_is_matrix(x):\n    # True if type(x).__name__ in [\"DataFrame\", \"ndarray\", \"Series\"] else False\n    if __pd and isinstance(x, __pd.DataFrame):\n        return True\n    if __pd and isinstance(x, __pd.Series):\n        return True\n    if __np and isinstance(x, __np.ndarray) and len(x.shape) <= 2:\n        return True\n    if __pyspark and isinstance(x, __pyspark.sql.DataFrame):\n        return True\n    if __tf and isinstance(x, __tf.Variable) and len(x.shape) <= 2:\n        return True\n    if __tf and isinstance(x, __tf.Tensor) and len(x.shape) <= 2:\n        return True\n    if __torch and isinstance(x, __torch.Tensor) and len(x.shape) <= 2:\n        return True\n    if isinstance(x, list):\n        return True\n    return False\n\n\ndef _jupyterlab_variableinspector_is_widget(x):\n    return __ipywidgets and issubclass(x, __ipywidgets.DOMWidget)\n\n\ndef _jupyterlab_variableinspector_dict_list():\n    _check_imported()\n    def keep_cond(v):\n        try:\n            obj = eval(v)\n            if isinstance(obj, (str, list, dict)):\n                return True\n            if __tf and isinstance(obj, __tf.Variable):\n                return True\n            if __torch and isinstance(obj, __torch.Tensor):\n                return True\n            if __pd and __pd is not None and (\n                isinstance(obj, __pd.core.frame.DataFrame)\n                or isinstance(obj, __pd.core.series.Series)):\n                return True\n            if v in ['__np', '__pd', '__pyspark', '__tf', '__K', '__torch', '__ipywidgets']:\n                return obj is not None\n            if str(obj)[0] == \"<\":\n                return False\n            if str(obj).startswith(\"_Feature\"):\n                # removes tf/keras objects\n                return False\n            return True\n        except:\n            return False\n    values = _jupyterlab_variableinspector_nms.who_ls()\n    if 'jlvi_brief' in values:\n        vardic = [\n            {\n                'varName': _v,\n                'varType': type(eval(_v)).__name__, \n                'varSize': '0', \n                'varShape': str(_jupyterlab_variableinspector_getshapeof(eval(_v))), \n                'varContent': '', \n                'isMatrix': False,\n                'isWidget': _jupyterlab_variableinspector_is_widget(type(eval(_v)))\n            }\n            for _v in values if keep_cond(_v)\n        ]\n    else:\n        vardic = [\n            {\n                'varName': _v,\n                'varType': type(eval(_v)).__name__, \n                'varSize': '0', \n                'varShape': str(_jupyterlab_variableinspector_getshapeof(eval(_v))), \n                'varContent': str(_jupyterlab_variableinspector_getcontentof(eval(_v))), \n                'isMatrix': False,\n                'isWidget': _jupyterlab_variableinspector_is_widget(type(eval(_v)))\n            }\n            for _v in values if keep_cond(_v)\n        ]\n    return json.dumps(vardic, ensure_ascii=False)\n\n\ndef _jupyterlab_variableinspector_getmatrixcontent(x, max_rows=10000):\n    # to do: add something to handle this in the future\n    threshold = max_rows\n\n    if __pd and __pyspark and isinstance(x, __pyspark.sql.DataFrame):\n        df = x.limit(threshold).toPandas()\n        return _jupyterlab_variableinspector_getmatrixcontent(df.copy())\n    elif __np and __pd and type(x).__name__ == \"DataFrame\":\n        if threshold is not None:\n            x = x.head(threshold)\n        x.columns = x.columns.map(str)\n        return x.to_json(orient=\"table\", default_handler=_jupyterlab_variableinspector_default, force_ascii=False)\n    elif __np and __pd and type(x).__name__ == \"Series\":\n        if threshold is not None:\n            x = x.head(threshold)\n        return x.to_json(orient=\"table\", default_handler=_jupyterlab_variableinspector_default, force_ascii=False)\n    elif __np and __pd and type(x).__name__ == \"ndarray\":\n        df = __pd.DataFrame(x)\n        return _jupyterlab_variableinspector_getmatrixcontent(df)\n    elif __tf and (isinstance(x, __tf.Variable) or isinstance(x, __tf.Tensor)):\n        df = __K.get_value(x)\n        return _jupyterlab_variableinspector_getmatrixcontent(df)\n    elif __torch and isinstance(x, __torch.Tensor):\n        df = x.cpu().numpy()\n        return _jupyterlab_variableinspector_getmatrixcontent(df)\n    elif isinstance(x, list):\n        s = __pd.Series(x)\n        return _jupyterlab_variableinspector_getmatrixcontent(s)\n\n\ndef _jupyterlab_variableinspector_displaywidget(widget):\n    display(widget)\n\n\ndef _jupyterlab_variableinspector_default(o):\n    if isinstance(o, __np.number): return int(o)  \n    raise TypeError\n\n\ndef _jupyterlab_variableinspector_deletevariable(x):\n    exec(\"del %s\" % x, globals())\n`;\nLanguages.r_script = `\nlibrary(repr)\n\n.Last.value = ''\n\n.ls.objects = function (pos = 1, pattern, order.by, decreasing = FALSE, head = FALSE, n = 5) \n{\n    napply <- function(names, fn) sapply(names, function(x) fn(get(x, pos = pos)))\n    names <- ls(pos = pos, pattern = pattern)\n\n    .Last.value <<- base::.Last.value\n\n    if (length(names) == 0) {\n        return(jsonlite::toJSON(data.frame()))\n    }\n\n    names = c('.Last.value',names)\n\n    obj.class <- napply(names, function(x) paste(as.character(class(x)),collapse=rawToChar(as.raw(c(92,110)))))\n    obj.mode <- napply(names, mode)\n    obj.type <- ifelse(is.na(obj.class), obj.mode, obj.class)\n    \n    obj.dim <- t(napply(names, function(x) as.numeric(dim(x))[1:2]))\n    has_no_dim <- is.na(obj.dim)[1:length(names)]                        \n    obj.dim[has_no_dim, 1] <- napply(names, length)[has_no_dim]\n    \n    obj.size = rep(0,length(names))\n    \n    obj.content = rep(\"NA\", length(names))\n    if (!\"jlvi_brief\" %in% names) {\n        obj.content <- napply(names, function(x) {\n            a = capture.output(try({str(x, max.level = 1, list.len = 3)}))\n            b = lapply(a[1:min(length(a), 4)], function(x) {\n                paste(substring(x, 1, 30), ifelse(nchar(x) > 30, \"...\", \"\"))\n            })\n            paste(b, collapse = rawToChar(as.raw(c(92, 110))))\n        })\n    }\n    \n    is_function <- (obj.type == \"function\")\n    if (!\"jlvi_brief\" %in% names) {\n        obj.content[is_function] <- napply(names[is_function], function(x) {\n            a = strsplit(repr_text(x), rawToChar(as.raw(c(92, 110))))[[1]]\n            if (length(a) >= 4) \n                a[[4]] = \"...\"\n            b = lapply(a[1:min(length(a), 4)], function(x) {\n                paste(substring(x, 1, 30), ifelse(nchar(x) > 30, \"...\", \"\"))\n            })\n            paste(b, collapse = rawToChar(as.raw(c(92, 110))))\n        })\n    }\n    \n    obj.content <- unlist(obj.content, use.names = FALSE)\n    \n    out <- data.frame(obj.type, obj.size, obj.dim)\n    names(out) <- c(\"varType\", \"varSize\", \"Rows\", \"Columns\")\n    out$varShape <- paste(out$Rows, \" x \", out$Columns)\n    out$varContent <- obj.content\n    out$isMatrix <- FALSE\n    out$varName <- row.names(out)\n    out <- out[, !(names(out) %in% c(\"Rows\", \"Columns\"))]\n    rownames(out) <- NULL\n    # print(out)\n    if (!missing(order.by)) \n        out <- out[order(out[[order.by]], decreasing = decreasing), \n            ]\n    if (head) \n        out <- head(out, n)\n    jsonlite::toJSON(out)\n}\n\n.deleteVariable <- function(x) {\n    remove(list=c(x), envir=.GlobalEnv)\n}\n      `;\nLanguages.scripts = {\n    python3: {\n        initScript: Languages.py_script,\n        queryCommand: '_jupyterlab_variableinspector_dict_list()',\n        matrixQueryCommand: '_jupyterlab_variableinspector_getmatrixcontent',\n        widgetQueryCommand: '_jupyterlab_variableinspector_displaywidget',\n        deleteCommand: '_jupyterlab_variableinspector_deletevariable',\n    },\n    python2: {\n        initScript: Languages.py_script,\n        queryCommand: '_jupyterlab_variableinspector_dict_list()',\n        matrixQueryCommand: '_jupyterlab_variableinspector_getmatrixcontent',\n        widgetQueryCommand: '_jupyterlab_variableinspector_displaywidget',\n        deleteCommand: '_jupyterlab_variableinspector_deletevariable',\n    },\n    python: {\n        initScript: Languages.py_script,\n        queryCommand: '_jupyterlab_variableinspector_dict_list()',\n        matrixQueryCommand: '_jupyterlab_variableinspector_getmatrixcontent',\n        widgetQueryCommand: '_jupyterlab_variableinspector_displaywidget',\n        deleteCommand: '_jupyterlab_variableinspector_deletevariable',\n    },\n    R: {\n        initScript: Languages.r_script,\n        queryCommand: '.ls.objects()',\n        matrixQueryCommand: '.ls.objects',\n        widgetQueryCommand: 'TODO',\n        deleteCommand: '.deleteVariable',\n    },\n    scala: {\n        initScript: '_root_.almond.api.JupyterAPIHolder.value.VariableInspector.init()',\n        queryCommand: '_root_.almond.api.JupyterAPIHolder.value.VariableInspector.dictList()',\n        matrixQueryCommand: '',\n        widgetQueryCommand: '',\n        deleteCommand: '',\n    },\n};\n",
         "import { Signal } from '@lumino/signaling';\n/**\n * Connector class that handles execute request to a kernel\n */\nexport class KernelConnector {\n    constructor(options) {\n        this._kernelRestarted = new Signal(this);\n        this._session = options.session;\n        this._session.statusChanged.connect((sender, newStatus) => {\n            switch (newStatus) {\n                case 'restarting':\n                case 'autorestarting':\n                    this._kernelRestarted.emit(this._session.ready);\n                    break;\n                default:\n                    break;\n            }\n        });\n    }\n    get kernelRestarted() {\n        return this._kernelRestarted;\n    }\n    get kernelLanguage() {\n        return this._session.session.kernel.info.then((infoReply) => {\n            return infoReply.language_info.name;\n        });\n    }\n    get kernelName() {\n        return this._session.kernelDisplayName;\n    }\n    /**\n     *  A Promise that is fulfilled when the session associated w/ the connector is ready.\n     */\n    get ready() {\n        return this._session.ready;\n    }\n    /**\n     *  A signal emitted for iopub messages of the kernel associated with the kernel.\n     */\n    get iopubMessage() {\n        return this._session.iopubMessage;\n    }\n    /**\n     * Executes the given request on the kernel associated with the connector.\n     * @param content: IExecuteRequestMsg to forward to the kernel.\n     * @param ioCallback: Callable to forward IOPub messages of the kernel to.\n     * @returns Promise<KernelMessage.IExecuteReplyMsg>\n     */\n    fetch(content, ioCallback) {\n        const kernel = this._session.session.kernel;\n        if (!kernel) {\n            return Promise.reject(new Error('Require kernel to perform variable inspection!'));\n        }\n        const future = kernel.requestExecute(content);\n        future.onIOPub = (msg) => {\n            ioCallback(msg);\n        };\n        return future.done;\n    }\n    execute(content) {\n        return this._session.session.kernel.requestExecute(content);\n    }\n}\n",
         "import { Token } from '@lumino/coreutils';\nexport const IVariableInspectorManager = new Token('jupyterlab_extension/variableinspector:IVariableInspectorManager');\n/**\n * A class that manages variable inspector widget instances and offers persistent\n * `IVariableInspector` instance that other plugins can communicate with.\n */\nexport class VariableInspectorManager {\n    constructor() {\n        this._source = null;\n        this._panel = null;\n        this._handlers = {};\n    }\n    hasHandler(id) {\n        if (this._handlers[id]) {\n            return true;\n        }\n        else {\n            return false;\n        }\n    }\n    getHandler(id) {\n        return this._handlers[id];\n    }\n    addHandler(handler) {\n        this._handlers[handler.id] = handler;\n    }\n    /**\n     * The current inspector panel.\n     */\n    get panel() {\n        return this._panel;\n    }\n    set panel(panel) {\n        if (this.panel === panel) {\n            return;\n        }\n        this._panel = panel;\n        if (panel && !panel.source) {\n            panel.source = this._source;\n        }\n    }\n    /**\n     * The source of events the inspector panel listens for.\n     */\n    get source() {\n        return this._source;\n    }\n    set source(source) {\n        if (this._source === source) {\n            return;\n        }\n        // remove subscriptions\n        if (this._source) {\n            this._source.disposed.disconnect(this._onSourceDisposed, this);\n        }\n        this._source = source;\n        if (this._panel && !this._panel.isDisposed) {\n            this._panel.source = this._source;\n        }\n        // Subscribe to new source\n        if (this._source) {\n            this._source.disposed.connect(this._onSourceDisposed, this);\n        }\n    }\n    _onSourceDisposed() {\n        this._source = null;\n    }\n}\n",
         "import { OutputAreaModel, SimplifiedOutputArea } from '@jupyterlab/outputarea';\nimport { Token } from '@lumino/coreutils';\nimport { Widget } from '@lumino/widgets';\nimport { DataGrid } from '@lumino/datagrid';\nimport { closeIcon, searchIcon } from '@jupyterlab/ui-components';\nimport '../style/index.css';\nconst TITLE_CLASS = 'jp-VarInspector-title';\nconst PANEL_CLASS = 'jp-VarInspector';\nconst TABLE_CLASS = 'jp-VarInspector-table';\nconst TABLE_BODY_CLASS = 'jp-VarInspector-content';\n/**\n * The inspector panel token.\n */\nexport const IVariableInspector = new Token('jupyterlab_extension/variableinspector:IVariableInspector');\n/**\n * A panel that renders the variables\n */\nexport class VariableInspectorPanel extends Widget {\n    constructor() {\n        super();\n        this._source = null;\n        this.addClass(PANEL_CLASS);\n        this._title = Private.createTitle();\n        this._title.className = TITLE_CLASS;\n        this._table = Private.createTable();\n        this._table.className = TABLE_CLASS;\n        this.node.appendChild(this._title);\n        this.node.appendChild(this._table);\n    }\n    get source() {\n        return this._source;\n    }\n    set source(source) {\n        if (this._source === source) {\n            // this._source.performInspection();\n            return;\n        }\n        //Remove old subscriptions\n        if (this._source) {\n            this._source.inspected.disconnect(this.onInspectorUpdate, this);\n            this._source.disposed.disconnect(this.onSourceDisposed, this);\n        }\n        this._source = source;\n        //Subscribe to new object\n        if (this._source) {\n            this._source.inspected.connect(this.onInspectorUpdate, this);\n            this._source.disposed.connect(this.onSourceDisposed, this);\n            this._source.performInspection();\n        }\n    }\n    /**\n     * Dispose resources\n     */\n    dispose() {\n        if (this.isDisposed) {\n            return;\n        }\n        this.source = null;\n        super.dispose();\n    }\n    onInspectorUpdate(sender, allArgs) {\n        if (!this.isAttached) {\n            return;\n        }\n        const title = allArgs.title;\n        const args = allArgs.payload;\n        if (title.contextName) {\n            this._title.innerHTML = title.contextName;\n        }\n        else {\n            this._title.innerHTML =\n                \"    Inspecting '\" + title.kernelName + \"' \" + title.contextName;\n        }\n        //Render new variable state\n        let row;\n        this._table.deleteTFoot();\n        this._table.createTFoot();\n        this._table.tFoot.className = TABLE_BODY_CLASS;\n        for (let index = 0; index < args.length; index++) {\n            const item = args[index];\n            console.log(item);\n            const name = item.varName;\n            const varType = item.varType;\n            row = this._table.tFoot.insertRow();\n            // Add delete icon and onclick event\n            let cell = row.insertCell(0);\n            cell.title = 'Delete Variable';\n            cell.className = 'jp-VarInspector-deleteButton';\n            const ico = closeIcon.element();\n            ico.onclick = (ev) => {\n                this.source.performDelete(name);\n            };\n            cell.append(ico);\n            // Add onclick event for inspection\n            cell = row.insertCell(1);\n            if (item.isMatrix) {\n                cell.title = 'View Contents';\n                cell.className = 'jp-VarInspector-inspectButton';\n                const ico = searchIcon.element();\n                ico.onclick = (ev) => {\n                    console.log('Click on ' + name);\n                    this._source\n                        .performMatrixInspection(name)\n                        .then((model) => {\n                        this._showMatrix(model, name, varType);\n                    });\n                };\n                cell.append(ico);\n            }\n            else {\n                cell.innerHTML = '';\n            }\n            // cell = row.insertCell(2);\n            cell.className = 'jp-VarInspector-varName';\n            cell.innerHTML = name;\n            // Add remaining cells\n            cell = row.insertCell(2);\n            cell.innerHTML = varType.replace(/\\\\n/g, \"</br>\");\n            ;\n            // cell = row.insertCell(4);\n            // cell.innerHTML = item.varSize;\n            cell = row.insertCell(3);\n            cell.innerHTML = item.varShape;\n            cell = row.insertCell(4);\n            const rendermime = this._source.rendermime;\n            if (item.isWidget && rendermime) {\n                const model = new OutputAreaModel({ trusted: true });\n                const output = new SimplifiedOutputArea({ model, rendermime });\n                output.future = this._source.performWidgetInspection(item.varName);\n                Widget.attach(output, cell);\n            }\n            else {\n                cell.innerHTML = Private.escapeHtml(item.varContent).replace(/\\\\n/g, '</br>');\n            }\n        }\n    }\n    /**\n     * Handle source disposed signals.\n     */\n    onSourceDisposed(sender, args) {\n        this.source = null;\n    }\n    _showMatrix(dataModel, name, varType) {\n        const datagrid = new DataGrid({\n            defaultSizes: {\n                rowHeight: 32,\n                columnWidth: 128,\n                rowHeaderWidth: 64,\n                columnHeaderHeight: 32,\n            },\n        });\n        datagrid.dataModel = dataModel;\n        datagrid.title.label = varType + ': ' + name;\n        datagrid.title.closable = true;\n        const lout = this.parent.layout;\n        lout.addWidget(datagrid, { mode: 'split-right' });\n        //todo activate/focus matrix widget\n    }\n}\nvar Private;\n(function (Private) {\n    const entityMap = new Map(Object.entries({\n        '&': '&amp;',\n        '<': '&lt;',\n        '>': '&gt;',\n        '\"': '&quot;',\n        \"'\": '&#39;',\n        '/': '&#x2F;',\n    }));\n    function escapeHtml(source) {\n        return String(source).replace(/[&<>\"'/]/g, (s) => entityMap.get(s));\n    }\n    Private.escapeHtml = escapeHtml;\n    function createTable() {\n        const table = document.createElement('table');\n        table.createTHead();\n        const hrow = table.tHead.insertRow(0);\n        const cell1 = hrow.insertCell(0);\n        cell1.innerHTML = '';\n        // const cell2 = hrow.insertCell(1);\n        // cell2.innerHTML = '';\n        const cell3 = hrow.insertCell(1);\n        cell3.innerHTML = 'Name';\n        const cell4 = hrow.insertCell(2);\n        cell4.innerHTML = 'Type';\n        // const cell5 = hrow.insertCell(4);\n        // cell5.innerHTML = 'Size';\n        const cell6 = hrow.insertCell(3);\n        cell6.innerHTML = 'Shape';\n        const cell7 = hrow.insertCell(4);\n        cell7.innerHTML = 'Content';\n        return table;\n    }\n    Private.createTable = createTable;\n    function createTitle(header = '') {\n        const title = document.createElement('p');\n        title.innerHTML = header;\n        return title;\n    }\n    Private.createTitle = createTitle;\n})(Private || (Private = {}));\n",
         "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../node_modules/css-loader/dist/runtime/cssWithMappingToString.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../node_modules/css-loader/dist/runtime/api.js\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, \"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\", \"\",{\"version\":3,\"sources\":[\"webpack://./style/base.css\"],\"names\":[],\"mappings\":\"AAAA;;;;CAIC\",\"sourcesContent\":[\"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\"],\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
         "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../node_modules/css-loader/dist/runtime/cssWithMappingToString.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../node_modules/css-loader/dist/runtime/api.js\";\nimport ___CSS_LOADER_AT_RULE_IMPORT_0___ from \"-!../node_modules/css-loader/dist/cjs.js!./base.css\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\n___CSS_LOADER_EXPORT___.i(___CSS_LOADER_AT_RULE_IMPORT_0___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, \"\\n.jp-VarInspector {\\n    flex-direction: column;\\n    overflow: auto;\\n    font-size: var(--jp-ui-font-size1);\\n  }\\n  \\n  .jp-VarInspector-table {\\n    border-collapse: collapse;\\n    margin: auto;\\n    width: 100%;\\n    color: var(--jp-content-font-color1);\\n  }\\n  \\n  .jp-VarInspector-table td,\\n  .jp-VarInspector-table thead {\\n    border: 1px solid;\\n    border-color: var(--jp-layout-color2);\\n    padding: 8px;\\n  }\\n  \\n  .jp-VarInspector-table tr:nth-child(even) {\\n    background-color: var(--jp-layout-color1);\\n  }\\n  \\n  .jp-VarInspector-content tr:hover {\\n    background-color: var(--jp-layout-color2);\\n  }\\n  \\n  .jp-VarInspector-table thead {\\n    font-size: var(--jp-ui-font-size0);\\n    text-align: center;\\n    background-color: var(--jp-layout-color2);\\n    color: var(--jp-ui-font-color1);\\n    font-weight: 600;\\n    letter-spacing: 1px;\\n    text-transform: uppercase;\\n  }\\n  \\n  .jp-VarInspector-title {\\n    font-size: var(--jp-ui-font-size1);\\n    color: var(--jp-content-font-color1);\\n    text-align: left;\\n    padding-left: 10px;\\n  }\\n  \\n  .jp-VarInspector-deleteButton {\\n    text-align: center;\\n    width: 1em;\\n  }\\n\\n  .jp-VarInspector-deleteButton:hover {\\n    text-shadow: 0 0 0 red;\\n    background-color: var(--jp-layout-color3);\\n  }\\n\\n  .jp-VarInspector-inspectButton {\\n    text-align: center;\\n    width: 1em;\\n  }\\n    \\n    \\n  .jp-VarInspector-varName {\\n    font-weight: 600;\\n  }\\n\\n\", \"\",{\"version\":3,\"sources\":[\"webpack://./style/index.css\"],\"names\":[],\"mappings\":\";AAGA;IACI,sBAAsB;IACtB,cAAc;IACd,kCAAkC;EACpC;;EAEA;IACE,yBAAyB;IACzB,YAAY;IACZ,WAAW;IACX,oCAAoC;EACtC;;EAEA;;IAEE,iBAAiB;IACjB,qCAAqC;IACrC,YAAY;EACd;;EAEA;IACE,yCAAyC;EAC3C;;EAEA;IACE,yCAAyC;EAC3C;;EAEA;IACE,kCAAkC;IAClC,kBAAkB;IAClB,yCAAyC;IACzC,+BAA+B;IAC/B,gBAAgB;IAChB,mBAAmB;IACnB,yBAAyB;EAC3B;;EAEA;IACE,kCAAkC;IAClC,oCAAoC;IACpC,gBAAgB;IAChB,kBAAkB;EACpB;;EAEA;IACE,kBAAkB;IAClB,UAAU;EACZ;;EAEA;IACE,sBAAsB;IACtB,yCAAyC;EAC3C;;EAEA;IACE,kBAAkB;IAClB,UAAU;EACZ;;;EAGA;IACE,gBAAgB;EAClB\",\"sourcesContent\":[\"\\n@import url('base.css');\\n\\n.jp-VarInspector {\\n    flex-direction: column;\\n    overflow: auto;\\n    font-size: var(--jp-ui-font-size1);\\n  }\\n  \\n  .jp-VarInspector-table {\\n    border-collapse: collapse;\\n    margin: auto;\\n    width: 100%;\\n    color: var(--jp-content-font-color1);\\n  }\\n  \\n  .jp-VarInspector-table td,\\n  .jp-VarInspector-table thead {\\n    border: 1px solid;\\n    border-color: var(--jp-layout-color2);\\n    padding: 8px;\\n  }\\n  \\n  .jp-VarInspector-table tr:nth-child(even) {\\n    background-color: var(--jp-layout-color1);\\n  }\\n  \\n  .jp-VarInspector-content tr:hover {\\n    background-color: var(--jp-layout-color2);\\n  }\\n  \\n  .jp-VarInspector-table thead {\\n    font-size: var(--jp-ui-font-size0);\\n    text-align: center;\\n    background-color: var(--jp-layout-color2);\\n    color: var(--jp-ui-font-color1);\\n    font-weight: 600;\\n    letter-spacing: 1px;\\n    text-transform: uppercase;\\n  }\\n  \\n  .jp-VarInspector-title {\\n    font-size: var(--jp-ui-font-size1);\\n    color: var(--jp-content-font-color1);\\n    text-align: left;\\n    padding-left: 10px;\\n  }\\n  \\n  .jp-VarInspector-deleteButton {\\n    text-align: center;\\n    width: 1em;\\n  }\\n\\n  .jp-VarInspector-deleteButton:hover {\\n    text-shadow: 0 0 0 red;\\n    background-color: var(--jp-layout-color3);\\n  }\\n\\n  .jp-VarInspector-inspectButton {\\n    text-align: center;\\n    width: 1em;\\n  }\\n    \\n    \\n  .jp-VarInspector-varName {\\n    font-weight: 600;\\n  }\\n\\n\"],\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
         "import api from \"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n            import content from \"!!../node_modules/css-loader/dist/cjs.js!./index.css\";\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nexport default content.locals || {};"
     ],
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/remoteEntry.01eb97769bed74d9aebb.js` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/remoteEntry.c589841968c12546b849.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -184,15 +184,15 @@
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
                 "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "572d68459ed6309c5fac",
                 "webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549": "fc8292ece253346aaf18",
-                "lib_index_js": "d8a6a68cd2c54907e293",
+                "lib_index_js": "92aa6d645091a304c589",
                 "style_index_js": "d4d79bc4853f68dc1d0e",
                 "vendors-node_modules_lumino_datagrid_dist_index_es6_js": "9a83b5da30d9d9a98e88",
                 "webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e": "280c5735d250b1b5e3d3"
             } [chunkId] + ".js";
             /******/
         };
         /******/
@@ -428,15 +428,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("@feiranzhang/jupyterlab-variableinspector", "0.1.3", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("@feiranzhang/jupyterlab-variableinspector", "0.1.4", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                     register("@lumino/datagrid", "0.32.0", () => (Promise.all([__webpack_require__.e("vendors-node_modules_lumino_datagrid_dist_index_es6_js"), __webpack_require__.e("webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e"), __webpack_require__.e("webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549")]).then(() => (() => (__webpack_require__( /*! ./node_modules/@lumino/datagrid/dist/index.es6.js */ "./node_modules/@lumino/datagrid/dist/index.es6.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
@@ -819,41 +819,41 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 1, 4, 3])),
+            "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 1, 10, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 1, 16, 1])),
+            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 1, 37, 2])),
             /******/
-            "webpack/sharing/consume/default/@lumino/coreutils": () => (loadSingletonVersionCheck("default", "@lumino/coreutils", [1, 1, 5, 3])),
+            "webpack/sharing/consume/default/@lumino/coreutils": () => (loadSingletonVersionCheck("default", "@lumino/coreutils", [1, 1, 11, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 0, 10])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 3, 0, 13])),
+            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/console": () => (loadSingletonVersionCheck("default", "@jupyterlab/console", [1, 3, 0, 12])),
+            "webpack/sharing/consume/default/@jupyterlab/console": () => (loadSingletonVersionCheck("default", "@jupyterlab/console", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 0, 13])),
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 0, 8])),
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/outputarea": () => (loadVersionCheck("default", "@jupyterlab/outputarea", [1, 3, 0, 12])),
+            "webpack/sharing/consume/default/@jupyterlab/outputarea": () => (loadVersionCheck("default", "@jupyterlab/outputarea", [1, 3, 6, 3])),
             /******/
             "webpack/sharing/consume/default/@lumino/datagrid/@lumino/datagrid": () => (loadStrictVersionCheckFallback("default", "@lumino/datagrid", [2, 0, 32, 0], () => (Promise.all([__webpack_require__.e("vendors-node_modules_lumino_datagrid_dist_index_es6_js"), __webpack_require__.e("webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e")]).then(() => (() => (__webpack_require__( /*! @lumino/datagrid */ "./node_modules/@lumino/datagrid/dist/index.es6.js"))))))),
             /******/
-            "webpack/sharing/consume/default/@lumino/domutils": () => (loadSingletonVersionCheck("default", "@lumino/domutils", [1, 1, 2, 3])),
+            "webpack/sharing/consume/default/@lumino/domutils": () => (loadSingletonVersionCheck("default", "@lumino/domutils", [1, 1, 8, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/dragdrop": () => (loadSingletonVersionCheck("default", "@lumino/dragdrop", [1, 1, 7, 1])),
+            "webpack/sharing/consume/default/@lumino/dragdrop": () => (loadSingletonVersionCheck("default", "@lumino/dragdrop", [1, 1, 13, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/algorithm": () => (loadSingletonVersionCheck("default", "@lumino/algorithm", [1, 1, 3, 3])),
+            "webpack/sharing/consume/default/@lumino/algorithm": () => (loadSingletonVersionCheck("default", "@lumino/algorithm", [1, 1, 9, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/messaging": () => (loadSingletonVersionCheck("default", "@lumino/messaging", [1, 1, 4, 3]))
+            "webpack/sharing/consume/default/@lumino/messaging": () => (loadSingletonVersionCheck("default", "@lumino/messaging", [1, 1, 10, 0]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549": [
@@ -1123,8 +1123,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/@feiranzhang/jupyterlab-variableinspector");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@feiranzhang/jupyterlab-variableinspector"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.01eb97769bed74d9aebb.js.map
+//# sourceMappingURL=remoteEntry.c589841968c12546b849.js.map
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/remoteEntry.01eb97769bed74d9aebb.js.map` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/remoteEntry.c589841968c12546b849.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9081632653061226%*

 * *Differences: {"'file'": "'remoteEntry.c589841968c12546b849.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1":"572d68459ed6309c5fac","webpack_sharing_consume_default_lumino_coreutils- […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.01eb97769bed74d9aebb.js",
+    "file": "remoteEntry.c589841968c12546b849.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,whBAAwhB;WACtjB;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC5CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCrMA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@feiranzhang/jupyterlab-variableinspector/webpack/container-entry",
         "webpack://@feiranzhang/jupyterlab-variableinspector/webpack/bootstrap",
         "webpack://@feiranzhang/jupyterlab-variableinspector/webpack/runtime/compat get default export",
@@ -25,22 +25,22 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"572d68459ed6309c5fac\",\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\":\"fc8292ece253346aaf18\",\"lib_index_js\":\"d8a6a68cd2c54907e293\",\"style_index_js\":\"d4d79bc4853f68dc1d0e\",\"vendors-node_modules_lumino_datagrid_dist_index_es6_js\":\"9a83b5da30d9d9a98e88\",\"webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e\":\"280c5735d250b1b5e3d3\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"572d68459ed6309c5fac\",\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\":\"fc8292ece253346aaf18\",\"lib_index_js\":\"92aa6d645091a304c589\",\"style_index_js\":\"d4d79bc4853f68dc1d0e\",\"vendors-node_modules_lumino_datagrid_dist_index_es6_js\":\"9a83b5da30d9d9a98e88\",\"webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e\":\"280c5735d250b1b5e3d3\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"@feiranzhang/jupyterlab-variableinspector:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@feiranzhang/jupyterlab-variableinspector\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@feiranzhang/jupyterlab-variableinspector\", \"0.1.3\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"@lumino/datagrid\", \"0.32.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_lumino_datagrid_dist_index_es6_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@lumino/datagrid/dist/index.es6.js */ \"./node_modules/@lumino/datagrid/dist/index.es6.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"@feiranzhang/jupyterlab-variableinspector\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@feiranzhang/jupyterlab-variableinspector\", \"0.1.4\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"@lumino/datagrid\", \"0.32.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_lumino_datagrid_dist_index_es6_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@lumino/datagrid/dist/index.es6.js */ \"./node_modules/@lumino/datagrid/dist/index.es6.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,4,3])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,16,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,0,10])),\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,0,13])),\n\t\"webpack/sharing/consume/default/@jupyterlab/console\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/console\", [1,3,0,12])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,0,13])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,0,8])),\n\t\"webpack/sharing/consume/default/@jupyterlab/outputarea\": () => (loadVersionCheck(\"default\", \"@jupyterlab/outputarea\", [1,3,0,12])),\n\t\"webpack/sharing/consume/default/@lumino/datagrid/@lumino/datagrid\": () => (loadStrictVersionCheckFallback(\"default\", \"@lumino/datagrid\", [2,0,32,0], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_lumino_datagrid_dist_index_es6_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e\")]).then(() => (() => (__webpack_require__(/*! @lumino/datagrid */ \"./node_modules/@lumino/datagrid/dist/index.es6.js\"))))))),\n\t\"webpack/sharing/consume/default/@lumino/domutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/domutils\", [1,1,2,3])),\n\t\"webpack/sharing/consume/default/@lumino/dragdrop\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/dragdrop\", [1,1,7,1])),\n\t\"webpack/sharing/consume/default/@lumino/algorithm\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,1,3,3])),\n\t\"webpack/sharing/consume/default/@lumino/messaging\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/messaging\", [1,1,4,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\": [\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\"\n\t],\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/console\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/outputarea\",\n\t\t\"webpack/sharing/consume/default/@lumino/datagrid/@lumino/datagrid\"\n\t],\n\t\"webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e\": [\n\t\t\"webpack/sharing/consume/default/@lumino/domutils\",\n\t\t\"webpack/sharing/consume/default/@lumino/dragdrop\",\n\t\t\"webpack/sharing/consume/default/@lumino/algorithm\",\n\t\t\"webpack/sharing/consume/default/@lumino/messaging\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,37,2])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/console\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/console\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/outputarea\": () => (loadVersionCheck(\"default\", \"@jupyterlab/outputarea\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@lumino/datagrid/@lumino/datagrid\": () => (loadStrictVersionCheckFallback(\"default\", \"@lumino/datagrid\", [2,0,32,0], () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_lumino_datagrid_dist_index_es6_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e\")]).then(() => (() => (__webpack_require__(/*! @lumino/datagrid */ \"./node_modules/@lumino/datagrid/dist/index.es6.js\"))))))),\n\t\"webpack/sharing/consume/default/@lumino/domutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/domutils\", [1,1,8,0])),\n\t\"webpack/sharing/consume/default/@lumino/dragdrop\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/dragdrop\", [1,1,13,0])),\n\t\"webpack/sharing/consume/default/@lumino/algorithm\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,1,9,0])),\n\t\"webpack/sharing/consume/default/@lumino/messaging\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/messaging\", [1,1,10,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_lumino_coreutils-webpack_sharing_consume_default_lumino_signa-d40549\": [\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\"\n\t],\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/console\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/outputarea\",\n\t\t\"webpack/sharing/consume/default/@lumino/datagrid/@lumino/datagrid\"\n\t],\n\t\"webpack_sharing_consume_default_lumino_algorithm-webpack_sharing_consume_default_lumino_domut-c9e14e\": [\n\t\t\"webpack/sharing/consume/default/@lumino/domutils\",\n\t\t\"webpack/sharing/consume/default/@lumino/dragdrop\",\n\t\t\"webpack/sharing/consume/default/@lumino/algorithm\",\n\t\t\"webpack/sharing/consume/default/@lumino/messaging\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@feiranzhang/jupyterlab-variableinspector\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(!/^webpack_sharing_consume_default_lumino_(algorithm\\-webpack_sharing_consume_default_lumino_domut\\-c9e14e|coreutils\\-webpack_sharing_consume_default_lumino_signa\\-d40549)$/.test(chunkId)) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_feiranzhang_jupyterlab_variableinspector\"] = self[\"webpackChunk_feiranzhang_jupyterlab_variableinspector\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/@feiranzhang/jupyterlab-variableinspector\");\n",
         ""
     ],
     "version": 3
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js.map` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js.map`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js.map` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js.map`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js.map` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js.map`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz_jupyterlab_variableinspector.egg-info/PKG-INFO` & `frz-jupyterlab-variableinspector-0.1.4/frz_jupyterlab_variableinspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frz-jupyterlab-variableinspector
-Version: 0.1.3
+Version: 0.1.4
 Summary: Customized Variable Inspector extension for JupyterLab.
 Home-page: https://github.com/zhangfeiran/jupyterlab-variableInspector
 Author: Feiran Zhang
 Author-email: feiranzhang@outlook.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/frz_jupyterlab_variableinspector.egg-info/SOURCES.txt` & `frz-jupyterlab-variableinspector-0.1.4/frz_jupyterlab_variableinspector.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 README.md
 RELEASE.md
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
+yarn.lock
 frz-jupyterlab-variableinspector/__init__.py
 frz-jupyterlab-variableinspector/_version.py
 frz-jupyterlab-variableinspector/labextension/build_log.json
 frz-jupyterlab-variableinspector/labextension/package.json
-frz-jupyterlab-variableinspector/labextension/static/lib_index_js.d8a6a68cd2c54907e293.js
-frz-jupyterlab-variableinspector/labextension/static/lib_index_js.d8a6a68cd2c54907e293.js.map
-frz-jupyterlab-variableinspector/labextension/static/remoteEntry.01eb97769bed74d9aebb.js
-frz-jupyterlab-variableinspector/labextension/static/remoteEntry.01eb97769bed74d9aebb.js.map
+frz-jupyterlab-variableinspector/labextension/static/lib_index_js.92aa6d645091a304c589.js
+frz-jupyterlab-variableinspector/labextension/static/lib_index_js.92aa6d645091a304c589.js.map
+frz-jupyterlab-variableinspector/labextension/static/remoteEntry.c589841968c12546b849.js
+frz-jupyterlab-variableinspector/labextension/static/remoteEntry.c589841968c12546b849.js.map
 frz-jupyterlab-variableinspector/labextension/static/style.js
 frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js
 frz-jupyterlab-variableinspector/labextension/static/style_index_js.d4d79bc4853f68dc1d0e.js.map
 frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js
 frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.572d68459ed6309c5fac.js.map
 frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js
 frz-jupyterlab-variableinspector/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.9a83b5da30d9d9a98e88.js.map
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/package.json` & `frz-jupyterlab-variableinspector-0.1.4/frz-jupyterlab-variableinspector/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9682539682539681%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.c589841968c12546b849.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.1.4'"}*

```diff
@@ -48,14 +48,19 @@
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.c589841968c12546b849.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "frz-jupyterlab-variableinspector/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension",
@@ -99,9 +104,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.4"
 }
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/pyproject.toml` & `frz-jupyterlab-variableinspector-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/setup.py` & `frz-jupyterlab-variableinspector-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/src/LICENCE.md` & `frz-jupyterlab-variableinspector-0.1.4/src/LICENCE.md`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/src/handler.ts` & `frz-jupyterlab-variableinspector-0.1.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/src/index.ts` & `frz-jupyterlab-variableinspector-0.1.4/src/index.ts`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/src/inspectorscripts.ts` & `frz-jupyterlab-variableinspector-0.1.4/src/inspectorscripts.ts`

 * *Files 2% similar despite different names*

```diff
@@ -251,28 +251,29 @@
 def _jupyterlab_variableinspector_deletevariable(x):
     exec("del %s" % x, globals())
 `;
 
   static r_script = `
 library(repr)
 
-.Last.value = 'wtf'
+.Last.value = ''
 
 .ls.objects = function (pos = 1, pattern, order.by, decreasing = FALSE, head = FALSE, n = 5) 
 {
-    napply <- function(names, fn) sapply(names, function(x) fn(get(x, 
-        pos = pos)))
+    napply <- function(names, fn) sapply(names, function(x) fn(get(x, pos = pos)))
     names <- ls(pos = pos, pattern = pattern)
-    
-    if (class(base::.Last.value) != 'json') .Last.value <<- base::.Last.value
-    names = c('.Last.value',names)
+
+    .Last.value <<- base::.Last.value
 
     if (length(names) == 0) {
         return(jsonlite::toJSON(data.frame()))
     }
+
+    names = c('.Last.value',names)
+
     obj.class <- napply(names, function(x) paste(as.character(class(x)),collapse=rawToChar(as.raw(c(92,110)))))
     obj.mode <- napply(names, mode)
     obj.type <- ifelse(is.na(obj.class), obj.mode, obj.class)
     
     obj.dim <- t(napply(names, function(x) as.numeric(dim(x))[1:2]))
     has_no_dim <- is.na(obj.dim)[1:length(names)]                        
     obj.dim[has_no_dim, 1] <- napply(names, length)[has_no_dim]
@@ -309,15 +310,15 @@
     names(out) <- c("varType", "varSize", "Rows", "Columns")
     out$varShape <- paste(out$Rows, " x ", out$Columns)
     out$varContent <- obj.content
     out$isMatrix <- FALSE
     out$varName <- row.names(out)
     out <- out[, !(names(out) %in% c("Rows", "Columns"))]
     rownames(out) <- NULL
-    print(out)
+    # print(out)
     if (!missing(order.by)) 
         out <- out[order(out[[order.by]], decreasing = decreasing), 
             ]
     if (head) 
         out <- head(out, n)
     jsonlite::toJSON(out)
 }
```

### Comparing `frz-jupyterlab-variableinspector-0.1.3/src/kernelconnector.ts` & `frz-jupyterlab-variableinspector-0.1.4/src/kernelconnector.ts`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/src/manager.ts` & `frz-jupyterlab-variableinspector-0.1.4/src/manager.ts`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/src/variableinspector.ts` & `frz-jupyterlab-variableinspector-0.1.4/src/variableinspector.ts`

 * *Files identical despite different names*

### Comparing `frz-jupyterlab-variableinspector-0.1.3/style/index.css` & `frz-jupyterlab-variableinspector-0.1.4/style/index.css`

 * *Files identical despite different names*

