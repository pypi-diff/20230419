# Comparing `tmp/widgets-lib-2.6.5.tar.gz` & `tmp/widgets-lib-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgets-lib-2.6.5.tar", last modified: Thu Apr 13 22:04:58 2023, max compression
+gzip compressed data, was "widgets-lib-2.7.0.tar", last modified: Wed Apr 19 13:38:07 2023, max compression
```

## Comparing `widgets-lib-2.6.5.tar` & `widgets-lib-2.7.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.980206 widgets-lib-2.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-13 22:04:58.980206 widgets-lib-2.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:04:58.980206 widgets-lib-2.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.964206 widgets-lib-2.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.964206 widgets-lib-2.6.5/src/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.968206 widgets-lib-2.6.5/src/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.968206 widgets-lib-2.6.5/src/widgets/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.968206 widgets-lib-2.6.5/src/widgets/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.968206 widgets-lib-2.6.5/src/widgets/streamlit/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/expander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.972206 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/download_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.972206 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/selectstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/textarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.972206 widgets-lib-2.6.5/src/widgets/streamlit/widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/widget/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.976206 widgets-lib-2.6.5/src/widgets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/templates/source.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/templates/streamlit_single.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/templates/streamlit_single.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.976206 widgets-lib-2.6.5/src/widgets_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.976206 widgets-lib-2.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_source_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.225399 widgets-lib-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-19 13:38:07.225399 widgets-lib-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:38:07.225399 widgets-lib-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.217399 widgets-lib-2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.221399 widgets-lib-2.7.0/src/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.221399 widgets-lib-2.7.0/src/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/base/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.221399 widgets-lib-2.7.0/src/widgets/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.221399 widgets-lib-2.7.0/src/widgets/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.221399 widgets-lib-2.7.0/src/widgets/streamlit/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/expander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.221399 widgets-lib-2.7.0/src/widgets/streamlit/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/files/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/files/download_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.221399 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/selectstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/resource/values/textarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.221399 widgets-lib-2.7.0/src/widgets/streamlit/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/streamlit/widget/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.225399 widgets-lib-2.7.0/src/widgets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/templates/source.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/templates/streamlit_single.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/src/widgets/templates/streamlit_single.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.225399 widgets-lib-2.7.0/src/widgets_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-19 13:38:07.000000 widgets-lib-2.7.0/src/widgets_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-19 13:38:07.000000 widgets-lib-2.7.0/src/widgets_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:38:07.000000 widgets-lib-2.7.0/src/widgets_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 13:38:07.000000 widgets-lib-2.7.0/src/widgets_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 13:38:07.000000 widgets-lib-2.7.0/src/widgets_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 13:38:07.000000 widgets-lib-2.7.0/src/widgets_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:38:07.225399 widgets-lib-2.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/tests/test_duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/tests/test_source_parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-19 13:37:30.000000 widgets-lib-2.7.0/tests/test_streamlit.py
```

### Comparing `widgets-lib-2.6.5/LICENSE` & `widgets-lib-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/PKG-INFO` & `widgets-lib-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.6.5
+Version: 2.7.0
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.6.5/README.md` & `widgets-lib-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/pyproject.toml` & `widgets-lib-2.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/base/exceptions.py` & `widgets-lib-2.7.0/src/widgets/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/base/helpers.py` & `widgets-lib-2.7.0/src/widgets/base/helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/base/io.py` & `widgets-lib-2.7.0/src/widgets/base/io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/base/resource.py` & `widgets-lib-2.7.0/src/widgets/base/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import deepcopy
 from inspect import getmro, getsource, isfunction, signature
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, Generator, List, Union
 from widgets.base.exceptions import ResourceConfigurationException
 from widgets.base.exceptions import ResourceExecutionException
 from widgets.base.exceptions import CLIExecutionException
 from widgets.base.helpers import render_template
 
 
 class Resource:
@@ -475,14 +475,23 @@
             # Recursively call the same function
             return r._get_child(*cont)
         # If no additional levels were requested
         else:
             # Return the element
             return r
 
+    def _find_child(self, id) -> Generator['Resource', None, None]:
+        """Yield all nested child elements with the matching id."""
+
+        if self.id == id:
+            yield self
+
+        for child in self.children:
+            yield from child._find_child(id)
+
     def get(
         self,
         path: List[str] = [],
         attr: str = "value",
         **kwargs
     ) -> Any:
         """
```

### Comparing `widgets-lib-2.6.5/src/widgets/base/widget.py` & `widgets-lib-2.7.0/src/widgets/base/widget.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/cli/main.py` & `widgets-lib-2.7.0/src/widgets/cli/main.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/__init__.py` & `widgets-lib-2.7.0/src/widgets/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/base.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Union
+from typing import Any, Generator, List, Union
 import streamlit as st
 from streamlit.delta_generator import DeltaGenerator
 from widgets.base.exceptions import ResourceExecutionException
 from widgets.base.resource import Resource
 
 
 class StResource(Resource):
@@ -143,7 +143,11 @@
                 self.sidebar_container = self.sidebar_empty.container()
 
     def on_change(self):
         """Function optionally called when the ui element is changed."""
 
         # Set the value attribute on the resource
         self.value = st.session_state[self.key()]
+
+    def _find_child(self, id) -> Generator['StResource', None, None]:
+        """Yield all nested child elements with the matching id."""
+        yield from super()._find_child(id)
```

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/columns.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/columns.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,10 +90,10 @@
         if not self.disable_sidebar:
             self.sidebar_columns = self.sidebar_empty.columns(
                 self.spec, gap=self.gap
             )
 
         # Set up the children within those containers
         for ix, child in enumerate(self.children):
-            child.main_empty = self.main_columns[ix]
+            child.main_empty = self.main_columns[ix].empty()
             if not self.disable_sidebar:
-                child.sidebar_empty = self.sidebar_columns[ix]
+                child.sidebar_empty = self.sidebar_columns[ix].empty()
```

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/duplicator.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/expander.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/expander.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/files/base.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/files/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/files/dataframe.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/files/dataframe.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/files/download_dataframe.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/files/download_dataframe.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/markdown.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/markdown.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/selector.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/selector.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/base.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/values/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/checkbox.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/values/checkbox.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/float.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/values/float.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/integer.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/values/integer.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/multiselect.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/values/multiselect.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/selectstring.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/values/selectstring.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/slider.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/values/slider.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/string.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/values/string.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/textarea.py` & `widgets-lib-2.7.0/src/widgets/streamlit/resource/values/textarea.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/streamlit/widget/base.py` & `widgets-lib-2.7.0/src/widgets/streamlit/widget/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets/templates/streamlit_single.html.j2` & `widgets-lib-2.7.0/src/widgets/templates/streamlit_single.html.j2`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/src/widgets_lib.egg-info/PKG-INFO` & `widgets-lib-2.7.0/src/widgets_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.6.5
+Version: 2.7.0
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.6.5/src/widgets_lib.egg-info/SOURCES.txt` & `widgets-lib-2.7.0/src/widgets_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/tests/test_base.py` & `widgets-lib-2.7.0/tests/test_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 import unittest
 from widgets.base.exceptions import ResourceConfigurationException
 from widgets.base.exceptions import WidgetFunctionException
 from widgets.base.exceptions import ResourceExecutionException
 from widgets.base.resource import Resource
 from widgets.base.widget import Widget
 import widgets
@@ -79,35 +80,41 @@
         )
 
         self.assertRaises(
             ResourceConfigurationException,
             lambda: r._assert_isinstance(str, case=True)
         )
 
+    def setup_example_resource(self):
+
+        return deepcopy(
+            Resource(
+                id='top_list',
+                children=[
+                    Resource(id='first_resource', value='foo'),
+                    Resource(
+                        id='second_list',
+                        children=[
+                            Resource(id='second_resource', value='bar'),
+                            Resource(
+                                id='third_list',
+                                children=[
+                                    Resource(id='third_resource', value='howdy') # noqa
+                                ]
+                            )
+                        ]
+                    )
+                ]
+            )
+        )
+
     def test_child_value_assignment(self):
 
         # Define a Resource
-        r = Resource(
-            id='top_list',
-            children=[
-                Resource(id='first_resource', value='foo'),
-                Resource(
-                    id='second_list',
-                    children=[
-                        Resource(id='second_resource', value='bar'),
-                        Resource(
-                            id='third_list',
-                            children=[
-                                Resource(id='third_resource', value='howdy')
-                            ]
-                        )
-                    ]
-                )
-            ]
-        )
+        r = self.setup_example_resource()
 
         self.assertEqual(r.get(path=['first_resource']), 'foo')
         self.assertEqual(r.get(path=['second_list', 'second_resource']), 'bar')
         self.assertEqual(r.get(path=['second_list', 'third_list', 'third_resource']), 'howdy') # noqa
 
         # Change the values
         r.set(path=['first_resource'], value='FOO')
@@ -133,14 +140,30 @@
 
         # Test the exception raised when an attribute doesn't exist
         self.assertRaises(
             ResourceExecutionException,
             lambda: r.get(attr='missing_attribute')
         )
 
+    def test_find_child(self):
+        """Test the _find_child method."""
+
+        # Define a Resource
+        r = self.setup_example_resource()
+
+        for id, val in [
+            ('first_resource', 'foo'),
+            ('second_resource', 'bar'),
+            ('third_resource', 'howdy')
+        ]:
+            all_matching = list(r._find_child(id))
+
+            self.assertEqual(len(all_matching), 1, id)
+            self.assertEqual(all_matching[0].get_value(), val)
+
     def test_all_values(self):
 
         # Define a Resource
         r = Resource(
             id='top_list',
             children=[
                 Resource(id='first_resource', value='foo'),
```

### Comparing `widgets-lib-2.6.5/tests/test_cli.py` & `widgets-lib-2.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/tests/test_duplicator.py` & `widgets-lib-2.7.0/tests/test_duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/tests/test_helpers.py` & `widgets-lib-2.7.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/tests/test_io.py` & `widgets-lib-2.7.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/tests/test_source_parents.py` & `widgets-lib-2.7.0/tests/test_source_parents.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.5/tests/test_streamlit.py` & `widgets-lib-2.7.0/tests/test_streamlit.py`

 * *Files identical despite different names*

