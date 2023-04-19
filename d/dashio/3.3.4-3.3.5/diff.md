# Comparing `tmp/dashio-3.3.4.tar.gz` & `tmp/dashio-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashio-3.3.4.tar", last modified: Mon Apr 17 02:20:18 2023, max compression
+gzip compressed data, was "dashio-3.3.5.tar", last modified: Wed Apr 19 06:24:43 2023, max compression
```

## Comparing `dashio-3.3.4.tar` & `dashio-3.3.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.635324 dashio-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-17 02:20:10.000000 dashio-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-17 02:20:18.635324 dashio-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-17 02:20:10.000000 dashio-3.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.627324 dashio-3.3.4/dashio/
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.627324 dashio-3.3.4/dashio/action_station_services/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/action_station_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/as_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/clock_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/modbus_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/timer_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/bleconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.631324 dashio-3.3.4/dashio/iotcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/audio_visual_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/knob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/mqttconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/serialconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/zeroconf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/zmqconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.627324 dashio-3.3.4/dashio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 02:20:10.000000 dashio-3.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-17 02:20:18.635324 dashio-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-17 02:20:10.000000 dashio-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.635324 dashio-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_dashdevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_knob.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_mqttconntection.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_zqmconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.550700 dashio-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 06:24:29.000000 dashio-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-19 06:24:43.550700 dashio-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-19 06:24:29.000000 dashio-3.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.534699 dashio-3.3.5/dashio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.534699 dashio-3.3.5/dashio/action_station_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/action_station_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/as_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/clock_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/modbus_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/timer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/bleconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.542700 dashio-3.3.5/dashio/iotcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/audio_visual_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/mqttconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/serialconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/zeroconf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/zmqconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.534699 dashio-3.3.5/dashio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 06:24:29.000000 dashio-3.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 06:24:43.550700 dashio-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-19 06:24:29.000000 dashio-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.550700 dashio-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_dashdevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_mqttconntection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_zqmconnection.py
```

### Comparing `dashio-3.3.4/LICENSE` & `dashio-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/PKG-INFO` & `dashio-3.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.4
+Version: 3.3.5
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dashio-3.3.4/README.md` & `dashio-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/__init__.py` & `dashio-3.3.5/dashio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,17 @@
     LabelStyle,
     KnobStyle,
     ChartXAxisLabelsStyle,
     TextFormat,
     DirectionStyle,
     ColorPickerStyle,
     ControlName,
-    ButtonStyle
+    ButtonStyle,
+    ButtonGroupStyle,
+    MenuStyle
 )
 from .iotcontrol.audio_visual_display import AudioVisualDisplay
 from .iotcontrol.chart import Chart, ChartLine
 from .iotcontrol.slider import Slider
 from .iotcontrol.textbox import TextBox
 from .iotcontrol.button import Button
 from .iotcontrol.time_graph import TimeGraph, TimeGraphLine, DataPoint
```

### Comparing `dashio-3.3.4/dashio/action_station.py` & `dashio-3.3.5/dashio/action_station.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/action_station_services/action_station_service_config.py` & `dashio-3.3.5/dashio/action_station_services/action_station_service_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/action_station_services/as_servicel.py` & `dashio-3.3.5/dashio/action_station_services/as_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/action_station_services/clock_servicel.py` & `dashio-3.3.5/dashio/action_station_services/clock_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/action_station_services/modbus_service.py` & `dashio-3.3.5/dashio/action_station_services/modbus_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/action_station_services/task_service.py` & `dashio-3.3.5/dashio/action_station_services/task_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/action_station_services/timer_service.py` & `dashio-3.3.5/dashio/action_station_services/timer_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/bleconnection.py` & `dashio-3.3.5/dashio/bleconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/constants.py` & `dashio-3.3.5/dashio/constants.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/dashconnection.py` & `dashio-3.3.5/dashio/dashconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/device.py` & `dashio-3.3.5/dashio/device.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/__init__.py` & `dashio-3.3.5/dashio/iotcontrol/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """The DashIO module is for creating devices, controls and connections for the DashIO app.
 """
 from .enums import Color, Icon, Precision, Keyboard, TextAlignment, SliderBarStyle, DialNumberPosition, DialStyle,\
     SoundName, ChartLineType, TimeGraphLineType, TimeGraphPositionOfKey, ButtonState, LabelStyle, KnobStyle,\
-    TitlePosition, ChartXAxisLabelsStyle, TextFormat, DirectionStyle, ColorPickerStyle, ControlName, ButtonStyle
+    TitlePosition, ChartXAxisLabelsStyle, TextFormat, DirectionStyle, ColorPickerStyle, ControlName, ButtonStyle,\
+    MenuStyle, ButtonGroupStyle
 from .audio_visual_display import AudioVisualDisplay
 from .chart import Chart, ChartLine, ChartConfig
 from .slider import Slider, SliderConfig
 from .textbox import TextBox, TextBoxConfig
 from .button import Button, ButtonConfig
 from .time_graph import TimeGraph, TimeGraphLine, DataPoint, TimeGraphConfig
 from .knob import Knob, KnobConfig
```

### Comparing `dashio-3.3.4/dashio/iotcontrol/alarm.py` & `dashio-3.3.5/dashio/iotcontrol/alarm.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/audio_visual_display.py` & `dashio-3.3.5/dashio/iotcontrol/audio_visual_display.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/button.py` & `dashio-3.3.5/dashio/iotcontrol/button.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,28 +60,27 @@
 
         Returns
         -------
         ButtonGroupConfig
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
-            cfg_dict["title"],
-            _get_title_position(cfg_dict["titlePosition"]),
-            cfg_dict["buttonEnabled"],
-            _get_button_style(cfg_dict["style"]),
-            _get_icon(cfg_dict["iconName"]),
-            _get_color(cfg_dict["onColor"]),
-            _get_color(cfg_dict["offColor"]),
-            cfg_dict["text"],
+            cfg_dict.get("title", ''),
+            _get_title_position(cfg_dict.get("titlePosition", 'bottom')),
+            cfg_dict.get("buttonEnabled", True),
+            _get_button_style(cfg_dict.get("style", 'basic')),
+            _get_icon(cfg_dict.get("iconName", 'none')),
+            _get_color(cfg_dict.get("onColor", 'blue')),
+            _get_color(cfg_dict.get("offColor", 'red')),
+            cfg_dict.get("text", ""),
             ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
-
 class Button(Control):
     """A Button control.
 
     Attributes
     ----------
     control_id : str
         An unique control identity string. The control identity string must be a unique string for each control per device
```

### Comparing `dashio-3.3.4/dashio/iotcontrol/button_group.py` & `dashio-3.3.5/dashio/iotcontrol/button_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,36 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from ..constants import BAD_CHARS
 from .button import Button
-from .control import Control, ControlPosition, ControlConfig, _get_icon, _get_title_position
-from .enums import Icon, TitlePosition
+from .control import Control, ControlPosition, ControlConfig, _get_icon, _get_title_position, _get_button_group_style
+from .enums import Icon, TitlePosition, ButtonGroupStyle
 
 
 class ButtonGroupConfig(ControlConfig):
     """ButtonGroupConfig"""
     def __init__(
         self,
         control_id: str,
         title: str,
         text: str,
+        style: ButtonGroupStyle,
         icon: Icon,
         grid_view: bool,
         control_position: ControlPosition,
         title_position: TitlePosition
     ) -> None:
         super().__init__(control_id, title, control_position, title_position)
         self.cfg["text"] = text.translate(BAD_CHARS)
         self.cfg["iconName"] = icon.value
         self.cfg["gridView"] = grid_view
+        self.cfg["style"] = str(style.value)
 
     @classmethod
     def from_dict(cls, cfg_dict: dict):
         """Instantiates ButtonGroupConfig from cfg dictionary
 
         Parameters
         ----------
@@ -55,18 +57,19 @@
 
         Returns
         -------
         ButtonGroupConfig
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
-            cfg_dict["title"],
-            cfg_dict["text"],
-            _get_icon(cfg_dict["iconName"]),
-            cfg_dict["gridView"],
+            cfg_dict.get("title", ""),
+            cfg_dict.get("text", ""),
+            _get_button_group_style(cfg_dict.get("style", 'basic')),
+            _get_icon(cfg_dict.get("iconName", 'none')),
+            cfg_dict.get("gridView", True),
             ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"]),
             _get_title_position(cfg_dict["titlePosition"])
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
 
@@ -90,39 +93,42 @@
 
     def __init__(
         self,
         control_id,
         title="A Button Group",
         text="A Button group with Text",
         title_position=TitlePosition.BOTTOM,
+        style=ButtonGroupStyle.BASIC,
         icon=Icon.MENU,
         grid_view=True,
         control_position=None,
     ):
         """ButtonGroup control that shows a popup of buttons.
 
         Parameters
         ----------
             control_id : str
                 An unique control identity string. The control identity string must be a unique string for each control per device
             title : str, optional:
                 [description]. Defaults to "A Button Group".
             text (str, optional):
                 [description]. Defaults to "A Button group with Text".
-            title_position ([type], optional):
+            title_position (TitlePosition, optional):
                 [description]. Defaults to TitlePosition.BOTTOM.
-            icon ([type], optional):
+            style (ButtonGroupStyle, optional)
+                The style of the ButtonGroup.
+            icon (Icon, optional):
                 [description]. Defaults to Icon.MENU.
             grid_view (bool, optional):
                 [description]. Defaults to True.
-            control_position ([type], optional):
+            control_position (ControlPosition, optional):
                 [description]. Defaults to None.
         """
         super().__init__("BTGP", control_id)
-        self._cfg_columnar.append(ButtonGroupConfig(control_id, title, text, icon, grid_view, control_position, title_position))
+        self._cfg_columnar.append(ButtonGroupConfig(control_id, title, text, style, icon, grid_view, control_position, title_position))
 
     @classmethod
     def from_cfg_dict(cls, cfg_dict: dict):
         """Instatiates ButtonGroup from cfg dictionary
 
         Parameters
         ----------
@@ -131,19 +137,20 @@
 
         Returns
         -------
         ButtonGroup
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
-            cfg_dict["title"],
-            cfg_dict["text"],
-            _get_title_position(cfg_dict["titlePosition"]),
-            _get_icon(cfg_dict["iconName"]),
-            cfg_dict["gridView"],
+            cfg_dict.get("title", ""),
+            cfg_dict.get("text", ""),
+            _get_title_position(cfg_dict.get("titlePosition", "Bottom")),
+            _get_button_group_style(cfg_dict.get("style", "basic")),
+            _get_icon(cfg_dict.get("iconName", "None")),
+            cfg_dict.get("gridView", True),
             ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def add_button(self, control):
         """[summary]
```

### Comparing `dashio-3.3.4/dashio/iotcontrol/chart.py` & `dashio-3.3.5/dashio/iotcontrol/chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/color_picker.py` & `dashio-3.3.5/dashio/iotcontrol/color_picker.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/control.py` & `dashio-3.3.5/dashio/iotcontrol/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import json
 import logging
 from ..constants import BAD_CHARS
-from .enums import ColorPickerStyle, DeviceViewStyle, DialNumberPosition, DirectionStyle, ChartXAxisLabelsStyle, Keyboard, KnobStyle, Precision,\
-    TextAlignment, TitlePosition, Icon, Color, TextFormat, LabelStyle, SliderBarStyle, DialStyle, TimeGraphPositionOfKey, ButtonStyle
+from .enums import ColorPickerStyle, DeviceViewStyle, DialNumberPosition, DirectionStyle, ChartXAxisLabelsStyle,\
+    Keyboard, KnobStyle, Precision, TextAlignment, TitlePosition, Icon, Color, TextFormat, LabelStyle, SliderBarStyle,\
+    DialStyle, TimeGraphPositionOfKey, ButtonStyle, ButtonGroupStyle, MenuStyle
 from .event import Event
 
 
 def _get_icon(icon_str: str) -> Icon:
     icon_name = icon_str.upper().replace(" ", "")
     return Icon[icon_name]
 
@@ -58,18 +59,30 @@
     return Precision(precision_int)
 
 
 def _get_keyboard_type(keyboard_str: str) -> Keyboard:
     t_keyboard = keyboard_str.upper().replace(" ", "")
     return Keyboard[t_keyboard]
 
+
 def _get_button_style(button_style: str) -> ButtonStyle:
     btn_style = button_style.upper()
     return ButtonStyle[btn_style]
 
+
+def _get_menu_style(button_style: str) -> MenuStyle:
+    menu_style = button_style.upper()
+    return MenuStyle[menu_style]
+
+
+def _get_button_group_style(button_group_style: str) -> ButtonGroupStyle:
+    btn_grp_style = button_group_style.upper()
+    return ButtonGroupStyle[btn_grp_style]
+
+
 def _get_device_view_style(device_view_style: str) -> DeviceViewStyle:
     dvs_name = device_view_style.upper().replace(" ", "")
     return DeviceViewStyle[dvs_name]
 
 
 def _get_color_picker_style(color_picker_style: str) -> ColorPickerStyle:
     cps_name = color_picker_style.upper().replace(" ", "")
```

### Comparing `dashio-3.3.4/dashio/iotcontrol/device_view.py` & `dashio-3.3.5/dashio/iotcontrol/device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/dial.py` & `dashio-3.3.5/dashio/iotcontrol/dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/direction.py` & `dashio-3.3.5/dashio/iotcontrol/direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/enums.py` & `dashio-3.3.5/dashio/iotcontrol/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,26 @@
 
 class ButtonStyle(Enum):
     """Button Styles"""
     BASIC = "basic"
     HIGHLIGHT = "highlight"
 
 
+class MenuStyle(Enum):
+    """Menu Styles"""
+    BASIC = "basic"
+    HIGHLIGHT = "highlight"
+
+
+class ButtonGroupStyle(Enum):
+    """Button Group Styles"""
+    BASIC = "basic"
+    HIGHLIGHT = "highlight"
+
+
 class DeviceViewStyle(Enum):
     """DeciveView Styles"""
     BASIC = "BASIC"
     BORDERS = "BORDERS"
 
 
 class ColorPickerStyle(Enum):
```

### Comparing `dashio-3.3.4/dashio/iotcontrol/event.py` & `dashio-3.3.5/dashio/iotcontrol/event.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/event_log.py` & `dashio-3.3.5/dashio/iotcontrol/event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/knob.py` & `dashio-3.3.5/dashio/iotcontrol/knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/label.py` & `dashio-3.3.5/dashio/iotcontrol/label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/map.py` & `dashio-3.3.5/dashio/iotcontrol/map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/menu.py` & `dashio-3.3.5/dashio/iotcontrol/menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,35 +19,37 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from ..constants import BAD_CHARS
 from .button import Button
-from .control import Control, ControlPosition, ControlConfig, _get_icon, _get_title_position
-from .enums import Icon, TitlePosition
+from .control import Control, ControlPosition, ControlConfig, _get_icon, _get_title_position, _get_menu_style
+from .enums import Icon, TitlePosition, MenuStyle
 from .selector import Selector
 from .slider import Slider
 from .textbox import TextBox
 
 
 class MenuConfig(ControlConfig):
     """MenuConfig"""
     def __init__(
         self,
         control_id: str,
         title: str,
         title_position: TitlePosition,
         text: str,
+        style: MenuStyle,
         icon_name: Icon,
         control_position: ControlPosition
     ) -> None:
         super().__init__(control_id, title, control_position, title_position)
         self.cfg["text"] = text.translate(BAD_CHARS)
         self.cfg["iconName"] = icon_name.value
+        self.cfg["style"] = str(style.value)
 
     @classmethod
     def from_dict(cls, cfg_dict: dict):
         """Instantiates MenuConfig from cfg dictionary
 
         Parameters
         ----------
@@ -56,18 +58,19 @@
 
         Returns
         -------
         MenuConfig
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
-            cfg_dict["title"],
-            _get_title_position(cfg_dict["titlePosition"]),
-            cfg_dict["text"],
-            _get_icon(cfg_dict["iconName"]),
+            cfg_dict.get("title", ""),
+            _get_title_position(cfg_dict.get("titlePosition", "Bottom")),
+            cfg_dict.get("text", ""),
+            _get_menu_style(cfg_dict.get("style", "basic")),
+            _get_icon(cfg_dict.get("iconName", "None")),
             ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
 
 class Menu(Control):
@@ -76,14 +79,15 @@
 
     def __init__(
         self,
         control_id: str,
         title="A Menu",
         title_position=TitlePosition.BOTTOM,
         text="A Menu with Text",
+        style=MenuStyle.BASIC,
         icon_name=Icon.MENU,
         control_position=None
     ):
         """A Menu control
 
         Parameters
         ----------
@@ -103,14 +107,15 @@
         super().__init__("MENU", control_id)
         self._cfg_columnar.append(
             MenuConfig(
                 control_id,
                 title,
                 title_position,
                 text,
+                style,
                 icon_name,
                 control_position
             )
         )
 
     @classmethod
     def from_cfg_dict(cls, cfg_dict: dict):
@@ -123,18 +128,19 @@
 
         Returns
         -------
         Menu
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
-            cfg_dict["title"],
-            _get_title_position(cfg_dict["titlePosition"]),
-            cfg_dict["text"],
-            _get_icon(cfg_dict["iconName"]),
+            cfg_dict.get("title", ""),
+            _get_title_position(cfg_dict.get("titlePosition", "Bottom")),
+            cfg_dict.get("text", ""),
+            _get_menu_style(cfg_dict.get("style", "basic")),
+            _get_icon(cfg_dict.get("iconName", "None")),
             ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
     def add_control(self, control):
         """Add a control to the menu
```

### Comparing `dashio-3.3.4/dashio/iotcontrol/ring_buffer.py` & `dashio-3.3.5/dashio/iotcontrol/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/selector.py` & `dashio-3.3.5/dashio/iotcontrol/selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/slider.py` & `dashio-3.3.5/dashio/iotcontrol/slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/textbox.py` & `dashio-3.3.5/dashio/iotcontrol/textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/iotcontrol/time_graph.py` & `dashio-3.3.5/dashio/iotcontrol/time_graph.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/ip.py` & `dashio-3.3.5/dashio/ip.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/load_config.py` & `dashio-3.3.5/dashio/load_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/mqttconnection.py` & `dashio-3.3.5/dashio/mqttconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/serialconnection.py` & `dashio-3.3.5/dashio/serialconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/tcpconnection.py` & `dashio-3.3.5/dashio/tcpconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/zeroconf_service.py` & `dashio-3.3.5/dashio/zeroconf_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio/zmqconnection.py` & `dashio-3.3.5/dashio/zmqconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/dashio.egg-info/PKG-INFO` & `dashio-3.3.5/dashio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.4
+Version: 3.3.5
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dashio-3.3.4/dashio.egg-info/SOURCES.txt` & `dashio-3.3.5/dashio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/setup.cfg` & `dashio-3.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/setup.py` & `dashio-3.3.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dashio",
-    version="3.3.4",
+    version="3.3.5",
     description="DashIO interface library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="James Boulton",
     author_email="james@dashio.com",
     url="https://dashio.io",
     download_url="https://github.com/dashio-connect/python-dashio",
```

### Comparing `dashio-3.3.4/tests/test_button.py` & `dashio-3.3.5/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_button_group.py` & `dashio-3.3.5/tests/test_button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_chart.py` & `dashio-3.3.5/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_dashdevice.py` & `dashio-3.3.5/tests/test_dashdevice.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_device_view.py` & `dashio-3.3.5/tests/test_device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_dial.py` & `dashio-3.3.5/tests/test_dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_direction.py` & `dashio-3.3.5/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_event_log.py` & `dashio-3.3.5/tests/test_event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_knob.py` & `dashio-3.3.5/tests/test_knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_label.py` & `dashio-3.3.5/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_map.py` & `dashio-3.3.5/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_menu.py` & `dashio-3.3.5/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_selector.py` & `dashio-3.3.5/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_slider.py` & `dashio-3.3.5/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_textbox.py` & `dashio-3.3.5/tests/test_textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.4/tests/test_time_graph.py` & `dashio-3.3.5/tests/test_time_graph.py`

 * *Files identical despite different names*

