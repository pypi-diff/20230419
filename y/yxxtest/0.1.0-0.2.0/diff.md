# Comparing `tmp/yxxtest-0.1.0.tar.gz` & `tmp/yxxtest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yxxtest-0.1.0.tar", last modified: Wed Apr 19 01:00:47 2023, max compression
+gzip compressed data, was "yxxtest-0.2.0.tar", last modified: Wed Apr 19 01:48:14 2023, max compression
```

## Comparing `yxxtest-0.1.0.tar` & `yxxtest-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 01:00:47.173288 yxxtest-0.1.0/
--rw-rw-rw-   0        0        0     1083 2023-04-19 01:00:27.000000 yxxtest-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      156 2023-04-19 01:00:47.173288 yxxtest-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-19 01:00:47.173288 yxxtest-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      305 2023-04-19 01:00:27.000000 yxxtest-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:00:47.159139 yxxtest-0.1.0/yTest/
--rw-rw-rw-   0        0        0        0 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:00:47.165981 yxxtest-0.1.0/yTest/common/
--rw-rw-rw-   0        0        0        0 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/common/__init__.py
--rw-rw-rw-   0        0        0      256 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/common/customize_error.py
--rw-rw-rw-   0        0        0      448 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/common/data_provider.py
--rw-rw-rw-   0        0        0    37242 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/common/html_reporter.py
--rw-rw-rw-   0        0        0     2720 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/common/my_logger.py
--rw-rw-rw-   0        0        0     4301 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/common/test_case_finder.py
--rw-rw-rw-   0        0        0      757 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/common/test_decorator.py
--rw-rw-rw-   0        0        0     1678 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/common/test_filter.py
--rw-rw-rw-   0        0        0     3356 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/common/user_options.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:00:47.166986 yxxtest-0.1.0/yTest/configs/
--rw-rw-rw-   0        0        0        0 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/configs/__init__.py
--rw-rw-rw-   0        0        0      259 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/configs/global_config.py
--rw-rw-rw-   0        0        0    11684 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/main.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:00:47.169283 yxxtest-0.1.0/yTest/utilities/
--rw-rw-rw-   0        0        0        0 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/utilities/__init__.py
--rw-rw-rw-   0        0        0      276 2023-04-04 09:46:44.000000 yxxtest-0.1.0/yTest/utilities/yaml_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:00:47.172288 yxxtest-0.1.0/yxxtest.egg-info/
--rw-rw-rw-   0        0        0      156 2023-04-19 01:00:47.000000 yxxtest-0.1.0/yxxtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-04-19 01:00:47.000000 yxxtest-0.1.0/yxxtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 01:00:47.000000 yxxtest-0.1.0/yxxtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-19 01:00:47.000000 yxxtest-0.1.0/yxxtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 01:00:47.000000 yxxtest-0.1.0/yxxtest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 01:48:14.947724 yxxtest-0.2.0/
+-rw-rw-rw-   0        0        0     1083 2023-04-19 01:00:27.000000 yxxtest-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      156 2023-04-19 01:48:14.946724 yxxtest-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-19 01:48:14.947724 yxxtest-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      305 2023-04-19 01:47:52.000000 yxxtest-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:48:14.931724 yxxtest-0.2.0/yTest/
+-rw-rw-rw-   0        0        0        0 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:48:14.939724 yxxtest-0.2.0/yTest/common/
+-rw-rw-rw-   0        0        0        0 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/common/__init__.py
+-rw-rw-rw-   0        0        0      256 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/common/customize_error.py
+-rw-rw-rw-   0        0        0      448 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/common/data_provider.py
+-rw-rw-rw-   0        0        0    37242 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/common/html_reporter.py
+-rw-rw-rw-   0        0        0     2720 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/common/my_logger.py
+-rw-rw-rw-   0        0        0     4301 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/common/test_case_finder.py
+-rw-rw-rw-   0        0        0      757 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/common/test_decorator.py
+-rw-rw-rw-   0        0        0     1678 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/common/test_filter.py
+-rw-rw-rw-   0        0        0     3356 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/common/user_options.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:48:14.940724 yxxtest-0.2.0/yTest/configs/
+-rw-rw-rw-   0        0        0        0 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/configs/__init__.py
+-rw-rw-rw-   0        0        0      259 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/configs/global_config.py
+-rw-rw-rw-   0        0        0    11684 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/main.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:48:14.941724 yxxtest-0.2.0/yTest/utilities/
+-rw-rw-rw-   0        0        0        0 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/utilities/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-04-04 09:46:44.000000 yxxtest-0.2.0/yTest/utilities/yaml_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:48:14.945724 yxxtest-0.2.0/yxxtest.egg-info/
+-rw-rw-rw-   0        0        0      156 2023-04-19 01:48:14.000000 yxxtest-0.2.0/yxxtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-04-19 01:48:14.000000 yxxtest-0.2.0/yxxtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 01:48:14.000000 yxxtest-0.2.0/yxxtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-19 01:48:14.000000 yxxtest-0.2.0/yxxtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 01:48:14.000000 yxxtest-0.2.0/yxxtest.egg-info/top_level.txt
```

### Comparing `yxxtest-0.1.0/LICENSE` & `yxxtest-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yxxtest-0.1.0/yTest/common/html_reporter.py` & `yxxtest-0.2.0/yTest/common/html_reporter.py`

 * *Files identical despite different names*

### Comparing `yxxtest-0.1.0/yTest/common/my_logger.py` & `yxxtest-0.2.0/yTest/common/my_logger.py`

 * *Files identical despite different names*

### Comparing `yxxtest-0.1.0/yTest/common/test_case_finder.py` & `yxxtest-0.2.0/yTest/common/test_case_finder.py`

 * *Files identical despite different names*

### Comparing `yxxtest-0.1.0/yTest/common/test_decorator.py` & `yxxtest-0.2.0/yTest/common/test_decorator.py`

 * *Files identical despite different names*

### Comparing `yxxtest-0.1.0/yTest/common/test_filter.py` & `yxxtest-0.2.0/yTest/common/test_filter.py`

 * *Files identical despite different names*

### Comparing `yxxtest-0.1.0/yTest/common/user_options.py` & `yxxtest-0.2.0/yTest/common/user_options.py`

 * *Files identical despite different names*

### Comparing `yxxtest-0.1.0/yTest/main.py` & `yxxtest-0.2.0/yTest/main.py`

 * *Files identical despite different names*

### Comparing `yxxtest-0.1.0/yxxtest.egg-info/SOURCES.txt` & `yxxtest-0.2.0/yxxtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

