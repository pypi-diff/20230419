# Comparing `tmp/integration_testing_environment_dev-0.0.8.tar.gz` & `tmp/integration_testing_environment_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integration_testing_environment_dev-0.0.8.tar", last modified: Tue Jul 26 13:36:05 2022, max compression
+gzip compressed data, was "integration_testing_environment_dev-0.0.9.tar", last modified: Tue Aug  2 15:54:25 2022, max compression
```

## Comparing `integration_testing_environment_dev-0.0.8.tar` & `integration_testing_environment_dev-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,77 @@
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.746191 integration_testing_environment_dev-0.0.8/
--rw-rw-rw-   0        0        0     1064 2022-06-07 07:13:35.000000 integration_testing_environment_dev-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      758 2022-07-26 13:36:05.745171 integration_testing_environment_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       33 2022-06-07 07:13:35.000000 integration_testing_environment_dev-0.0.8/README.md
--rw-rw-rw-   0        0        0     1093 2022-07-26 13:35:51.000000 integration_testing_environment_dev-0.0.8/dev_setup.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.621177 integration_testing_environment_dev-0.0.8/integration_testing_environment/
--rw-rw-rw-   0        0        0        2 2022-06-29 11:18:55.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/__init__.py
--rw-rw-rw-   0        0        0        0 2022-06-08 07:32:37.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/__main__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.622180 integration_testing_environment_dev-0.0.8/integration_testing_environment/extend/
--rw-rw-rw-   0        0        0        0 2022-06-23 09:12:21.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.625180 integration_testing_environment_dev-0.0.8/integration_testing_environment/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:11:09.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1629 2022-07-21 09:38:29.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.626372 integration_testing_environment_dev-0.0.8/integration_testing_environment/integration_testing_environment_ui/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:07:06.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/integration_testing_environment_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.637029 integration_testing_environment_dev-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/
--rw-rw-rw-   0        0        0        0 2022-06-23 09:09:49.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/__init__.py
--rw-rw-rw-   0        0        0     5673 2022-07-25 23:32:53.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/integration_testing_environment_ui/editor/extend_je_editor_ui.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.639037 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:11:18.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.643037 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/exception/
--rw-rw-rw-   0        0        0        0 2022-06-28 01:07:29.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1138 2022-07-16 14:34:25.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/exception/exception_tag.py
--rw-rw-rw-   0        0        0      329 2022-07-16 13:53:38.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.645037 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:13:36.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.647561 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/executor_manager/
--rw-rw-rw-   0        0        0        0 2022-06-08 07:13:53.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/executor_manager/__init__.py
--rw-rw-rw-   0        0        0     2174 2022-07-07 15:29:44.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/executor_manager/executor_manager.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.650560 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/generate_html_manager/
--rw-rw-rw-   0        0        0        0 2022-06-08 01:42:55.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/generate_html_manager/__init__.py
--rw-rw-rw-   0        0        0      873 2022-06-25 12:41:20.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/generate_html_manager/generate_html_manager.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.661293 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2022-06-24 04:24:37.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0     1227 2022-06-26 10:14:00.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.670842 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/redirect_manager/
--rw-rw-rw-   0        0        0        0 2022-07-11 05:49:53.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/redirect_manager/__init__.py
--rw-rw-rw-   0        0        0     1727 2022-07-16 05:13:31.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/redirect_manager/redirect_manager_class.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.681361 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.689912 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     1556 2022-07-21 09:45:59.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.699899 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     1568 2022-07-21 09:45:59.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/auto_control/auto_control_process.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.708423 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     1568 2022-07-21 09:45:59.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     6318 2022-07-22 15:29:01.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.716965 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     1556 2022-07-21 09:45:59.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2022-07-26 13:36:05.743663 integration_testing_environment_dev-0.0.8/integration_testing_environment_dev.egg-info/
--rw-rw-rw-   0        0        0      758 2022-07-26 13:36:05.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2631 2022-07-26 13:36:05.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-26 13:36:05.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2022-07-26 13:36:05.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2022-07-26 13:36:05.000000 integration_testing_environment_dev-0.0.8/integration_testing_environment_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-26 13:36:05.746191 integration_testing_environment_dev-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1089 2022-07-26 13:35:51.000000 integration_testing_environment_dev-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.916479 integration_testing_environment_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1064 2022-06-07 07:13:35.000000 integration_testing_environment_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      758 2022-08-02 15:54:25.914481 integration_testing_environment_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2022-06-07 07:13:35.000000 integration_testing_environment_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1093 2022-08-02 15:54:19.000000 integration_testing_environment_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.281409 integration_testing_environment_dev-0.0.9/integration_testing_environment/
+-rw-rw-rw-   0        0        0        2 2022-06-29 11:18:55.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:32:37.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/__main__.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.308477 integration_testing_environment_dev-0.0.9/integration_testing_environment/extend/
+-rw-rw-rw-   0        0        0        0 2022-06-23 09:12:21.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.338828 integration_testing_environment_dev-0.0.9/integration_testing_environment/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:11:09.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1629 2022-07-21 09:38:29.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.345847 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:07:06.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.353426 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/
+-rw-rw-rw-   0        0        0        0 2022-06-23 09:09:49.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/__init__.py
+-rw-rw-rw-   0        0        0     1155 2022-08-02 15:52:14.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/extend_je_editor_ui.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.375540 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/menu/
+-rw-rw-rw-   0        0        0        0 2022-08-02 11:00:06.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/menu/__init__.py
+-rw-rw-rw-   0        0        0     4021 2022-08-02 15:52:14.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/menu/build_ite_ui_menu.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.389090 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/redirect_output/
+-rw-rw-rw-   0        0        0        0 2022-08-02 11:00:40.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/redirect_output/__init__.py
+-rw-rw-rw-   0        0        0     1001 2022-08-02 15:52:14.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/integration_testing_environment_ui/editor/redirect_output/redirect_output_to_tkinter_ui.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.397110 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:11:18.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.438428 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/content/
+-rw-rw-rw-   0        0        0        0 2022-07-31 09:28:24.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/content/__init__.py
+-rw-rw-rw-   0        0        0     2137 2022-07-31 21:04:44.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/content/content_save.py
+-rw-rw-rw-   0        0        0       29 2022-07-31 10:10:52.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/content/ite_content_data.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.448953 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/exception/
+-rw-rw-rw-   0        0        0        0 2022-06-28 01:07:29.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1266 2022-08-02 10:52:46.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/exception/exception_tag.py
+-rw-rw-rw-   0        0        0      442 2022-07-31 20:56:14.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.494140 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/json_format/
+-rw-rw-rw-   0        0        0       42 2022-05-25 14:21:50.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1003 2022-07-31 21:04:44.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.496138 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:13:36.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.514247 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/executor_manager/
+-rw-rw-rw-   0        0        0        0 2022-06-08 07:13:53.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/executor_manager/__init__.py
+-rw-rw-rw-   0        0        0     2174 2022-07-07 15:29:44.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/executor_manager/executor_manager.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.542222 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/generate_html_manager/
+-rw-rw-rw-   0        0        0        0 2022-06-08 01:42:55.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/generate_html_manager/__init__.py
+-rw-rw-rw-   0        0        0      873 2022-06-25 12:41:20.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/generate_html_manager/generate_html_manager.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.567237 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2022-06-24 04:24:37.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     1227 2022-06-26 10:14:00.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.606456 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/redirect_manager/
+-rw-rw-rw-   0        0        0        0 2022-07-11 05:49:53.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/redirect_manager/__init__.py
+-rw-rw-rw-   0        0        0     1727 2022-07-16 05:13:31.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/redirect_manager/redirect_manager_class.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.631101 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/project/
+-rw-rw-rw-   0        0        0        0 2022-07-27 18:46:45.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/project/__init__.py
+-rw-rw-rw-   0        0        0      369 2022-07-28 09:27:55.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/project/create_project.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.637102 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.676753 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     1556 2022-07-21 09:45:59.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.721101 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     1568 2022-07-21 09:45:59.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/auto_control/auto_control_process.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.756703 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     1568 2022-07-21 09:45:59.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     6334 2022-08-02 15:47:45.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.821139 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2022-07-20 13:40:25.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     1556 2022-07-21 09:45:59.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2022-08-02 15:54:25.899877 integration_testing_environment_dev-0.0.9/integration_testing_environment_dev.egg-info/
+-rw-rw-rw-   0        0        0      758 2022-08-02 15:54:24.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3483 2022-08-02 15:54:24.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-02 15:54:24.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2022-08-02 15:54:24.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2022-08-02 15:54:24.000000 integration_testing_environment_dev-0.0.9/integration_testing_environment_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-08-02 15:54:25.918479 integration_testing_environment_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2022-07-26 13:35:51.000000 integration_testing_environment_dev-0.0.9/setup.py
```

### Comparing `integration_testing_environment_dev-0.0.8/LICENSE` & `integration_testing_environment_dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/PKG-INFO` & `integration_testing_environment_dev-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integration_testing_environment_dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: Integration testing environment for web gui api load testing
 Home-page: https://github.com/JE-Chen/WebRunner
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `integration_testing_environment_dev-0.0.8/dev_setup.py` & `integration_testing_environment_dev-0.0.9/dev_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="integration_testing_environment_dev",
-    version="0.0.8",
+    version="0.0.9",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="Integration testing environment for web gui api load testing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/WebRunner",
     packages=setuptools.find_packages(),
```

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/extend/mail_thunder_extend/mail_thunder_setting.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/exception/exception_tag.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/exception/exception_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,7 +16,10 @@
 # ui exception
 wrong_test_data_format_exception_tag = "get the wrong test data format"
 # exec exception
 exec_error = "ITE exec error"
 file_not_fond_error = "File not found"
 compiler_not_found_error = "Compiler not found"
 not_install_package_error = "not install required package"
+# json exception
+cant_reformat_json_error = "Can't reformat json is type right?"
+wrong_json_data_error = "Can't parser json"
```

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/executor_manager/executor_manager.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/executor_manager/executor_manager.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/generate_html_manager/generate_html_manager.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/generate_html_manager/generate_html_manager.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/package_manager/package_manager_class.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/manager/redirect_manager/redirect_manager_class.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/manager/redirect_manager/redirect_manager_class.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/api_testka/api_testka_process.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/auto_control/auto_control_process.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/load_density/load_density_process.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/task_process_manager.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/task_process_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(
             self, title_name: str,
             task_done_trigger_function: typing.Callable = None,
             error_trigger_function: typing.Callable = None,
             use_theme=None
     ):
         super().__init__()
-        # self param
+        # ite_instance param
         self.read_program_error_output_from_thread = None
         self.read_program_output_from_thread = None
         self.still_run_program = True
         self.program_encoding = "utf-8"
         self.run_output_queue = Queue()
         self.run_error_queue = Queue()
         self.process = None
@@ -33,15 +33,15 @@
         self.tkinter_text_scrollbar_y = None
         self.tkinter_text_scrollbar_x = None
         self.style = ttk.Style()
         if use_theme is not None:
             self.style.theme_use(use_theme)
 
     def set_ui(self):
-        # self tkinter ui
+        # ite_instance tkinter ui
         self.tkinter_top_level = Toplevel()
         self.tkinter_text_frame = ttk.Frame(self.tkinter_top_level, padding="3 3 12 12")
         self.tkinter_text = Text(self.tkinter_text_frame, wrap="none")
         self.tkinter_text_scrollbar_y = ttk.Scrollbar(self.tkinter_text_frame, orient="vertical",
                                                       command=self.tkinter_text.yview)
         self.tkinter_text_scrollbar_x = ttk.Scrollbar(self.tkinter_text_frame, orient="horizontal",
                                                       command=self.tkinter_text.xview)
```

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment/utils/test_executor/web_runner/web_runner_process.py` & `integration_testing_environment_dev-0.0.9/integration_testing_environment/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment_dev.egg-info/PKG-INFO` & `integration_testing_environment_dev-0.0.9/integration_testing_environment_dev.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integration-testing-environment-dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: Integration testing environment for web gui api load testing
 Home-page: https://github.com/JE-Chen/WebRunner
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `integration_testing_environment_dev-0.0.8/integration_testing_environment_dev.egg-info/SOURCES.txt` & `integration_testing_environment_dev-0.0.9/integration_testing_environment_dev.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,27 +6,38 @@
 integration_testing_environment/__main__.py
 integration_testing_environment/extend/__init__.py
 integration_testing_environment/extend/mail_thunder_extend/__init__.py
 integration_testing_environment/extend/mail_thunder_extend/mail_thunder_setting.py
 integration_testing_environment/integration_testing_environment_ui/__init__.py
 integration_testing_environment/integration_testing_environment_ui/editor/__init__.py
 integration_testing_environment/integration_testing_environment_ui/editor/extend_je_editor_ui.py
+integration_testing_environment/integration_testing_environment_ui/editor/menu/__init__.py
+integration_testing_environment/integration_testing_environment_ui/editor/menu/build_ite_ui_menu.py
+integration_testing_environment/integration_testing_environment_ui/editor/redirect_output/__init__.py
+integration_testing_environment/integration_testing_environment_ui/editor/redirect_output/redirect_output_to_tkinter_ui.py
 integration_testing_environment/utils/__init__.py
+integration_testing_environment/utils/content/__init__.py
+integration_testing_environment/utils/content/content_save.py
+integration_testing_environment/utils/content/ite_content_data.py
 integration_testing_environment/utils/exception/__init__.py
 integration_testing_environment/utils/exception/exception_tag.py
 integration_testing_environment/utils/exception/exceptions.py
+integration_testing_environment/utils/json_format/__init__.py
+integration_testing_environment/utils/json_format/json_process.py
 integration_testing_environment/utils/manager/__init__.py
 integration_testing_environment/utils/manager/executor_manager/__init__.py
 integration_testing_environment/utils/manager/executor_manager/executor_manager.py
 integration_testing_environment/utils/manager/generate_html_manager/__init__.py
 integration_testing_environment/utils/manager/generate_html_manager/generate_html_manager.py
 integration_testing_environment/utils/manager/package_manager/__init__.py
 integration_testing_environment/utils/manager/package_manager/package_manager_class.py
 integration_testing_environment/utils/manager/redirect_manager/__init__.py
 integration_testing_environment/utils/manager/redirect_manager/redirect_manager_class.py
+integration_testing_environment/utils/project/__init__.py
+integration_testing_environment/utils/project/create_project.py
 integration_testing_environment/utils/test_executor/__init__.py
 integration_testing_environment/utils/test_executor/task_process_manager.py
 integration_testing_environment/utils/test_executor/api_testka/__init__.py
 integration_testing_environment/utils/test_executor/api_testka/api_testka_process.py
 integration_testing_environment/utils/test_executor/auto_control/__init__.py
 integration_testing_environment/utils/test_executor/auto_control/auto_control_process.py
 integration_testing_environment/utils/test_executor/load_density/__init__.py
```

### Comparing `integration_testing_environment_dev-0.0.8/setup.py` & `integration_testing_environment_dev-0.0.9/setup.py`

 * *Files identical despite different names*

