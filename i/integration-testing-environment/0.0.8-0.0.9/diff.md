# Comparing `tmp/integration_testing_environment-0.0.8.tar.gz` & `tmp/integration_testing_environment-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integration_testing_environment-0.0.8.tar", last modified: Mon Sep 12 05:55:12 2022, max compression
+gzip compressed data, was "integration_testing_environment-0.0.9.tar", last modified: Mon Sep 12 07:23:28 2022, max compression
```

## Comparing `integration_testing_environment-0.0.8.tar` & `integration_testing_environment-0.0.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.562308 integration_testing_environment-0.0.8/
--rw-rw-rw-   0        0        0     1064 2022-06-07 07:13:35.000000 integration_testing_environment-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      776 2022-09-12 05:55:12.561306 integration_testing_environment-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       33 2022-06-07 07:13:35.000000 integration_testing_environment-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.479330 integration_testing_environment-0.0.8/integration_testing_environment/
--rw-rw-rw-   0        0        0      117 2022-09-05 08:14:36.000000 integration_testing_environment-0.0.8/integration_testing_environment/__init__.py
--rw-rw-rw-   0        0        0        0 2022-06-08 07:32:37.000000 integration_testing_environment-0.0.8/integration_testing_environment/__main__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.500332 integration_testing_environment-0.0.8/integration_testing_environment/extend/
--rw-rw-rw-   0        0        0        0 2022-06-23 09:12:21.000000 integration_testing_environment-0.0.8/integration_testing_environment/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.502293 integration_testing_environment-0.0.8/integration_testing_environment/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:11:09.000000 integration_testing_environment-0.0.8/integration_testing_environment/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1629 2022-07-21 09:38:29.000000 integration_testing_environment-0.0.8/integration_testing_environment/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.504291 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:07:06.000000 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.507337 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/
--rw-rw-rw-   0        0        0        0 2022-06-23 09:09:49.000000 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/__init__.py
--rw-rw-rw-   0        0        0     1131 2022-09-07 17:00:29.000000 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/extend_je_editor_ui.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.510337 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/ite_content_init/
--rw-rw-rw-   0        0        0        0 2022-08-05 13:23:32.000000 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/ite_content_init/__init__.py
--rw-rw-rw-   0        0        0      702 2022-09-02 15:59:49.000000 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/ite_content_init/ite_content_init.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.513294 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/menu/
--rw-rw-rw-   0        0        0        0 2022-08-02 11:00:06.000000 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/menu/__init__.py
--rw-rw-rw-   0        0        0     6399 2022-09-08 12:12:14.000000 integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/menu/build_ite_ui_menu.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.515292 integration_testing_environment-0.0.8/integration_testing_environment/utils/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:11:18.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.519293 integration_testing_environment-0.0.8/integration_testing_environment/utils/content/
--rw-rw-rw-   0        0        0        0 2022-07-31 09:28:24.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/content/__init__.py
--rw-rw-rw-   0        0        0     2113 2022-08-05 13:54:35.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/content/content_save.py
--rw-rw-rw-   0        0        0       60 2022-08-05 14:07:44.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/content/ite_content_data.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.523339 integration_testing_environment-0.0.8/integration_testing_environment/utils/exception/
--rw-rw-rw-   0        0        0        0 2022-06-28 01:07:29.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1266 2022-08-02 10:52:46.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/exception/exception_tag.py
--rw-rw-rw-   0        0        0      442 2022-07-31 20:56:14.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.526624 integration_testing_environment-0.0.8/integration_testing_environment/utils/file_process/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1094 2022-09-07 16:24:33.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.529635 integration_testing_environment-0.0.8/integration_testing_environment/utils/json_format/
--rw-rw-rw-   0        0        0       42 2022-05-25 14:21:50.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1003 2022-07-31 21:04:44.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.532747 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:13:36.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.534798 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/executor_manager/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:13:53.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/executor_manager/__init__.py
--rw-rw-rw-   0        0        0     2174 2022-07-07 15:29:44.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/executor_manager/executor_manager.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.537797 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/generate_html_manager/
--rw-rw-rw-   0        0        0        0 2022-06-08 01:42:55.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/generate_html_manager/__init__.py
--rw-rw-rw-   0        0        0      873 2022-06-25 12:41:20.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/generate_html_manager/generate_html_manager.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.540758 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2022-06-24 04:24:37.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0     1227 2022-06-26 10:14:00.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.544005 integration_testing_environment-0.0.8/integration_testing_environment/utils/project/
--rw-rw-rw-   0        0        0        0 2022-07-27 18:46:45.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/project/__init__.py
--rw-rw-rw-   0        0        0      345 2022-08-05 15:29:14.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/project/create_project.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.547041 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.550261 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3006 2022-09-08 11:25:04.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.553306 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     2999 2022-09-08 11:39:38.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/auto_control/auto_control_process.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.556305 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     2999 2022-09-08 11:49:08.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     7120 2022-09-02 15:59:49.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.559306 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     2979 2022-09-08 11:49:08.000000 integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2022-09-12 05:55:12.498292 integration_testing_environment-0.0.8/integration_testing_environment.egg-info/
--rw-rw-rw-   0        0        0      776 2022-09-12 05:55:12.000000 integration_testing_environment-0.0.8/integration_testing_environment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3410 2022-09-12 05:55:12.000000 integration_testing_environment-0.0.8/integration_testing_environment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-12 05:55:12.000000 integration_testing_environment-0.0.8/integration_testing_environment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2022-09-12 05:55:12.000000 integration_testing_environment-0.0.8/integration_testing_environment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2022-09-12 05:55:12.000000 integration_testing_environment-0.0.8/integration_testing_environment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-12 05:55:12.562308 integration_testing_environment-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1111 2022-09-12 05:55:04.000000 integration_testing_environment-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.639380 integration_testing_environment-0.0.9/
+-rw-rw-rw-   0        0        0     1064 2022-06-07 07:13:35.000000 integration_testing_environment-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1693 2022-09-12 07:23:28.639380 integration_testing_environment-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2022-09-12 07:22:15.000000 integration_testing_environment-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.558076 integration_testing_environment-0.0.9/integration_testing_environment/
+-rw-rw-rw-   0        0        0      117 2022-09-05 08:14:36.000000 integration_testing_environment-0.0.9/integration_testing_environment/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:32:37.000000 integration_testing_environment-0.0.9/integration_testing_environment/__main__.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.578042 integration_testing_environment-0.0.9/integration_testing_environment/extend/
+-rw-rw-rw-   0        0        0        0 2022-06-23 09:12:21.000000 integration_testing_environment-0.0.9/integration_testing_environment/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.581095 integration_testing_environment-0.0.9/integration_testing_environment/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:11:09.000000 integration_testing_environment-0.0.9/integration_testing_environment/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1629 2022-07-21 09:38:29.000000 integration_testing_environment-0.0.9/integration_testing_environment/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.582085 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:07:06.000000 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.585040 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/
+-rw-rw-rw-   0        0        0        0 2022-06-23 09:09:49.000000 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/__init__.py
+-rw-rw-rw-   0        0        0     1131 2022-09-07 17:00:29.000000 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/extend_je_editor_ui.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.588039 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/ite_content_init/
+-rw-rw-rw-   0        0        0        0 2022-08-05 13:23:32.000000 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/ite_content_init/__init__.py
+-rw-rw-rw-   0        0        0      702 2022-09-02 15:59:49.000000 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/ite_content_init/ite_content_init.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.594084 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/menu/
+-rw-rw-rw-   0        0        0        0 2022-08-02 11:00:06.000000 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/menu/__init__.py
+-rw-rw-rw-   0        0        0     6399 2022-09-08 12:12:14.000000 integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/menu/build_ite_ui_menu.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.595039 integration_testing_environment-0.0.9/integration_testing_environment/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:11:18.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.600082 integration_testing_environment-0.0.9/integration_testing_environment/utils/content/
+-rw-rw-rw-   0        0        0        0 2022-07-31 09:28:24.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/content/__init__.py
+-rw-rw-rw-   0        0        0     2113 2022-08-05 13:54:35.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/content/content_save.py
+-rw-rw-rw-   0        0        0       60 2022-08-05 14:07:44.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/content/ite_content_data.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.604039 integration_testing_environment-0.0.9/integration_testing_environment/utils/exception/
+-rw-rw-rw-   0        0        0        0 2022-06-28 01:07:29.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1266 2022-08-02 10:52:46.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/exception/exception_tag.py
+-rw-rw-rw-   0        0        0      442 2022-07-31 20:56:14.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.607040 integration_testing_environment-0.0.9/integration_testing_environment/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1094 2022-09-07 16:24:33.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.610045 integration_testing_environment-0.0.9/integration_testing_environment/utils/json_format/
+-rw-rw-rw-   0        0        0       42 2022-05-25 14:21:50.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1003 2022-07-31 21:04:44.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.611039 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:13:36.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.614036 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/executor_manager/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:13:53.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/executor_manager/__init__.py
+-rw-rw-rw-   0        0        0     2174 2022-07-07 15:29:44.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/executor_manager/executor_manager.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.617086 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/generate_html_manager/
+-rw-rw-rw-   0        0        0        0 2022-06-08 01:42:55.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/generate_html_manager/__init__.py
+-rw-rw-rw-   0        0        0      873 2022-06-25 12:41:20.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/generate_html_manager/generate_html_manager.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.619035 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2022-06-24 04:24:37.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     1227 2022-06-26 10:14:00.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.623077 integration_testing_environment-0.0.9/integration_testing_environment/utils/project/
+-rw-rw-rw-   0        0        0        0 2022-07-27 18:46:45.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/project/__init__.py
+-rw-rw-rw-   0        0        0      345 2022-08-05 15:29:14.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/project/create_project.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.626074 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.628047 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3006 2022-09-08 11:25:04.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.631039 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     2999 2022-09-08 11:39:38.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/auto_control/auto_control_process.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.634204 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     2999 2022-09-08 11:49:08.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     7120 2022-09-02 15:59:49.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.637214 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     2979 2022-09-08 11:49:08.000000 integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2022-09-12 07:23:28.576038 integration_testing_environment-0.0.9/integration_testing_environment.egg-info/
+-rw-rw-rw-   0        0        0     1693 2022-09-12 07:23:28.000000 integration_testing_environment-0.0.9/integration_testing_environment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3410 2022-09-12 07:23:28.000000 integration_testing_environment-0.0.9/integration_testing_environment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-12 07:23:28.000000 integration_testing_environment-0.0.9/integration_testing_environment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2022-09-12 07:23:28.000000 integration_testing_environment-0.0.9/integration_testing_environment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2022-09-12 07:23:28.000000 integration_testing_environment-0.0.9/integration_testing_environment.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-09-12 07:23:28.640391 integration_testing_environment-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2022-09-12 07:23:19.000000 integration_testing_environment-0.0.9/setup.py
```

### Comparing `integration_testing_environment-0.0.8/LICENSE` & `integration_testing_environment-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/extend/mail_thunder_extend/mail_thunder_setting.py` & `integration_testing_environment-0.0.9/integration_testing_environment/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/extend_je_editor_ui.py` & `integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/extend_je_editor_ui.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/ite_content_init/ite_content_init.py` & `integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/ite_content_init/ite_content_init.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/menu/build_ite_ui_menu.py` & `integration_testing_environment-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/menu/build_ite_ui_menu.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/content/content_save.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/content/content_save.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/exception/exception_tag.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/exception/exception_tag.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/file_process/get_dir_file_list.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/json_format/json_process.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/executor_manager/executor_manager.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/executor_manager/executor_manager.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/generate_html_manager/generate_html_manager.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/generate_html_manager/generate_html_manager.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/manager/package_manager/package_manager_class.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/api_testka/api_testka_process.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/auto_control/auto_control_process.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/load_density/load_density_process.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/task_process_manager.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/task_process_manager.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment/utils/test_executor/web_runner/web_runner_process.py` & `integration_testing_environment-0.0.9/integration_testing_environment/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/integration_testing_environment.egg-info/SOURCES.txt` & `integration_testing_environment-0.0.9/integration_testing_environment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `integration_testing_environment-0.0.8/setup.py` & `integration_testing_environment-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="integration_testing_environment",
-    version="0.0.8",
+    version="0.0.9",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="Integration testing environment for web gui api load testing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/Integration-testing-environment",
     packages=setuptools.find_packages(),
```

