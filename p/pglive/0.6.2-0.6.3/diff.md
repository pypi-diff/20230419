# Comparing `tmp/pglive-0.6.2.tar.gz` & `tmp/pglive-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pglive-0.6.2.tar", max compression
+gzip compressed data, was "pglive-0.6.3.tar", max compression
```

## Comparing `pglive-0.6.2.tar` & `pglive-0.6.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rwxr-xr-x   0        0        0     1067 2022-07-09 17:29:11.350000 pglive-0.6.2/LICENSE
--rw-r--r--   0        0        0     4832 2022-10-05 09:41:55.714371 pglive-0.6.2/README.md
--rw-r--r--   0        0        0        0 2022-08-12 14:14:02.223971 pglive-0.6.2/pglive/__init__.py
--rw-r--r--   0        0        0     2631 2022-10-30 15:40:38.383067 pglive-0.6.2/pglive/examples_pyqt5/__init__.py
--rw-r--r--   0        0        0     1087 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt5/all_plot_types.py
--rw-r--r--   0        0        0     1992 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt5/axis.py
--rw-r--r--   0        0        0      677 2022-10-04 11:16:03.707471 pglive-0.6.2/pglive/examples_pyqt5/candlestick_plot.py
--rw-r--r--   0        0        0     1416 2022-10-15 14:26:45.414357 pglive-0.6.2/pglive/examples_pyqt5/categorized_bar_plot.py
--rw-r--r--   0        0        0     2967 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt5/crop_offset_to_data.py
--rw-r--r--   0        0        0     2651 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt5/crosshair.py
--rw-r--r--   0        0        0        0 2022-08-12 14:14:02.227972 pglive-0.6.2/pglive/examples_pyqt5/designer_example/__init__.py
--rw-r--r--   0        0        0      813 2022-08-12 14:14:02.227972 pglive-0.6.2/pglive/examples_pyqt5/designer_example/main_example.py
--rw-r--r--   0        0        0     2203 2022-08-12 14:14:02.227972 pglive-0.6.2/pglive/examples_pyqt5/designer_example/win_template.py
--rw-r--r--   0        0        0     1489 2022-08-12 14:14:02.227972 pglive-0.6.2/pglive/examples_pyqt5/designer_example/win_template.ui
--rw-r--r--   0        0        0      610 2022-08-12 14:14:02.227972 pglive-0.6.2/pglive/examples_pyqt5/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2498 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt5/leading_line.py
--rw-r--r--   0        0        0      630 2022-10-02 18:40:13.661184 pglive-0.6.2/pglive/examples_pyqt5/line_plot.py
--rw-r--r--   0        0        0     6533 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt5/live_plot_range.py
--rw-r--r--   0        0        0     2061 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1767 2022-09-17 09:24:32.115182 pglive-0.6.2/pglive/examples_pyqt5/pause_resume.py
--rw-r--r--   0        0        0      998 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt5/plot_rate.py
--rw-r--r--   0        0        0      642 2022-08-12 14:14:02.227972 pglive-0.6.2/pglive/examples_pyqt5/scatter_plot.py
--rw-r--r--   0        0        0     1249 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt5/update_rate.py
--rw-r--r--   0        0        0      683 2022-08-12 14:14:02.227972 pglive-0.6.2/pglive/examples_pyqt5/vertical_bar_plot.py
--rw-r--r--   0        0        0     1143 2022-08-12 14:14:02.227972 pglive-0.6.2/pglive/examples_pyqt5/vertical_bar_plot_color.py
--rw-r--r--   0        0        0     2631 2022-11-24 13:54:15.682940 pglive-0.6.2/pglive/examples_pyqt6/__init__.py
--rw-r--r--   0        0        0     1085 2023-02-24 16:49:46.388993 pglive-0.6.2/pglive/examples_pyqt6/all_plot_types.py
--rw-r--r--   0        0        0     1992 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt6/axis.py
--rw-r--r--   0        0        0      677 2022-09-17 17:13:21.940234 pglive-0.6.2/pglive/examples_pyqt6/candlestick_plot.py
--rw-r--r--   0        0        0     1416 2022-10-11 05:50:18.848975 pglive-0.6.2/pglive/examples_pyqt6/categorized_bar_plot.py
--rw-r--r--   0        0        0     2966 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt6/crop_offset_to_data.py
--rw-r--r--   0        0        0     2651 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt6/crosshair.py
--rw-r--r--   0        0        0        0 2022-08-12 14:14:02.227972 pglive-0.6.2/pglive/examples_pyqt6/designer_example/__init__.py
--rw-r--r--   0        0        0      813 2022-11-24 15:39:08.017064 pglive-0.6.2/pglive/examples_pyqt6/designer_example/main_example.py
--rw-r--r--   0        0        0     2191 2022-11-24 15:39:08.017064 pglive-0.6.2/pglive/examples_pyqt6/designer_example/win_template.py
--rw-r--r--   0        0        0     1489 2022-11-24 15:39:08.021064 pglive-0.6.2/pglive/examples_pyqt6/designer_example/win_template.ui
--rw-r--r--   0        0        0      610 2022-10-11 05:57:05.067239 pglive-0.6.2/pglive/examples_pyqt6/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2498 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt6/leading_line.py
--rw-r--r--   0        0        0      630 2023-02-25 08:15:41.220788 pglive-0.6.2/pglive/examples_pyqt6/line_plot.py
--rw-r--r--   0        0        0     6546 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt6/live_plot_range.py
--rw-r--r--   0        0        0     2061 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1767 2022-08-12 14:14:02.231972 pglive-0.6.2/pglive/examples_pyqt6/pause_resume.py
--rw-r--r--   0        0        0     1003 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt6/plot_rate.py
--rw-r--r--   0        0        0      642 2022-08-12 17:26:56.467504 pglive-0.6.2/pglive/examples_pyqt6/scatter_plot.py
--rw-r--r--   0        0        0     1250 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyqt6/update_rate.py
--rw-r--r--   0        0        0      683 2022-09-17 16:59:56.187449 pglive-0.6.2/pglive/examples_pyqt6/vertical_bar_plot.py
--rw-r--r--   0        0        0     1143 2022-08-12 18:20:15.589032 pglive-0.6.2/pglive/examples_pyqt6/vertical_bar_plot_color.py
--rw-r--r--   0        0        0     2635 2022-10-05 10:08:23.688683 pglive-0.6.2/pglive/examples_pyside2/__init__.py
--rw-r--r--   0        0        0     1090 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyside2/all_plot_types.py
--rw-r--r--   0        0        0     1995 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyside2/axis.py
--rw-r--r--   0        0        0      680 2022-08-13 16:38:22.033015 pglive-0.6.2/pglive/examples_pyside2/candlestick_plot.py
--rw-r--r--   0        0        0     1419 2022-10-11 05:50:18.880975 pglive-0.6.2/pglive/examples_pyside2/categorized_bar_plot.py
--rw-r--r--   0        0        0     2970 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyside2/crop_offset_to_data.py
--rw-r--r--   0        0        0     2658 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyside2/crosshair.py
--rw-r--r--   0        0        0      613 2022-08-12 14:14:02.231972 pglive-0.6.2/pglive/examples_pyside2/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2501 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyside2/leading_line.py
--rw-r--r--   0        0        0      633 2022-08-12 14:14:02.231972 pglive-0.6.2/pglive/examples_pyside2/line_plot.py
--rw-r--r--   0        0        0     6615 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyside2/live_plot_range.py
--rw-r--r--   0        0        0     2064 2023-02-22 17:37:04.242169 pglive-0.6.2/pglive/examples_pyside2/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1772 2022-08-12 14:14:02.231972 pglive-0.6.2/pglive/examples_pyside2/pause_resume.py
--rw-r--r--   0        0        0     1044 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/examples_pyside2/plot_rate.py
--rw-r--r--   0        0        0      645 2022-08-12 14:14:02.231972 pglive-0.6.2/pglive/examples_pyside2/scatter_plot.py
--rw-r--r--   0        0        0     1252 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/examples_pyside2/update_rate.py
--rw-r--r--   0        0        0      686 2022-08-12 14:14:02.231972 pglive-0.6.2/pglive/examples_pyside2/vertical_bar_plot.py
--rw-r--r--   0        0        0     1146 2022-08-12 14:14:02.231972 pglive-0.6.2/pglive/examples_pyside2/vertical_bar_plot_color.py
--rw-r--r--   0        0        0     2635 2022-10-05 10:08:23.684683 pglive-0.6.2/pglive/examples_pyside6/__init__.py
--rw-r--r--   0        0        0     1089 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/examples_pyside6/all_plot_types.py
--rw-r--r--   0        0        0     1994 2023-03-10 13:07:31.775296 pglive-0.6.2/pglive/examples_pyside6/axis.py
--rw-r--r--   0        0        0      679 2022-08-13 16:39:37.789759 pglive-0.6.2/pglive/examples_pyside6/candlestick_plot.py
--rw-r--r--   0        0        0     1418 2022-10-11 05:50:18.868975 pglive-0.6.2/pglive/examples_pyside6/categorized_bar_plot.py
--rw-r--r--   0        0        0     2969 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/examples_pyside6/crop_offset_to_data.py
--rw-r--r--   0        0        0     2657 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/examples_pyside6/crosshair.py
--rw-r--r--   0        0        0      612 2022-08-12 14:14:02.231972 pglive-0.6.2/pglive/examples_pyside6/horizontal_bar_plot.py
--rw-r--r--   0        0        0     2500 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/examples_pyside6/leading_line.py
--rw-r--r--   0        0        0      632 2022-08-12 14:14:02.231972 pglive-0.6.2/pglive/examples_pyside6/line_plot.py
--rw-r--r--   0        0        0     6614 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/examples_pyside6/live_plot_range.py
--rw-r--r--   0        0        0     2063 2023-03-10 12:21:40.267461 pglive-0.6.2/pglive/examples_pyside6/one_plot_multiple_plot_rates.py
--rw-r--r--   0        0        0     1771 2023-02-22 17:02:27.405619 pglive-0.6.2/pglive/examples_pyside6/pause_resume.py
--rw-r--r--   0        0        0     1000 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/examples_pyside6/plot_rate.py
--rw-r--r--   0        0        0      644 2022-08-12 18:42:45.412326 pglive-0.6.2/pglive/examples_pyside6/scatter_plot.py
--rw-r--r--   0        0        0     1251 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/examples_pyside6/update_rate.py
--rw-r--r--   0        0        0      685 2022-08-12 14:14:02.235972 pglive-0.6.2/pglive/examples_pyside6/vertical_bar_plot.py
--rw-r--r--   0        0        0     1145 2022-08-12 14:14:02.235972 pglive-0.6.2/pglive/examples_pyside6/vertical_bar_plot_color.py
--rw-r--r--   0        0        0      967 2022-10-05 06:34:53.511344 pglive-0.6.2/pglive/kwargs.py
--rw-r--r--   0        0        0        0 2022-08-12 14:14:02.235972 pglive-0.6.2/pglive/sources/__init__.py
--rw-r--r--   0        0        0     6859 2023-03-10 13:02:08.227569 pglive-0.6.2/pglive/sources/data_connector.py
--rw-r--r--   0        0        0     4694 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/sources/live_axis.py
--rw-r--r--   0        0        0     7701 2023-03-10 12:02:20.144602 pglive-0.6.2/pglive/sources/live_axis_range.py
--rw-r--r--   0        0        0     3256 2023-02-24 16:11:35.050513 pglive-0.6.2/pglive/sources/live_candleStickPlot.py
--rw-r--r--   0        0        0     4510 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/sources/live_categorized_bar_plot.py
--rw-r--r--   0        0        0     5883 2023-02-22 17:37:04.246169 pglive-0.6.2/pglive/sources/live_mixins.py
--rw-r--r--   0        0        0     5276 2023-02-25 08:20:48.929494 pglive-0.6.2/pglive/sources/live_plot.py
--rw-r--r--   0        0        0    11000 2023-03-10 12:21:37.547452 pglive-0.6.2/pglive/sources/live_plot_widget.py
--rw-r--r--   0        0        0     1599 2023-02-25 08:15:41.220788 pglive-0.6.2/pglive/sources/utils.py
--rw-r--r--   0        0        0      955 2023-03-10 13:07:45.447569 pglive-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5830 1970-01-01 00:00:00.000000 pglive-0.6.2/setup.py
--rw-r--r--   0        0        0     5769 1970-01-01 00:00:00.000000 pglive-0.6.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1067 2022-07-09 17:29:11.350000 pglive-0.6.3/LICENSE
+-rw-r--r--   0        0        0     4832 2023-04-14 17:18:13.360265 pglive-0.6.3/README.md
+-rw-r--r--   0        0        0        0 2022-08-12 14:14:02.223971 pglive-0.6.3/pglive/__init__.py
+-rw-r--r--   0        0        0     2631 2023-03-25 07:41:59.485596 pglive-0.6.3/pglive/examples_pyqt5/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-14 16:57:54.239777 pglive-0.6.3/pglive/examples_pyqt5/all_plot_types.py
+-rw-r--r--   0        0        0     1992 2023-04-14 16:58:27.839960 pglive-0.6.3/pglive/examples_pyqt5/axis.py
+-rw-r--r--   0        0        0      685 2023-04-14 16:59:03.904220 pglive-0.6.3/pglive/examples_pyqt5/candlestick_plot.py
+-rw-r--r--   0        0        0     1416 2023-04-14 16:59:03.892220 pglive-0.6.3/pglive/examples_pyqt5/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2957 2023-04-14 17:00:55.641092 pglive-0.6.3/pglive/examples_pyqt5/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2650 2023-04-14 17:01:32.765324 pglive-0.6.3/pglive/examples_pyqt5/crosshair.py
+-rw-r--r--   0        0        0        0 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt5/designer_example/__init__.py
+-rw-r--r--   0        0        0      813 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt5/designer_example/main_example.py
+-rw-r--r--   0        0        0     2203 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt5/designer_example/win_template.py
+-rw-r--r--   0        0        0     1489 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt5/designer_example/win_template.ui
+-rw-r--r--   0        0        0      610 2023-04-14 17:01:53.765447 pglive-0.6.3/pglive/examples_pyqt5/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2498 2023-04-14 17:02:17.081578 pglive-0.6.3/pglive/examples_pyqt5/leading_line.py
+-rw-r--r--   0        0        0      630 2023-04-14 17:02:55.533785 pglive-0.6.3/pglive/examples_pyqt5/line_plot.py
+-rw-r--r--   0        0        0     6533 2023-04-14 17:02:55.545785 pglive-0.6.3/pglive/examples_pyqt5/live_plot_range.py
+-rw-r--r--   0        0        0     2061 2023-04-14 17:03:31.953971 pglive-0.6.3/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1767 2023-04-14 17:11:38.123162 pglive-0.6.3/pglive/examples_pyqt5/pause_resume.py
+-rw-r--r--   0        0        0      999 2023-04-14 17:04:45.710330 pglive-0.6.3/pglive/examples_pyqt5/plot_rate.py
+-rw-r--r--   0        0        0      642 2023-04-14 17:05:01.810406 pglive-0.6.3/pglive/examples_pyqt5/scatter_plot.py
+-rw-r--r--   0        0        0     1248 2023-04-14 17:05:38.346576 pglive-0.6.3/pglive/examples_pyqt5/update_rate.py
+-rw-r--r--   0        0        0      683 2023-04-14 17:05:38.358576 pglive-0.6.3/pglive/examples_pyqt5/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1143 2023-04-14 17:12:56.975330 pglive-0.6.3/pglive/examples_pyqt5/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0     2631 2022-11-24 13:54:15.682940 pglive-0.6.3/pglive/examples_pyqt6/__init__.py
+-rw-r--r--   0        0        0     1091 2023-04-14 17:17:10.096057 pglive-0.6.3/pglive/examples_pyqt6/all_plot_types.py
+-rw-r--r--   0        0        0     1992 2023-04-14 17:08:29.834979 pglive-0.6.3/pglive/examples_pyqt6/axis.py
+-rw-r--r--   0        0        0      685 2023-04-14 17:08:48.934979 pglive-0.6.3/pglive/examples_pyqt6/candlestick_plot.py
+-rw-r--r--   0        0        0     1416 2023-04-14 17:09:04.442982 pglive-0.6.3/pglive/examples_pyqt6/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2955 2023-04-14 17:21:40.620984 pglive-0.6.3/pglive/examples_pyqt6/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2650 2023-04-14 17:09:54.127013 pglive-0.6.3/pglive/examples_pyqt6/crosshair.py
+-rw-r--r--   0        0        0        0 2022-08-12 14:14:02.227972 pglive-0.6.3/pglive/examples_pyqt6/designer_example/__init__.py
+-rw-r--r--   0        0        0      813 2022-11-24 15:39:08.017064 pglive-0.6.3/pglive/examples_pyqt6/designer_example/main_example.py
+-rw-r--r--   0        0        0     2191 2022-11-24 15:39:08.017064 pglive-0.6.3/pglive/examples_pyqt6/designer_example/win_template.py
+-rw-r--r--   0        0        0     1489 2022-11-24 15:39:08.021064 pglive-0.6.3/pglive/examples_pyqt6/designer_example/win_template.ui
+-rw-r--r--   0        0        0      610 2023-04-14 17:10:09.555029 pglive-0.6.3/pglive/examples_pyqt6/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2498 2023-04-14 17:10:33.699058 pglive-0.6.3/pglive/examples_pyqt6/leading_line.py
+-rw-r--r--   0        0        0      630 2023-04-14 17:10:50.079081 pglive-0.6.3/pglive/examples_pyqt6/line_plot.py
+-rw-r--r--   0        0        0     6546 2023-04-14 17:11:03.675102 pglive-0.6.3/pglive/examples_pyqt6/live_plot_range.py
+-rw-r--r--   0        0        0     2061 2023-04-14 17:11:23.751136 pglive-0.6.3/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1767 2023-04-14 17:11:41.735169 pglive-0.6.3/pglive/examples_pyqt6/pause_resume.py
+-rw-r--r--   0        0        0     1002 2023-04-14 17:11:55.499195 pglive-0.6.3/pglive/examples_pyqt6/plot_rate.py
+-rw-r--r--   0        0        0      642 2023-04-14 17:12:12.039229 pglive-0.6.3/pglive/examples_pyqt6/scatter_plot.py
+-rw-r--r--   0        0        0     1249 2023-04-14 17:12:23.487254 pglive-0.6.3/pglive/examples_pyqt6/update_rate.py
+-rw-r--r--   0        0        0      683 2023-04-14 17:12:38.967288 pglive-0.6.3/pglive/examples_pyqt6/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1143 2023-04-14 17:12:56.979330 pglive-0.6.3/pglive/examples_pyqt6/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0     2635 2022-10-05 10:08:23.688683 pglive-0.6.3/pglive/examples_pyside2/__init__.py
+-rw-r--r--   0        0        0     1090 2023-04-14 17:17:00.544026 pglive-0.6.3/pglive/examples_pyside2/all_plot_types.py
+-rw-r--r--   0        0        0     1995 2023-04-14 17:18:13.344265 pglive-0.6.3/pglive/examples_pyside2/axis.py
+-rw-r--r--   0        0        0      688 2023-04-14 17:20:19.060696 pglive-0.6.3/pglive/examples_pyside2/candlestick_plot.py
+-rw-r--r--   0        0        0     1419 2023-04-14 17:21:00.912843 pglive-0.6.3/pglive/examples_pyside2/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2959 2023-04-14 17:21:40.908985 pglive-0.6.3/pglive/examples_pyside2/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2657 2023-04-14 17:21:55.837039 pglive-0.6.3/pglive/examples_pyside2/crosshair.py
+-rw-r--r--   0        0        0      613 2023-04-14 17:22:09.325087 pglive-0.6.3/pglive/examples_pyside2/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2501 2023-04-14 17:22:31.713167 pglive-0.6.3/pglive/examples_pyside2/leading_line.py
+-rw-r--r--   0        0        0      633 2023-04-14 17:18:13.360265 pglive-0.6.3/pglive/examples_pyside2/line_plot.py
+-rw-r--r--   0        0        0     6615 2023-04-14 17:22:51.313238 pglive-0.6.3/pglive/examples_pyside2/live_plot_range.py
+-rw-r--r--   0        0        0     2064 2023-04-14 17:23:07.897298 pglive-0.6.3/pglive/examples_pyside2/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1772 2023-04-14 17:23:28.477373 pglive-0.6.3/pglive/examples_pyside2/pause_resume.py
+-rw-r--r--   0        0        0     1043 2023-04-14 17:23:43.229426 pglive-0.6.3/pglive/examples_pyside2/plot_rate.py
+-rw-r--r--   0        0        0      645 2023-04-14 17:23:56.865476 pglive-0.6.3/pglive/examples_pyside2/scatter_plot.py
+-rw-r--r--   0        0        0     1251 2023-04-14 17:24:11.373529 pglive-0.6.3/pglive/examples_pyside2/update_rate.py
+-rw-r--r--   0        0        0      686 2023-04-14 17:24:22.181568 pglive-0.6.3/pglive/examples_pyside2/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1146 2023-04-14 17:24:22.181568 pglive-0.6.3/pglive/examples_pyside2/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0     2635 2022-10-05 10:08:23.684683 pglive-0.6.3/pglive/examples_pyside6/__init__.py
+-rw-r--r--   0        0        0     1089 2023-04-14 17:17:00.536026 pglive-0.6.3/pglive/examples_pyside6/all_plot_types.py
+-rw-r--r--   0        0        0     1994 2023-04-14 17:18:13.356265 pglive-0.6.3/pglive/examples_pyside6/axis.py
+-rw-r--r--   0        0        0      687 2023-04-14 17:20:23.324711 pglive-0.6.3/pglive/examples_pyside6/candlestick_plot.py
+-rw-r--r--   0        0        0     1418 2023-04-14 17:21:00.920843 pglive-0.6.3/pglive/examples_pyside6/categorized_bar_plot.py
+-rw-r--r--   0        0        0     2958 2023-04-14 17:21:40.916985 pglive-0.6.3/pglive/examples_pyside6/crop_offset_to_data.py
+-rw-r--r--   0        0        0     2656 2023-04-14 17:21:55.825039 pglive-0.6.3/pglive/examples_pyside6/crosshair.py
+-rw-r--r--   0        0        0      612 2023-04-14 17:22:09.329087 pglive-0.6.3/pglive/examples_pyside6/horizontal_bar_plot.py
+-rw-r--r--   0        0        0     2500 2023-04-14 17:22:31.721167 pglive-0.6.3/pglive/examples_pyside6/leading_line.py
+-rw-r--r--   0        0        0      632 2023-04-14 17:18:13.356265 pglive-0.6.3/pglive/examples_pyside6/line_plot.py
+-rw-r--r--   0        0        0     6614 2023-04-14 17:22:51.301238 pglive-0.6.3/pglive/examples_pyside6/live_plot_range.py
+-rw-r--r--   0        0        0     2063 2023-04-14 17:23:07.897298 pglive-0.6.3/pglive/examples_pyside6/one_plot_multiple_plot_rates.py
+-rw-r--r--   0        0        0     1771 2023-04-14 17:23:28.485373 pglive-0.6.3/pglive/examples_pyside6/pause_resume.py
+-rw-r--r--   0        0        0      999 2023-04-14 17:23:43.217426 pglive-0.6.3/pglive/examples_pyside6/plot_rate.py
+-rw-r--r--   0        0        0      644 2023-04-14 17:23:56.857476 pglive-0.6.3/pglive/examples_pyside6/scatter_plot.py
+-rw-r--r--   0        0        0     1250 2023-04-14 17:24:11.361528 pglive-0.6.3/pglive/examples_pyside6/update_rate.py
+-rw-r--r--   0        0        0      685 2023-04-14 17:24:22.177568 pglive-0.6.3/pglive/examples_pyside6/vertical_bar_plot.py
+-rw-r--r--   0        0        0     1145 2023-04-14 17:24:22.169568 pglive-0.6.3/pglive/examples_pyside6/vertical_bar_plot_color.py
+-rw-r--r--   0        0        0      967 2022-10-05 06:34:53.511344 pglive-0.6.3/pglive/kwargs.py
+-rw-r--r--   0        0        0        0 2022-08-12 14:14:02.235972 pglive-0.6.3/pglive/sources/__init__.py
+-rw-r--r--   0        0        0     6859 2023-03-10 13:02:08.227569 pglive-0.6.3/pglive/sources/data_connector.py
+-rw-r--r--   0        0        0     4694 2023-02-22 17:37:04.246169 pglive-0.6.3/pglive/sources/live_axis.py
+-rw-r--r--   0        0        0     7701 2023-03-10 12:02:20.144602 pglive-0.6.3/pglive/sources/live_axis_range.py
+-rw-r--r--   0        0        0     3256 2023-04-14 16:55:56.062555 pglive-0.6.3/pglive/sources/live_candleStickPlot.py
+-rw-r--r--   0        0        0     4510 2023-02-22 17:37:04.246169 pglive-0.6.3/pglive/sources/live_categorized_bar_plot.py
+-rw-r--r--   0        0        0     5883 2023-02-22 17:37:04.246169 pglive-0.6.3/pglive/sources/live_mixins.py
+-rw-r--r--   0        0        0     5274 2023-04-14 17:54:49.990162 pglive-0.6.3/pglive/sources/live_plot.py
+-rw-r--r--   0        0        0    11010 2023-04-14 17:48:11.264140 pglive-0.6.3/pglive/sources/live_plot_widget.py
+-rw-r--r--   0        0        0     1599 2023-02-25 08:15:41.220788 pglive-0.6.3/pglive/sources/utils.py
+-rw-r--r--   0        0        0      973 2023-04-19 05:43:29.658908 pglive-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 pglive-0.6.3/setup.py
+-rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 pglive-0.6.3/PKG-INFO
```

### Comparing `pglive-0.6.2/LICENSE` & `pglive-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/README.md` & `pglive-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from PyQt6.QtWidgets import QApplication
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Line plot is displayed in this example.
 """
 app = QApplication(sys.argv)
 running = True
 
 plot_widget = LivePlotWidget(title="Line Plot @ 100Hz")
 plot_curve = LiveLinePlot()
 plot_widget.addItem(plot_curve)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/__init__.py` & `pglive-0.6.3/pglive/examples_pyqt5/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/all_plot_types.py` & `pglive-0.6.3/pglive/examples_pyside2/all_plot_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Tuple
 
-import pglive.examples_pyqt5 as examples
+import pglive.examples_pyside2 as examples
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot, LiveVBarPlot, LiveLinePlot, LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example all plot types are displayed.
+All plot types are displayed in this example.
 """
 
 layout = pg.LayoutWidget()
 args = []
 plots: List[Tuple[str, LivePlotWidget]] = [
     ("Horizontal Bar Plot", LiveHBarPlot(bar_height=2, brush="blue", pen="blue")),
     ("Vertical Bar Plot", LiveVBarPlot(bar_width=2, brush="green", pen="green")),
@@ -27,9 +27,9 @@
     widget.addItem(plot)
     layout.addWidget(widget)
     args.append(DataConnector(plot, max_points=300, update_rate=50))
 
 layout.show()
 
 Thread(target=examples.sin_wave_generator, args=args).start()
-examples.app.exec()
+examples.app.exec_()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/axis.py` & `pglive-0.6.3/pglive/examples_pyqt5/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Line plot is displayed in this example.
 """
 connectors = []
 
 layout = pg.LayoutWidget()
 # Define Time plot
 left_axis = LiveAxis("left", axisPen="red", textPen="red")
 bottom_axis = LiveAxis("bottom", axisPen="green", textPen="green", **{Axis.TICK_FORMAT: Axis.TIME})
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/candlestick_plot.py` & `pglive-0.6.3/pglive/examples_pyqt5/scatter_plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+import pglive.examples_pyqt5 as examples
 import signal
 from threading import Thread
 
-import pglive.examples_pyqt5 as examples
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_candleStickPlot import LiveCandleStickPlot
+from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Scatter plot is displayed.
+Scatter plot is displayed in this example.
 """
-win = LivePlotWidget(title="Candlestick Plot @ 10Hz")
-plot = LiveCandleStickPlot()
+win = LivePlotWidget(title="Scatter Plot @ 100Hz")
+plot = LiveScatterPlot()
 win.addItem(plot)
 
-data_connector = DataConnector(plot, max_points=50, update_rate=10)
+data_connector = DataConnector(plot, max_points=600)
 
 win.show()
 
-Thread(target=examples.candle_generator, args=(data_connector,)).start()
+Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
 examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/categorized_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyqt5/categorized_bar_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_categorized_bar_plot import LiveCategorizedBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Categorized Bar plot is displayed.
+Categorized Bar plot is displayed in this example.
 """
 categories = ["On", "Off", "Idle", "Warning", "Failure"]
 plot = LiveCategorizedBarPlot(categories,
                               category_color={"Failure": "r", "Warning": "orange", "Off": "silver", "Idle": "blue"})
 # Make sure to give plot.categories to Axis.CATEGORIES param (it's dynamic list)
 # If you're using static categories and your data won't yield not listed category you can use static categories list
 left_axis = LiveAxis("left", **{Axis.TICK_FORMAT: Axis.CATEGORY, Axis.CATEGORIES: plot.categories})
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/crop_offset_to_data.py` & `pglive-0.6.3/pglive/examples_pyqt5/crop_offset_to_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import pyqtgraph as pg   # type: ignore
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example live axis range crop offset to data is displayed.
+Range crop offset to data is displayed In this example.
 """
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
 
 '''
-We want to display view 30 seconds long and pan right every 1 second. 
+We want to display 30 seconds long view and pan right every 1 second. 
 '''
 widget = LivePlotWidget(title="Roll plot view every 1 sec, offset 30 sec, crop left = False",
                         x_range_controller=LiveAxisRange(roll_on_tick=100, offset_left=30),
                         y_range_controller=LiveAxisRange(fixed_range=[-1, 1]))
 plot = LiveLinePlot(pen="red")
 widget.addItem(plot)
 layout.addWidget(widget, row=0, col=0)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/crosshair.py` & `pglive-0.6.3/pglive/examples_pyqt5/crosshair.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pglive.kwargs import Crosshair
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, we create plot with Crosshair.
+We create plot with Crosshair in this example.
 Crosshair has few signals implemented:
     sig_crosshair_moved - fired when crosshair is moved within plot area
     sig_crosshair_out - fired when crosshair leaves plot area
     sig_crosshair_in - fired when crosshair enters plot area
 There are three text labels displayed below plot showing crosshair status, X and Y value.
 """
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/designer_example/main_example.py` & `pglive-0.6.3/pglive/examples_pyqt5/designer_example/main_example.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/designer_example/win_template.py` & `pglive-0.6.3/pglive/examples_pyqt5/designer_example/win_template.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/designer_example/win_template.ui` & `pglive-0.6.3/pglive/examples_pyqt5/designer_example/win_template.ui`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/horizontal_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyqt5/horizontal_bar_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Horizontal Bar plot is displayed.
+Horizontal Bar plot is displayed in this example.
 """
 win = LivePlotWidget(title="Horizontal Bar Plot @ 100Hz")
 plot = LiveHBarPlot(bar_height=1, brush="green", pen="green")
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
 win.show()
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/leading_line.py` & `pglive-0.6.3/pglive/examples_pyside6/leading_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pglive.examples_pyqt5 as examples
+import pglive.examples_pyside6 as examples
 from pyqtgraph import mkPen  # type: ignore
 
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.kwargs import LeadingLine
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot, LiveScatterPlot, LiveHBarPlot, LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example leading line is displayed.
+Leading line is displayed in this example.
 Pglive can plot Vertical or Horizontal leading line.
 User can choose orientation and which value is displayed by using text_axis parameter.
 Please note, that X might be swapped with Y, when plotting horizontally or vertically.
 Color of leading line is set with pen parameter.
 """
 
 layout = pg.LayoutWidget()
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/line_plot.py` & `pglive-0.6.3/pglive/examples_pyqt5/line_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Line plot is displayed in this example.
 """
 win = LivePlotWidget(title="Line Plot @ 100Hz")
 plot = LiveLinePlot()
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/live_plot_range.py` & `pglive-0.6.3/pglive/examples_pyqt5/live_plot_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example live plot range is used to increase plotting performance.
+Live plot range is used to increase plotting performance in this example.
 """
 
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
 args = []
 args2 = []
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py` & `pglive-0.6.3/pglive/examples_pyqt5/one_plot_multiple_plot_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example we are plotting two signals in one plot with different plot_rate.
+We are plotting two signals in one plot with different plot_rate in this example.
 Since LiveAxisRange is calculating range from plot_rate, it might result in unwanted results.
 You can use ignore_auto_range flag for DataConnector.
 If it's set to True, this DataConnector is not causing change of range.
 You can in fact use it to all LiveAxisRanges and implement your own custom Range calculation.
 """
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/pause_resume.py` & `pglive-0.6.3/pglive/examples_pyside6/pause_resume.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import pglive.examples_pyqt5 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
-from PyQt5.QtWidgets import QWidget, QGridLayout, QPushButton, QLabel
+from PySide6.QtWidgets import QWidget, QGridLayout, QPushButton, QLabel
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Pause and Resume functionality of DataConnector is demonstrated.
+Pause and Resume functionality of DataConnector is demonstrated in this example.
 There are two buttons, that pause and resume live plotting.
 When Live plot is paused, data are not collected.
 """
 # Create parent widget
 widget = LivePlotWidget(title="Line Plot @ 100Hz")
 plot = LiveScatterPlot()
 widget.addItem(plot)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/plot_rate.py` & `pglive-0.6.3/pglive/examples_pyqt6/plot_rate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import pglive.examples_pyqt5 as examples
+import pglive.examples_pyqt6 as examples
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, different plot rate is demonstrated.
+Different plot rate is demonstrated in this example.
 Display four plots, each slower by 1/4 of previous plot rate.
 Plot rate is set in Hz unit.
 """
 layout = pg.LayoutWidget()
 args = []
-# Initial rate of 100Hz
+# Initial plot rate of 100Hz
 plot_rate = 100.
 max_len = 600
 # Initial delta Y is 1
 bar_height = 1
 for index in range(4):
     widget = LivePlotWidget(title=f"Horizontal Bar Plot @ {plot_rate}Hz")
     plot = LiveHBarPlot(bar_height=bar_height, brush="green", pen="green")
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/scatter_plot.py` & `pglive-0.6.3/pglive/examples_pyside6/scatter_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import pglive.examples_pyqt5 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Scatter plot is displayed.
+Scatter plot is displayed in this example.
 """
 win = LivePlotWidget(title="Scatter Plot @ 100Hz")
 plot = LiveScatterPlot()
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/update_rate.py` & `pglive-0.6.3/pglive/examples_pyqt5/update_rate.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, different update rate is demonstrated.
+Different update rate is demonstrated in this example.
 Display four plots, each slower by 1/4 of previous update rate.
 Update rate is set in Hz unit.
 """
 layout = pg.LayoutWidget()
 args = []
 # Initial rate of 100Hz
 update_rate = 100.
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/vertical_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyqt5/vertical_bar_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Vertical Bar plot is displayed.
+Vertical Bar plot is displayed in this example.
 """
 win = LivePlotWidget(title="Vertical Bar Plot @ 100Hz")
 plot = LiveVBarPlot(bar_width=1, brush="blue", pen="blue")
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt5/vertical_bar_plot_color.py` & `pglive-0.6.3/pglive/examples_pyqt5/vertical_bar_plot_color.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from time import sleep
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Vertical Bar plot is displayed.
+Vertical Bar plot is displayed in this example.
 Every update bar color is changed as well.
 """
 win = LivePlotWidget(title="Coloured Vertical Bar Plot @ 100Hz")
 plot = LiveVBarPlot(bar_width=1)
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/__init__.py` & `pglive-0.6.3/pglive/examples_pyqt6/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/all_plot_types.py` & `pglive-0.6.3/pglive/examples_pyside6/all_plot_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from threading import Thread
 from typing import List, Tuple
 
-import pglive.examples_pyqt6 as examples
+import pglive.examples_pyside6 as examples
+from threading import Thread
+
 import pyqtgraph as pg  # type: ignore
+
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_plot import LiveVBarPlot, LiveLinePlot, LiveScatterPlot, LiveHBarPlot
+from pglive.sources.live_plot import LiveHBarPlot, LiveVBarPlot, LiveLinePlot, LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example all plot types are displayed.
+All plot types are displayed in this example.
 """
 
 layout = pg.LayoutWidget()
 args = []
 plots: List[Tuple[str, LivePlotWidget]] = [
     ("Horizontal Bar Plot", LiveHBarPlot(bar_height=2, brush="blue", pen="blue")),
     ("Vertical Bar Plot", LiveVBarPlot(bar_width=2, brush="green", pen="green")),
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/axis.py` & `pglive-0.6.3/pglive/examples_pyqt6/axis.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Line plot is displayed in this example.
 """
 connectors = []
 
 layout = pg.LayoutWidget()
 # Define Time plot
 left_axis = LiveAxis("left", axisPen="red", textPen="red")
 bottom_axis = LiveAxis("bottom", axisPen="green", textPen="green", **{Axis.TICK_FORMAT: Axis.TIME})
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/candlestick_plot.py` & `pglive-0.6.3/pglive/examples_pyside2/scatter_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+import pglive.examples_pyside2 as examples
 import signal
 from threading import Thread
 
-import pglive.examples_pyqt6 as examples
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_candleStickPlot import LiveCandleStickPlot
+from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Scatter plot is displayed.
+Scatter plot is displayed in this example.
 """
-win = LivePlotWidget(title="Candlestick Plot @ 10Hz")
-plot = LiveCandleStickPlot()
+win = LivePlotWidget(title="Scatter Plot @ 100Hz")
+plot = LiveScatterPlot()
 win.addItem(plot)
 
-data_connector = DataConnector(plot, max_points=50, update_rate=10)
+data_connector = DataConnector(plot, max_points=600)
 
 win.show()
 
-Thread(target=examples.candle_generator, args=(data_connector,)).start()
+Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec()
+examples.app.exec_()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/categorized_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyside6/categorized_bar_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import signal
 from threading import Thread
 
-import pglive.examples_pyqt6 as examples
+import pglive.examples_pyside6 as examples
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_categorized_bar_plot import LiveCategorizedBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Categorized Bar plot is displayed.
+Categorized Bar plot is displayed in this example.
 """
 categories = ["On", "Off", "Idle", "Warning", "Failure"]
 plot = LiveCategorizedBarPlot(categories,
                               category_color={"Failure": "r", "Warning": "orange", "Off": "silver", "Idle": "blue"})
 # Make sure to give plot.categories to Axis.CATEGORIES param (it's dynamic list)
 # If you're using static categories and your data won't yield not listed category you can use static categories list
 left_axis = LiveAxis("left", **{Axis.TICK_FORMAT: Axis.CATEGORY, Axis.CATEGORIES: plot.categories})
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/crop_offset_to_data.py` & `pglive-0.6.3/pglive/examples_pyqt6/crop_offset_to_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import pyqtgraph as pg  # type: ignore
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example live axis range crop offset to data is displayed.
+Range crop offset to data is displayed In this example.
 """
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
 
 '''
-We want to display view 30 seconds long and pan right every 1 second. 
+We want to display 30 seconds long view and pan right every 1 second.
 '''
 widget = LivePlotWidget(title="Roll plot view every 1 sec, offset 30 sec, crop left = False",
                         x_range_controller=LiveAxisRange(roll_on_tick=100, offset_left=30),
                         y_range_controller=LiveAxisRange(fixed_range=[-1, 1]))
 plot = LiveLinePlot(pen="red")
 widget.addItem(plot)
 layout.addWidget(widget, row=0, col=0)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/crosshair.py` & `pglive-0.6.3/pglive/examples_pyqt6/crosshair.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pglive.kwargs import Crosshair
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, we create plot with Crosshair.
+We create plot with Crosshair in this example.
 Crosshair has few signals implemented:
     sig_crosshair_moved - fired when crosshair is moved within plot area
     sig_crosshair_out - fired when crosshair leaves plot area
     sig_crosshair_in - fired when crosshair enters plot area
 There are three text labels displayed below plot showing crosshair status, X and Y value.
 """
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/designer_example/main_example.py` & `pglive-0.6.3/pglive/examples_pyqt6/designer_example/main_example.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/designer_example/win_template.py` & `pglive-0.6.3/pglive/examples_pyqt6/designer_example/win_template.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/designer_example/win_template.ui` & `pglive-0.6.3/pglive/examples_pyqt6/designer_example/win_template.ui`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/horizontal_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyqt6/horizontal_bar_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pglive.examples_pyqt6 as examples
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Horizontal Bar plot is displayed.
+Horizontal Bar plot is displayed in this example.
 """
 win = LivePlotWidget(title="Horizontal Bar Plot @ 100Hz")
 plot = LiveHBarPlot(bar_height=1, brush="green", pen="green")
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
 win.show()
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/leading_line.py` & `pglive-0.6.3/pglive/examples_pyqt5/leading_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pglive.examples_pyqt6 as examples
+import pglive.examples_pyqt5 as examples
 from pyqtgraph import mkPen  # type: ignore
 
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.kwargs import LeadingLine
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot, LiveScatterPlot, LiveHBarPlot, LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example leading line is displayed.
+Leading line is displayed in this example.
 Pglive can plot Vertical or Horizontal leading line.
 User can choose orientation and which value is displayed by using text_axis parameter.
 Please note, that X might be swapped with Y, when plotting horizontally or vertically.
 Color of leading line is set with pen parameter.
 """
 
 layout = pg.LayoutWidget()
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/line_plot.py` & `pglive-0.6.3/pglive/examples_pyqt6/line_plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Line plot is displayed in this example.
 """
 win = LivePlotWidget(title="Line Plot @ 100Hz")
 plot = LiveLinePlot()
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/live_plot_range.py` & `pglive-0.6.3/pglive/examples_pyqt6/live_plot_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example live plot range is used to increase plotting performance.
+Live plot range is used to increase plotting performance in this example.
 """
 
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
 args = []
 args2 = []
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py` & `pglive-0.6.3/pglive/examples_pyqt6/one_plot_multiple_plot_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example we are plotting two signals in one plot with different plot_rate.
+We are plotting two signals in one plot with different plot_rate in this example.
 Since LiveAxisRange is calculating range from plot_rate, it might result in unwanted results.
 You can use ignore_auto_range flag for DataConnector.
 If it's set to True, this DataConnector is not causing change of range.
 You can in fact use it to all LiveAxisRanges and implement your own custom Range calculation.
 """
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/pause_resume.py` & `pglive-0.6.3/pglive/examples_pyqt6/pause_resume.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from PyQt6.QtWidgets import QWidget, QGridLayout, QPushButton, QLabel
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Pause and Resume functionality of DataConnector is demonstrated.
+Pause and Resume functionality of DataConnector is demonstrated in this example.
 There are two buttons, that pause and resume live plotting.
 When Live plot is paused, data are not collected.
 """
 # Create parent widget
 widget = LivePlotWidget(title="Line Plot @ 100Hz")
 plot = LiveScatterPlot()
 widget.addItem(plot)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/plot_rate.py` & `pglive-0.6.3/pglive/examples_pyside6/plot_rate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import pglive.examples_pyqt6 as examples
+import pglive.examples_pyside6 as examples
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, different plot rate is demonstrated.
+Different plot rate is demonstrated in this example.
 Display four plots, each slower by 1/4 of previous plot rate.
 Plot rate is set in Hz unit.
 """
 layout = pg.LayoutWidget()
 args = []
-# Initial plot rate of 100Hz
+# Initial rate of 100Hz
 plot_rate = 100.
 max_len = 600
 # Initial delta Y is 1
 bar_height = 1
 for index in range(4):
     widget = LivePlotWidget(title=f"Horizontal Bar Plot @ {plot_rate}Hz")
     plot = LiveHBarPlot(bar_height=bar_height, brush="green", pen="green")
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/scatter_plot.py` & `pglive-0.6.3/pglive/examples_pyqt6/scatter_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Scatter plot is displayed.
+Scatter plot is displayed in this example.
 """
 win = LivePlotWidget(title="Scatter Plot @ 100Hz")
 plot = LiveScatterPlot()
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/update_rate.py` & `pglive-0.6.3/pglive/examples_pyqt6/update_rate.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, different update rate is demonstrated.
+Different update rate is demonstrated in this example.
 Display four plots, each slower by 1/4 of previous update rate.
 Update rate is set in Hz unit.
 """
 layout = pg.LayoutWidget()
 args = []
 # Initial rate of 100Hz
 update_rate = 100.
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/vertical_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyqt6/vertical_bar_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Vertical Bar plot is displayed.
+Vertical Bar plot is displayed in this example.
 """
 win = LivePlotWidget(title="Vertical Bar Plot @ 100Hz")
 plot = LiveVBarPlot(bar_width=1, brush="blue", pen="blue")
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
```

### Comparing `pglive-0.6.2/pglive/examples_pyqt6/vertical_bar_plot_color.py` & `pglive-0.6.3/pglive/examples_pyside2/vertical_bar_plot_color.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import pglive.examples_pyqt6 as examples
+import pglive.examples_pyside2 as examples
 import signal
 from math import sin
 from threading import Thread
 from time import sleep
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Vertical Bar plot is displayed.
+Vertical Bar plot is displayed in this example.
 Every update bar color is changed as well.
 """
 win = LivePlotWidget(title="Coloured Vertical Bar Plot @ 100Hz")
 plot = LiveVBarPlot(bar_width=1)
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
@@ -30,9 +30,9 @@
         sleep(0.01)
 
 
 win.show()
 
 Thread(target=sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec()
+examples.app.exec_()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/__init__.py` & `pglive-0.6.3/pglive/examples_pyside2/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyside2/all_plot_types.py` & `pglive-0.6.3/pglive/examples_pyqt5/all_plot_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Tuple
 
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyqt5 as examples
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot, LiveVBarPlot, LiveLinePlot, LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example all plot types are displayed.
+All basic plot types are displayed in this example.
 """
 
 layout = pg.LayoutWidget()
 args = []
 plots: List[Tuple[str, LivePlotWidget]] = [
     ("Horizontal Bar Plot", LiveHBarPlot(bar_height=2, brush="blue", pen="blue")),
     ("Vertical Bar Plot", LiveVBarPlot(bar_width=2, brush="green", pen="green")),
@@ -27,9 +27,9 @@
     widget.addItem(plot)
     layout.addWidget(widget)
     args.append(DataConnector(plot, max_points=300, update_rate=50))
 
 layout.show()
 
 Thread(target=examples.sin_wave_generator, args=args).start()
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/axis.py` & `pglive-0.6.3/pglive/examples_pyside6/axis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 import time
 from math import sin
 from threading import Thread
 from time import sleep
 
 import pyqtgraph as pg  # type: ignore
@@ -10,15 +10,15 @@
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Line plot is displayed in this example.
 """
 connectors = []
 
 layout = pg.LayoutWidget()
 # Define Time plot
 left_axis = LiveAxis("left", axisPen="red", textPen="red")
 bottom_axis = LiveAxis("bottom", axisPen="green", textPen="green", **{Axis.TICK_FORMAT: Axis.TIME})
@@ -51,9 +51,9 @@
         for data_connector in data_connectors:
             data_connector.cb_append_data_point(sin(x * 0.01), time.time())
         sleep(0.01)
 
 
 Thread(target=sin_wave_generator, args=connectors).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/candlestick_plot.py` & `pglive-0.6.3/pglive/examples_pyside6/horizontal_bar_plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import signal
+import pglive.examples_pyside6 as examples
 from threading import Thread
 
-import pglive.examples_pyside2 as examples
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_candleStickPlot import LiveCandleStickPlot
+from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Scatter plot is displayed.
+Horizontal Bar plot is displayed in this example.
 """
-win = LivePlotWidget(title="Candlestick Plot @ 10Hz")
-plot = LiveCandleStickPlot()
+win = LivePlotWidget(title="Horizontal Bar Plot @ 100Hz")
+plot = LiveHBarPlot(bar_height=1, brush="green", pen="green")
 win.addItem(plot)
 
-data_connector = DataConnector(plot, max_points=50, update_rate=10)
-
+data_connector = DataConnector(plot, max_points=600)
 win.show()
 
-Thread(target=examples.candle_generator, args=(data_connector,)).start()
-signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/categorized_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyside2/categorized_bar_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_categorized_bar_plot import LiveCategorizedBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Categorized Bar plot is displayed.
+Categorized Bar plot is displayed in this example.
 """
 categories = ["On", "Off", "Idle", "Warning", "Failure"]
 plot = LiveCategorizedBarPlot(categories,
                               category_color={"Failure": "r", "Warning": "orange", "Off": "silver", "Idle": "blue"})
 # Make sure to give plot.categories to Axis.CATEGORIES param (it's dynamic list)
 # If you're using static categories and your data won't yield not listed category you can use static categories list
 left_axis = LiveAxis("left", **{Axis.TICK_FORMAT: Axis.CATEGORY, Axis.CATEGORIES: plot.categories})
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/crop_offset_to_data.py` & `pglive-0.6.3/pglive/examples_pyside2/crop_offset_to_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import pyqtgraph as pg  # type: ignore
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example live axis range crop offset to data is displayed.
+Range crop offset to data is displayed In this example.
 """
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
 
 '''
-We want to display view 30 seconds long and pan right every 1 second. 
+We want to display 30 seconds long view and pan right every 1 second.
 '''
 widget = LivePlotWidget(title="Roll plot view every 1 sec, offset 30 sec, crop left = False",
                         x_range_controller=LiveAxisRange(roll_on_tick=100, offset_left=30),
                         y_range_controller=LiveAxisRange(fixed_range=[-1, 1]))
 plot = LiveLinePlot(pen="red")
 widget.addItem(plot)
 layout.addWidget(widget, row=0, col=0)
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/crosshair.py` & `pglive-0.6.3/pglive/examples_pyside2/crosshair.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pglive.kwargs import Crosshair
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, we create plot with Crosshair.
+We create plot with Crosshair in this example.
 Crosshair has few signals implemented:
     sig_crosshair_moved - fired when crosshair is moved within plot area
     sig_crosshair_out - fired when crosshair leaves plot area
     sig_crosshair_in - fired when crosshair enters plot area
 There are three text labels displayed below plot showing crosshair status, X and Y value.
 """
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/horizontal_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyside6/line_plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
+import signal
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_plot import LiveHBarPlot
+from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Horizontal Bar plot is displayed.
+Line plot is displayed in this example.
 """
-win = LivePlotWidget(title="Horizontal Bar Plot @ 100Hz")
-plot = LiveHBarPlot(bar_height=1, brush="green", pen="green")
+win = LivePlotWidget(title="Line Plot @ 100Hz")
+plot = LiveLinePlot()
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
+
 win.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
-examples.app.exec_()
+signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/leading_line.py` & `pglive-0.6.3/pglive/examples_pyside2/leading_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from pglive.kwargs import LeadingLine
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot, LiveScatterPlot, LiveHBarPlot, LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example leading line is displayed.
+Leading line is displayed in this example.
 Pglive can plot Vertical or Horizontal leading line.
 User can choose orientation and which value is displayed by using text_axis parameter.
 Please note, that X might be swapped with Y, when plotting horizontally or vertically.
 Color of leading line is set with pen parameter.
 """
 
 layout = pg.LayoutWidget()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/line_plot.py` & `pglive-0.6.3/pglive/examples_pyside2/line_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Line plot is displayed in this example.
 """
 win = LivePlotWidget(title="Line Plot @ 100Hz")
 plot = LiveLinePlot()
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/live_plot_range.py` & `pglive-0.6.3/pglive/examples_pyside6/live_plot_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example live plot range is used to increase plotting performance.
+Live plot range is used to increase plotting performance in this example.
 """
 
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
 args = []
 args2 = []
 
@@ -148,9 +148,9 @@
 # ---
 
 layout.show()
 Thread(target=examples.sin_wave_generator, args=args).start()
 Thread(target=examples.sin_wave_generator, args=args2, kwargs={"flip": True}).start()
 
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/one_plot_multiple_plot_rates.py` & `pglive-0.6.3/pglive/examples_pyside2/one_plot_multiple_plot_rates.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example we are plotting two signals in one plot with different plot_rate.
+We are plotting two signals in one plot with different plot_rate in this example.
 Since LiveAxisRange is calculating range from plot_rate, it might result in unwanted results.
 You can use ignore_auto_range flag for DataConnector.
 If it's set to True, this DataConnector is not causing change of range.
 You can in fact use it to all LiveAxisRanges and implement your own custom Range calculation.
 """
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/pause_resume.py` & `pglive-0.6.3/pglive/examples_pyside2/pause_resume.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from PySide2.QtWidgets import QWidget, QGridLayout, QPushButton, QLabel
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Pause and Resume functionality of DataConnector is demonstrated.
+Pause and Resume functionality of DataConnector is demonstrated in this example.
 There are two buttons, that pause and resume live plotting.
 When Live plot is paused, data are not collected.
 """
 # Create parent widget
 widget = LivePlotWidget(title="Line Plot @ 100Hz")
 plot = LiveScatterPlot()
 widget.addItem(plot)
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/plot_rate.py` & `pglive-0.6.3/pglive/examples_pyside2/plot_rate.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, different plot rate is demonstrated.
+Different plot rate is demonstrated in this example.
 Display four plots, each slower by 1/4 of previous plot rate.
 Plot rate is set in Hz unit.
 """
 layout = pg.LayoutWidget()
 args = []
 # Initial rate of 100Hz
 plot_rate = 100.
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/scatter_plot.py` & `pglive-0.6.3/pglive/examples_pyside2/vertical_bar_plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pglive.examples_pyside2 as examples
 import signal
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_plot import LiveScatterPlot
+from pglive.sources.live_plot import LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Scatter plot is displayed.
+Vertical Bar plot is displayed in this example.
 """
-win = LivePlotWidget(title="Scatter Plot @ 100Hz")
-plot = LiveScatterPlot()
+win = LivePlotWidget(title="Vertical Bar Plot @ 100Hz")
+plot = LiveVBarPlot(bar_width=1, brush="blue", pen="blue")
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
 
 win.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/update_rate.py` & `pglive-0.6.3/pglive/examples_pyside2/update_rate.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, different update rate is demonstrated.
+Different update rate is demonstrated in this example.
 Display four plots, each slower by 1/4 of previous update rate.
 Update rate is set in Hz unit.
 """
 layout = pg.LayoutWidget()
 args = []
 # Initial rate of 100Hz
 update_rate = 100.
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/vertical_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyside6/vertical_bar_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Vertical Bar plot is displayed.
+Vertical Bar plot is displayed in this example.
 """
 win = LivePlotWidget(title="Vertical Bar Plot @ 100Hz")
 plot = LiveVBarPlot(bar_width=1, brush="blue", pen="blue")
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
 
 win.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside2/vertical_bar_plot_color.py` & `pglive-0.6.3/pglive/examples_pyside6/vertical_bar_plot_color.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import pglive.examples_pyside2 as examples
+import pglive.examples_pyside6 as examples
 import signal
 from math import sin
 from threading import Thread
 from time import sleep
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Vertical Bar plot is displayed.
+Vertical Bar plot is displayed in this example.
 Every update bar color is changed as well.
 """
 win = LivePlotWidget(title="Coloured Vertical Bar Plot @ 100Hz")
 plot = LiveVBarPlot(bar_width=1)
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
@@ -30,9 +30,9 @@
         sleep(0.01)
 
 
 win.show()
 
 Thread(target=sin_wave_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec_()
+examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/__init__.py` & `pglive-0.6.3/pglive/examples_pyside6/__init__.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/examples_pyside6/all_plot_types.py` & `pglive-0.6.3/pglive/examples_pyqt6/all_plot_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from typing import List, Tuple
-
-import pglive.examples_pyside6 as examples
 from threading import Thread
+from typing import List, Tuple
 
+import pglive.examples_pyqt6 as examples
 import pyqtgraph as pg  # type: ignore
-
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_plot import LiveHBarPlot, LiveVBarPlot, LiveLinePlot, LiveScatterPlot
+from pglive.sources.live_plot import LiveVBarPlot, LiveLinePlot, LiveScatterPlot, LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example all plot types are displayed.
+All basic plot types are displayed in this example.
 """
 
 layout = pg.LayoutWidget()
 args = []
 plots: List[Tuple[str, LivePlotWidget]] = [
     ("Horizontal Bar Plot", LiveHBarPlot(bar_height=2, brush="blue", pen="blue")),
     ("Vertical Bar Plot", LiveVBarPlot(bar_width=2, brush="green", pen="green")),
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/axis.py` & `pglive-0.6.3/pglive/examples_pyside2/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pglive.examples_pyside6 as examples
+import pglive.examples_pyside2 as examples
 import signal
 import time
 from math import sin
 from threading import Thread
 from time import sleep
 
 import pyqtgraph as pg  # type: ignore
@@ -10,15 +10,15 @@
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Line plot is displayed in this example.
 """
 connectors = []
 
 layout = pg.LayoutWidget()
 # Define Time plot
 left_axis = LiveAxis("left", axisPen="red", textPen="red")
 bottom_axis = LiveAxis("bottom", axisPen="green", textPen="green", **{Axis.TICK_FORMAT: Axis.TIME})
@@ -51,9 +51,9 @@
         for data_connector in data_connectors:
             data_connector.cb_append_data_point(sin(x * 0.01), time.time())
         sleep(0.01)
 
 
 Thread(target=sin_wave_generator, args=connectors).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec()
+examples.app.exec_()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/candlestick_plot.py` & `pglive-0.6.3/pglive/examples_pyside2/candlestick_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import signal
 from threading import Thread
 
-import pglive.examples_pyside6 as examples
+import pglive.examples_pyside2 as examples
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_candleStickPlot import LiveCandleStickPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Scatter plot is displayed.
+Candlestick Bar plot is displayed in this example.
 """
 win = LivePlotWidget(title="Candlestick Plot @ 10Hz")
 plot = LiveCandleStickPlot()
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=50, update_rate=10)
 
 win.show()
 
 Thread(target=examples.candle_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec()
+examples.app.exec_()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/categorized_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyqt6/categorized_bar_plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import signal
 from threading import Thread
 
-import pglive.examples_pyside6 as examples
+import pglive.examples_pyqt6 as examples
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_categorized_bar_plot import LiveCategorizedBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Categorized Bar plot is displayed.
+Categorized Bar plot is displayed in this example.
 """
 categories = ["On", "Off", "Idle", "Warning", "Failure"]
 plot = LiveCategorizedBarPlot(categories,
                               category_color={"Failure": "r", "Warning": "orange", "Off": "silver", "Idle": "blue"})
 # Make sure to give plot.categories to Axis.CATEGORIES param (it's dynamic list)
 # If you're using static categories and your data won't yield not listed category you can use static categories list
 left_axis = LiveAxis("left", **{Axis.TICK_FORMAT: Axis.CATEGORY, Axis.CATEGORIES: plot.categories})
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/crop_offset_to_data.py` & `pglive-0.6.3/pglive/examples_pyside6/crop_offset_to_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import pyqtgraph as pg  # type: ignore
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example live axis range crop offset to data is displayed.
+Range crop offset to data is displayed In this example.
 """
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
 
 '''
-We want to display view 30 seconds long and pan right every 1 second. 
+We want to display 30 seconds long view and pan right every 1 second.
 '''
 widget = LivePlotWidget(title="Roll plot view every 1 sec, offset 30 sec, crop left = False",
                         x_range_controller=LiveAxisRange(roll_on_tick=100, offset_left=30),
                         y_range_controller=LiveAxisRange(fixed_range=[-1, 1]))
 plot = LiveLinePlot(pen="red")
 widget.addItem(plot)
 layout.addWidget(widget, row=0, col=0)
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/crosshair.py` & `pglive-0.6.3/pglive/examples_pyside6/crosshair.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pglive.kwargs import Crosshair
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, we create plot with Crosshair.
+We create plot with Crosshair in this example.
 Crosshair has few signals implemented:
     sig_crosshair_moved - fired when crosshair is moved within plot area
     sig_crosshair_out - fired when crosshair leaves plot area
     sig_crosshair_in - fired when crosshair enters plot area
 There are three text labels displayed below plot showing crosshair status, X and Y value.
 """
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/horizontal_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyside2/horizontal_bar_plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import pglive.examples_pyside6 as examples
+import pglive.examples_pyside2 as examples
 from threading import Thread
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Horizontal Bar plot is displayed.
+Horizontal Bar plot is displayed in this example.
 """
 win = LivePlotWidget(title="Horizontal Bar Plot @ 100Hz")
 plot = LiveHBarPlot(bar_height=1, brush="green", pen="green")
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
 win.show()
 
 Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
-examples.app.exec()
+examples.app.exec_()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/leading_line.py` & `pglive-0.6.3/pglive/examples_pyqt6/leading_line.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pglive.examples_pyside6 as examples
+import pglive.examples_pyqt6 as examples
 from pyqtgraph import mkPen  # type: ignore
 
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.kwargs import LeadingLine
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot, LiveScatterPlot, LiveHBarPlot, LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example leading line is displayed.
+Leading line is displayed in this example.
 Pglive can plot Vertical or Horizontal leading line.
 User can choose orientation and which value is displayed by using text_axis parameter.
 Please note, that X might be swapped with Y, when plotting horizontally or vertically.
 Color of leading line is set with pen parameter.
 """
 
 layout = pg.LayoutWidget()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/line_plot.py` & `pglive-0.6.3/pglive/examples_pyside6/candlestick_plot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
+import pglive.examples_pyside6 as examples
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_plot import LiveLinePlot
+from pglive.sources.live_candleStickPlot import LiveCandleStickPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Candlestick Bar plot is displayed in this example.
 """
-win = LivePlotWidget(title="Line Plot @ 100Hz")
-plot = LiveLinePlot()
+win = LivePlotWidget(title="Candlestick Plot @ 10Hz")
+plot = LiveCandleStickPlot()
 win.addItem(plot)
 
-data_connector = DataConnector(plot, max_points=600)
+data_connector = DataConnector(plot, max_points=50, update_rate=10)
 
 win.show()
 
-Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
+Thread(target=examples.candle_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
 examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/live_plot_range.py` & `pglive-0.6.3/pglive/examples_pyside2/live_plot_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pglive.examples_pyside6 as examples
+import pglive.examples_pyside2 as examples
 import signal
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 from pglive.kwargs import Axis
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example live plot range is used to increase plotting performance.
+Live plot range is used to increase plotting performance in this example.
 """
 
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
 args = []
 args2 = []
 
@@ -148,9 +148,9 @@
 # ---
 
 layout.show()
 Thread(target=examples.sin_wave_generator, args=args).start()
 Thread(target=examples.sin_wave_generator, args=args2, kwargs={"flip": True}).start()
 
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
-examples.app.exec()
+examples.app.exec_()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/one_plot_multiple_plot_rates.py` & `pglive-0.6.3/pglive/examples_pyside6/one_plot_multiple_plot_rates.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_axis_range import LiveAxisRange
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example we are plotting two signals in one plot with different plot_rate.
+We are plotting two signals in one plot with different plot_rate in this example.
 Since LiveAxisRange is calculating range from plot_rate, it might result in unwanted results.
 You can use ignore_auto_range flag for DataConnector.
 If it's set to True, this DataConnector is not causing change of range.
 You can in fact use it to all LiveAxisRanges and implement your own custom Range calculation.
 """
 layout = pg.LayoutWidget()
 layout.layout.setSpacing(0)
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/pause_resume.py` & `pglive-0.6.3/pglive/examples_pyqt5/pause_resume.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import pglive.examples_pyside6 as examples
+import pglive.examples_pyqt5 as examples
 import signal
 from threading import Thread
 
-from PySide6.QtWidgets import QWidget, QGridLayout, QPushButton, QLabel
+from PyQt5.QtWidgets import QWidget, QGridLayout, QPushButton, QLabel
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveScatterPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Pause and Resume functionality of DataConnector is demonstrated.
+Pause and Resume functionality of DataConnector is demonstrated in this example.
 There are two buttons, that pause and resume live plotting.
 When Live plot is paused, data are not collected.
 """
 # Create parent widget
 widget = LivePlotWidget(title="Line Plot @ 100Hz")
 plot = LiveScatterPlot()
 widget.addItem(plot)
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/plot_rate.py` & `pglive-0.6.3/pglive/examples_pyside6/update_rate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import pglive.examples_pyside6 as examples
+from math import ceil
 from threading import Thread
 
 import pyqtgraph as pg  # type: ignore
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveHBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example, different plot rate is demonstrated.
-Display four plots, each slower by 1/4 of previous plot rate.
-Plot rate is set in Hz unit.
+Different update rate is demonstrated in this example.
+Display four plots, each slower by 1/4 of previous update rate.
+Update rate is set in Hz unit.
 """
 layout = pg.LayoutWidget()
 args = []
 # Initial rate of 100Hz
-plot_rate = 100.
-max_len = 600
+update_rate = 100.
+max_len = 600.
 # Initial delta Y is 1
 bar_height = 1
 for index in range(4):
-    widget = LivePlotWidget(title=f"Horizontal Bar Plot @ {plot_rate}Hz")
+    widget = LivePlotWidget(title=f"Horizontal Bar Plot @ {update_rate}Hz")
     plot = LiveHBarPlot(bar_height=bar_height, brush="green", pen="green")
     widget.addItem(plot)
     layout.addWidget(widget)
-    args.append(DataConnector(plot, max_points=max_len, plot_rate=plot_rate))
-    plot_rate /= 4.
+    args.append(DataConnector(plot, max_points=ceil(max_len), update_rate=update_rate))
+    # divide all important parameters by 4
+    update_rate /= 4.
+    max_len /= 4.
+    # bar height depends on Y distance, that's why we should multiply it by 4
+    # if we leave it at 1, we get smaller bars
+    bar_height *= 4
 
 layout.show()
 
 Thread(target=examples.sin_wave_generator, args=args).start()
 examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/scatter_plot.py` & `pglive-0.6.3/pglive/examples_pyqt5/candlestick_plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
+import pglive.examples_pyqt5 as examples
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_plot import LiveScatterPlot
+from pglive.sources.live_candleStickPlot import LiveCandleStickPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Scatter plot is displayed.
+Candlestick Bar plot is displayed in this example.
 """
-win = LivePlotWidget(title="Scatter Plot @ 100Hz")
-plot = LiveScatterPlot()
+win = LivePlotWidget(title="Candlestick Plot @ 10Hz")
+plot = LiveCandleStickPlot()
 win.addItem(plot)
 
-data_connector = DataConnector(plot, max_points=600)
+data_connector = DataConnector(plot, max_points=50, update_rate=10)
 
 win.show()
 
-Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
+Thread(target=examples.candle_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
 examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/vertical_bar_plot.py` & `pglive-0.6.3/pglive/examples_pyqt6/candlestick_plot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import pglive.examples_pyside6 as examples
 import signal
 from threading import Thread
 
+import pglive.examples_pyqt6 as examples
 from pglive.sources.data_connector import DataConnector
-from pglive.sources.live_plot import LiveVBarPlot
+from pglive.sources.live_candleStickPlot import LiveCandleStickPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Vertical Bar plot is displayed.
+Candlestick Bar plot is displayed in this example.
 """
-win = LivePlotWidget(title="Vertical Bar Plot @ 100Hz")
-plot = LiveVBarPlot(bar_width=1, brush="blue", pen="blue")
+win = LivePlotWidget(title="Candlestick Plot @ 10Hz")
+plot = LiveCandleStickPlot()
 win.addItem(plot)
 
-data_connector = DataConnector(plot, max_points=600)
+data_connector = DataConnector(plot, max_points=50, update_rate=10)
 
 win.show()
 
-Thread(target=examples.sin_wave_generator, args=(data_connector,)).start()
+Thread(target=examples.candle_generator, args=(data_connector,)).start()
 signal.signal(signal.SIGINT, lambda sig, frame: examples.stop())
 examples.app.exec()
 examples.stop()
```

### Comparing `pglive-0.6.2/pglive/examples_pyside6/vertical_bar_plot_color.py` & `pglive-0.6.3/pglive/examples_pyqt6/vertical_bar_plot_color.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import pglive.examples_pyside6 as examples
+import pglive.examples_pyqt6 as examples
 import signal
 from math import sin
 from threading import Thread
 from time import sleep
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveVBarPlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Vertical Bar plot is displayed.
+Vertical Bar plot is displayed in this example.
 Every update bar color is changed as well.
 """
 win = LivePlotWidget(title="Coloured Vertical Bar Plot @ 100Hz")
 plot = LiveVBarPlot(bar_width=1)
 win.addItem(plot)
 
 data_connector = DataConnector(plot, max_points=600)
```

### Comparing `pglive-0.6.2/pglive/kwargs.py` & `pglive-0.6.3/pglive/kwargs.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/sources/data_connector.py` & `pglive-0.6.3/pglive/sources/data_connector.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/sources/live_axis.py` & `pglive-0.6.3/pglive/sources/live_axis.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/sources/live_axis_range.py` & `pglive-0.6.3/pglive/sources/live_axis_range.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/sources/live_candleStickPlot.py` & `pglive-0.6.3/pglive/sources/live_candleStickPlot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/sources/live_categorized_bar_plot.py` & `pglive-0.6.3/pglive/sources/live_categorized_bar_plot.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/sources/live_mixins.py` & `pglive-0.6.3/pglive/sources/live_mixins.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pglive/sources/live_plot.py` & `pglive-0.6.3/pglive/sources/live_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict, Any, Tuple, List
 
 import numpy as np  # type: ignore
 import pyqtgraph as pg  # type: ignore
-from numpy import ndarray
 
 from pglive.sources.live_mixins import MixinLivePlot, MixinLeadingLine, MixinLiveBarPlot
 
 
 class LiveLinePlot(pg.PlotDataItem, MixinLivePlot, MixinLeadingLine):
     """Line plot"""
 
@@ -35,15 +34,15 @@
         if self._vl_kwargs is not None:
             self._vl_kwargs["line"].setPos(last_point[0])
         if self._hl_kwargs is not None:
             self._hl_kwargs["line"].setPos(last_point[1])
 
         self.update_leading_text(last_point[0], last_point[1])
 
-    def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[ndarray, ndarray]:
+    def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[np.ndarray, np.ndarray]:
         x, y = self.getData()
         if ax == 0:
             sub_range = x[-offset:]
         else:
             sub_range = y[-offset:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
 
@@ -66,15 +65,15 @@
     def update_leading_line(self) -> None:
         if self._vl_kwargs is not None:
             self._vl_kwargs["line"].setPos(self.opts["width"][-1])
         if self._hl_kwargs is not None:
             self._hl_kwargs["line"].setPos(self.opts["y"][-1])
         self.update_leading_text(self.opts["width"][-1], self.opts["y"][-1])
 
-    def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[ndarray, ndarray]:
+    def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[np.ndarray, np.ndarray]:
         x, y = self.getData()
         if ax == 0:
             sub_range = x[-offset:]
         else:
             sub_range = y[-offset:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
 
@@ -94,15 +93,15 @@
     def update_leading_line(self) -> None:
         if self._vl_kwargs is not None:
             self._vl_kwargs["line"].setPos(self.opts["x"][-1])
         if self._hl_kwargs is not None:
             self._hl_kwargs["line"].setPos(self.opts["height"][-1])
         self.update_leading_text(self.opts["x"][-1], self.opts["height"][-1])
 
-    def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[ndarray, ndarray]:
+    def data_bounds(self, ax: int = 0, offset: int = 0) -> Tuple[np.ndarray, np.ndarray]:
         x, y = self.getData()
         if ax == 0:
             sub_range = x[-offset:]
         else:
             sub_range = y[-offset:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
 
@@ -116,15 +115,15 @@
         plot.slot_new_data = lambda y, x, kwargs: plot.setOpts(y0=plot.y0, x=x, height=y, width=plot.bar_width,
                                                                **kwargs)
     elif isinstance(plot, pg.PlotCurveItem):
         plot.slot_new_data = lambda y, x, kwargs: plot.setData(np.array(x), np.array(y), **kwargs)
     else:
         plot.slot_new_data = lambda y, x, kwargs: plot.setData(x, y, **kwargs)
 
-    def data_bounds(ax: int = 0, offset: int = 0) -> Tuple[ndarray, ndarray]:
+    def data_bounds(ax: int = 0, offset: int = 0) -> Tuple[np.ndarray, np.ndarray]:
         x, y = plot.getData()
         if ax == 0:
             sub_range = x[-offset:]
         else:
             sub_range = y[-offset:]
         return np.nanmin(sub_range), np.nanmax(sub_range)
```

### Comparing `pglive-0.6.2/pglive/sources/live_plot_widget.py` & `pglive-0.6.3/pglive/sources/live_plot_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
+
 from typing import Union, Optional, Any, List, Dict, TYPE_CHECKING
 
 import pyqtgraph as pg  # type: ignore
 from pyqtgraph import ViewBox  # type: ignore
 from pyqtgraph.Qt import QtCore  # type: ignore
 from pyqtgraph.Qt import QtGui  # type: ignore
 
 from pglive.kwargs import Crosshair
 from pglive.sources.live_axis import LiveAxis
 from pglive.sources.live_axis_range import LiveAxisRange
 
 if TYPE_CHECKING:
     from pglive.sources.data_connector import DataConnector
 
+
 class LivePlotWidget(pg.PlotWidget):
     """Implements main plot widget for all live plots"""
     mouse_position: Optional[QtCore.QPointF] = None
     sig_crosshair_moved = QtCore.Signal(QtCore.QPointF)
     sig_crosshair_out = QtCore.Signal()
     sig_crosshair_in = QtCore.Signal()
 
@@ -70,15 +72,15 @@
 
         self.disableAutoRange()
         self.getPlotItem().vb.setRange = self.set_range
         self.getPlotItem().vb.sigRangeChangedManually.connect(self.sm)
         self.addItem = addItem
         self.removeItem = removeItem
 
-    def sm(self, *args, **kwargs):
+    def sm(self, *args, **kwargs) -> None:
         self.manual_range = True
 
     def _add_crosshair(self, crosshair_pen: QtGui.QPen, crosshair_text_kwargs: dict) -> None:
         """Add crosshair into plot"""
         self.vLine = pg.InfiniteLine(angle=90, movable=False, pen=crosshair_pen)
         self.hLine = pg.InfiniteLine(angle=0, movable=False, pen=crosshair_pen)
         self.x_value_label = pg.TextItem(**crosshair_text_kwargs)
```

### Comparing `pglive-0.6.2/pglive/sources/utils.py` & `pglive-0.6.3/pglive/sources/utils.py`

 * *Files identical despite different names*

### Comparing `pglive-0.6.2/pyproject.toml` & `pglive-0.6.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pglive"
-version = "0.6.2"
+version = "0.6.3"
 description = "Pyqtgraph live plot"
 authors = ["Martin Domaracky <domarm@comat.sk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/domarm-comat/pglive"
 repository = "https://github.com/domarm-comat/pglive"
 keywords = ["pyqtgraph", "realtime", "live", "plotting", "pyqt5", "pyqt6", "pyside2", "pyside6"]
@@ -15,15 +15,16 @@
 "License :: OSI Approved :: MIT License",
 "Natural Language :: English",
 "Intended Audience :: Science/Research",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
-pyqtgraph = "^0.13.1"
+pyqtgraph = "^0.13.3"
+numpy = "^1.24.2"
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pyqt5 = "^5.15.9"
 pyqt6 = "^6.4.2"
```

### Comparing `pglive-0.6.2/setup.py` & `pglive-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
  'pglive.examples_pyside6',
  'pglive.sources']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyqtgraph>=0.13.1,<0.14.0']
+['numpy>=1.24.2,<2.0.0', 'pyqtgraph>=0.13.3,<0.14.0']
 
 setup_kwargs = {
     'name': 'pglive',
-    'version': '0.6.2',
+    'version': '0.6.3',
     'description': 'Pyqtgraph live plot',
-    'long_description': '# Live pyqtgraph plot\n\nPglive package adds support for thread-safe live plotting to pyqtgraph.  \nIt supports PyQt5, PyQt6, PySide2 and PySide6.\n\n# Description #\n\nBy default, pyqtgraph doesn\'t support live plotting. Aim of this package is to provide easy implementation of Line,\nScatter and Bar Live plot. Every plot is connected with it\'s DataConnector, which sole purpose is to consume data points\nand manage data re-plotting. DataConnector interface provides Pause and Resume method, update rate and maximum number of\nplotted points. Each time data point is collected, call `DataConnector.cb_set_data`\nor `DataConnector.cb_append_data_point` callback. That\'s all You need to update plot with new data. Callbacks are Thread\nsafe, so it works nicely in applications with multiple data collection Threads.\n\n**Focus on data collection and leave plotting to pglive.**\n\nTo make firsts steps easy, package comes with many examples implemented in PyQt5 or PyQt6.\nSupport for PySide2 and PySide6 was added in version 0.3.0.\n\n# Code examples #\n\n```python\nimport sys\nfrom math import sin\nfrom threading import Thread\nfrom time import sleep\n\nfrom PyQt6.QtWidgets import QApplication\n\nfrom pglive.sources.data_connector import DataConnector\nfrom pglive.sources.live_plot import LiveLinePlot\nfrom pglive.sources.live_plot_widget import LivePlotWidget\n\n"""\nIn this example Line plot is displayed.\n"""\napp = QApplication(sys.argv)\nrunning = True\n\nplot_widget = LivePlotWidget(title="Line Plot @ 100Hz")\nplot_curve = LiveLinePlot()\nplot_widget.addItem(plot_curve)\n# DataConnector holding 600 points and plots @ 100Hz\ndata_connector = DataConnector(plot_curve, max_points=600, update_rate=100)\n\n\ndef sin_wave_generator(connector):\n    """Sine wave generator"""\n    x = 0\n    while running:\n        x += 1\n        data_point = sin(x * 0.01)\n        # Callback to plot new data point\n        connector.cb_append_data_point(data_point, x)\n\n        sleep(0.01)\n\n\nplot_widget.show()\nThread(target=sin_wave_generator, args=(data_connector,)).start()\napp.exec()\nrunning = False\n```\n\nOutput:\n\n![Plot example](https://i.postimg.cc/RFYGfNS6/pglive.gif)\n\nTo run built-in examples, use python3 -m parameter like:  \n`python3 -m pglive.examples_pyqt6.all_plot_types`  \n`python3 -m pglive.examples_pyqt6.crosshair`\n\n# Using PyQt5/6 designer #\n\n1. Add QWidget to Your layout\n2. Promote QWidget to `LivePlotWidget` and set header file to `pglive.sources.live_plot_widget`\n3. Click `Add` and `Promote` button\n\n![All plot types](https://i.postimg.cc/m25NVJZm/designer-promotion.png)\n\n# Available plot types #\n\nPglive supports four plot types: `LiveLinePlot`, `LiveScatterPlot`, `LiveHBarPlot` (horizontal bar plot),\n`LiveVBarPlot` (vertical bar plot) and `LiveCandleStickPlot`.\n\n![All plot types](https://i.postimg.cc/637CsKRC/pglive-allplots.gif)\n![CandleStick plot](https://i.postimg.cc/0QcmMMb0/plot-candlestick.gif)\n![live-categorized-bar.gif](https://i.postimg.cc/xqrwXXjY/live-categorized-bar.gif)\n\n# Plot speed optimizations  #\n\nScaling plot view to plotted data has a huge impact on plotting performance.\nRe-plotting might be laggy when using high update frequencies and multiple plots.    \nTo increase plotting performance, pglive introduces `LiveAxisRange`, that can be used in `LivePlotWidget`.\nUser can now specify when and how is new view of plotted data calculated.\n\nHave a look in the `live_plot_range.py` example, to see how it can be used.\n\n![Range_optimization](https://i.postimg.cc/3wrMbbTY/a.gif)\n\nIn case you want to plot wider area with LiveAxisRange you can use crop_offset_to_data flag.\nFor example, you want to store 60 seconds, display 30 seconds in a view and move view every 1 second.\nYou will have big empty space to the left without setting flag to True.\nHave a look into crop_offset_to_data example.\n\n![crop_offset_to_data](https://i.postimg.cc/90X40Ng7/Peek-2022-09-24-15-20.gif)\n\nIntroduced in *v0.4.0*\n\n# Crosshair #\n\nPglive comes with built-in Crosshair as well.\n\n![Crosshair](https://i.postimg.cc/1z75GZLV/pglive-crosshair.gif)\n\n# Leading lines #\n\nLeading line displays horizontal or vertical line (or both) at the last plotted point.  \nYou can choose it\'s color and which axis value is displayed along with it.  \n\n![Leading lines](https://i.postimg.cc/bYKQGBNp/leading-line.gif)\n\n# Axis #\n\nTo make life easier, pglive includes few axis improvements:\n\n- Colored axis line using new `axisPen` attribute\n- Time and DateTime tick format, converting timestamp into human-readable format\n\n![Crosshair](https://i.postimg.cc/8kr0L2YJ/pglive-axis.gif)\n\n# Summary #\n\n- With Pglive You\'ve got easy Thread-safe implementation of fast Live plots\n- You can use all `kwargs` specified in pyqtgraph\n- Use your pyqtgraph plots with `DataConnector` directly, no need to use specific `LivePlot` class \n- **Focus on Data Handling, not Data Plotting**',
+    'long_description': '# Live pyqtgraph plot\n\nPglive package adds support for thread-safe live plotting to pyqtgraph.  \nIt supports PyQt5, PyQt6, PySide2 and PySide6.\n\n# Description #\n\nBy default, pyqtgraph doesn\'t support live plotting. Aim of this package is to provide easy implementation of Line,\nScatter and Bar Live plot. Every plot is connected with it\'s DataConnector, which sole purpose is to consume data points\nand manage data re-plotting. DataConnector interface provides Pause and Resume method, update rate and maximum number of\nplotted points. Each time data point is collected, call `DataConnector.cb_set_data`\nor `DataConnector.cb_append_data_point` callback. That\'s all You need to update plot with new data. Callbacks are Thread\nsafe, so it works nicely in applications with multiple data collection Threads.\n\n**Focus on data collection and leave plotting to pglive.**\n\nTo make firsts steps easy, package comes with many examples implemented in PyQt5 or PyQt6.\nSupport for PySide2 and PySide6 was added in version 0.3.0.\n\n# Code examples #\n\n```python\nimport sys\nfrom math import sin\nfrom threading import Thread\nfrom time import sleep\n\nfrom PyQt6.QtWidgets import QApplication\n\nfrom pglive.sources.data_connector import DataConnector\nfrom pglive.sources.live_plot import LiveLinePlot\nfrom pglive.sources.live_plot_widget import LivePlotWidget\n\n"""\nLine plot is displayed in this example.\n"""\napp = QApplication(sys.argv)\nrunning = True\n\nplot_widget = LivePlotWidget(title="Line Plot @ 100Hz")\nplot_curve = LiveLinePlot()\nplot_widget.addItem(plot_curve)\n# DataConnector holding 600 points and plots @ 100Hz\ndata_connector = DataConnector(plot_curve, max_points=600, update_rate=100)\n\n\ndef sin_wave_generator(connector):\n    """Sine wave generator"""\n    x = 0\n    while running:\n        x += 1\n        data_point = sin(x * 0.01)\n        # Callback to plot new data point\n        connector.cb_append_data_point(data_point, x)\n\n        sleep(0.01)\n\n\nplot_widget.show()\nThread(target=sin_wave_generator, args=(data_connector,)).start()\napp.exec()\nrunning = False\n```\n\nOutput:\n\n![Plot example](https://i.postimg.cc/RFYGfNS6/pglive.gif)\n\nTo run built-in examples, use python3 -m parameter like:  \n`python3 -m pglive.examples_pyqt6.all_plot_types`  \n`python3 -m pglive.examples_pyqt6.crosshair`\n\n# Using PyQt5/6 designer #\n\n1. Add QWidget to Your layout\n2. Promote QWidget to `LivePlotWidget` and set header file to `pglive.sources.live_plot_widget`\n3. Click `Add` and `Promote` button\n\n![All plot types](https://i.postimg.cc/m25NVJZm/designer-promotion.png)\n\n# Available plot types #\n\nPglive supports four plot types: `LiveLinePlot`, `LiveScatterPlot`, `LiveHBarPlot` (horizontal bar plot),\n`LiveVBarPlot` (vertical bar plot) and `LiveCandleStickPlot`.\n\n![All plot types](https://i.postimg.cc/637CsKRC/pglive-allplots.gif)\n![CandleStick plot](https://i.postimg.cc/0QcmMMb0/plot-candlestick.gif)\n![live-categorized-bar.gif](https://i.postimg.cc/xqrwXXjY/live-categorized-bar.gif)\n\n# Plot speed optimizations  #\n\nScaling plot view to plotted data has a huge impact on plotting performance.\nRe-plotting might be laggy when using high update frequencies and multiple plots.    \nTo increase plotting performance, pglive introduces `LiveAxisRange`, that can be used in `LivePlotWidget`.\nUser can now specify when and how is new view of plotted data calculated.\n\nHave a look in the `live_plot_range.py` example, to see how it can be used.\n\n![Range_optimization](https://i.postimg.cc/3wrMbbTY/a.gif)\n\nIn case you want to plot wider area with LiveAxisRange you can use crop_offset_to_data flag.\nFor example, you want to store 60 seconds, display 30 seconds in a view and move view every 1 second.\nYou will have big empty space to the left without setting flag to True.\nHave a look into crop_offset_to_data example.\n\n![crop_offset_to_data](https://i.postimg.cc/90X40Ng7/Peek-2022-09-24-15-20.gif)\n\nIntroduced in *v0.4.0*\n\n# Crosshair #\n\nPglive comes with built-in Crosshair as well.\n\n![Crosshair](https://i.postimg.cc/1z75GZLV/pglive-crosshair.gif)\n\n# Leading lines #\n\nLeading line displays horizontal or vertical line (or both) at the last plotted point.  \nYou can choose it\'s color and which axis value is displayed along with it.  \n\n![Leading lines](https://i.postimg.cc/bYKQGBNp/leading-line.gif)\n\n# Axis #\n\nTo make life easier, pglive includes few axis improvements:\n\n- Colored axis line using new `axisPen` attribute\n- Time and DateTime tick format, converting timestamp into human-readable format\n\n![Crosshair](https://i.postimg.cc/8kr0L2YJ/pglive-axis.gif)\n\n# Summary #\n\n- With Pglive You\'ve got easy Thread-safe implementation of fast Live plots\n- You can use all `kwargs` specified in pyqtgraph\n- Use your pyqtgraph plots with `DataConnector` directly, no need to use specific `LivePlot` class \n- **Focus on Data Handling, not Data Plotting**',
     'author': 'Martin Domaracky',
     'author_email': 'domarm@comat.sk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/domarm-comat/pglive',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pglive-0.6.2/PKG-INFO` & `pglive-0.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglive
-Version: 0.6.2
+Version: 0.6.3
 Summary: Pyqtgraph live plot
 Home-page: https://github.com/domarm-comat/pglive
 License: MIT
 Keywords: pyqtgraph,realtime,live,plotting,pyqt5,pyqt6,pyside2,pyside6
 Author: Martin Domaracky
 Author-email: domarm@comat.sk
 Requires-Python: >=3.8,<3.11
@@ -14,15 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: pyqtgraph (>=0.13.1,<0.14.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pyqtgraph (>=0.13.3,<0.14.0)
 Project-URL: Repository, https://github.com/domarm-comat/pglive
 Description-Content-Type: text/markdown
 
 # Live pyqtgraph plot
 
 Pglive package adds support for thread-safe live plotting to pyqtgraph.  
 It supports PyQt5, PyQt6, PySide2 and PySide6.
@@ -52,15 +53,15 @@
 from PyQt6.QtWidgets import QApplication
 
 from pglive.sources.data_connector import DataConnector
 from pglive.sources.live_plot import LiveLinePlot
 from pglive.sources.live_plot_widget import LivePlotWidget
 
 """
-In this example Line plot is displayed.
+Line plot is displayed in this example.
 """
 app = QApplication(sys.argv)
 running = True
 
 plot_widget = LivePlotWidget(title="Line Plot @ 100Hz")
 plot_curve = LiveLinePlot()
 plot_widget.addItem(plot_curve)
```

