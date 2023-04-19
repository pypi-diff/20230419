# Comparing `tmp/shiny-0.3.0.tar.gz` & `tmp/shiny-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny-0.3.0.tar", last modified: Mon Apr  3 22:12:43 2023, max compression
+gzip compressed data, was "shiny-0.3.1.tar", last modified: Wed Apr 19 02:03:12 2023, max compression
```

## Comparing `shiny-0.3.0.tar` & `shiny-0.3.1.tar`

### file list

```diff
@@ -1,475 +1,463 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.848434 shiny-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 22:11:43.000000 shiny-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-03 22:11:43.000000 shiny-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-03 22:12:43.848434 shiny-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-03 22:11:43.000000 shiny-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.784433 shiny-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-03 22:11:43.000000 shiny-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.784433 shiny-0.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.784433 shiny-0.3.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-03 22:11:43.000000 shiny-0.3.0/docs/source/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-03 22:11:43.000000 shiny-0.3.0/docs/source/_templates/justattributes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-03 22:11:43.000000 shiny-0.3.0/docs/source/_templates/tag_func.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-03 22:11:43.000000 shiny-0.3.0/docs/source/_templates/tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-03 22:11:43.000000 shiny-0.3.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.784433 shiny-0.3.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   183015 2023-04-03 22:11:43.000000 shiny-0.3.0/docs/source/images/shiny-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-03 22:11:43.000000 shiny-0.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-03 22:12:43.852434 shiny-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 22:11:43.000000 shiny-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.788433 shiny-0.3.0/shiny/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_fileupload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_hostenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_launchbrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_shinyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_static.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.780433 shiny-0.3.0/shiny/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/Calc/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/Calc/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/Effect/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/Effect/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/Module/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/Module/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/Progress/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/Progress/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/SafeException/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/SafeException/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/SilentCancelOutputException/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/SilentCancelOutputException/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/SilentException/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/SilentException/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/Value/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/Value/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/close/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/close/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/download/
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/download/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/download/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny/examples/download_button/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/download_button/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/download_button/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/download_link/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/download_link/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/download_link/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/dynamic_route/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/dynamic_route/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/event/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/event/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/file_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/file_reader/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/file_reader/mtcars.csv
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/file_reader/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_action_button/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_action_button/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_action_link/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_action_link/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_checkbox/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_checkbox_group/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_checkbox_group/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_date/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_date/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_date_range/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_date_range/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_file/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_file/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_numeric/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_password/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_password/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_radio_buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_radio_buttons/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_select/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_select/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_selectize/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_selectize/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_slider/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_slider/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_switch/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_switch/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_text/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/input_text_area/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/input_text_area/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/insert_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/insert_ui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/invalidate_later/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/invalidate_later/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/isolate/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/isolate/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/layout_sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/layout_sidebar/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/markdown/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.796433 shiny-0.3.0/shiny/examples/modal/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/modal/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/nav/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/nav/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/navset_hidden/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/navset_hidden/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/notification_show/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/notification_show/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/on_ended/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/on_ended/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/on_flush/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/on_flush/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/on_flushed/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/on_flushed/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/output_image/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/output_image/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/output_image/rstudio-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/output_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/output_plot/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/output_table/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/output_table/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/output_table/mtcars.csv
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/output_table/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/output_text/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/output_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/output_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/output_ui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/page_fixed/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/page_fixed/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/page_fluid/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/page_fluid/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/panel_absolute/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/panel_absolute/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/panel_conditional/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/panel_conditional/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/panel_title/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/panel_title/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/poll/
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/poll/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/remove_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/remove_ui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/render_image/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/render_image/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/req/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/req/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/row/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/row/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/send_custom_message/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/send_custom_message/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/template/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/update_action_button/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_action_button/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/update_checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_checkbox/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/update_checkbox_group/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_checkbox_group/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/update_date/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_date/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.800433 shiny-0.3.0/shiny/examples/update_date_range/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_date_range/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/update_navs/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_navs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/update_numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_numeric/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/update_radio_buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_radio_buttons/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/update_select/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_select/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/update_selectize/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_selectize/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/update_slider/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_slider/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/update_text/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/update_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/www_dir/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/www_dir/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.780433 shiny-0.3.0/shiny/examples/www_dir/www/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/www_dir/www/css/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/www_dir/www/css/more-styles.css
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/www_dir/www/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/examples/www_dir/www/js/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/examples/www_dir/www/js/changetext.js
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/html_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/http_staticfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/input_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/plotutils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/reactive/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/reactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/reactive/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/reactive/_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)    29615 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/reactive/_reactives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/render/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/render/_coordmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    25087 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/render/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/render/_try_render_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.804433 shiny-0.3.0/shiny/session/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39319 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/session/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/session/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.808434 shiny-0.3.0/shiny/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_download_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_html_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_action_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_check_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_input_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    26782 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_navs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_plot_output_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/ui/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.780433 shiny-0.3.0/shiny/www/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.812434 shiny-0.3.0/shiny/www/shared/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.816434 shiny-0.3.0/shiny/www/shared/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)    78468 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   327261 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   207811 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/bootstrap/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.780433 shiny-0.3.0/shiny/www/shared/bootstrap/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.816434 shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.816434 shiny-0.3.0/shiny/www/shared/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.816434 shiny-0.3.0/shiny/www/shared/datatables/css/
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/css/dataTables.bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/css/dataTables.extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.816434 shiny-0.3.0/shiny/www/shared/datatables/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/images/sort_asc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/images/sort_desc_disabled.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.816434 shiny-0.3.0/shiny/www/shared/datatables/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/js/dataTables.bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)    78980 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datatables/upgrade1.10.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.780433 shiny-0.3.0/shiny/www/shared/datepicker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.816434 shiny-0.3.0/shiny/www/shared/datepicker/css/
--rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css
--rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.816434 shiny-0.3.0/shiny/www/shared/datepicker/js/
--rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   106348 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.828434 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.br.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cy.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.gl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.id.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.is.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ja.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.me.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ms.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt-BR.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ro.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sw.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.828434 shiny-0.3.0/shiny/www/shared/datepicker/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/scss/build3.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/datepicker/scss/datepicker3.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.828434 shiny-0.3.0/shiny/www/shared/highlight/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/highlight/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/highlight/classref.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/highlight/highlight.pack.js
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/highlight/rstudio.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.780433 shiny-0.3.0/shiny/www/shared/ionrangeslider/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.832434 shiny-0.3.0/shiny/www/shared/ionrangeslider/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.836434 shiny-0.3.0/shiny/www/shared/ionrangeslider/js/
--rw-r--r--   0 runner    (1001) docker     (123)    84956 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js
--rw-r--r--   0 runner    (1001) docker     (123)    41602 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.836434 shiny-0.3.0/shiny/www/shared/ionrangeslider/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/ionrangeslider/scss/_base.scss
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/ionrangeslider/scss/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/ionrangeslider/scss/shiny.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.836434 shiny-0.3.0/shiny/www/shared/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jquery/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jquery/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jquery/jquery-3.6.0.min.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.840434 shiny-0.3.0/shiny/www/shared/jqueryui/
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.844434 shiny-0.3.0/shiny/www/shared/jqueryui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    37452 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   529159 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    32130 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.structure.css
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.structure.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.theme.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.844434 shiny-0.3.0/shiny/www/shared/requirejs/
--rw-r--r--   0 runner    (1001) docker     (123)    19715 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/requirejs/require.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.780433 shiny-0.3.0/shiny/www/shared/selectize/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.780433 shiny-0.3.0/shiny/www/shared/selectize/accessibility/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.844434 shiny-0.3.0/shiny/www/shared/selectize/accessibility/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.844434 shiny-0.3.0/shiny/www/shared/selectize/css/
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/css/selectize.bootstrap3.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.844434 shiny-0.3.0/shiny/www/shared/selectize/js/
--rw-r--r--   0 runner    (1001) docker     (123)    45139 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/js/selectize.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.844434 shiny-0.3.0/shiny/www/shared/selectize/scss/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.844434 shiny-0.3.0/shiny/www/shared/selectize/scss/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/scss/plugins/drag_drop.scss
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/scss/plugins/optgroup_columns.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/scss/plugins/remove_button.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/scss/selectize.bootstrap5.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/scss/selectize.default.scss
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/selectize/scss/selectize.scss
--rw-r--r--   0 runner    (1001) docker     (123)    23760 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny-autoreload.js
--rw-r--r--   0 runner    (1001) docker     (123)   125989 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny-autoreload.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny-showcase.css
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny-showcase.js
--rw-r--r--   0 runner    (1001) docker     (123)   126645 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny-showcase.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny-testmode.js
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny-testmode.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   757524 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny.js
--rw-r--r--   0 runner    (1001) docker     (123)  1314664 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   306317 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1349172 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.844434 shiny-0.3.0/shiny/www/shared/shiny_scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny_scss/bootstrap.scss
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/shiny_scss/shiny.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.844434 shiny-0.3.0/shiny/www/shared/showdown/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.848434 shiny-0.3.0/shiny/www/shared/showdown/compressed/
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/showdown/compressed/showdown.js
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/showdown/license.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.848434 shiny-0.3.0/shiny/www/shared/showdown/src/
--rw-r--r--   0 runner    (1001) docker     (123)    37933 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/showdown/src/showdown.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.848434 shiny-0.3.0/shiny/www/shared/strftime/
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-03 22:11:43.000000 shiny-0.3.0/shiny/www/shared/strftime/strftime-min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.792433 shiny-0.3.0/shiny.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-03 22:12:43.000000 shiny-0.3.0/shiny.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-04-03 22:12:43.000000 shiny-0.3.0/shiny.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 22:12:43.000000 shiny-0.3.0/shiny.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-03 22:12:43.000000 shiny-0.3.0/shiny.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 22:12:43.000000 shiny-0.3.0/shiny.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-03 22:12:43.000000 shiny-0.3.0/shiny.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-03 22:12:43.000000 shiny-0.3.0/shiny.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:12:43.848434 shiny-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/asyncio_prevent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/mocktime.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_e2e_regex_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_navs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)    31010 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_reactives.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_shinysession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-03 22:11:43.000000 shiny-0.3.0/tests/test_utils_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.852359 shiny-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 02:02:08.000000 shiny-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-19 02:02:08.000000 shiny-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-19 02:03:12.852359 shiny-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-19 02:02:08.000000 shiny-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-19 02:03:12.852359 shiny-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 02:02:08.000000 shiny-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_fileupload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_hostenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_launchbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_shinyenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.788359 shiny-0.3.1/shiny/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/Calc/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/Calc/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/Effect/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/Effect/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/Module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/Module/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/Progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/Progress/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/SafeException/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/SafeException/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/SilentCancelOutputException/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/SilentCancelOutputException/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/SilentException/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/SilentException/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/Value/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/Value/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/close/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/close/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/download/
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/download/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/download/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny/examples/download_button/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/download_button/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/download_button/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/download_link/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/download_link/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/download_link/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/dynamic_route/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/dynamic_route/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/event/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/event/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/file_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/file_reader/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/file_reader/mtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/file_reader/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_action_button/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_action_button/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_action_link/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_action_link/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_checkbox/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_checkbox_group/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_checkbox_group/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_date/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_date/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_date_range/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_date_range/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_file/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_file/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_numeric/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_password/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_password/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_radio_buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_radio_buttons/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_select/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_select/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_selectize/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_selectize/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_slider/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_slider/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_switch/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_switch/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/input_text_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/input_text_area/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/insert_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/insert_ui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/invalidate_later/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/invalidate_later/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/isolate/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/isolate/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/layout_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/layout_sidebar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/markdown/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/modal/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/nav/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.800359 shiny-0.3.1/shiny/examples/navset_hidden/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/navset_hidden/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/notification_show/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/notification_show/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/on_ended/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/on_ended/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/on_flush/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/on_flush/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/on_flushed/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/on_flushed/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/output_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/output_image/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/output_image/rstudio-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/output_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/output_plot/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/output_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/output_table/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/output_table/mtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/output_table/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/output_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/output_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/output_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/output_ui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/page_fixed/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/page_fixed/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/page_fluid/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/page_fluid/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/panel_absolute/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/panel_absolute/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/panel_conditional/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/panel_conditional/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/panel_title/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/panel_title/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/poll/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/poll/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/remove_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/remove_ui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/render_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/render_image/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/req/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/req/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/row/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/row/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/send_custom_message/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/send_custom_message/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_action_button/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_action_button/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_checkbox/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_checkbox_group/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_checkbox_group/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_date/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_date/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_date_range/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_date_range/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_navs/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_navs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_numeric/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_radio_buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_radio_buttons/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_select/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_select/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.804359 shiny-0.3.1/shiny/examples/update_selectize/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_selectize/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.808359 shiny-0.3.1/shiny/examples/update_slider/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_slider/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.808359 shiny-0.3.1/shiny/examples/update_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/update_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.808359 shiny-0.3.1/shiny/examples/www_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/www_dir/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.788359 shiny-0.3.1/shiny/examples/www_dir/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.808359 shiny-0.3.1/shiny/examples/www_dir/www/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/www_dir/www/css/more-styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/www_dir/www/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.808359 shiny-0.3.1/shiny/examples/www_dir/www/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/examples/www_dir/www/js/changetext.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/html_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/http_staticfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/input_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/plotutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.808359 shiny-0.3.1/shiny/reactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/reactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/reactive/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/reactive/_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30436 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/reactive/_reactives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.808359 shiny-0.3.1/shiny/render/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/render/_coordmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25137 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/render/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/render/_try_render_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.808359 shiny-0.3.1/shiny/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39788 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/session/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/session/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.812359 shiny-0.3.1/shiny/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_download_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_html_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_action_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_check_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26041 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_input_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27410 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_navs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_plot_output_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/ui/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.788359 shiny-0.3.1/shiny/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.816359 shiny-0.3.1/shiny/www/shared/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.820359 shiny-0.3.1/shiny/www/shared/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    78468 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/bootstrap/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   327261 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   207811 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/bootstrap/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.788359 shiny-0.3.1/shiny/www/shared/bootstrap/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.820359 shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.820359 shiny-0.3.1/shiny/www/shared/datatables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.820359 shiny-0.3.1/shiny/www/shared/datatables/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/css/dataTables.bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/css/dataTables.extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.824359 shiny-0.3.1/shiny/www/shared/datatables/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/images/sort_asc_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/images/sort_desc_disabled.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.824359 shiny-0.3.1/shiny/www/shared/datatables/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/js/dataTables.bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78980 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datatables/upgrade1.10.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.788359 shiny-0.3.1/shiny/www/shared/datepicker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.824359 shiny-0.3.1/shiny/www/shared/datepicker/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.824359 shiny-0.3.1/shiny/www/shared/datepicker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/bootstrap-datepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   106348 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.840359 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.br.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cy.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.gl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.id.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.is.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ja.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.me.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ms.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt-BR.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ro.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sw.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.840359 shiny-0.3.1/shiny/www/shared/datepicker/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/scss/build3.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/datepicker/scss/datepicker3.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.840359 shiny-0.3.1/shiny/www/shared/highlight/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/highlight/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/highlight/classref.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/highlight/highlight.pack.js
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/highlight/rstudio.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.788359 shiny-0.3.1/shiny/www/shared/ionrangeslider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.840359 shiny-0.3.1/shiny/www/shared/ionrangeslider/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.840359 shiny-0.3.1/shiny/www/shared/ionrangeslider/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    84956 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41602 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.840359 shiny-0.3.1/shiny/www/shared/ionrangeslider/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/ionrangeslider/scss/_base.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/ionrangeslider/scss/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/ionrangeslider/scss/shiny.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.840359 shiny-0.3.1/shiny/www/shared/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jquery/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jquery/jquery-3.6.0.min.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.844359 shiny-0.3.1/shiny/www/shared/jqueryui/
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.844359 shiny-0.3.1/shiny/www/shared/jqueryui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37452 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   529159 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32130 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.structure.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.structure.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.theme.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.844359 shiny-0.3.1/shiny/www/shared/requirejs/
+-rw-r--r--   0 runner    (1001) docker     (123)    19715 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/requirejs/require.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.792358 shiny-0.3.1/shiny/www/shared/selectize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.788359 shiny-0.3.1/shiny/www/shared/selectize/accessibility/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.844359 shiny-0.3.1/shiny/www/shared/selectize/accessibility/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.844359 shiny-0.3.1/shiny/www/shared/selectize/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/css/selectize.bootstrap3.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.844359 shiny-0.3.1/shiny/www/shared/selectize/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    45139 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/js/selectize.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.848359 shiny-0.3.1/shiny/www/shared/selectize/scss/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.848359 shiny-0.3.1/shiny/www/shared/selectize/scss/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/scss/plugins/drag_drop.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/scss/plugins/optgroup_columns.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/scss/plugins/remove_button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/scss/selectize.bootstrap5.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/scss/selectize.default.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/selectize/scss/selectize.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    23760 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny-autoreload.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125989 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny-autoreload.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny-showcase.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny-showcase.js
+-rw-r--r--   0 runner    (1001) docker     (123)   126645 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny-showcase.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny-testmode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny-testmode.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   757524 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1314664 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   306317 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1349172 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.848359 shiny-0.3.1/shiny/www/shared/shiny_scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny_scss/bootstrap.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/shiny_scss/shiny.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.848359 shiny-0.3.1/shiny/www/shared/showdown/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.848359 shiny-0.3.1/shiny/www/shared/showdown/compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/showdown/compressed/showdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/showdown/license.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.848359 shiny-0.3.1/shiny/www/shared/showdown/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    37933 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/showdown/src/showdown.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.848359 shiny-0.3.1/shiny/www/shared/strftime/
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-19 02:02:08.000000 shiny-0.3.1/shiny/www/shared/strftime/strftime-min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.796359 shiny-0.3.1/shiny.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-19 02:03:12.000000 shiny-0.3.1/shiny.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-19 02:03:12.000000 shiny-0.3.1/shiny.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:03:12.000000 shiny-0.3.1/shiny.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 02:03:12.000000 shiny-0.3.1/shiny.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:03:12.000000 shiny-0.3.1/shiny.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 02:03:12.000000 shiny-0.3.1/shiny.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 02:03:12.000000 shiny-0.3.1/shiny.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:03:12.852359 shiny-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/asyncio_prevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/mocktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_e2e_regex_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_navs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31010 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_reactives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_shinysession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-19 02:02:08.000000 shiny-0.3.1/tests/test_utils_async.py
```

### Comparing `shiny-0.3.0/LICENSE` & `shiny-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/PKG-INFO` & `shiny-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny
-Version: 0.3.0
+Version: 0.3.1
 Summary: A web development framework for Python.
 Home-page: https://github.com/rstudio/py-shiny
 Author: Winston Chang
 Author-email: winston@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shiny/issues
 Project-URL: Documentation, https://shiny.rstudio.com/py/
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 Shiny for Python
 ================
 
 See the [Shiny for Python website](https://shiny.rstudio.com/py/).
@@ -49,15 +48,15 @@
 More detailed installation instructions, including the use of `conda`, are [also available](https://shiny.rstudio.com/py/docs/install.html).
 
 ## Development
 
 If you want to do development on Shiny for Python:
 
 ```sh
-pip install -e ".[dev,docs,test]"
+pip install -e ".[dev,test]"
 ```
 
 Additionally, you can install pre-commit hooks which will automatically reformat and lint the code when you make a commit:
 
 ```sh
 pre-commit install
```

### Comparing `shiny-0.3.0/README.md` & `shiny-0.3.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 More detailed installation instructions, including the use of `conda`, are [also available](https://shiny.rstudio.com/py/docs/install.html).
 
 ## Development
 
 If you want to do development on Shiny for Python:
 
 ```sh
-pip install -e ".[dev,docs,test]"
+pip install -e ".[dev,test]"
 ```
 
 Additionally, you can install pre-commit hooks which will automatically reformat and lint the code when you make a commit:
 
 ```sh
 pre-commit install
```

### Comparing `shiny-0.3.0/setup.cfg` & `shiny-0.3.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -53,28 +53,24 @@
 
 [options.extras_require]
 test = 
 	pytest>=6.2.4
 	pytest-asyncio>=0.17.2
 	pytest-playwright>=0.3.0
 	pytest-xdist
+	pytest-timeout
 	psutil
 	astropy
 	suntime
 	timezonefinder
 	ipyleaflet
 	shinywidgets
 	seaborn
 	plotnine
 	plotly
-docs = 
-	sphinx>=4.4.0
-	sphinx-autodoc-typehints==1.15.3
-	myst-parser>=0.16.1
-	sphinx-book-theme>=0.2.0
 dev = 
 	black>=23.1.0
 	flake8==3.9.2;python_version<="3.7"
 	flake8>=6.0.0;python_version>"3.7"
 	flake8-bugbear>=23.2.13
 	isort>=5.10.1
 	pyright>=1.1.244
```

### Comparing `shiny-0.3.0/shiny/__init__.py` & `shiny-0.3.1/shiny/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A package for building reactive web applications."""
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 from ._shinyenv import is_pyodide as _is_pyodide
 
 # User-facing subpackages that should be available on `from shiny import *`
 from . import reactive
 from . import render
 from .session import (
```

### Comparing `shiny-0.3.0/shiny/_app.py` & `shiny-0.3.1/shiny/_app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_autoreload.py` & `shiny-0.3.1/shiny/_autoreload.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_connection.py` & `shiny-0.3.1/shiny/_connection.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_datastructures.py` & `shiny-0.3.1/shiny/_datastructures.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_deprecated.py` & `shiny-0.3.1/shiny/_deprecated.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_docstring.py` & `shiny-0.3.1/shiny/_docstring.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_error.py` & `shiny-0.3.1/shiny/_error.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_fileupload.py` & `shiny-0.3.1/shiny/_fileupload.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_hostenv.py` & `shiny-0.3.1/shiny/_hostenv.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_launchbrowser.py` & `shiny-0.3.1/shiny/_launchbrowser.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_main.py` & `shiny-0.3.1/shiny/_main.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_namespaces.py` & `shiny-0.3.1/shiny/_namespaces.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_static.py` & `shiny-0.3.1/shiny/_static.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_typing_extensions.py` & `shiny-0.3.1/shiny/_typing_extensions.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/_utils.py` & `shiny-0.3.1/shiny/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     # From https://github.com/rstudio/httpuv/blob/main/R/random_port.R
     unsafe_ports = [1, 7, 9, 11, 13, 15, 17, 19, 20, 21, 22, 23, 25, 37, 42, 43, 53, 77, 79, 87, 95, 101, 102, 103, 104, 109, 110, 111, 113, 115, 117, 119, 123, 135, 139, 143, 179, 389, 427, 465, 512, 513, 514, 515, 526, 530, 531, 532, 540, 548, 556, 563, 587, 601, 636, 993, 995, 2049, 3659, 4045, 6000, 6665, 6666, 6667, 6668, 6669, 6697]
     # fmt: on
     unusable = set([x for x in unsafe_ports if x >= min and x <= max])
     while n > 0:
         if (max - min + 1) <= len(unusable):
             break
-        port = round(random.random() * (max - min) + min)
+        port = random.randint(min, max)
         if port in unusable:
             continue
         try:
             # See if we can successfully bind
             with socketserver.TCPServer(
                 (host, port), socketserver.BaseRequestHandler, bind_and_activate=False
             ) as s:
```

### Comparing `shiny-0.3.0/shiny/_validation.py` & `shiny-0.3.1/shiny/_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         Any number of arguments to check.
     cancel_output
         If ``True``, throw :func:`~shiny.types.SilentCancelOutputException` instead of
         :func:`~shiny.types.SilentException`.
 
     Returns
     -------
+    :
         The first argument. If no arguments are provided, returns ``None``.
     """
     if len(args) == 0:
         return None
 
     for arg in args:
         if not arg:
```

### Comparing `shiny-0.3.0/shiny/examples/Calc/app.py` & `shiny-0.3.1/shiny/examples/Calc/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/Module/app.py` & `shiny-0.3.1/shiny/examples/Module/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/Progress/app.py` & `shiny-0.3.1/shiny/examples/Progress/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/SilentCancelOutputException/app.py` & `shiny-0.3.1/shiny/examples/SilentCancelOutputException/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/Value/app.py` & `shiny-0.3.1/shiny/examples/Value/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/close/app.py` & `shiny-0.3.1/shiny/examples/close/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/download/app.py` & `shiny-0.3.1/shiny/examples/download/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/download/mtcars.csv` & `shiny-0.3.1/shiny/examples/download/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/download_button/app.py` & `shiny-0.3.1/shiny/examples/download_button/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/download_button/mtcars.csv` & `shiny-0.3.1/shiny/examples/download_button/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/download_link/app.py` & `shiny-0.3.1/shiny/examples/download_link/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/download_link/mtcars.csv` & `shiny-0.3.1/shiny/examples/download_link/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/dynamic_route/app.py` & `shiny-0.3.1/shiny/examples/dynamic_route/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/event/app.py` & `shiny-0.3.1/shiny/examples/event/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/file_reader/mtcars.csv` & `shiny-0.3.1/shiny/examples/file_reader/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/input_action_button/app.py` & `shiny-0.3.1/shiny/examples/input_action_button/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/input_action_link/app.py` & `shiny-0.3.1/shiny/examples/input_action_link/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/input_checkbox_group/app.py` & `shiny-0.3.1/shiny/examples/input_checkbox_group/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/input_date/app.py` & `shiny-0.3.1/shiny/examples/input_date/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/input_date_range/app.py` & `shiny-0.3.1/shiny/examples/input_date_range/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/input_file/app.py` & `shiny-0.3.1/shiny/examples/input_file/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/input_select/app.py` & `shiny-0.3.1/shiny/examples/input_select/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/input_selectize/app.py` & `shiny-0.3.1/shiny/examples/input_selectize/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/input_slider/app.py` & `shiny-0.3.1/shiny/examples/input_slider/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/isolate/app.py` & `shiny-0.3.1/shiny/examples/isolate/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/layout_sidebar/app.py` & `shiny-0.3.1/shiny/examples/layout_sidebar/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/nav/app.py` & `shiny-0.3.1/shiny/examples/nav/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/navset_hidden/app.py` & `shiny-0.3.1/shiny/examples/navset_hidden/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/notification_show/app.py` & `shiny-0.3.1/shiny/examples/notification_show/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/on_flush/app.py` & `shiny-0.3.1/shiny/examples/on_flush/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/on_flushed/app.py` & `shiny-0.3.1/shiny/examples/on_flushed/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/output_image/rstudio-logo.png` & `shiny-0.3.1/shiny/examples/output_image/rstudio-logo.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/output_plot/app.py` & `shiny-0.3.1/shiny/examples/output_plot/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/output_table/app.py` & `shiny-0.3.1/shiny/examples/output_table/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/output_table/mtcars.csv` & `shiny-0.3.1/shiny/examples/output_table/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/output_text/app.py` & `shiny-0.3.1/shiny/examples/output_text/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/page_fixed/app.py` & `shiny-0.3.1/shiny/examples/page_fixed/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/page_fluid/app.py` & `shiny-0.3.1/shiny/examples/page_fluid/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/panel_conditional/app.py` & `shiny-0.3.1/shiny/examples/panel_conditional/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/poll/app.py` & `shiny-0.3.1/shiny/examples/poll/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/req/app.py` & `shiny-0.3.1/shiny/examples/req/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/row/app.py` & `shiny-0.3.1/shiny/examples/row/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/send_custom_message/app.py` & `shiny-0.3.1/shiny/examples/send_custom_message/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_action_button/app.py` & `shiny-0.3.1/shiny/examples/update_action_button/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_checkbox_group/app.py` & `shiny-0.3.1/shiny/examples/update_checkbox_group/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_date/app.py` & `shiny-0.3.1/shiny/examples/update_date/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_date_range/app.py` & `shiny-0.3.1/shiny/examples/update_date_range/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_navs/app.py` & `shiny-0.3.1/shiny/examples/update_navs/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_numeric/app.py` & `shiny-0.3.1/shiny/examples/update_numeric/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_radio_buttons/app.py` & `shiny-0.3.1/shiny/examples/update_radio_buttons/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_select/app.py` & `shiny-0.3.1/shiny/examples/update_select/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_slider/app.py` & `shiny-0.3.1/shiny/examples/update_slider/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/update_text/app.py` & `shiny-0.3.1/shiny/examples/update_text/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/examples/www_dir/app.py` & `shiny-0.3.1/shiny/examples/www_dir/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/html_dependencies.py` & `shiny-0.3.1/shiny/html_dependencies.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/http_staticfiles.py` & `shiny-0.3.1/shiny/http_staticfiles.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/input_handler.py` & `shiny-0.3.1/shiny/input_handler.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/module.py` & `shiny-0.3.1/shiny/module.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/plotutils.py` & `shiny-0.3.1/shiny/plotutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         If `False` (the default), return a data frame containing only the rows that are
         selected. If `True`, then all rows from the data frame will be returned, along
         with an additional column named `selected_`, which indicates whether or not each
         row was selected.
 
     Returns
     -------
+    :
         A pandas DataFrame containing the rows selected by the brush. If `all_rows` is
         `True`, then all rows from the original data will be returned, along with an
         additional column named `selected_`, which indicates whether or not each row was
         selected.
     """
     import pandas as pd
 
@@ -206,14 +207,15 @@
         If `False` (the default), return a data frame containing only the rows that are
         selected. If `True`, then all rows from the data frame will be returned, along
         with an additional column named `selected_`, which indicates whether or not each
         row was selected.
 
     Returns
     -------
+    :
         A pandas DataFrame containing the rows selected by the brush. If `all_rows` is
         `True`, then all rows from the original data will be returned, along with an
         additional column named `selected_`, which indicates whether or not each row was
         selected.
     """
     import numpy as np
```

### Comparing `shiny-0.3.0/shiny/reactive/__init__.py` & `shiny-0.3.1/shiny/reactive/__init__.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/reactive/_core.py` & `shiny-0.3.1/shiny/reactive/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,26 +197,27 @@
 def isolate():
     """
     Create a non-reactive scope within a reactive scope.
 
     Ordinarily, the simple act of reading a reactive value causes a relationship to be
     established between the caller and the reactive value, where a change to the
     reactive value will cause the caller to re-execute. (The same applies for the act of
-    getting a reactive expression's value.) `with isolate()` lets you read a
-    reactive value or expression without establishing this relationship.
+    getting a reactive expression's value.) `with isolate()` lets you read a reactive
+    value or expression without establishing this relationship.
 
-    ``with isolate()`` can also be useful for calling reactive expression at the console,
-    which can be useful for debugging. To do so, wrap the calls to the reactive
+    ``with isolate()`` can also be useful for calling reactive expression at the
+    console, which can be useful for debugging. To do so, wrap the calls to the reactive
     expression with ``with isolate()``.
 
     Returns
     -------
-    A context manager that executes the given expression in a scope where reactive
-    values can be read, but do not cause the reactive scope of the caller to be
-    re-evaluated when they change.
+    :
+        A context manager that executes the given expression in a scope where reactive
+        values can be read, but do not cause the reactive scope of the caller to be
+        re-evaluated when they change.
 
     See Also
     --------
     ~shiny.event
     """
     with _reactive_environment.isolate():
         yield
@@ -224,15 +225,16 @@
 
 def get_current_context() -> Context:
     """
     Get the current reactive context.
 
     Returns
     -------
-    A :class:`~Context`.
+    :
+        A :class:`~Context`.
 
     Raises
     ------
     RuntimeError
         If called outside of a reactive context.
     """
     return _reactive_environment.current_context()
@@ -261,15 +263,16 @@
     func
         The function to be called when the reactive environment is flushed
     once
         If True, the function will only be called once, and then removed from the
 
     Returns
     -------
-    A function that can be used to unregister the callback.
+    :
+        A function that can be used to unregister the callback.
 
     See Also
     --------
     flush
     """
 
     return _reactive_environment.on_flushed(func, once)
```

### Comparing `shiny-0.3.0/shiny/reactive/_poll.py` & `shiny-0.3.1/shiny/reactive/_poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
         :func:`~shiny.session.get_current_session`. If there is no current session (i.e.
         `poll` is being created outside of the server function), the lifetime of this
         reactive poll object will not be tied to any specific session.
 
     Returns
     -------
-    A decorator that should be applied to a no-argument function that (expensively)
+    :
+        A decorator that should be applied to a no-argument function that (expensively)
     reads whatever data is desired. (This function may be a regular function or a
     coroutine function.) The result of the decorator is a reactive ~shiny.reactive.Calc
     that always returns up-to-date data, and invalidates callers when changes are
     detected via polling.
 
     See Also
     --------
@@ -239,31 +240,29 @@
 
         If a function is used, make sure it is high performance (or is cached, i.e. use
         a ~shiny.reactive.Calc), as it will be called very frequently.
     interval_secs
         The number of seconds to wait after each time the file metadata is checked.
         Note: depending on what other tasks are executing, the actual wait time may far
         exceed this value.
-    equals
-        The function that will be used to compare each `poll_func` return value with its
-        immediate predecessor.
     priority
         Reactive polling is implemented using an ~shiny.reactive.Effect to call
         `poll_func` on a timer; use the `priority` argument to control the order of this
         Effect's execution versus other Effects in your app. See ~shiny.reactive.Effect
         for more details.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
         :func:`~shiny.session.get_current_session`. If there is no current session (i.e.
         `poll` is being created outside of the server function), the lifetime of this
         reactive poll object will not be tied to any specific session.
 
     Returns
     -------
-    A decorator that should be applied to a no-argument function that (expensively)
+    :
+        A decorator that should be applied to a no-argument function that (expensively)
     reads whatever data is desired. (This function may be a regular function or a
     coroutine function.) The result of the decorator is a reactive ~shiny.reactive.Calc
     that always returns up-to-date data, and invalidates callers when changes are
     detected via polling.
 
     See Also
     --------
```

### Comparing `shiny-0.3.0/shiny/reactive/_reactives.py` & `shiny-0.3.1/shiny/reactive/_reactives.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,44 +34,54 @@
 
 # ==============================================================================
 # Value
 # ==============================================================================
 @add_example()
 class Value(Generic[T]):
     """
-    Create a reactive value
+    Create a reactive value.
+
+    Reactive values are the source of reactivity in Shiny. Changes to reactive values
+    invalidate downstream reactive functions (:func:`~shiny.reactive.Calc`,
+    :func:`~shiny.reactive.Effect`, and `render` functions decorated with `@output`).
+    When these functions are invalidated, they get scheduled to re-execute.
+
+    Shiny input values are read-only reactive values. For example, `input.x` is a
+    reactive value object, and to get the current value, you can call `input.x()` or
+    `input.x.get()`. When you do that inside of a reactive function, the function takes
+    a dependency on the reactive value.
 
     Parameters
     ----------
     value
         An optional initial value.
     read_only
         If ``True``, then the reactive value cannot be `set()`.
 
     Returns
     -------
-    An instance of a reactive value.
+    :
+        An instance of a reactive value.
 
     Raises
     ------
     ~shiny.types.SilentException
         If :func:`~Value.get` is called before a value is provided/set.
 
     Note
     ----
     A reactive value may only be read from within a reactive function (e.g.,
-    :func:`Calc`, :func:`Effect`, :func:`shiny.render.text`, etc.) and, when doing so,
-    the function takes a reactive dependency on the value (i.e., when the value changes,
-    the calling reactive function will re-execute).
+    :func:`~shiny.reactive.Calc`, :func:`~shiny.reactive.Effect`,
+    :func:`shiny.render.text`, etc.) and, when doing so, the function takes a reactive
+    dependency on the value (i.e., when the value changes, the calling reactive function
+    will re-execute).
 
     See Also
     --------
-    ~shiny.Inputs
-    Calc
-    Effect
+    ~shiny.Inputs ~shiny.reactive.Calc ~shiny.reactive.Effect
     """
 
     # These overloads are necessary so that the following hold:
     # - Value() is marked by the type checker as an error, because the type T is
     #   unknown. (It is not a run-time error.)
     # - Value[int]() works.
     # - Value[int](1) works.
@@ -101,15 +111,16 @@
 
     def get(self) -> T:
         """
         Read the reactive value.
 
         Returns
         -------
-        The reactive value.
+        :
+            A value.
 
         Raises
         ------
         ~shiny.types.SilentException
             If the value is not set.
         RuntimeError
             If called from outside a reactive function.
@@ -129,15 +140,16 @@
         Parameters
         ----------
         value
             A value.
 
         Returns
         -------
-        ``True`` if the value was set to a different value and ``False`` otherwise.
+        :
+            ``True`` if the value was set to a different value and ``False`` otherwise.
 
         Raises
         ------
         RuntimeError
             If called on a read-only reactive value.
         """
         if self._read_only:
@@ -161,25 +173,27 @@
 
     def unset(self) -> None:
         """
         Unset the reactive value.
 
         Returns
         -------
-        ``True`` if the value was set prior to this unsetting.
+        :
+            ``True`` if the value was set prior to this unsetting.
         """
         self.set(MISSING)  # type: ignore
 
     def is_set(self) -> bool:
         """
         Check if the reactive value is set.
 
         Returns
         -------
-        ``True`` if the value is set, ``False`` otherwise.
+        :
+            ``True`` if the value is set, ``False`` otherwise.
         """
 
         self._is_set_dependents.register()
         return not isinstance(self._value, MISSING_TYPE)
 
     def freeze(self) -> None:
         """
@@ -202,15 +216,15 @@
 class Calc_(Generic[T]):
     """
     Mark a function as a reactive calculation.
 
     Warning
     -------
     Most users shouldn't use this class directly to initialize a reactive calculation
-    (instead, use the :func:`Calc` decorator).
+    (instead, use the :func:`~shiny.reactive.Calc` decorator).
     """
 
     def __init__(
         self,
         fn: CalcFunction[T],
         *,
         session: "MISSING_TYPE | Session | None" = MISSING,
@@ -307,15 +321,15 @@
 class CalcAsync_(Calc_[T]):
     """
     Mark an async function as a reactive calculation.
 
     Warning
     -------
     Most users shouldn't use this class directly to initialize a reactive calculation
-    (instead, use the :func:`Calc` decorator).
+    (instead, use the :func:`~shiny.reactive.Calc` decorator).
     """
 
     def __init__(
         self,
         fn: CalcFunctionAsync[T],
         *,
         session: "MISSING_TYPE | Session | None" = MISSING,
@@ -383,19 +397,20 @@
     calculations that recently called it are also marked as invalidated. In this way,
     invalidations ripple through reactive calculations that depend on each other.
 
     Parameters
     ----------
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Returns
     -------
-    A decorator that marks a function as a reactive calculation.
+    :
+        A decorator that marks a function as a reactive calculation.
 
     Tip
     ---
     Reactive calculations should not produce any side effects; to reactively produce
     side effects, use :func:`~shiny.reactive.Effect` instead.
 
     See Also
@@ -637,19 +652,20 @@
     suspended: bool = False,
     priority: int = 0,
     session: "MISSING_TYPE | Session | None" = MISSING,
 ) -> Effect_ | Callable[[EffectFunction | EffectFunctionAsync], Effect_]:
     """
     Mark a function as a reactive side effect.
 
-    A reactive effect is like a reactive calculation (:func:`Calc`) in that it can read
-    reactive values and call reactive calculations, and will automatically re-execute
-    when those dependencies change. But unlike reactive calculations, it doesn't return
-    a result and can't be used as an input to other reactive expressions. Thus,
-    observers are only useful for their side effects (for example, performing I/O).
+    A reactive effect is like a reactive calculation (:func:`~shiny.reactive.Calc`) in
+    that it can read reactive values and call reactive calculations, and will
+    automatically re-execute when those dependencies change. But unlike reactive
+    calculations, it doesn't return a result and can't be used as an input to other
+    reactive expressions. Thus, observers are only useful for their side effects (for
+    example, performing I/O).
 
     Another contrast between reactive calculations and effects is their execution
     strategy. Reactive calculations use lazy evaluation; that is, when their
     dependencies change, they don't re-execute right away but rather wait until they are
     called by someone else. Indeed, if they are not called then they will never
     re-execute. In contrast, effects use eager evaluation; as soon as their dependencies
     change, they schedule themselves to re-execute.
@@ -661,19 +677,20 @@
         until resumed and invalidated).
     priority
         The new priority. A higher value means higher priority: an effect with a higher
         priority value will execute before all effects with lower priority values.
         Positive, negative, and zero values are allowed.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Returns
     -------
-    A decorator that marks a function as a reactive effect (:class:`Effect_`).
+    :
+        A decorator that marks a function as a reactive effect (:class:`Effect_`).
 
     See Also
     --------
     ~shiny.Inputs
     ~shiny.reactive.Value
     ~shiny.reactive.Effect
     ~shiny.reactive.invalidate_later
@@ -726,15 +743,16 @@
     ignore_none
         Whether to ignore the event if the value is ``None`` or ``0``.
     ignore_init
         If ``False``, the event trigger on the first run.
 
     Returns
     -------
-    A decorator that marks a function as an event handler.
+    :
+        A decorator that marks a function as an event handler.
 
     Tip
     ----
     This decorator must be applied before the relevant reactivity decorator (i.e.,
     ``@reactive.event`` must be applied before ``@reactive.Effect``, ``@reactive.Calc``,
     ``@render.ui``, etc).
     """
```

### Comparing `shiny-0.3.0/shiny/render/__init__.py` & `shiny-0.3.1/shiny/render/__init__.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/render/_coordmap.py` & `shiny-0.3.1/shiny/render/_coordmap.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/render/_render.py` & `shiny-0.3.1/shiny/render/_render.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,16 @@
     fn: Optional[RenderTextFunc | RenderTextFuncAsync] = None,
 ) -> RenderText | Callable[[RenderTextFunc | RenderTextFuncAsync], RenderText]:
     """
     Reactively render text.
 
     Returns
     -------
-    A decorator for a function that returns a string.
+    :
+        A decorator for a function that returns a string.
 
     Tip
     ----
     This decorator should be applied **before** the ``@output`` decorator. Also, the
     name of the decorated function (or ``@output(id=...)``) should match the ``id`` of
     a :func:`~shiny.ui.output_text` container (see :func:`~shiny.ui.output_text` for
     example usage).
@@ -325,15 +326,16 @@
     **kwargs
         Additional keyword arguments passed to the relevant method for saving the image
         (e.g., for matplotlib, arguments to ``savefig()``; for PIL and plotnine,
         arguments to ``save()``).
 
     Returns
     -------
-    A decorator for a function that returns any of the following:
+    :
+        A decorator for a function that returns any of the following:
 
         1. A :class:`matplotlib.figure.Figure` instance.
         2. An :class:`matplotlib.artist.Artist` instance.
         3. A list/tuple of Figure/Artist instances.
         4. An object with a 'figure' attribute pointing to a
            :class:`matplotlib.figure.Figure` instance.
         5. A :class:`PIL.Image.Image` instance.
@@ -449,15 +451,16 @@
     Parameters
     ----------
     delete_file
         If ``True``, the image file will be deleted after rendering.
 
     Returns
     -------
-    A decorator for a function that returns an `~shiny.types.ImgData` object.
+    :
+        A decorator for a function that returns an `~shiny.types.ImgData` object.
 
     Tip
     ----
     This decorator should be applied **before** the ``@output`` decorator. Also, the
     name of the decorated function (or ``@output(id=...)``) should match the ``id`` of
     a :func:`~shiny.ui.output_image` container (see :func:`~shiny.ui.output_image` for
     example usage).
@@ -624,15 +627,16 @@
         from user code instead.)
     **kwargs
         Additional keyword arguments passed to ``pandas.DataFrame.to_html()`` or
         ``pandas.io.formats.style.Styler.to_html()``.
 
     Returns
     -------
-    A decorator for a function that returns any of the following:
+    :
+        A decorator for a function that returns any of the following:
 
         1. A pandas :class:`DataFrame` object.
         2. A pandas :class:`Styler` object.
         3. Any object that has a `.to_pandas()` method (e.g., a Polars data frame or
            Arrow table).
 
     Tip
@@ -715,15 +719,16 @@
     fn: Optional[RenderUIFunc | RenderUIFuncAsync] = None,
 ) -> RenderUI | Callable[[RenderUIFunc | RenderUIFuncAsync], RenderUI]:
     """
     Reactively render HTML content.
 
     Returns
     -------
-    A decorator for a function that returns an object of type `~shiny.ui.TagChild`.
+    :
+        A decorator for a function that returns an object of type `~shiny.ui.TagChild`.
 
     Tip
     ----
     This decorator should be applied **before** the ``@output`` decorator. Also, the
     name of the decorated function (or ``@output(id=...)``) should match the ``id`` of
     a :func:`~shiny.ui.output_ui` container (see :func:`~shiny.ui.output_ui` for example
     usage).
```

### Comparing `shiny-0.3.0/shiny/render/_try_render_plot.py` & `shiny-0.3.1/shiny/render/_try_render_plot.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/session/_session.py` & `shiny-0.3.1/shiny/session/_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,14 +512,20 @@
                                             if isinstance(chunk, str):
                                                 yield chunk.encode(download.encoding)
                                             else:
                                                 yield chunk
 
                             wrapped_contents = wrap_content_sync()
 
+                        # In streaming downloads, we send a 200 response, but if an
+                        # error occurs in the middle of it, the client needs to know.
+                        # With chunked encoding, the client will know if an error occurs
+                        # if it does not receive a terminating (empty) chunk.
+                        headers["Transfer-Encoding"] = "chunked"
+
                         return StreamingResponse(
                             wrapped_contents,
                             200,
                             headers=headers,
                             media_type=content_type,  # type: ignore
                         )
 
@@ -636,15 +642,16 @@
         fn
             The function to call.
         once
             Whether to call the function only once or on every flush.
 
         Returns
         -------
-        A function that can be used to cancel the registration.
+        :
+            A function that can be used to cancel the registration.
         """
         return self._flush_callbacks.register(fn, once)
 
     @add_example()
     def on_flushed(
         self, fn: Callable[[], None], once: bool = True
     ) -> Callable[[], None]:
@@ -656,15 +663,16 @@
         fn
             The function to call.
         once
             Whether to call the function only once or on every flush.
 
         Returns
         -------
-        A function that can be used to cancel the registration.
+        :
+            A function that can be used to cancel the registration.
         """
         return self._flushed_callbacks.register(fn, once)
 
     def _request_flush(self) -> None:
         self.app._request_flush(self)
 
     async def _flush(self) -> None:
@@ -707,15 +715,16 @@
         Parameters
         ----------
         fn
             The function to call.
 
         Returns
         -------
-        A function that can be used to cancel the registration.
+        :
+            A function that can be used to cancel the registration.
         """
         return self._on_ended_callbacks.register(fn)
 
     # ==========================================================================
     # Misc
     # ==========================================================================
     async def _unhandled_error(self, e: Exception) -> None:
@@ -742,15 +751,16 @@
         media_type
             The media type of the download.
         encoding
             The encoding of the download.
 
         Returns
         -------
-        The decorated function.
+        :
+            The decorated function.
         """
 
         def wrapper(fn: DownloadHandler):
             effective_name = id or fn.__name__
 
             self._downloads[effective_name] = DownloadInfo(
                 filename=filename,
@@ -785,14 +795,15 @@
             The function to call when a request is made to the route. This function
             should take a single argument (a :class:`starlette.requests.Request` object)
             and return a :class:`starlette.types.ASGIApp` object.
 
 
         Returns
         -------
+        :
             The URL path for the route.
         """
 
         self._dynamic_routes.update({name: handler})
         nonce = _utils.rand_hex(8)
         return f"session/{urllib.parse.quote(self.id)}/dynamic_route/{urllib.parse.quote(name)}?nonce={urllib.parse.quote(nonce)}"
```

### Comparing `shiny-0.3.0/shiny/session/_utils.py` & `shiny-0.3.1/shiny/session/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 def get_current_session() -> Optional[Session]:
     """
     Get the current user session.
 
     Returns
     -------
-    The current session if one is active, otherwise ``None``.
+    :
+        The current session if one is active, otherwise ``None``.
 
     Note
     ----
     Shiny apps should not need to call this function directly. Instead, it's intended to
     be used by Shiny developing who wish to create new functions that should only be
     called from within an active Shiny session.
 
@@ -76,15 +77,16 @@
     ----------
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
         :func:`~shiny.session.get_current_session`.
 
     Returns
     -------
-    The session.
+    :
+        The session.
 
     Note
     ----
     Shiny apps should not need to call this function directly. Instead, it's intended to
     be used by Shiny developing who wish to create new functions that should only be
     called from within an active Shiny session.
```

### Comparing `shiny-0.3.0/shiny/types.py` & `shiny-0.3.1/shiny/types.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/ui/__init__.py` & `shiny-0.3.1/shiny/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/ui/_bootstrap.py` & `shiny-0.3.1/shiny/ui/_bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,28 +42,29 @@
 def row(*args: TagChild | TagAttrs, **kwargs: TagAttrValue) -> Tag:
     """
     Responsive row-column based layout
 
     Layout UI components using Bootstrap's grid layout system. Use ``row()`` to group
     elements that should appear on the same line (if the browser has adequate width) and
     :func:`~shiny.ui.column` to define how much horizontal space within a 12-unit wide
-    grid each on of these elements should occupy. See the `layout guide
-    <https://shiny.rstudio.com/articles/layout-guide.html>`_ for more context and
+    grid each on of these elements should occupy. See the [layout
+    guide](https://shiny.rstudio.com/articles/layout-guide.html>) for more context and
     examples.
 
     Parameters
     ----------
     args
         Any number of child elements.
     kwargs
         Attributes to place on the row tag.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.column`
     """
     return div({"class": "row"}, *args, **kwargs)
 
@@ -85,15 +86,16 @@
     offset
         The number of columns to offset this column from the end of the previous column.
     kwargs
         Attributes to place on the column tag.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.row`
     """
 
     if width < 1 or width > 12:
@@ -132,15 +134,16 @@
         A UI element to place in the main area (typically a
         :func:`~shiny.ui.panel_main`)
     position
         The position of the sidebar (left or right)
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     See Also
     -------
     :func:`~shiny.ui.panel_sidebar`
     :func:`~shiny.ui.panel_main`
     """
     return row(sidebar, main) if position == "left" else row(main, sidebar)
@@ -158,15 +161,16 @@
     args
         UI elements to include inside the panel.
     kwargs
         Attributes to place on the panel tag.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.panel_sidebar`
     :func:`~shiny.ui.panel_main`
     """
     return div({"class": "well"}, *args, **kwargs)
@@ -188,15 +192,16 @@
     width
         The width of the sidebar (an integer between 1 and 12)
     kwargs
         Attributes to place on the sidebar tag.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.panel_sidebar`
     :func:`~shiny.ui.panel_main`
     """
     return div(
@@ -221,15 +226,16 @@
     width
         The width of the main area (an integer between 1 and 12).
     kwargs
         Attributes to place on the main area tag.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.panel_sidebar`
     :func:`~shiny.ui.layout_sidebar`
     """
     return div(
@@ -265,15 +271,16 @@
     args
         UI elements to include inside the panel.
     kwargs
         Attributes to place on the panel tag.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Note
     ----
     In the JS expression, you can refer to input and output JavaScript objects that
     contain the current values of input and output. For example, if you have an input
     with an id of foo, then you can use input.foo to read its value. (Be sure not to
     modify the input/output objects, as this may cause unpredictable behavior.)
@@ -314,15 +321,16 @@
     title
         A title to display in the app's UI.
     window_title
         A title to display on the browser tab.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Note
     ----
     This result of this function causes a side effect of adding a title tag to the head
     of the document (this is necessary for the browser to display the title in the
     browser window). You can also specify a page title explicitly using the title
     parameter of the top-level page function (e.g., :func:`~shiny.ui.page_fluid`).
@@ -347,15 +355,16 @@
     args
         UI elements to include inside the panel.
     kwargs
         Arguments passed along to :func:`~shiny.ui.panel_absolute`.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.panel_absolute`
     """
     return panel_absolute(*args, fixed=True, **kwargs)
 
@@ -416,15 +425,16 @@
         I-beam when the cursor is over text). The default is ``"auto"``, which is
         equivalent to ``"move" if draggable else "inherit"``.
     kwargs
         Attributes added to the content's container tag.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     Tip
     ----
     The position (``top``, ``left``, ``right``, ``bottom``) and size (``width``,
     ``height``) parameters are all optional, but you should specify exactly two of top,
     bottom, and height and exactly two of left, right, and width for predictable
     results.
@@ -466,11 +476,12 @@
     args
         UI elements to include inside the help text.
     kwargs
         Attributes to add to the text container.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
     """
 
     return span({"class": "help-block"}, *args, **kwargs)
```

### Comparing `shiny-0.3.0/shiny/ui/_download_button.py` & `shiny-0.3.1/shiny/ui/_download_button.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     width
         The width of the button.
     kwargs
         Additional attributes for the button.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     See Also
     --------
     ~shiny.Session.download
     ~shiny.ui.download_link
     """
 
@@ -86,15 +87,16 @@
     width
         The width of the button.
     kwargs
         Additional attributes for the button.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     See Also
     --------
     ~shiny.Session.download
     ~shiny.ui.download_link
     """
```

### Comparing `shiny-0.3.0/shiny/ui/_html_dependencies.py` & `shiny-0.3.1/shiny/ui/_html_dependencies.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/ui/_input_action_button.py` & `shiny-0.3.1/shiny/ui/_input_action_button.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     width
         The CSS width, e.g. '400px', or '100%'
     kwargs
         Attributes to be applied to the button.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     Notes
     ------
     .. admonition:: Server value
 
         An integer representing the number of clicks.
 
@@ -82,15 +83,16 @@
     icon
         An icon to appear inline with the button/link.
     kwargs
         Attributes to be applied to the link.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     Notes
     ------
     .. admonition:: Server value
 
         An integer representing the number of clicks.
```

### Comparing `shiny-0.3.0/shiny/ui/_input_check_radio.py` & `shiny-0.3.1/shiny/ui/_input_check_radio.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     value
         Initial value.
     width
         The CSS width, e.g. '400px', or '100%'
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Notes
     ------
     .. admonition:: Server value
 
         ``True`` if checked, ``False`` otherwise.
 
@@ -100,15 +101,16 @@
     value
         Initial value.
     width
         The CSS width, e.g. '400px', or '100%'
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Notes
     ------
     .. admonition:: Server value
 
         ``True`` if checked, ``False`` otherwise.
 
@@ -177,15 +179,16 @@
     inline
         If `True`, the result is displayed inline
     width
         The CSS width, e.g. '400px', or '100%'
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Notes
     ------
     .. admonition:: Server value
 
         A tuple of string(s) with the selected value(s) (if any).
 
@@ -242,17 +245,19 @@
         that the dictionary values can hold HTML labels.
     selected
         The values that should be initially selected, if any.
     inline
         If ``True``, the result is displayed inline
     width
         The CSS width, e.g. '400px', or '100%'
+
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     Notes
     ------
     .. admonition:: Server value
 
         A string with the selected value.
```

### Comparing `shiny-0.3.0/shiny/ui/_input_date.py` & `shiny-0.3.1/shiny/ui/_input_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,22 +38,22 @@
     Parameters
     ----------
     id
         An input id.
     label
         An input label.
     value
-        The starting date. Either a :func:`~datetime.date` object, or a string in
+        The starting date. Either a :class:`~datetime.date` object, or a string in
         `yyyy-mm-dd` format. If None (the default), will use the current date in the
         client's time zone.
     min
-        The minimum allowed date. Either a :func:`~datetime.date` object, or a string in
+        The minimum allowed date. Either a :class:`~datetime.date` object, or a string in
         yyyy-mm-dd format.
     max
-        The maximum allowed date. Either a :func:`~datetime.date` object, or a string in
+        The maximum allowed date. Either a :class:`~datetime.date` object, or a string in
         yyyy-mm-dd format.
     format
         The format of the date to display in the browser. Defaults to `"yyyy-mm-dd"`.
     startview
         The date range shown when the input object is first clicked. Can be "month" (the
         default), "year", or "decade".
     weekstart
@@ -75,15 +75,16 @@
         Which dates should be disabled (in `yyyy-mm-dd` format).
     daysofweekdisabled
         Days of the week that should be disabled. Should be a integer vector with values
         from 0 (Sunday) to 6 (Saturday).
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Note
     ----
     The date ``format`` string specifies how the date will be displayed in the browser.
     It allows the following values:
 
     - ``yy``: Year without century (12)
@@ -97,15 +98,15 @@
     - ``D``: Abbreviated weekday name
     - ``DD``: Full weekday name
 
     Notes
     ------
     .. admonition:: Server value
 
-        A :func:`~datetime.date` object.
+        A :class:`~datetime.date` object.
 
     See Also
     -------
     ~shiny.ui.update_date
     ~shiny.ui.input_date_range
     """
 
@@ -154,26 +155,26 @@
     Parameters
     ----------
     id
         An input id.
     label
         An input label.
     start
-        The initial start date. Either a :func:`~datetime.date` object, or a string in
+        The initial start date. Either a :class:`~datetime.date` object, or a string in
         yyyy-mm-dd format. If ``None`` (the default), will use the current date in the
         client's time zone.
     end
-        The initial end date. Either a :func:`~datetime.date` object, or a string in
+        The initial end date. Either a :class:`~datetime.date` object, or a string in
         yyyy-mm-dd format. If ``None`` (the default), will use the current date in the
         client's time zone.
     min
-        The minimum allowed date. Either a :func:`~datetime.date` object, or a string in
+        The minimum allowed date. Either a :class:`~datetime.date` object, or a string in
         yyyy-mm-dd format.
     max
-        The maximum allowed date. Either a :func:`~datetime.date` object, or a string in
+        The maximum allowed date. Either a :class:`~datetime.date` object, or a string in
         yyyy-mm-dd format.
     format
         The format of the date to display in the browser.
     startview
         The date range shown when the input object is first clicked. Can be "month" (the
         default), "year", or "decade".
     weekstart
@@ -192,15 +193,16 @@
     width
         The CSS width, e.g. '400px', or '100%'
     autoclose
         Whether or not to close the datepicker immediately when a date is selected.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Note
     ----
     The date ``format`` string specifies how the date will be displayed in the browser.
     It allows the following values:
 
     - ``yy``: Year without century (12)
@@ -214,15 +216,15 @@
     - ``D``: Abbreviated weekday name
     - ``DD``: Full weekday name
 
     Notes
     ------
     .. admonition:: Server value
 
-        A tuple of :func:`~datetime.date` objects.
+        A tuple of :class:`~datetime.date` objects.
 
     See Also
     -------
     ~shiny.ui.update_date_range
     ~shiny.ui.input_date
     """
```

### Comparing `shiny-0.3.0/shiny/ui/_input_file.py` & `shiny-0.3.1/shiny/ui/_input_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,16 @@
         "environment", it will open the rear-facing camera. If "user", it will open the
         front-facing camera. By default, it will accept either still photos or video. To
         accept only still photos, use ``accept="image/*"``; to accept only video, use
         ``accept="video/*"``.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Notes
     -----
 
     .. admonition:: Server value
 
         A list of dictionaries (one for each file upload) with the following keys:
```

### Comparing `shiny-0.3.0/shiny/ui/_input_numeric.py` & `shiny-0.3.1/shiny/ui/_input_numeric.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     step
         Interval to use when stepping between min and max.
     width
         The CSS width, e.g. '400px', or '100%'
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Notes
     ------
     .. admonition:: Server value
 
         A numeric value.
```

### Comparing `shiny-0.3.0/shiny/ui/_input_password.py` & `shiny-0.3.1/shiny/ui/_input_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     width
         The CSS width, e.g. '400px', or '100%'
     placeholder
         The placeholder of the input.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Notes
     ------
     .. admonition:: Server value
 
         A string of the password input. The default value is unless value is provided.
```

### Comparing `shiny-0.3.0/shiny/ui/_input_select.py` & `shiny-0.3.1/shiny/ui/_input_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,16 @@
     multiple
         Is selection of multiple items allowed?
     width
         The CSS width, e.g. '400px', or '100%'
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Notes
     ------
     .. admonition:: Server value
 
         A list of strings, usually of length 1, with the value of the selected items. When
         ``multiple=True`` and nothing is selected, this value will be ``None``.
@@ -142,15 +143,16 @@
     size
         Number of items to show in the selection box; a larger number will result in a
         taller box. Normally, when ``multiple=False``, a select input will be a
         drop-down list, but when size is set, it will be a box instead.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     Notes
     ------
     .. admonition:: Server value
 
         A list of strings, usually of length 1, with the value of the selected items. When
         ``multiple=True`` and nothing is selected, this value will be ``None``.
```

### Comparing `shiny-0.3.0/shiny/ui/_input_slider.py` & `shiny-0.3.1/shiny/ui/_input_slider.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     play_button
         Play button text or HTML.
     pause_button
         Pause button text or HTML.
 
     Returns
     -------
-    A TypedDict.
+    :
+        A TypedDict.
 
     See Also
     --------
     ~shiny.ui.input_slider
     """
 
     interval: NotRequired[int]
@@ -103,32 +104,33 @@
     sep
         Separator between thousands places in numbers.
     pre
         A prefix string to put in front of the value.
     post
         A suffix string to put after the value.
     time_format
-        Only used if the slider values are :func:`~datetime.date` or
-        :func:`~datetime.datetime` objects. A time format string, to be passed to the
+        Only used if the slider values are :class:`~datetime.date` or
+        :class:`~datetime.datetime` objects. A time format string, to be passed to the
         Javascript strftime library. See https://github.com/samsonjs/strftime for more
         details. For Dates, the default is "%F" (like "2015-07-01"), and for Datetimes,
         the default is "%F %T" (like "2015-07-01 15:32:10").
     timezone
-        Only used if the values are :func:`~datetime.datetime` objects. A string
+        Only used if the values are :class:`~datetime.datetime` objects. A string
         specifying the time zone offset for the displayed times, in the format "+HHMM"
         or "-HHMM". If ``None`` (the default), times will be displayed in the browser's
         time zone. The value "+0000" will result in UTC time.
     drag_range
         This option is used only if it is a range slider (with two values). If ``True``
         (the default), the range can be dragged. In other words, the min and max can be
         dragged together. If ``False``, the range cannot be dragged.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     Notes
     ------
     .. admonition:: Server value
 
        A number, date, or date-time (depending on the class of value), or in the case of
        slider range, a list of two numbers/dates/date-times.
```

### Comparing `shiny-0.3.0/shiny/ui/_input_text.py` & `shiny-0.3.1/shiny/ui/_input_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         more.
     spellcheck
         Whether to enable browser spell checking of the text input (default is None). If
         None, then it will use the browser's default behavior.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     Notes
     ------
     .. admonition:: Server value
 
         A string containing the current text input. The default value is ``""`` unless
         ``value`` is provided.
@@ -130,15 +131,16 @@
         more.
     spellcheck
         Whether to enable browser spell checking of the text input (default is None). If
         None, then it will use the browser's default behavior.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     Notes
     ------
     .. admonition:: Server value
 
         A string containing the current text input. The default value is ``""`` unless
         ``value`` is provided.
```

### Comparing `shiny-0.3.0/shiny/ui/_input_update.py` & `shiny-0.3.1/shiny/ui/_input_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         An input id.
     label
         An input label.
     value
         A new value.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -161,15 +161,15 @@
         An input id.
     label
         An input label.
     value
         A new value.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -207,15 +207,15 @@
         that the dictionary values can hold HTML labels.
     selected
         The values that should be initially selected, if any.
     inline
         If ``True``, the result is displayed inline
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -259,15 +259,15 @@
         that the dictionary values can hold HTML labels.
     selected
         The values that should be initially selected, if any.
     inline
         If ``True```, the result is displayed inline
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -338,15 +338,15 @@
         If ``None`` (the default), will use the current date in the client's time zone.
     min
         The minimum allowed value.
     max
         The maximum allowed value.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -381,28 +381,28 @@
     Parameters
     ----------
     id
         An input id.
     label
         An input label.
     start
-        The initial start date. Either a :func:`~datetime.date` object, or a string in
+        The initial start date. Either a :class:`~datetime.date` object, or a string in
         yyyy-mm-dd format. If ``None`` (the default), will use the current date in the
         client's time zone.
     end
-        The initial end date. Either a :func:`~datetime.date` object, or a string in
+        The initial end date. Either a :class:`~datetime.date` object, or a string in
         yyyy-mm-dd format. If ``None`` (the default), will use the current date in the
         client's time zone.
     min
         The minimum allowed value.
     max
         The maximum allowed value.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -503,15 +503,15 @@
         that the dictionary values can hold HTML labels. A dictionary of dictionaries is
         also supported, and in that case, the top-level keys are treated as
         ``<optgroup>`` labels.
     selected
         The values that should be initially selected, if any.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -579,15 +579,15 @@
         The values that should be initially selected, if any.
     server
         Whether to store choices on the server side, and load the select options
         dynamically on searching, instead of writing all choices into the page at once
         (i.e., only use the client-side version of selectize.js)
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -745,27 +745,27 @@
         The maximum allowed value.
     step
         Specifies the interval between each selectable value on the slider. Either
         ``None`` (the default), which uses a heuristic to determine the step size or a
         single number. If the values are dates, step is in days; if the values are
         date-times, step is in seconds.
     time_format
-        Only used if the slider values are :func:`~datetime.date` or
-        :func:`~datetime.datetime` objects. A time format string, to be passed to the
+        Only used if the slider values are :class:`~datetime.date` or
+        :class:`~datetime.datetime` objects. A time format string, to be passed to the
         Javascript strftime library. See https://github.com/samsonjs/strftime for more
         details. For Dates, the default is "%F" (like "2015-07-01"), and for Datetimes,
         the default is "%F %T" (like "2015-07-01 15:32:10").
     timezone
-        Only used if the values are :func:`~datetime.datetime` objects. A string
+        Only used if the values are :class:`~datetime.datetime` objects. A string
         specifying the time zone offset for the displayed times, in the format "+HHMM"
         or "-HHMM". If ``None`` (the default), times will be displayed in the browser's
         time zone. The value "+0000" will result in UTC time.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -823,15 +823,15 @@
         An input label.
     value
         A new value.
     placeholder
         A hint as to what can be entered into the control.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
@@ -865,15 +865,15 @@
     ----------
     id
         An input id.
     selected
         The values that should be initially selected, if any.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     {note}
 
     See Also
     -------
```

### Comparing `shiny-0.3.0/shiny/ui/_insert.py` & `shiny-0.3.1/shiny/ui/_insert.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         relative to the first matched element (default).
     immediate
         Whether the UI object should be immediately inserted or removed, or whether
         Shiny should wait until all outputs have been updated and all effects have been
         run (default).
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Note
     ----
     This function allows you to dynamically add arbitrary UI into your app, whenever you
     want, as many times as you want. Unlike :func:`~shiny.render.ui`, the UI generated
     with `insert_ui` is persistent: once it's created, it stays there until removed by
     :func:`remove_ui`. Each new call to `insert_ui` creates more UI objects, in addition
@@ -113,15 +113,15 @@
         relative to the first matched element (default).
     immediate
         Whether the UI object should be immediately inserted or removed, or whether
         Shiny should wait until all outputs have been updated and all effects have been
         run (default).
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     See Also
     -------
     ~shiny.ui.insert_ui
     ~shiny.render.ui
     """
```

### Comparing `shiny-0.3.0/shiny/ui/_markdown.py` & `shiny-0.3.1/shiny/ui/_markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         :class:`MarkdownIt` class (which supports Github-flavored markdown) from the
         ``markdown-it`` package is used.
     **kwargs
         Additional keyword arguments passed to the ``render_func``.
 
     Returns
     -------
+    :
         An :func:`ui.HTML` string of the rendered markdown.
 
     Note
     ----
     Use :func:`ui.include_markdown` instead if you want to include local images (or
     other files) in the markdown.
```

### Comparing `shiny-0.3.0/shiny/ui/_modal.py` & `shiny-0.3.1/shiny/ui/_modal.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     icon
         An icon to appear inline with the button/link.
     kwargs
         Attributes to be applied to the button.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     See Also
     -------
     ~shiny.ui.modal
     ~shiny.ui.modal_show
     ~shiny.ui.modal_remove
 
@@ -90,15 +91,16 @@
         If ``False``, the modal dialog will have no fade-in animation (it will simply
         appear rather than fade in to view).
     kwargs
         Attributes to be applied to the modal's body tag.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     See Also
     -------
     ~shiny.ui.modal_show
     ~shiny.ui.modal_remove
     ~shiny.ui.modal_button
     """
@@ -157,15 +159,15 @@
 
     Parameters
     ----------
     modal
         Typically a :func:`modal` instance.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     See Also
     -------
     ~shiny.ui.modal_remove
     ~shiny.ui.modal
 
     Example
@@ -181,15 +183,15 @@
     """
     Remove a modal dialog.
 
     Parameters
     ----------
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     See Also
     -------
     ~shiny.ui.modal_show
     ~shiny.ui.modal
 
     Example
```

### Comparing `shiny-0.3.0/shiny/ui/_navs.py` & `shiny-0.3.1/shiny/ui/_navs.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     "navset_pill_list",
     "navset_hidden",
     "navset_bar",
 )
 
 import copy
 import re
-from typing import Any, Optional, cast
+from typing import Any, Optional, Sequence, cast
 
-from htmltools import Tag, TagChild, TagList, div, tags
+from htmltools import MetadataNode, Tag, TagChild, TagList, div, tags
 
 from .._docstring import add_example
 from .._namespaces import resolve_id
 from .._typing_extensions import Literal
 from .._utils import private_random_int
 from ..types import NavSetArg
 from ._bootstrap import column, row
@@ -301,15 +301,16 @@
     icon
         An icon to appear inline with the button/link.
     align
         Horizontal alignment of the dropdown menu relative to dropdown toggle.
 
     Returns
     -------
-    A UI element representing both the navigation menu.
+    :
+        A UI element representing both the navigation menu.
 
     See Also
     -------
     ~shiny.ui.nav
     ~shiny.ui.nav_control
     ~shiny.ui.nav_spacer
     ~shiny.ui.navset_bar
@@ -330,24 +331,24 @@
         title=TagList(icon, title),
         value=value,
         align=align,
     )
 
 
 class NavSet:
-    args: tuple[NavSetArg]
+    args: tuple[NavSetArg | MetadataNode]
     ul_class: str
     id: Optional[str]
     selected: Optional[str]
     header: TagChild
     footer: TagChild
 
     def __init__(
         self,
-        *args: NavSetArg,
+        *args: NavSetArg | MetadataNode,
         ul_class: str,
         id: Optional[str],
         selected: Optional[str],
         header: TagChild = None,
         footer: TagChild = None,
     ) -> None:
         self.args = args
@@ -671,15 +672,15 @@
 
 class NavSetPillList(NavSet):
     well: bool
     widths: tuple[int, int]
 
     def __init__(
         self,
-        *args: NavSetArg,
+        *args: NavSetArg | MetadataNode,
         ul_class: str,
         id: Optional[str],
         selected: Optional[str],
         header: TagChild = None,
         footer: TagChild = None,
         well: bool = True,
         widths: tuple[int, int] = (4, 8),
@@ -700,15 +701,15 @@
         return row(
             column(widths[0], nav, class_="well" if self.well else None),
             column(widths[1], self.header, content, self.footer),
         )
 
 
 def navset_pill_list(
-    *args: NavSetArg,
+    *args: NavSetArg | MetadataNode,
     id: Optional[str] = None,
     selected: Optional[str] = None,
     header: TagChild = None,
     footer: TagChild = None,
     well: bool = True,
     widths: tuple[int, int] = (4, 8),
 ) -> NavSet:
@@ -727,16 +728,14 @@
         ``value``).
     header
         UI to display above the selected content.
     footer
         UI to display below the selected content.
     well
         ``True`` to place a well (gray rounded rectangle) around the navigation list.
-    fluid
-        ``True`` to use fluid layout; `False` to use fixed layout.
     widths
         Column widths of the navigation list and tabset content areas respectively.
 
     See Also
     -------
     ~shiny.ui.nav
     ~shiny.ui.nav_menu
@@ -773,15 +772,15 @@
     bg: Optional[str]
     inverse: bool
     collapsible: bool
     fluid: bool
 
     def __init__(
         self,
-        *args: NavSetArg,
+        *args: NavSetArg | MetadataNode,
         ul_class: str,
         title: TagChild,
         id: Optional[str],
         selected: Optional[str],
         position: Literal[
             "static-top", "fixed-top", "fixed-bottom", "sticky-top"
         ] = "static-top",
@@ -850,15 +849,15 @@
                 row(self.footer) if self.footer else None,
                 class_="container-fluid" if self.fluid else "container",
             ),
         )
 
 
 def navset_bar(
-    *args: NavSetArg,
+    *args: NavSetArg | MetadataNode | Sequence[MetadataNode],
     title: TagChild,
     id: Optional[str] = None,
     selected: Optional[str] = None,
     position: Literal[
         "static-top", "fixed-top", "fixed-bottom", "sticky-top"
     ] = "static-top",
     header: TagChild = None,
@@ -919,16 +918,24 @@
     ~shiny.ui.navset_hidden
 
     Example
     -------
     See :func:`~shiny.ui.nav`.
     """
 
+    # If args contains any lists, flatten them into args.
+    new_args: Sequence[NavSetArg | MetadataNode] = []
+    for arg in args:
+        if isinstance(arg, (list, tuple)):
+            new_args.extend(arg)
+        else:
+            new_args.append(cast(NavSetArg, arg))
+
     return NavSetBar(
-        *args,
+        *new_args,
         ul_class="nav navbar-nav",
         id=resolve_id(id) if id else None,
         selected=selected,
         title=title,
         position=position,
         header=header,
         footer=footer,
@@ -939,32 +946,42 @@
     )
 
 
 # -----------------------------------------------------------------------------
 # Utilities for rendering navs
 # -----------------------------------------------------------------------------\
 def render_navset(
-    *items: NavSetArg,
+    *items: NavSetArg | MetadataNode,
     ul_class: str,
     id: Optional[str],
     selected: Optional[str],
     context: dict[str, Any],
 ) -> tuple[Tag, Tag]:
     tabsetid = private_random_int(1000, 10000)
 
+    # Separate MetadataNodes from NavSetArgs.
+    metadata_args = [x for x in items if isinstance(x, MetadataNode)]
+    navset_args = [x for x in items if not isinstance(x, MetadataNode)]
+
     # If the user hasn't provided a selected value, use the first one
     if selected is None:
-        for x in items:
+        for x in navset_args:
             selected = x.get_value()
             if selected is not None:
                 break
 
-    ul_tag = tags.ul(bootstrap_deps(), class_=ul_class, id=id, data_tabsetid=tabsetid)
+    ul_tag = tags.ul(
+        bootstrap_deps(),
+        metadata_args,
+        class_=ul_class,
+        id=id,
+        data_tabsetid=tabsetid,
+    )
     div_tag = div(class_="tab-content", data_tabsetid=tabsetid)
-    for i, x in enumerate(items):
+    for i, x in enumerate(navset_args):
         nav, contents = x.resolve(
             selected, {**context, "tabsetid": tabsetid, "index": i}
         )
         ul_tag.append(nav)
         div_tag.append(contents)
 
     return ul_tag, div_tag
```

### Comparing `shiny-0.3.0/shiny/ui/_notification.py` & `shiny-0.3.1/shiny/ui/_notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,19 +45,20 @@
         notification with the same ``id`` will be replaced with this one (otherwise, a
         new notification is created).
     type
         A string which controls the color of the notification. One of "default" (gray),
         "message" (blue), "warning" (yellow), or "error" (red).
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Returns
     -------
-    The notification's ``id``.
+    :
+        The notification's ``id``.
 
     See Also
     -------
     ~shiny.ui.notification_remove
     ~shiny.ui.modal
     """
 
@@ -91,19 +92,20 @@
 
     Parameters
     ----------
     id
         A notification ``id``.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
 
     Returns
     -------
-    The notification's ``id``.
+    :
+        The notification's ``id``.
 
     See Also
     -------
     ~shiny.ui.notification_show
     ~shiny.ui.modal
 
     Example
```

### Comparing `shiny-0.3.0/shiny/ui/_output.py` & `shiny-0.3.1/shiny/ui/_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,16 @@
         elements indicating the brush area. To control the brush behavior, use
         :func:`~shiny.ui.brush_opts`. Multiple `output_image`/`output_plot` calls may
         share the same `id` value; brushing one image or plot will cause any other
         brushes with the same `id` to disappear.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     See Also
     -------
     ~shiny.render.plot ~shiny.ui.output_image
     """
     res = output_image(
         id=id,
@@ -161,15 +162,16 @@
         elements indicating the brush area. To control the brush behavior, use
         :func:`~shiny.ui.brush_opts`. Multiple `output_image`/`output_plot` calls may
         share the same `id` value; brushing one image or plot will cause any other
         brushes with the same `id` to disappear.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     See Also
     -------
     ~shiny.render.image
     ~shiny.ui.output_plot
     """
     func = tags.span if inline else div
@@ -225,15 +227,16 @@
     inline
         If ``True``, the result is displayed inline
     container
         A Callable that returns the output container.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     Note
     ----
     Text is HTML-escaped prior to rendering.
 
     See Also
     -------
@@ -260,15 +263,16 @@
         An input id.
     placeholder
         If the output is empty or ``None``, should an empty rectangle be displayed to
         serve as a placeholder? (does not affect behavior when the output is nonempty)
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     See Also
     -------
     ~shiny.render.text
     ~shiny.ui.output_text
 
     Example
@@ -290,14 +294,15 @@
     id
         An input id.
     **kwargs
         Additional attributes to add to the container.
 
     Returns
     -------
+    :
 
     See Also
     -------
     ~shiny.render.table
     """
     return tags.div({"class": "shiny-html-output"}, id=resolve_id(id), **kwargs)
 
@@ -321,15 +326,16 @@
     container
         A Callable that returns the output container.
     kwargs
         Attributes to be applied to the output container.
 
     Returns
     -------
-    A UI element
+    :
+        A UI element
 
     See Also
     -------
     ~shiny.render.ui
     ~shiny.ui.output_text
     """
```

### Comparing `shiny-0.3.0/shiny/ui/_page.py` & `shiny-0.3.1/shiny/ui/_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,47 +3,44 @@
 __all__ = (
     "page_navbar",
     "page_fluid",
     "page_fixed",
     "page_bootstrap",
 )
 
-from typing import Any, Optional
+from typing import Optional, Sequence
 
-# Tagifiable isn't used directly in this file, but it seems to necessary to import
-# it somewhere for Sphinx to work cleanly.
-from htmltools import Tagifiable  # pyright: ignore[reportUnusedImport] # noqa: F401
-from htmltools import Tag, TagChild, TagList, div, tags
+from htmltools import MetadataNode, Tag, TagAttrs, TagChild, TagList, div, tags
 
 from .._docstring import add_example
 from .._namespaces import resolve_id
 from .._typing_extensions import Literal
 from ..types import MISSING, MISSING_TYPE, NavSetArg
 from ._html_dependencies import bootstrap_deps
 from ._navs import navset_bar
 from ._utils import get_window_title
 
 
 def page_navbar(
-    *args: NavSetArg,
+    *args: NavSetArg | MetadataNode | Sequence[MetadataNode],
     title: Optional[str | Tag | TagList] = None,
     id: Optional[str] = None,
     selected: Optional[str] = None,
     position: Literal["static-top", "fixed-top", "fixed-bottom"] = "static-top",
     header: Optional[TagChild] = None,
     footer: Optional[TagChild] = None,
     bg: Optional[str] = None,
     inverse: bool = False,
     collapsible: bool = True,
     fluid: bool = True,
     window_title: str | MISSING_TYPE = MISSING,
     lang: Optional[str] = None,
 ) -> Tag:
     """
-    Create a navbar with a navs bar and a title.
+    Create a page with a navbar and a title.
 
     Parameters
     ----------
 
     args
         UI elements.
     title
@@ -81,15 +78,16 @@
     lang
         ISO 639-1 language code for the HTML page, such as ``"en"`` or ``"ko"``. This
         will be used as the lang in the ``<html>`` tag, as in ``<html lang="en">``. The
         default, `None`, results in an empty string.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.nav`
     :func:`~shiny.ui.nav_menu`
     :func:`~shiny.ui.navset_bar`
     :func:`~shiny.ui.page_fluid`
@@ -118,15 +116,18 @@
         ),
         lang=lang,
     )
 
 
 @add_example()
 def page_fluid(
-    *args: Any, title: Optional[str] = None, lang: Optional[str] = None, **kwargs: str
+    *args: TagChild | TagAttrs,
+    title: Optional[str] = None,
+    lang: Optional[str] = None,
+    **kwargs: str,
 ) -> Tag:
     """
     Create a fluid page.
 
     Parameters
     ----------
 
@@ -140,15 +141,16 @@
         be used as the lang in the ``<html>`` tag, as in ``<html lang="en">``. The default,
         `None`, results in an empty string.
     kwargs
         Attributes on the page level container.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.page_fixed`
     :func:`~shiny.ui.page_bootstrap`
     :func:`~shiny.ui.page_navbar`
     """
@@ -156,15 +158,18 @@
     return page_bootstrap(
         div({"class": "container-fluid"}, *args, **kwargs), title=title, lang=lang
     )
 
 
 @add_example()
 def page_fixed(
-    *args: Any, title: Optional[str] = None, lang: Optional[str] = None, **kwargs: str
+    *args: TagChild | TagAttrs,
+    title: Optional[str] = None,
+    lang: Optional[str] = None,
+    **kwargs: str,
 ) -> Tag:
     """
     Create a fixed page.
 
     Parameters
     ----------
 
@@ -178,15 +183,16 @@
         be used as the lang in the ``<html>`` tag, as in ``<html lang="en">``. The default,
         `None`, results in an empty string.
 
     kwargs
         Attributes on the page level container.
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.page_fluid`
     :func:`~shiny.ui.page_bootstrap`
     :func:`~shiny.ui.page_navbar`
     """
@@ -194,15 +200,15 @@
     return page_bootstrap(
         div({"class": "container"}, *args, **kwargs), title=title, lang=lang
     )
 
 
 # TODO: implement theme (just Bootswatch for now?)
 def page_bootstrap(
-    *args: Any, title: Optional[str] = None, lang: Optional[str] = None
+    *args: TagChild | TagAttrs, title: Optional[str] = None, lang: Optional[str] = None
 ) -> Tag:
     """
     Create a Bootstrap UI page container.
 
     Parameters
     ----------
 
@@ -214,18 +220,18 @@
     lang
         ISO 639-1 language code for the HTML page, such as ``"en"`` or ``"ko"``. This will
         be used as the lang in the ``<html>`` tag, as in ``<html lang="en">``. The default,
         `None`, results in an empty string.
 
     Returns
     -------
-    A UI element.
+    :
+        A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.page_fluid`
     :func:`~shiny.ui.page_navbar`
     """
 
-    page = TagList(*bootstrap_deps(), *args)
     head = tags.title(title) if title else None
-    return tags.html(tags.head(head), tags.body(page), lang=lang)
+    return tags.html(tags.head(head), tags.body(*bootstrap_deps(), *args), lang=lang)
```

### Comparing `shiny-0.3.0/shiny/ui/_plot_output_opts.py` & `shiny-0.3.1/shiny/ui/_plot_output_opts.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/ui/_progress.py` & `shiny-0.3.1/shiny/ui/_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         The value that represents the starting point of the progress bar. Must be less
         than ``max``.
     max
         The value that represents the end of the progress bar. Must be greater than
         ``min``.
     session
         A :class:`~shiny.Session` instance. If not provided, it is inferred via
-       :func:`~shiny.session.get_current_session`.
+        :func:`~shiny.session.get_current_session`.
     """
 
     _style = "notification"
 
     min: int
     max: int
     value: float | None
```

### Comparing `shiny-0.3.0/shiny/ui/_utils.py` & `shiny-0.3.1/shiny/ui/_utils.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js` & `shiny-0.3.1/shiny/www/shared/bootstrap/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map` & `shiny-0.3.1/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/bootstrap/bootstrap.min.css` & `shiny-0.3.1/shiny/www/shared/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot` & `shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg` & `shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf` & `shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff` & `shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2` & `shiny-0.3.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/css/dataTables.bootstrap.css` & `shiny-0.3.1/shiny/www/shared/datatables/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/css/dataTables.extra.css` & `shiny-0.3.1/shiny/www/shared/datatables/css/dataTables.extra.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/images/sort_asc.png` & `shiny-0.3.1/shiny/www/shared/datatables/images/sort_asc.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/images/sort_asc_disabled.png` & `shiny-0.3.1/shiny/www/shared/datatables/images/sort_asc_disabled.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/images/sort_both.png` & `shiny-0.3.1/shiny/www/shared/datatables/images/sort_both.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/images/sort_desc.png` & `shiny-0.3.1/shiny/www/shared/datatables/images/sort_desc.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/images/sort_desc_disabled.png` & `shiny-0.3.1/shiny/www/shared/datatables/images/sort_desc_disabled.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/js/dataTables.bootstrap.js` & `shiny-0.3.1/shiny/www/shared/datatables/js/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/js/jquery.dataTables.min.js` & `shiny-0.3.1/shiny/www/shared/datatables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datatables/upgrade1.10.txt` & `shiny-0.3.1/shiny/www/shared/datatables/upgrade1.10.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css` & `shiny-0.3.1/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css` & `shiny-0.3.1/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js` & `shiny-0.3.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/scss/build3.scss` & `shiny-0.3.1/shiny/www/shared/datepicker/scss/build3.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/datepicker/scss/datepicker3.scss` & `shiny-0.3.1/shiny/www/shared/datepicker/scss/datepicker3.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/highlight/LICENSE` & `shiny-0.3.1/shiny/www/shared/highlight/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/highlight/classref.txt` & `shiny-0.3.1/shiny/www/shared/highlight/classref.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/highlight/highlight.pack.js` & `shiny-0.3.1/shiny/www/shared/highlight/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/highlight/rstudio.css` & `shiny-0.3.1/shiny/www/shared/highlight/rstudio.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css` & `shiny-0.3.1/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js` & `shiny-0.3.1/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js` & `shiny-0.3.1/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/ionrangeslider/scss/_base.scss` & `shiny-0.3.1/shiny/www/shared/ionrangeslider/scss/_base.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/ionrangeslider/scss/shiny.scss` & `shiny-0.3.1/shiny/www/shared/ionrangeslider/scss/shiny.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jquery/jquery-3.6.0.js` & `shiny-0.3.1/shiny/www/shared/jquery/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jquery/jquery-3.6.0.min.js` & `shiny-0.3.1/shiny/www/shared/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jquery/jquery-3.6.0.min.map` & `shiny-0.3.1/shiny/www/shared/jquery/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/AUTHORS.txt` & `shiny-0.3.1/shiny/www/shared/jqueryui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/LICENSE.txt` & `shiny-0.3.1/shiny/www/shared/jqueryui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png` & `shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png` & `shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png` & `shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png` & `shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png` & `shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png` & `shiny-0.3.1/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/index.html` & `shiny-0.3.1/shiny/www/shared/jqueryui/index.html`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.css` & `shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.js` & `shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.min.css` & `shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.min.js` & `shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.structure.css` & `shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.structure.min.css` & `shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.theme.css` & `shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/jqueryui/jquery-ui.theme.min.css` & `shiny-0.3.1/shiny/www/shared/jqueryui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/requirejs/require.min.js` & `shiny-0.3.1/shiny/www/shared/requirejs/require.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js` & `shiny-0.3.1/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js` & `shiny-0.3.1/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/css/selectize.bootstrap3.css` & `shiny-0.3.1/shiny/www/shared/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/js/selectize.min.js` & `shiny-0.3.1/shiny/www/shared/selectize/js/selectize.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss` & `shiny-0.3.1/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/scss/plugins/remove_button.scss` & `shiny-0.3.1/shiny/www/shared/selectize/scss/plugins/remove_button.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss` & `shiny-0.3.1/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss` & `shiny-0.3.1/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/scss/selectize.default.scss` & `shiny-0.3.1/shiny/www/shared/selectize/scss/selectize.default.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/selectize/scss/selectize.scss` & `shiny-0.3.1/shiny/www/shared/selectize/scss/selectize.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny-autoreload.js` & `shiny-0.3.1/shiny/www/shared/shiny-autoreload.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny-autoreload.js.map` & `shiny-0.3.1/shiny/www/shared/shiny-autoreload.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny-showcase.css` & `shiny-0.3.1/shiny/www/shared/shiny-showcase.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny-showcase.js` & `shiny-0.3.1/shiny/www/shared/shiny-showcase.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny-showcase.js.map` & `shiny-0.3.1/shiny/www/shared/shiny-showcase.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny-testmode.js.map` & `shiny-0.3.1/shiny/www/shared/shiny-testmode.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny.js` & `shiny-0.3.1/shiny/www/shared/shiny.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny.js.map` & `shiny-0.3.1/shiny/www/shared/shiny.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny.min.css` & `shiny-0.3.1/shiny/www/shared/shiny.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny.min.js` & `shiny-0.3.1/shiny/www/shared/shiny.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny.min.js.map` & `shiny-0.3.1/shiny/www/shared/shiny.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny_scss/bootstrap.scss` & `shiny-0.3.1/shiny/www/shared/shiny_scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/shiny_scss/shiny.scss` & `shiny-0.3.1/shiny/www/shared/shiny_scss/shiny.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/showdown/compressed/showdown.js` & `shiny-0.3.1/shiny/www/shared/showdown/compressed/showdown.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/showdown/license.txt` & `shiny-0.3.1/shiny/www/shared/showdown/license.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/showdown/src/showdown.js` & `shiny-0.3.1/shiny/www/shared/showdown/src/showdown.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny/www/shared/strftime/strftime-min.js` & `shiny-0.3.1/shiny/www/shared/strftime/strftime-min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/shiny.egg-info/PKG-INFO` & `shiny-0.3.1/shiny.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny
-Version: 0.3.0
+Version: 0.3.1
 Summary: A web development framework for Python.
 Home-page: https://github.com/rstudio/py-shiny
 Author: Winston Chang
 Author-email: winston@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shiny/issues
 Project-URL: Documentation, https://shiny.rstudio.com/py/
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 Shiny for Python
 ================
 
 See the [Shiny for Python website](https://shiny.rstudio.com/py/).
@@ -49,15 +48,15 @@
 More detailed installation instructions, including the use of `conda`, are [also available](https://shiny.rstudio.com/py/docs/install.html).
 
 ## Development
 
 If you want to do development on Shiny for Python:
 
 ```sh
-pip install -e ".[dev,docs,test]"
+pip install -e ".[dev,test]"
 ```
 
 Additionally, you can install pre-commit hooks which will automatically reformat and lint the code when you make a commit:
 
 ```sh
 pre-commit install
```

### Comparing `shiny-0.3.0/shiny.egg-info/SOURCES.txt` & `shiny-0.3.1/shiny.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-docs/Makefile
-docs/source/conf.py
-docs/source/index.rst
-docs/source/_templates/class.rst
-docs/source/_templates/justattributes.rst
-docs/source/_templates/tag_func.rst
-docs/source/_templates/tags.rst
-docs/source/images/shiny-logo.png
 shiny/__init__.py
 shiny/__main__.py
 shiny/_app.py
 shiny/_autoreload.py
 shiny/_connection.py
 shiny/_datastructures.py
 shiny/_deprecated.py
```

### Comparing `shiny-0.3.0/tests/asyncio_prevent.py` & `shiny-0.3.1/tests/asyncio_prevent.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/mocktime.py` & `shiny-0.3.1/tests/mocktime.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_e2e_regex_matching.py` & `shiny-0.3.1/tests/test_e2e_regex_matching.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_markdown.py` & `shiny-0.3.1/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_modules.py` & `shiny-0.3.1/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_namespaces.py` & `shiny-0.3.1/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_navs.py` & `shiny-0.3.1/tests/test_navs.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_poll.py` & `shiny-0.3.1/tests/test_poll.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_reactives.py` & `shiny-0.3.1/tests/test_reactives.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_shinysession.py` & `shiny-0.3.1/tests/test_shinysession.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_static.py` & `shiny-0.3.1/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_ui.py` & `shiny-0.3.1/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.0/tests/test_utils.py` & `shiny-0.3.1/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -132,23 +132,59 @@
     await callbacks.invoke()
     assert cb1.exec_count == 2  # Regular registration was called again
     assert cb2.exec_count == 1  # Unregistered by previous invoke, not called again
     assert cb3.exec_count == 1  # once=True, so not called again
     assert cb4.exec_count == 1  # Registered during previous invoke(), was called
 
 
+# Timeout within 2 seconds
+@pytest.mark.timeout(2)
 def test_random_port():
     assert random_port(9000, 9000) == 9000
 
+    # Starting port
+    port = 9001
+    # Test a set of continguous ports
+    num_ports = 10
+    # Number of times to try to find a port range
+    n = 100
+
+    # Find a range of `num_ports` ports that are all available
+    attempts = 0
+    for _ in range(n):
+        attempts += 1
+        j = 0
+        try:
+            for j in range(num_ports):
+                random_port(port + j, port + j)
+            # If we reach this point, we have found a plausible range of ports to use
+            break
+
+        except RuntimeError as e:
+            print(e)
+            # Port `port + j` is busy,
+            # Shift the test range and try again
+            port += j + 1
+            print(port)
+    # If no port is available, throw an error
+    # `attempts` should be << n
+    if attempts == n:
+        raise RuntimeError(
+            f"Could not find {num_ports} continguous ports to use for testing in {n} tries"
+        )
+
     seen: Set[int] = set()
-    # Ensure that 10 unique random ports are eventually generated. If not (e.g. if the
+    # Ensure that `num_ports` unique random ports are eventually generated. If not (e.g. if the
     # max port number is treated as exclusive instead of inclusive, say) then the while
     # loop will not exit and the test will timeout.
-    while len(seen) < 10:
-        seen.add(random_port(9001, 9010))
+    max_port = port + num_ports - 1
+    while len(seen) < num_ports:
+        seen.add(random_port(port, max_port))
+
+    assert len(seen) == num_ports
 
 
 def test_random_port_unusable():
     # 6000 is an unsafe port, make sure that it fails
     with pytest.raises(RuntimeError, match="Failed to find a usable random port"):
         random_port(6000, 6000)
```

### Comparing `shiny-0.3.0/tests/test_utils_async.py` & `shiny-0.3.1/tests/test_utils_async.py`

 * *Files identical despite different names*

