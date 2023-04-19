# Comparing `tmp/pyjoulescope_driver-1.3.2.tar.gz` & `tmp/pyjoulescope_driver-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjoulescope_driver-1.3.2.tar", last modified: Thu Apr 13 20:57:22 2023, max compression
+gzip compressed data, was "pyjoulescope_driver-1.3.3.tar", last modified: Wed Apr 19 20:44:27 2023, max compression
```

## Comparing `pyjoulescope_driver-1.3.2.tar` & `pyjoulescope_driver-1.3.3.tar`

### file list

```diff
@@ -1,404 +1,405 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.576144 pyjoulescope_driver-1.3.2/
--rw-rw-rw-   0        0        0     6826 2023-04-13 20:47:37.000000 pyjoulescope_driver-1.3.2/CHANGELOG.md
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjoulescope_driver-1.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0      345 2022-11-19 20:38:00.000000 pyjoulescope_driver-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5170 2023-04-13 20:57:22.576144 pyjoulescope_driver-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3360 2023-01-03 21:53:29.000000 pyjoulescope_driver-1.3.2/README.md
--rw-rw-rw-   0        0        0     6268 2022-09-20 19:25:49.000000 pyjoulescope_driver-1.3.2/credits.html
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.597465 pyjoulescope_driver-1.3.2/include/
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.624975 pyjoulescope_driver-1.3.2/include/jsdrv/
--rw-rw-rw-   0        0        0     2698 2022-11-08 21:41:45.000000 pyjoulescope_driver-1.3.2/include/jsdrv/cmacro_inc.h
--rw-rw-rw-   0        0        0     8332 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.2/include/jsdrv/cstr.h
--rw-rw-rw-   0        0        0     5878 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.2/include/jsdrv/error_code.h
--rw-rw-rw-   0        0        0     6818 2022-08-01 20:41:28.000000 pyjoulescope_driver-1.3.2/include/jsdrv/log.h
--rw-rw-rw-   0        0        0     2002 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/include/jsdrv/meta.h
--rw-rw-rw-   0        0        0    13833 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/include/jsdrv/time.h
--rw-rw-rw-   0        0        0     3827 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.2/include/jsdrv/topic.h
--rw-rw-rw-   0        0        0    12351 2022-08-01 20:41:48.000000 pyjoulescope_driver-1.3.2/include/jsdrv/union.h
--rw-rw-rw-   0        0        0     4042 2023-04-11 14:09:34.000000 pyjoulescope_driver-1.3.2/include/jsdrv/version.h
--rw-rw-rw-   0        0        0    29160 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/include/jsdrv.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.627480 pyjoulescope_driver-1.3.2/include_private/
--rw-rw-rw-   0        0        0    13394 2022-10-27 14:05:41.000000 pyjoulescope_driver-1.3.2/include_private/js220_api.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.717653 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/
--rw-rw-rw-   0        0        0     1683 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/assert.h
--rw-rw-rw-   0        0        0     2116 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/backend.h
--rw-rw-rw-   0        0        0     2774 2023-04-12 17:01:55.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/buffer.h
--rw-rw-rw-   0        0        0     3935 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/buffer_signal.h
--rw-rw-rw-   0        0        0     7138 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/cdef.h
--rw-rw-rw-   0        0        0     5647 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/dbc.h
--rw-rw-rw-   0        0        0     1385 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/device.h
--rw-rw-rw-   0        0        0     1291 2022-07-28 13:15:21.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/devices.h
--rw-rw-rw-   0        0        0     1633 2022-10-23 16:50:55.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/downsample.h
--rw-rw-rw-   0        0        0     1960 2022-09-19 13:38:02.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/event.h
--rw-rw-rw-   0        0        0     6987 2023-03-19 15:49:32.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/frontend.h
--rw-rw-rw-   0        0        0     1408 2022-08-01 19:59:27.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js110_cal.h
--rw-rw-rw-   0        0        0     3046 2022-11-01 14:07:32.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js110_sample_processor.h
--rw-rw-rw-   0        0        0     2858 2022-11-01 15:41:07.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js110_stats.h
--rw-rw-rw-   0        0        0     1647 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js220_i128.h
--rw-rw-rw-   0        0        0     1558 2022-10-04 22:55:17.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js220_stats.h
--rw-rw-rw-   0        0        0     3780 2022-08-01 13:11:32.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/json.h
--rw-rw-rw-   0        0        0    14035 2022-09-18 11:31:10.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/list.h
--rw-rw-rw-   0        0        0     8973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/log.h
--rw-rw-rw-   0        0        0     1650 2022-09-19 12:36:34.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/msg_queue.h
--rw-rw-rw-   0        0        0     2561 2022-07-28 13:01:35.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/mutex.h
--rw-rw-rw-   0        0        0     5267 2022-09-26 20:28:04.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/platform.h
--rw-rw-rw-   0        0        0     4061 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/pubsub.h
--rw-rw-rw-   0        0        0     2799 2022-10-07 12:17:37.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/sample_buffer_f32.h
--rw-rw-rw-   0        0        0     4561 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/statistics.h
--rw-rw-rw-   0        0        0     1939 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/thread.h
--rw-rw-rw-   0        0        0     8210 2022-07-29 18:34:03.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/usb_spec.h
--rw-rw-rw-   0        0        0     1533 2022-10-09 18:53:30.000000 pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/windows.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.724659 pyjoulescope_driver-1.3.2/pyjoulescope_driver/
--rw-rw-rw-   0        0        0      964 2023-03-29 21:30:50.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-03-29 21:47:21.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/__main__.py
--rw-rw-rw-   0        0        0  1596797 2023-04-04 17:51:40.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/binding.c
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.735181 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/
--rw-rw-rw-   0        0        0      961 2023-03-29 21:29:14.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/__init__.py
--rw-rw-rw-   0        0        0     1830 2023-01-25 14:57:14.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/gpi.py
--rw-rw-rw-   0        0        0     3702 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/info.py
--rw-rw-rw-   0        0        0     4213 2022-10-30 15:18:19.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/program.py
--rw-rw-rw-   0        0        0     5031 2023-04-13 12:02:12.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/record.py
--rw-rw-rw-   0        0        0      932 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/scan.py
--rw-rw-rw-   0        0        0     2410 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/set_parameter.py
--rw-rw-rw-   0        0        0     2981 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/statistics.py
--rw-rw-rw-   0        0        0     2807 2022-10-08 20:50:48.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/threads.py
--rw-rw-rw-   0        0        0   609280 2023-04-13 20:57:19.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/img_alpha.img
--rw-rw-rw-   0        0        0   609280 2023-04-13 20:57:19.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/img_beta.img
--rw-rw-rw-   0        0        0   609280 2023-04-13 20:57:19.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/img_stable.img
--rw-rw-rw-   0        0        0    10359 2022-10-30 15:59:38.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/program.py
--rw-rw-rw-   0        0        0     8003 2023-04-13 12:15:14.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/record.py
--rw-rw-rw-   0        0        0     8980 2022-11-11 19:24:16.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/release.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.735680 pyjoulescope_driver-1.3.2/pyjoulescope_driver/test/
--rw-rw-rw-   0        0        0        0 2022-10-09 12:38:26.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/test/__init__.py
--rw-rw-rw-   0        0        0     1901 2022-10-09 17:17:09.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/test/test_release.py
--rw-rw-rw-   0        0        0     2304 2023-03-29 16:02:01.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/test/test_time64.py
--rw-rw-rw-   0        0        0     4660 2023-03-29 16:00:59.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/time64.py
--rw-rw-rw-   0        0        0     1063 2023-04-11 14:09:34.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.730670 pyjoulescope_driver-1.3.2/pyjoulescope_driver.egg-info/
--rw-rw-rw-   0        0        0     5170 2023-04-13 20:57:21.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13646 2023-04-13 20:57:21.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:57:21.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-13 20:57:21.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-04-13 20:57:21.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-13 20:57:21.000000 pyjoulescope_driver-1.3.2/pyjoulescope_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      868 2022-11-30 13:52:01.000000 pyjoulescope_driver-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0      117 2023-04-13 20:57:22.576144 pyjoulescope_driver-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0    10610 2023-03-09 19:24:23.000000 pyjoulescope_driver-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.822301 pyjoulescope_driver-1.3.2/src/
--rw-rw-rw-   0        0        0     2655 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/src/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.837815 pyjoulescope_driver-1.3.2/src/backend/
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.847820 pyjoulescope_driver-1.3.2/src/backend/libusb/
--rw-rw-rw-   0        0        0    30330 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/src/backend/libusb/backend.c
--rw-rw-rw-   0        0        0     4580 2022-09-19 12:40:12.000000 pyjoulescope_driver-1.3.2/src/backend/libusb/msg_queue.c
--rw-rw-rw-   0        0        0     4890 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/src/backend/posix.c
--rw-rw-rw-   0        0        0     6392 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/src/backend/windows.c
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.851820 pyjoulescope_driver-1.3.2/src/backend/winusb/
--rw-rw-rw-   0        0        0    38641 2023-04-04 15:07:16.000000 pyjoulescope_driver-1.3.2/src/backend/winusb/backend.c
--rw-rw-rw-   0        0        0     7713 2022-09-18 12:51:07.000000 pyjoulescope_driver-1.3.2/src/backend/winusb/device_change_notifier.c
--rw-rw-rw-   0        0        0     2798 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/src/backend/winusb/device_change_notifier.h
--rw-rw-rw-   0        0        0     4807 2023-03-19 16:29:53.000000 pyjoulescope_driver-1.3.2/src/backend/winusb/msg_queue.c
--rw-rw-rw-   0        0        0    25596 2023-03-15 17:50:15.000000 pyjoulescope_driver-1.3.2/src/buffer.c
--rw-rw-rw-   0        0        0    32515 2023-03-30 18:49:53.000000 pyjoulescope_driver-1.3.2/src/buffer_signal.c
--rw-rw-rw-   0        0        0    11771 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/src/cstr.c
--rw-rw-rw-   0        0        0     1671 2022-09-19 11:52:36.000000 pyjoulescope_driver-1.3.2/src/devices.c
--rw-rw-rw-   0        0        0     8709 2022-10-24 15:34:41.000000 pyjoulescope_driver-1.3.2/src/downsample.c
--rw-rw-rw-   0        0        0     5925 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.2/src/emu.c
--rw-rw-rw-   0        0        0     4649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/src/emulated.c
--rw-rw-rw-   0        0        0     4817 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.2/src/error_code.c
--rw-rw-rw-   0        0        0     9335 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/src/js110_api.h
--rw-rw-rw-   0        0        0     3972 2022-09-18 11:26:57.000000 pyjoulescope_driver-1.3.2/src/js110_cal.c
--rw-rw-rw-   0        0        0     9038 2022-11-01 14:07:47.000000 pyjoulescope_driver-1.3.2/src/js110_sample_processor.c
--rw-rw-rw-   0        0        0     4551 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.2/src/js110_stats.c
--rw-rw-rw-   0        0        0    49080 2023-04-04 13:28:44.000000 pyjoulescope_driver-1.3.2/src/js110_usb.c
--rw-rw-rw-   0        0        0     5162 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/src/js220_i128.c
--rw-rw-rw-   0        0        0     1188 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.2/src/js220_params.c
--rw-rw-rw-   0        0        0     2893 2022-10-05 01:35:24.000000 pyjoulescope_driver-1.3.2/src/js220_stats.c
--rw-rw-rw-   0        0        0    62812 2023-04-12 17:35:21.000000 pyjoulescope_driver-1.3.2/src/js220_usb.c
--rw-rw-rw-   0        0        0    37455 2023-03-19 17:28:55.000000 pyjoulescope_driver-1.3.2/src/jsdrv.c
--rw-rw-rw-   0        0        0    10974 2022-08-01 18:37:59.000000 pyjoulescope_driver-1.3.2/src/json.c
--rw-rw-rw-   0        0        0    13012 2023-03-19 15:25:39.000000 pyjoulescope_driver-1.3.2/src/log.c
--rw-rw-rw-   0        0        0    10627 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/src/meta.c
--rw-rw-rw-   0        0        0    24211 2023-03-19 15:32:24.000000 pyjoulescope_driver-1.3.2/src/pubsub.c
--rw-rw-rw-   0        0        0     4944 2022-10-07 12:24:15.000000 pyjoulescope_driver-1.3.2/src/sample_buffer_f32.c
--rw-rw-rw-   0        0        0     5262 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.2/src/statistics.c
--rw-rw-rw-   0        0        0     2814 2023-03-09 19:53:59.000000 pyjoulescope_driver-1.3.2/src/time.c
--rw-rw-rw-   0        0        0     3763 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.2/src/topic.c
--rw-rw-rw-   0        0        0    12780 2022-09-18 11:32:07.000000 pyjoulescope_driver-1.3.2/src/union.c
--rw-rw-rw-   0        0        0     1001 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/src/version.c
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.855320 pyjoulescope_driver-1.3.2/third-party/
--rw-rw-rw-   0        0        0      810 2022-09-20 18:21:09.000000 pyjoulescope_driver-1.3.2/third-party/CMakeLists.txt
--rw-rw-rw-   0        0        0      364 2022-08-01 20:40:07.000000 pyjoulescope_driver-1.3.2/third-party/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.903389 pyjoulescope_driver-1.3.2/third-party/cmocka/
--rw-rw-rw-   0        0        0       18 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/.clang_complete
--rw-rw-rw-   0        0        0     9611 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/.gitlab-ci.yml
--rw-rw-rw-   0        0        0     3508 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/.ycm_extra_conf.py
--rw-rw-rw-   0        0        0     1209 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/5.patch
--rw-rw-rw-   0        0        0     3601 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/CMakeLists.txt
--rw-rw-rw-   0        0        0     1845 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/CPackConfig.cmake
--rw-rw-rw-   0        0        0      284 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/CTestConfig.cmake
--rw-rw-rw-   0        0        0     5331 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/CompilerChecks.cmake
--rw-rw-rw-   0        0        0     4648 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/ConfigureChecks.cmake
--rw-rw-rw-   0        0        0      431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/DefineOptions.cmake
--rw-rw-rw-   0        0        0     3217 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/INSTALL.md
--rw-rw-rw-   0        0        0      658 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.908395 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.934925 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/
--rw-rw-rw-   0        0        0      866 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake
--rw-rw-rw-   0        0        0     3360 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake
--rw-rw-rw-   0        0        0     1952 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake
--rw-rw-rw-   0        0        0      811 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake
--rw-rw-rw-   0        0        0     3973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake
--rw-rw-rw-   0        0        0      585 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake
--rw-rw-rw-   0        0        0     1480 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/FindNSIS.cmake
--rw-rw-rw-   0        0        0      680 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake
--rw-rw-rw-   0        0        0      656 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake
--rw-rw-rw-   0        0        0     1145 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Toolchain-cross-m32.cmake
--rw-rw-rw-   0        0        0       53 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmocka-build-tree-settings.cmake.in
--rw-rw-rw-   0        0        0      507 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmocka-config.cmake.in
--rw-rw-rw-   0        0        0      189 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/cmocka.pc.cmake
--rw-rw-rw-   0        0        0     5161 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/config.h.cmake
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.939929 pyjoulescope_driver-1.3.2/third-party/cmocka/coverity/
--rw-rw-rw-   0        0        0     3918 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/coverity/coverity_assert_model.c
--rw-rw-rw-   0        0        0      142 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/coverity/coverity_internal_model.c
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.950446 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/
--rw-rw-rw-   0        0        0     2206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/CMakeLists.txt
--rw-rw-rw-   0        0        0    26974 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/index.html
--rw-rw-rw-   0        0        0     5291 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/mainpage.dox
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.959459 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/
--rw-rw-rw-   0        0        0     1301 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/README.md
--rw-rw-rw-   0        0        0     2121 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/header.html
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.971483 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/
--rw-rw-rw-   0        0        0     6714 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/doc.svg
--rw-rw-rw-   0        0        0     3604 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/folderclosed.svg
--rw-rw-rw-   0        0        0     4299 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/folderopen.svg
--rw-rw-rw-   0        0        0     3955 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/mag_glass.svg
--rw-rw-rw-   0        0        0     3988 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg
--rw-rw-rw-   0        0        0     3249 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/nav_edge_left.svg
--rw-rw-rw-   0        0        0     3262 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/nav_edge_right.svg
--rw-rw-rw-   0        0        0     7409 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/splitbar_handle.svg
--rw-rw-rw-   0        0        0      483 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/sync_off.png
--rw-rw-rw-   0        0        0      488 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/sync_on.png
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.981493 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/js/
--rw-rw-rw-   0        0        0      977 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/js/striped_bg.js
--rw-rw-rw-   0        0        0    32455 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/that_style.css
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.021046 pyjoulescope_driver-1.3.2/third-party/cmocka/example/
--rw-rw-rw-   0        0        0     2562 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/CMakeLists.txt
--rw-rw-rw-   0        0        0     1755 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/allocate_module.c
--rw-rw-rw-   0        0        0     1640 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/allocate_module_test.c
--rw-rw-rw-   0        0        0     1254 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_macro.c
--rw-rw-rw-   0        0        0      144 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_macro.h
--rw-rw-rw-   0        0        0     1649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_macro_test.c
--rw-rw-rw-   0        0        0     1216 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_module.c
--rw-rw-rw-   0        0        0      692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_module.h
--rw-rw-rw-   0        0        0     1692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_module_test.c
--rw-rw-rw-   0        0        0     9746 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/calculator.c
--rw-rw-rw-   0        0        0    16244 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/calculator_test.c
--rw-rw-rw-   0        0        0     1439 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/database.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.023546 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/
--rw-rw-rw-   0        0        0      197 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.039056 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/
--rw-rw-rw-   0        0        0      620 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt
--rw-rw-rw-   0        0        0     1431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/chef.c
--rw-rw-rw-   0        0        0      789 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/chef.h
--rw-rw-rw-   0        0        0     5222 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c
--rw-rw-rw-   0        0        0       61 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.056062 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/
--rw-rw-rw-   0        0        0      685 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/CMakeLists.txt
--rw-rw-rw-   0        0        0     2033 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/README.md
--rw-rw-rw-   0        0        0     1882 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/proc_uptime.c
--rw-rw-rw-   0        0        0      793 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/proc_uptime.h
--rw-rw-rw-   0        0        0     5237 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/test_uptime.c
--rw-rw-rw-   0        0        0     3305 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/uptime.c
--rw-rw-rw-   0        0        0      415 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/example/simple_test.c
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.071589 pyjoulescope_driver-1.3.2/third-party/cmocka/include/
--rw-rw-rw-   0        0        0      465 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/include/CMakeLists.txt
--rw-rw-rw-   0        0        0    77952 2022-08-01 20:01:08.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/include/cmocka.h
--rw-rw-rw-   0        0        0     1893 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/include/cmocka_pbc.h
--rw-rw-rw-   0        0        0     4137 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/include/cmocka_private.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.076089 pyjoulescope_driver-1.3.2/third-party/cmocka/include/cmockery/
--rw-rw-rw-   0        0        0       21 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/include/cmockery/cmockery.h
--rw-rw-rw-   0        0        0       25 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/include/cmockery/pbc.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.086099 pyjoulescope_driver-1.3.2/third-party/cmocka/src/
--rw-rw-rw-   0        0        0     3668 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/src/CMakeLists.txt
--rw-rw-rw-   0        0        0   119941 2022-09-18 17:05:56.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/src/cmocka.c
--rw-rw-rw-   0        0        0     1174 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/src/cmocka.def
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.157207 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/
--rw-rw-rw-   0        0        0     7657 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0     6215 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/cmocka_test.cmake
--rw-rw-rw-   0        0        0     2758 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/ctest-default.cmake
--rw-rw-rw-   0        0        0     1922 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_alloc.c
--rw-rw-rw-   0        0        0      818 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_assert_macros.c
--rw-rw-rw-   0        0        0      862 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_assert_macros_fail.c
--rw-rw-rw-   0        0        0     1550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_basics.c
--rw-rw-rw-   0        0        0      970 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_cmockery.c
--rw-rw-rw-   0        0        0      869 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_exception_handler.c
--rw-rw-rw-   0        0        0     1774 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_fixtures.c
--rw-rw-rw-   0        0        0     1206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_float_macros.c
--rw-rw-rw-   0        0        0      992 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_group_fixtures.c
--rw-rw-rw-   0        0        0      699 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_group_setup_assert.c
--rw-rw-rw-   0        0        0      696 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_group_setup_fail.c
--rw-rw-rw-   0        0        0     1757 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_groups.c
--rw-rw-rw-   0        0        0     2767 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_ordering.c
--rw-rw-rw-   0        0        0     2420 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_ordering_fail.c
--rw-rw-rw-   0        0        0     1577 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_returns.c
--rw-rw-rw-   0        0        0     1704 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_returns_fail.c
--rw-rw-rw-   0        0        0     1092 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_setup_fail.c
--rw-rw-rw-   0        0        0     1043 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_skip.c
--rw-rw-rw-   0        0        0     1362 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_skip_filter.c
--rw-rw-rw-   0        0        0     2280 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_strmatch.c
--rw-rw-rw-   0        0        0     1260 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_wildcard.c
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.202256 pyjoulescope_driver-1.3.2/third-party/libusb/
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.203755 pyjoulescope_driver-1.3.2/third-party/libusb/.github/
--rw-rw-rw-   0        0        0      719 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.github/cifuzz.yml
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.211771 pyjoulescope_driver-1.3.2/third-party/libusb/.github/workflows/
--rw-rw-rw-   0        0        0     1188 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.github/workflows/linux.yml
--rw-rw-rw-   0        0        0     1023 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0      527 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.github/workflows/msys2.yml
--rw-rw-rw-   0        0        0      827 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.232292 pyjoulescope_driver-1.3.2/third-party/libusb/.private/
--rw-rw-rw-   0        0        0      202 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.private/README.txt
--rw-rw-rw-   0        0        0      548 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.private/appveyor_build.sh
--rw-rw-rw-   0        0        0     1424 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.private/bm.sh
--rw-rw-rw-   0        0        0     1109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.private/ci-build.sh
--rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.private/ci-container-build.sh
--rw-rw-rw-   0        0        0      959 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.private/post-rewrite.sh
--rw-rw-rw-   0        0        0     1995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.private/pre-commit.sh
--rw-rw-rw-   0        0        0     2545 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.private/wbs.txt
--rw-rw-rw-   0        0        0     1465 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/.travis.yml
--rw-rw-rw-   0        0        0     2523 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.2/third-party/libusb/CMakeLists.txt
--rw-rw-rw-   0        0        0     1972 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/INSTALL_WIN.txt
--rw-rw-rw-   0        0        0     1495 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/Makefile.am
--rw-rw-rw-   0        0        0     1395 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/README-FORK.md
--rw-rw-rw-   0        0        0     1894 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/README.git
--rw-rw-rw-   0        0        0        6 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.254309 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/
--rw-rw-rw-   0        0        0     2409 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/common.xcconfig
--rw-rw-rw-   0        0        0      995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/config.h
--rw-rw-rw-   0        0        0     1135 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/debug.xcconfig
--rw-rw-rw-   0        0        0      988 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/libusb.xcconfig
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.259313 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/libusb.xcodeproj/
--rw-rw-rw-   0        0        0    62286 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj
--rw-rw-rw-   0        0        0      963 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/libusb_debug.xcconfig
--rw-rw-rw-   0        0        0      965 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/libusb_release.xcconfig
--rw-rw-rw-   0        0        0     1208 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/release.xcconfig
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.262814 pyjoulescope_driver-1.3.2/third-party/libusb/android/
--rw-rw-rw-   0        0        0     2016 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/android/config.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.268330 pyjoulescope_driver-1.3.2/third-party/libusb/android/examples/
--rw-rw-rw-   0        0        0    11355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/android/examples/unrooted_android.c
--rw-rw-rw-   0        0        0     1156 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/android/examples/unrooted_android.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.281842 pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/
--rw-rw-rw-   0        0        0      997 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/Android.mk
--rw-rw-rw-   0        0        0     1370 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/Application.mk
--rw-rw-rw-   0        0        0     3425 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/examples.mk
--rw-rw-rw-   0        0        0     2056 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/libusb.mk
--rw-rw-rw-   0        0        0     1355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/tests.mk
--rw-rw-rw-   0        0        0     3820 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/appveyor.yml
--rw-rw-rw-   0        0        0      191 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/autogen.sh
--rw-rw-rw-   0        0        0      109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/bootstrap.sh
--rw-rw-rw-   0        0        0    16514 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/configure.ac
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.287847 pyjoulescope_driver-1.3.2/third-party/libusb/doc/
--rw-rw-rw-   0        0        0      685 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/doc/Makefile.in
--rw-rw-rw-   0        0        0   115647 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/doc/doxygen.cfg.in
--rw-rw-rw-   0        0        0     2923 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/doc/libusb.png
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.315874 pyjoulescope_driver-1.3.2/third-party/libusb/examples/
--rw-rw-rw-   0        0        0      416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/Makefile.am
--rw-rw-rw-   0        0        0    15812 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/dpfp.c
--rw-rw-rw-   0        0        0    24573 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/ezusb.c
--rw-rw-rw-   0        0        0     4247 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/ezusb.h
--rw-rw-rw-   0        0        0     9593 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/fxload.c
--rw-rw-rw-   0        0        0     3580 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/hotplugtest.c
--rw-rw-rw-   0        0        0     2081 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/listdevs.c
--rw-rw-rw-   0        0        0     6149 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/sam3u_benchmark.c
--rw-rw-rw-   0        0        0     9765 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/testlibusb.c
--rw-rw-rw-   0        0        0    40008 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/examples/xusb.c
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:21.584934 pyjoulescope_driver-1.3.2/third-party/libusb/include/
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.319379 pyjoulescope_driver-1.3.2/third-party/libusb/include/linux/
--rw-rw-rw-   0        0        0     5104 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.2/third-party/libusb/include/linux/config.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.322883 pyjoulescope_driver-1.3.2/third-party/libusb/include/macos/
--rw-rw-rw-   0        0        0     5130 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/include/macos/config.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.371437 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/
--rw-rw-rw-   0        0        0     2539 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/Makefile.am
--rw-rw-rw-   0        0        0      780 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/Makefile.am.extra
--rw-rw-rw-   0        0        0    99186 2022-09-20 23:33:57.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/core.c
--rw-rw-rw-   0        0        0    37583 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/descriptor.c
--rw-rw-rw-   0        0        0    15552 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/hotplug.c
--rw-rw-rw-   0        0        0   113897 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/io.c
--rw-rw-rw-   0        0        0     8221 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/libusb-1.0.def
--rw-rw-rw-   0        0        0     1642 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/libusb-1.0.rc
--rw-rw-rw-   0        0        0    78746 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/libusb.h
--rw-rw-rw-   0        0        0    53532 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/libusbi.h
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.459532 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/
--rw-rw-rw-   0        0        0   103226 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/darwin_usb.c
--rw-rw-rw-   0        0        0     7071 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/darwin_usb.h
--rw-rw-rw-   0        0        0    24325 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/emscripten_webusb.cpp
--rw-rw-rw-   0        0        0     9581 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/events_posix.c
--rw-rw-rw-   0        0        0     1776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/events_posix.h
--rw-rw-rw-   0        0        0     6948 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/events_windows.c
--rw-rw-rw-   0        0        0     1520 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/events_windows.h
--rw-rw-rw-   0        0        0     7884 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_pollfs.cpp
--rw-rw-rw-   0        0        0     3386 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_usb.h
--rw-rw-rw-   0        0        0    16687 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_usb_backend.cpp
--rw-rw-rw-   0        0        0     7477 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_usb_raw.cpp
--rw-rw-rw-   0        0        0     4080 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_usb_raw.h
--rw-rw-rw-   0        0        0    10778 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/linux_netlink.c
--rw-rw-rw-   0        0        0     8864 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/linux_udev.c
--rw-rw-rw-   0        0        0    83335 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/linux_usbfs.c
--rw-rw-rw-   0        0        0     6551 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/linux_usbfs.h
--rw-rw-rw-   0        0        0    16279 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/netbsd_usb.c
--rw-rw-rw-   0        0        0     2996 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/null_usb.c
--rw-rw-rw-   0        0        0    18179 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/openbsd_usb.c
--rw-rw-rw-   0        0        0    45204 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/sunos_usb.c
--rw-rw-rw-   0        0        0     2254 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/sunos_usb.h
--rw-rw-rw-   0        0        0     3488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/threads_posix.c
--rw-rw-rw-   0        0        0     3052 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/threads_posix.h
--rw-rw-rw-   0        0        0     1416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/threads_windows.c
--rw-rw-rw-   0        0        0     3280 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/threads_windows.h
--rw-rw-rw-   0        0        0    30524 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_common.c
--rw-rw-rw-   0        0        0    14347 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_common.h
--rw-rw-rw-   0        0        0    24491 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_usbdk.c
--rw-rw-rw-   0        0        0     2926 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_usbdk.h
--rw-rw-rw-   0        0        0   171316 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_winusb.c
--rw-rw-rw-   0        0        0    24670 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_winusb.h
--rw-rw-rw-   0        0        0     8776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/strerror.c
--rw-rw-rw-   0        0        0    13160 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/sync.c
--rw-rw-rw-   0        0        0      449 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/version.h
--rw-rw-rw-   0        0        0       27 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb/version_nano.h
--rw-rw-rw-   0        0        0      323 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/libusb-1.0.pc.in
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.545112 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/
--rw-rw-rw-   0        0        0      136 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/.gitattributes
--rw-rw-rw-   0        0        0     2982 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/Base.props
--rw-rw-rw-   0        0        0      287 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/Configuration.Application.props
--rw-rw-rw-   0        0        0     2817 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/Configuration.Base.props
--rw-rw-rw-   0        0        0      612 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/Configuration.DynamicLibrary.props
--rw-rw-rw-   0        0        0      289 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/Configuration.StaticLibrary.props
--rw-rw-rw-   0        0        0     1438 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/ProjectConfigurations.Base.props
--rw-rw-rw-   0        0        0      713 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/build_all.ps1
--rw-rw-rw-   0        0        0     2007 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/config.h
--rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/dpfp.vcxproj
--rw-rw-rw-   0        0        0     1659 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/dpfp_threaded.vcxproj
--rw-rw-rw-   0        0        0     2125 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/fxload.vcxproj
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.553621 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/getopt/
--rw-rw-rw-   0        0        0    31341 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/getopt/getopt.c
--rw-rw-rw-   0        0        0     6627 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/getopt/getopt.h
--rw-rw-rw-   0        0        0     4708 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/getopt/getopt1.c
--rw-rw-rw-   0        0        0     1522 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/getopt.vcxproj
--rw-rw-rw-   0        0        0     1444 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/hotplugtest.vcxproj
--rw-rw-rw-   0        0        0    17271 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/libusb.sln
--rw-rw-rw-   0        0        0     2762 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/libusb_dll.vcxproj
--rw-rw-rw-   0        0        0     2336 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/libusb_static.vcxproj
--rw-rw-rw-   0        0        0     1441 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/listdevs.vcxproj
--rw-rw-rw-   0        0        0     1488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/sam3u_benchmark.vcxproj
--rw-rw-rw-   0        0        0     1579 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/stress.vcxproj
--rw-rw-rw-   0        0        0     1443 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/testlibusb.vcxproj
--rw-rw-rw-   0        0        0     1709 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/msvc/xusb.vcxproj
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.567639 pyjoulescope_driver-1.3.2/third-party/libusb/tests/
--rw-rw-rw-   0        0        0      623 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/tests/Makefile.am
--rw-rw-rw-   0        0        0     2490 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/tests/libusb_testlib.h
--rw-rw-rw-   0        0        0     4935 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/tests/stress.c
--rw-rw-rw-   0        0        0     4919 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/tests/testlib.c
--rw-rw-rw-   0        0        0    37223 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.2/third-party/libusb/tests/umockdev.c
-drwxrwxrwx   0        0        0        0 2023-04-13 20:57:22.575644 pyjoulescope_driver-1.3.2/third-party/tinyprintf/
--rw-rw-rw-   0        0        0      122 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/tinyprintf/CMakeLists.txt
--rw-rw-rw-   0        0        0    13188 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/tinyprintf/tinyprintf.c
--rw-rw-rw-   0        0        0     6550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/tinyprintf/tinyprintf.h
--rw-rw-rw-   0        0        0     1554 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.2/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.211270 pyjoulescope_driver-1.3.3/
+-rw-rw-rw-   0        0        0     7274 2023-04-19 19:57:15.000000 pyjoulescope_driver-1.3.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjoulescope_driver-1.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      345 2022-11-19 20:38:00.000000 pyjoulescope_driver-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5170 2023-04-19 20:44:27.211270 pyjoulescope_driver-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3360 2023-01-03 21:53:29.000000 pyjoulescope_driver-1.3.3/README.md
+-rw-rw-rw-   0        0        0     6268 2022-09-20 19:25:49.000000 pyjoulescope_driver-1.3.3/credits.html
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.056554 pyjoulescope_driver-1.3.3/include/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.060565 pyjoulescope_driver-1.3.3/include/jsdrv/
+-rw-rw-rw-   0        0        0     2698 2022-11-08 21:41:45.000000 pyjoulescope_driver-1.3.3/include/jsdrv/cmacro_inc.h
+-rw-rw-rw-   0        0        0     8332 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.3/include/jsdrv/cstr.h
+-rw-rw-rw-   0        0        0     5878 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.3/include/jsdrv/error_code.h
+-rw-rw-rw-   0        0        0     6817 2023-04-14 18:25:40.000000 pyjoulescope_driver-1.3.3/include/jsdrv/log.h
+-rw-rw-rw-   0        0        0     2002 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include/jsdrv/meta.h
+-rw-rw-rw-   0        0        0    13833 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include/jsdrv/time.h
+-rw-rw-rw-   0        0        0     3827 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/include/jsdrv/topic.h
+-rw-rw-rw-   0        0        0    12351 2022-08-01 20:41:48.000000 pyjoulescope_driver-1.3.3/include/jsdrv/union.h
+-rw-rw-rw-   0        0        0     4042 2023-04-14 11:59:37.000000 pyjoulescope_driver-1.3.3/include/jsdrv/version.h
+-rw-rw-rw-   0        0        0    29282 2023-04-14 12:30:28.000000 pyjoulescope_driver-1.3.3/include/jsdrv.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.060565 pyjoulescope_driver-1.3.3/include_private/
+-rw-rw-rw-   0        0        0    13394 2022-10-27 14:05:41.000000 pyjoulescope_driver-1.3.3/include_private/js220_api.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.074586 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/
+-rw-rw-rw-   0        0        0     1683 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/assert.h
+-rw-rw-rw-   0        0        0     2116 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/backend.h
+-rw-rw-rw-   0        0        0     2774 2023-04-12 17:01:55.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/buffer.h
+-rw-rw-rw-   0        0        0     3935 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/buffer_signal.h
+-rw-rw-rw-   0        0        0     7138 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/cdef.h
+-rw-rw-rw-   0        0        0     5647 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/dbc.h
+-rw-rw-rw-   0        0        0     1385 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/device.h
+-rw-rw-rw-   0        0        0     1291 2022-07-28 13:15:21.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/devices.h
+-rw-rw-rw-   0        0        0     1633 2022-10-23 16:50:55.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/downsample.h
+-rw-rw-rw-   0        0        0     1960 2022-09-19 13:38:02.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/event.h
+-rw-rw-rw-   0        0        0     6987 2023-03-19 15:49:32.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/frontend.h
+-rw-rw-rw-   0        0        0     1408 2022-08-01 19:59:27.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_cal.h
+-rw-rw-rw-   0        0        0     3046 2022-11-01 14:07:32.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_sample_processor.h
+-rw-rw-rw-   0        0        0     2858 2022-11-01 15:41:07.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_stats.h
+-rw-rw-rw-   0        0        0     1647 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js220_i128.h
+-rw-rw-rw-   0        0        0     1558 2022-10-04 22:55:17.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js220_stats.h
+-rw-rw-rw-   0        0        0     3780 2022-08-01 13:11:32.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/json.h
+-rw-rw-rw-   0        0        0    14035 2022-09-18 11:31:10.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/list.h
+-rw-rw-rw-   0        0        0     8973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/log.h
+-rw-rw-rw-   0        0        0     1650 2022-09-19 12:36:34.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/msg_queue.h
+-rw-rw-rw-   0        0        0     2561 2022-07-28 13:01:35.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/mutex.h
+-rw-rw-rw-   0        0        0     5093 2023-04-14 19:17:27.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/platform.h
+-rw-rw-rw-   0        0        0     4061 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/pubsub.h
+-rw-rw-rw-   0        0        0     2799 2022-10-07 12:17:37.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/sample_buffer_f32.h
+-rw-rw-rw-   0        0        0     4561 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/statistics.h
+-rw-rw-rw-   0        0        0     1939 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/thread.h
+-rw-rw-rw-   0        0        0     8210 2022-07-29 18:34:03.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/usb_spec.h
+-rw-rw-rw-   0        0        0     1533 2022-10-09 18:53:30.000000 pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/windows.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.081605 pyjoulescope_driver-1.3.3/pyjoulescope_driver/
+-rw-rw-rw-   0        0        0      964 2023-03-29 21:30:50.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-03-29 21:47:21.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/__main__.py
+-rw-rw-rw-   0        0        0  1592888 2023-04-19 20:28:54.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/binding.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.091619 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/
+-rw-rw-rw-   0        0        0      987 2023-04-14 12:52:01.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-04-14 19:51:53.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/api_timeout.py
+-rw-rw-rw-   0        0        0     1830 2023-01-25 14:57:14.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/gpi.py
+-rw-rw-rw-   0        0        0     3702 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/info.py
+-rw-rw-rw-   0        0        0     4213 2022-10-30 15:18:19.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/program.py
+-rw-rw-rw-   0        0        0     5031 2023-04-13 12:02:12.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/record.py
+-rw-rw-rw-   0        0        0      932 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/scan.py
+-rw-rw-rw-   0        0        0     2410 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/set_parameter.py
+-rw-rw-rw-   0        0        0     2981 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/statistics.py
+-rw-rw-rw-   0        0        0     3723 2023-04-14 13:21:57.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/threads.py
+-rw-rw-rw-   0        0        0   609280 2023-04-19 20:44:25.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_alpha.img
+-rw-rw-rw-   0        0        0   609280 2023-04-19 20:44:25.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_beta.img
+-rw-rw-rw-   0        0        0   609280 2023-04-19 20:44:25.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_stable.img
+-rw-rw-rw-   0        0        0    10359 2023-04-15 14:37:51.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/program.py
+-rw-rw-rw-   0        0        0     8508 2023-04-14 15:05:28.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/record.py
+-rw-rw-rw-   0        0        0     8980 2022-11-11 19:24:16.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/release.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.092619 pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/
+-rw-rw-rw-   0        0        0        0 2022-10-09 12:38:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/__init__.py
+-rw-rw-rw-   0        0        0     1901 2022-10-09 17:17:09.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/test_release.py
+-rw-rw-rw-   0        0        0     2304 2023-03-29 16:02:01.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/test_time64.py
+-rw-rw-rw-   0        0        0     4660 2023-03-29 16:00:59.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/time64.py
+-rw-rw-rw-   0        0        0     1063 2023-04-14 11:59:37.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver/version.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.087612 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/
+-rw-rw-rw-   0        0        0     5170 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13694 2023-04-19 20:44:27.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-19 20:44:26.000000 pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      868 2022-11-30 13:52:01.000000 pyjoulescope_driver-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0      117 2023-04-19 20:44:27.216777 pyjoulescope_driver-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0    10610 2023-04-14 19:59:13.000000 pyjoulescope_driver-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.105631 pyjoulescope_driver-1.3.3/src/
+-rw-rw-rw-   0        0        0     2655 2023-04-14 19:59:17.000000 pyjoulescope_driver-1.3.3/src/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.108138 pyjoulescope_driver-1.3.3/src/backend/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.109138 pyjoulescope_driver-1.3.3/src/backend/libusb/
+-rw-rw-rw-   0        0        0    30330 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/src/backend/libusb/backend.c
+-rw-rw-rw-   0        0        0     4580 2022-09-19 12:40:12.000000 pyjoulescope_driver-1.3.3/src/backend/libusb/msg_queue.c
+-rw-rw-rw-   0        0        0     5503 2023-04-14 20:55:21.000000 pyjoulescope_driver-1.3.3/src/backend/posix.c
+-rw-rw-rw-   0        0        0     6886 2023-04-14 20:54:20.000000 pyjoulescope_driver-1.3.3/src/backend/windows.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.109138 pyjoulescope_driver-1.3.3/src/backend/winusb/
+-rw-rw-rw-   0        0        0    38641 2023-04-04 15:07:16.000000 pyjoulescope_driver-1.3.3/src/backend/winusb/backend.c
+-rw-rw-rw-   0        0        0     7713 2022-09-18 12:51:07.000000 pyjoulescope_driver-1.3.3/src/backend/winusb/device_change_notifier.c
+-rw-rw-rw-   0        0        0     2798 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/backend/winusb/device_change_notifier.h
+-rw-rw-rw-   0        0        0     4807 2023-03-19 16:29:53.000000 pyjoulescope_driver-1.3.3/src/backend/winusb/msg_queue.c
+-rw-rw-rw-   0        0        0    25596 2023-03-15 17:50:15.000000 pyjoulescope_driver-1.3.3/src/buffer.c
+-rw-rw-rw-   0        0        0    32515 2023-03-30 18:49:53.000000 pyjoulescope_driver-1.3.3/src/buffer_signal.c
+-rw-rw-rw-   0        0        0    11771 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/cstr.c
+-rw-rw-rw-   0        0        0     1671 2022-09-19 11:52:36.000000 pyjoulescope_driver-1.3.3/src/devices.c
+-rw-rw-rw-   0        0        0     8709 2022-10-24 15:34:41.000000 pyjoulescope_driver-1.3.3/src/downsample.c
+-rw-rw-rw-   0        0        0     5925 2022-07-28 14:45:35.000000 pyjoulescope_driver-1.3.3/src/emu.c
+-rw-rw-rw-   0        0        0     4649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/emulated.c
+-rw-rw-rw-   0        0        0     4817 2022-08-01 20:21:28.000000 pyjoulescope_driver-1.3.3/src/error_code.c
+-rw-rw-rw-   0        0        0     9335 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/js110_api.h
+-rw-rw-rw-   0        0        0     3972 2022-09-18 11:26:57.000000 pyjoulescope_driver-1.3.3/src/js110_cal.c
+-rw-rw-rw-   0        0        0     9038 2022-11-01 14:07:47.000000 pyjoulescope_driver-1.3.3/src/js110_sample_processor.c
+-rw-rw-rw-   0        0        0     4551 2022-12-19 21:27:23.000000 pyjoulescope_driver-1.3.3/src/js110_stats.c
+-rw-rw-rw-   0        0        0    52566 2023-04-19 20:14:10.000000 pyjoulescope_driver-1.3.3/src/js110_usb.c
+-rw-rw-rw-   0        0        0     5162 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/src/js220_i128.c
+-rw-rw-rw-   0        0        0     1188 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/src/js220_params.c
+-rw-rw-rw-   0        0        0     2893 2022-10-05 01:35:24.000000 pyjoulescope_driver-1.3.3/src/js220_stats.c
+-rw-rw-rw-   0        0        0    62891 2023-04-14 13:07:09.000000 pyjoulescope_driver-1.3.3/src/js220_usb.c
+-rw-rw-rw-   0        0        0    37782 2023-04-14 12:55:05.000000 pyjoulescope_driver-1.3.3/src/jsdrv.c
+-rw-rw-rw-   0        0        0    10974 2022-08-01 18:37:59.000000 pyjoulescope_driver-1.3.3/src/json.c
+-rw-rw-rw-   0        0        0    16499 2023-04-14 20:57:15.000000 pyjoulescope_driver-1.3.3/src/log.c
+-rw-rw-rw-   0        0        0    10627 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/src/meta.c
+-rw-rw-rw-   0        0        0    24211 2023-03-19 15:32:24.000000 pyjoulescope_driver-1.3.3/src/pubsub.c
+-rw-rw-rw-   0        0        0     4944 2022-10-07 12:24:15.000000 pyjoulescope_driver-1.3.3/src/sample_buffer_f32.c
+-rw-rw-rw-   0        0        0     5262 2023-03-09 18:16:24.000000 pyjoulescope_driver-1.3.3/src/statistics.c
+-rw-rw-rw-   0        0        0     2814 2023-03-09 19:53:59.000000 pyjoulescope_driver-1.3.3/src/time.c
+-rw-rw-rw-   0        0        0     3763 2022-09-02 14:38:38.000000 pyjoulescope_driver-1.3.3/src/topic.c
+-rw-rw-rw-   0        0        0    12780 2022-09-18 11:32:07.000000 pyjoulescope_driver-1.3.3/src/union.c
+-rw-rw-rw-   0        0        0     1001 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/src/version.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.110646 pyjoulescope_driver-1.3.3/third-party/
+-rw-rw-rw-   0        0        0      810 2022-09-20 18:21:09.000000 pyjoulescope_driver-1.3.3/third-party/CMakeLists.txt
+-rw-rw-rw-   0        0        0      364 2022-08-01 20:40:07.000000 pyjoulescope_driver-1.3.3/third-party/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.117149 pyjoulescope_driver-1.3.3/third-party/cmocka/
+-rw-rw-rw-   0        0        0       18 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/.clang_complete
+-rw-rw-rw-   0        0        0     9611 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0     3508 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/.ycm_extra_conf.py
+-rw-rw-rw-   0        0        0     1209 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/5.patch
+-rw-rw-rw-   0        0        0     3601 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1845 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/CPackConfig.cmake
+-rw-rw-rw-   0        0        0      284 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/CTestConfig.cmake
+-rw-rw-rw-   0        0        0     5331 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/CompilerChecks.cmake
+-rw-rw-rw-   0        0        0     4648 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/ConfigureChecks.cmake
+-rw-rw-rw-   0        0        0      431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/DefineOptions.cmake
+-rw-rw-rw-   0        0        0     3217 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/INSTALL.md
+-rw-rw-rw-   0        0        0      658 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.118151 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.121677 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/
+-rw-rw-rw-   0        0        0      866 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake
+-rw-rw-rw-   0        0        0     3360 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake
+-rw-rw-rw-   0        0        0     1952 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake
+-rw-rw-rw-   0        0        0      811 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake
+-rw-rw-rw-   0        0        0     3973 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake
+-rw-rw-rw-   0        0        0      585 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake
+-rw-rw-rw-   0        0        0     1480 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/FindNSIS.cmake
+-rw-rw-rw-   0        0        0      680 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake
+-rw-rw-rw-   0        0        0      656 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake
+-rw-rw-rw-   0        0        0     1145 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Toolchain-cross-m32.cmake
+-rw-rw-rw-   0        0        0       53 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmocka-build-tree-settings.cmake.in
+-rw-rw-rw-   0        0        0      507 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmocka-config.cmake.in
+-rw-rw-rw-   0        0        0      189 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/cmocka.pc.cmake
+-rw-rw-rw-   0        0        0     5161 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/config.h.cmake
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.122677 pyjoulescope_driver-1.3.3/third-party/cmocka/coverity/
+-rw-rw-rw-   0        0        0     3918 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/coverity/coverity_assert_model.c
+-rw-rw-rw-   0        0        0      142 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/coverity/coverity_internal_model.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.123677 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/
+-rw-rw-rw-   0        0        0     2206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/CMakeLists.txt
+-rw-rw-rw-   0        0        0    26974 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/index.html
+-rw-rw-rw-   0        0        0     5291 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/mainpage.dox
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.125177 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/
+-rw-rw-rw-   0        0        0     1301 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/README.md
+-rw-rw-rw-   0        0        0     2121 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/header.html
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.129185 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/
+-rw-rw-rw-   0        0        0     6714 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/doc.svg
+-rw-rw-rw-   0        0        0     3604 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/folderclosed.svg
+-rw-rw-rw-   0        0        0     4299 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/folderopen.svg
+-rw-rw-rw-   0        0        0     3955 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/mag_glass.svg
+-rw-rw-rw-   0        0        0     3988 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg
+-rw-rw-rw-   0        0        0     3249 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_left.svg
+-rw-rw-rw-   0        0        0     3262 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_right.svg
+-rw-rw-rw-   0        0        0     7409 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/splitbar_handle.svg
+-rw-rw-rw-   0        0        0      483 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/sync_off.png
+-rw-rw-rw-   0        0        0      488 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/sync_on.png
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.129685 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/js/
+-rw-rw-rw-   0        0        0      977 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/js/striped_bg.js
+-rw-rw-rw-   0        0        0    32455 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/that_style.css
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.135692 pyjoulescope_driver-1.3.3/third-party/cmocka/example/
+-rw-rw-rw-   0        0        0     2562 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1755 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/allocate_module.c
+-rw-rw-rw-   0        0        0     1640 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/allocate_module_test.c
+-rw-rw-rw-   0        0        0     1254 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro.c
+-rw-rw-rw-   0        0        0      144 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro.h
+-rw-rw-rw-   0        0        0     1649 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro_test.c
+-rw-rw-rw-   0        0        0     1216 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module.c
+-rw-rw-rw-   0        0        0      692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module.h
+-rw-rw-rw-   0        0        0     1692 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module_test.c
+-rw-rw-rw-   0        0        0     9746 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/calculator.c
+-rw-rw-rw-   0        0        0    16244 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/calculator_test.c
+-rw-rw-rw-   0        0        0     1439 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/database.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.136192 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/
+-rw-rw-rw-   0        0        0      197 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.137691 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/
+-rw-rw-rw-   0        0        0      620 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1431 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/chef.c
+-rw-rw-rw-   0        0        0      789 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/chef.h
+-rw-rw-rw-   0        0        0     5222 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c
+-rw-rw-rw-   0        0        0       61 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.140197 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/
+-rw-rw-rw-   0        0        0      685 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/CMakeLists.txt
+-rw-rw-rw-   0        0        0     2033 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/README.md
+-rw-rw-rw-   0        0        0     1882 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/proc_uptime.c
+-rw-rw-rw-   0        0        0      793 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/proc_uptime.h
+-rw-rw-rw-   0        0        0     5237 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/test_uptime.c
+-rw-rw-rw-   0        0        0     3305 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/uptime.c
+-rw-rw-rw-   0        0        0      415 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/example/simple_test.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.142206 pyjoulescope_driver-1.3.3/third-party/cmocka/include/
+-rw-rw-rw-   0        0        0      465 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/CMakeLists.txt
+-rw-rw-rw-   0        0        0    77952 2022-08-01 20:01:08.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka.h
+-rw-rw-rw-   0        0        0     1893 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka_pbc.h
+-rw-rw-rw-   0        0        0     4137 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka_private.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.142705 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmockery/
+-rw-rw-rw-   0        0        0       21 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmockery/cmockery.h
+-rw-rw-rw-   0        0        0       25 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmockery/pbc.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.144204 pyjoulescope_driver-1.3.3/third-party/cmocka/src/
+-rw-rw-rw-   0        0        0     3668 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/src/CMakeLists.txt
+-rw-rw-rw-   0        0        0   119941 2022-09-18 17:05:56.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/src/cmocka.c
+-rw-rw-rw-   0        0        0     1174 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/src/cmocka.def
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.154711 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/
+-rw-rw-rw-   0        0        0     7657 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0     6215 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/cmocka_test.cmake
+-rw-rw-rw-   0        0        0     2758 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/ctest-default.cmake
+-rw-rw-rw-   0        0        0     1922 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_alloc.c
+-rw-rw-rw-   0        0        0      818 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_assert_macros.c
+-rw-rw-rw-   0        0        0      862 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_assert_macros_fail.c
+-rw-rw-rw-   0        0        0     1550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_basics.c
+-rw-rw-rw-   0        0        0      970 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_cmockery.c
+-rw-rw-rw-   0        0        0      869 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_exception_handler.c
+-rw-rw-rw-   0        0        0     1774 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_fixtures.c
+-rw-rw-rw-   0        0        0     1206 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_float_macros.c
+-rw-rw-rw-   0        0        0      992 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_fixtures.c
+-rw-rw-rw-   0        0        0      699 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_setup_assert.c
+-rw-rw-rw-   0        0        0      696 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_setup_fail.c
+-rw-rw-rw-   0        0        0     1757 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_groups.c
+-rw-rw-rw-   0        0        0     2767 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_ordering.c
+-rw-rw-rw-   0        0        0     2420 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_ordering_fail.c
+-rw-rw-rw-   0        0        0     1577 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_returns.c
+-rw-rw-rw-   0        0        0     1704 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_returns_fail.c
+-rw-rw-rw-   0        0        0     1092 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_setup_fail.c
+-rw-rw-rw-   0        0        0     1043 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_skip.c
+-rw-rw-rw-   0        0        0     1362 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_skip_filter.c
+-rw-rw-rw-   0        0        0     2280 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_strmatch.c
+-rw-rw-rw-   0        0        0     1260 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_wildcard.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.158712 pyjoulescope_driver-1.3.3/third-party/libusb/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.159716 pyjoulescope_driver-1.3.3/third-party/libusb/.github/
+-rw-rw-rw-   0        0        0      719 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.github/cifuzz.yml
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.161220 pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/
+-rw-rw-rw-   0        0        0     1188 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/linux.yml
+-rw-rw-rw-   0        0        0     1023 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0      527 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/msys2.yml
+-rw-rw-rw-   0        0        0      827 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.164719 pyjoulescope_driver-1.3.3/third-party/libusb/.private/
+-rw-rw-rw-   0        0        0      202 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/README.txt
+-rw-rw-rw-   0        0        0      548 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/appveyor_build.sh
+-rw-rw-rw-   0        0        0     1424 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/bm.sh
+-rw-rw-rw-   0        0        0     1109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/ci-build.sh
+-rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/ci-container-build.sh
+-rw-rw-rw-   0        0        0      959 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/post-rewrite.sh
+-rw-rw-rw-   0        0        0     1995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/pre-commit.sh
+-rw-rw-rw-   0        0        0     2545 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.private/wbs.txt
+-rw-rw-rw-   0        0        0     1465 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/.travis.yml
+-rw-rw-rw-   0        0        0     2523 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.3/third-party/libusb/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1972 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/INSTALL_WIN.txt
+-rw-rw-rw-   0        0        0     1495 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Makefile.am
+-rw-rw-rw-   0        0        0     1395 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/README-FORK.md
+-rw-rw-rw-   0        0        0     1894 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/README.git
+-rw-rw-rw-   0        0        0        6 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.167719 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/
+-rw-rw-rw-   0        0        0     2409 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/common.xcconfig
+-rw-rw-rw-   0        0        0      995 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/config.h
+-rw-rw-rw-   0        0        0     1135 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/debug.xcconfig
+-rw-rw-rw-   0        0        0      988 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcconfig
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.168219 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcodeproj/
+-rw-rw-rw-   0        0        0    62286 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj
+-rw-rw-rw-   0        0        0      963 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb_debug.xcconfig
+-rw-rw-rw-   0        0        0      965 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb_release.xcconfig
+-rw-rw-rw-   0        0        0     1208 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/release.xcconfig
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.168219 pyjoulescope_driver-1.3.3/third-party/libusb/android/
+-rw-rw-rw-   0        0        0     2016 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/config.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.169219 pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/
+-rw-rw-rw-   0        0        0    11355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/unrooted_android.c
+-rw-rw-rw-   0        0        0     1156 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/unrooted_android.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.171225 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/
+-rw-rw-rw-   0        0        0      997 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/Android.mk
+-rw-rw-rw-   0        0        0     1370 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/Application.mk
+-rw-rw-rw-   0        0        0     3425 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/examples.mk
+-rw-rw-rw-   0        0        0     2056 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/libusb.mk
+-rw-rw-rw-   0        0        0     1355 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/tests.mk
+-rw-rw-rw-   0        0        0     3820 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/appveyor.yml
+-rw-rw-rw-   0        0        0      191 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/autogen.sh
+-rw-rw-rw-   0        0        0      109 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/bootstrap.sh
+-rw-rw-rw-   0        0        0    16514 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/configure.ac
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.172225 pyjoulescope_driver-1.3.3/third-party/libusb/doc/
+-rw-rw-rw-   0        0        0      685 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/doc/Makefile.in
+-rw-rw-rw-   0        0        0   115647 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/doc/doxygen.cfg.in
+-rw-rw-rw-   0        0        0     2923 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/doc/libusb.png
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.176726 pyjoulescope_driver-1.3.3/third-party/libusb/examples/
+-rw-rw-rw-   0        0        0      416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/Makefile.am
+-rw-rw-rw-   0        0        0    15812 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/dpfp.c
+-rw-rw-rw-   0        0        0    24573 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/ezusb.c
+-rw-rw-rw-   0        0        0     4247 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/ezusb.h
+-rw-rw-rw-   0        0        0     9593 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/fxload.c
+-rw-rw-rw-   0        0        0     3580 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/hotplugtest.c
+-rw-rw-rw-   0        0        0     2081 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/listdevs.c
+-rw-rw-rw-   0        0        0     6149 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/sam3u_benchmark.c
+-rw-rw-rw-   0        0        0     9765 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/testlibusb.c
+-rw-rw-rw-   0        0        0    40008 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/examples/xusb.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.052046 pyjoulescope_driver-1.3.3/third-party/libusb/include/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.176726 pyjoulescope_driver-1.3.3/third-party/libusb/include/linux/
+-rw-rw-rw-   0        0        0     5104 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.3/third-party/libusb/include/linux/config.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.177226 pyjoulescope_driver-1.3.3/third-party/libusb/include/macos/
+-rw-rw-rw-   0        0        0     5130 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/include/macos/config.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.183734 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/
+-rw-rw-rw-   0        0        0     2539 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/Makefile.am
+-rw-rw-rw-   0        0        0      780 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/Makefile.am.extra
+-rw-rw-rw-   0        0        0    99186 2022-09-20 23:33:57.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/core.c
+-rw-rw-rw-   0        0        0    37583 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/descriptor.c
+-rw-rw-rw-   0        0        0    15552 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/hotplug.c
+-rw-rw-rw-   0        0        0   113897 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/io.c
+-rw-rw-rw-   0        0        0     8221 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb-1.0.def
+-rw-rw-rw-   0        0        0     1642 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb-1.0.rc
+-rw-rw-rw-   0        0        0    78746 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb.h
+-rw-rw-rw-   0        0        0    53532 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusbi.h
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.197249 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/
+-rw-rw-rw-   0        0        0   103226 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/darwin_usb.c
+-rw-rw-rw-   0        0        0     7071 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/darwin_usb.h
+-rw-rw-rw-   0        0        0    24325 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/emscripten_webusb.cpp
+-rw-rw-rw-   0        0        0     9581 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_posix.c
+-rw-rw-rw-   0        0        0     1776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_posix.h
+-rw-rw-rw-   0        0        0     6948 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_windows.c
+-rw-rw-rw-   0        0        0     1520 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_windows.h
+-rw-rw-rw-   0        0        0     7884 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_pollfs.cpp
+-rw-rw-rw-   0        0        0     3386 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb.h
+-rw-rw-rw-   0        0        0    16687 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_backend.cpp
+-rw-rw-rw-   0        0        0     7477 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_raw.cpp
+-rw-rw-rw-   0        0        0     4080 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_raw.h
+-rw-rw-rw-   0        0        0    10778 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_netlink.c
+-rw-rw-rw-   0        0        0     8864 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_udev.c
+-rw-rw-rw-   0        0        0    83335 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_usbfs.c
+-rw-rw-rw-   0        0        0     6551 2022-09-20 20:43:20.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_usbfs.h
+-rw-rw-rw-   0        0        0    16279 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/netbsd_usb.c
+-rw-rw-rw-   0        0        0     2996 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/null_usb.c
+-rw-rw-rw-   0        0        0    18179 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/openbsd_usb.c
+-rw-rw-rw-   0        0        0    45204 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/sunos_usb.c
+-rw-rw-rw-   0        0        0     2254 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/sunos_usb.h
+-rw-rw-rw-   0        0        0     3488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_posix.c
+-rw-rw-rw-   0        0        0     3052 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_posix.h
+-rw-rw-rw-   0        0        0     1416 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_windows.c
+-rw-rw-rw-   0        0        0     3280 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_windows.h
+-rw-rw-rw-   0        0        0    30524 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_common.c
+-rw-rw-rw-   0        0        0    14347 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_common.h
+-rw-rw-rw-   0        0        0    24491 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_usbdk.c
+-rw-rw-rw-   0        0        0     2926 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_usbdk.h
+-rw-rw-rw-   0        0        0   171316 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_winusb.c
+-rw-rw-rw-   0        0        0    24670 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_winusb.h
+-rw-rw-rw-   0        0        0     8776 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/strerror.c
+-rw-rw-rw-   0        0        0    13160 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/sync.c
+-rw-rw-rw-   0        0        0      449 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/version.h
+-rw-rw-rw-   0        0        0       27 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb/version_nano.h
+-rw-rw-rw-   0        0        0      323 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/libusb-1.0.pc.in
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.206762 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/
+-rw-rw-rw-   0        0        0      136 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/.gitattributes
+-rw-rw-rw-   0        0        0     2982 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Base.props
+-rw-rw-rw-   0        0        0      287 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.Application.props
+-rw-rw-rw-   0        0        0     2817 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.Base.props
+-rw-rw-rw-   0        0        0      612 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.DynamicLibrary.props
+-rw-rw-rw-   0        0        0      289 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.StaticLibrary.props
+-rw-rw-rw-   0        0        0     1438 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/ProjectConfigurations.Base.props
+-rw-rw-rw-   0        0        0      713 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/build_all.ps1
+-rw-rw-rw-   0        0        0     2007 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/config.h
+-rw-rw-rw-   0        0        0     1474 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/dpfp.vcxproj
+-rw-rw-rw-   0        0        0     1659 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/dpfp_threaded.vcxproj
+-rw-rw-rw-   0        0        0     2125 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/fxload.vcxproj
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.207762 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/
+-rw-rw-rw-   0        0        0    31341 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt.c
+-rw-rw-rw-   0        0        0     6627 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt.h
+-rw-rw-rw-   0        0        0     4708 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt1.c
+-rw-rw-rw-   0        0        0     1522 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt.vcxproj
+-rw-rw-rw-   0        0        0     1444 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/hotplugtest.vcxproj
+-rw-rw-rw-   0        0        0    17271 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb.sln
+-rw-rw-rw-   0        0        0     2762 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb_dll.vcxproj
+-rw-rw-rw-   0        0        0     2336 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb_static.vcxproj
+-rw-rw-rw-   0        0        0     1441 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/listdevs.vcxproj
+-rw-rw-rw-   0        0        0     1488 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/sam3u_benchmark.vcxproj
+-rw-rw-rw-   0        0        0     1579 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/stress.vcxproj
+-rw-rw-rw-   0        0        0     1443 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/testlibusb.vcxproj
+-rw-rw-rw-   0        0        0     1709 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/msvc/xusb.vcxproj
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.209263 pyjoulescope_driver-1.3.3/third-party/libusb/tests/
+-rw-rw-rw-   0        0        0      623 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/Makefile.am
+-rw-rw-rw-   0        0        0     2490 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/libusb_testlib.h
+-rw-rw-rw-   0        0        0     4935 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/stress.c
+-rw-rw-rw-   0        0        0     4919 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/testlib.c
+-rw-rw-rw-   0        0        0    37223 2022-09-20 18:20:07.000000 pyjoulescope_driver-1.3.3/third-party/libusb/tests/umockdev.c
+drwxrwxrwx   0        0        0        0 2023-04-19 20:44:27.211270 pyjoulescope_driver-1.3.3/third-party/tinyprintf/
+-rw-rw-rw-   0        0        0      122 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/tinyprintf/CMakeLists.txt
+-rw-rw-rw-   0        0        0    13188 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf.c
+-rw-rw-rw-   0        0        0     6550 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf.h
+-rw-rw-rw-   0        0        0     1554 2022-07-26 15:46:29.000000 pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new
```

### Comparing `pyjoulescope_driver-1.3.2/CHANGELOG.md` & `pyjoulescope_driver-1.3.3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the Joulescope driver.
 
 
+## 1.3.3
+
+2023 Apr 19
+
+* Cleared all message fields at allocation.
+* Added api_timeout entry point test.
+* Improved thread entry point test.
+* Reordered unsubscribe to ensure callback validity.
+* Added malloc/free mutex for guaranteed thread safety.
+* Added runtime pyjls version check.
+* Improved logging robustness and thread safety.
+* Fixed JS110 open causing IN+ to OUT+ disconnect.
+* Added JS110 open modes: defaults, resume.
+
+
 ## 1.3.2
 
 2023 Apr 13
 
 * Improved record close error handling.
 * Added JS220 streaming data ignore when device not open.
 * Improved record entry point.
```

### Comparing `pyjoulescope_driver-1.3.2/LICENSE.txt` & `pyjoulescope_driver-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/PKG-INFO` & `pyjoulescope_driver-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoulescope_driver
-Version: 1.3.2
+Version: 1.3.3
 Summary: Joulescope™ driver
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjoulescope_driver-1.3.2/README.md` & `pyjoulescope_driver-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/credits.html` & `pyjoulescope_driver-1.3.3/credits.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv/cmacro_inc.h` & `pyjoulescope_driver-1.3.3/include/jsdrv/cmacro_inc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv/cstr.h` & `pyjoulescope_driver-1.3.3/include/jsdrv/cstr.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv/error_code.h` & `pyjoulescope_driver-1.3.3/include/jsdrv/error_code.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv/log.h` & `pyjoulescope_driver-1.3.3/include/jsdrv/log.h`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     /// The jsdrv_log_level_e.
     uint8_t level;
     uint8_t rsvu8_1;    ///< reserved u8 for future use
     uint8_t rsvu8_2;    ///< reserved u8 for future use
     /// The originating file line number number.
     uint32_t line;
     /// The Joulescope driver UTC time.
-    uint64_t timestamp;
+    int64_t timestamp;
 };
 
 /**
  * @brief Receive a log message.
  *
  * @param user_data The arbitrary user data.
  * @param header The log record header.
```

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv/meta.h` & `pyjoulescope_driver-1.3.3/include/jsdrv/meta.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv/time.h` & `pyjoulescope_driver-1.3.3/include/jsdrv/time.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv/topic.h` & `pyjoulescope_driver-1.3.3/include/jsdrv/topic.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv/union.h` & `pyjoulescope_driver-1.3.3/include/jsdrv/union.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv/version.h` & `pyjoulescope_driver-1.3.3/include/jsdrv/version.h`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 #define JSDRV_VERSION_MINOR 3
 
 /**
  * @brief The Joulescope driver patch version.
  *
  * Changes in the patch version indicate bug fixes and improvements.
  */
-#define JSDRV_VERSION_PATCH 2
+#define JSDRV_VERSION_PATCH 3
 
 /**
  * \brief The maximum version string length.
  *
  * The actual length is 14 bytes (MMM.mmm.ppppp\\x00), but round up
  * to simplify packing.
  */
```

### Comparing `pyjoulescope_driver-1.3.2/include/jsdrv.h` & `pyjoulescope_driver-1.3.3/include/jsdrv.h`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
 #define JSDRV_MSG_COMMAND_PREFIX_CHAR   '@'             ///< Topic command prefix character
 #define JSDRV_MSG_DEVICE_ADD            "@/!add"        ///< Device added: subscribe only (published automatically)
 #define JSDRV_MSG_DEVICE_REMOVE         "@/!remove"     ///< Device removed: subscribe only (published automatically)
 #define JSDRV_MSG_DEVICE_LIST           "@/list"        ///< Device list: subscribe only comma-separated device list, updated with each add & remove
 #define JSDRV_MSG_INITIALIZE            "@/!init"       // CAUTION: internal use only
 #define JSDRV_MSG_FINALIZE              "@/!final"      // CAUTION: internal use only
 #define JSDRV_MSG_VERSION               "@/version"     ///< Driver version: subscribe only JSDRV version (u32)
+#define JSDRV_MSG_TIMEOUT               "@/timeout"     ///< UnhandledDriver version: subscribe only JSDRV version (u32)
 
 
 // device-specific commands in format {device}/{command}
 #define JSDRV_MSG_OPEN                  "@/!open"       ///< Device open: use only with device prefix
 #define JSDRV_MSG_CLOSE                 "@/!close"      ///< Device close: use only with device prefix
 
 /** @} */
```

### Comparing `pyjoulescope_driver-1.3.2/include_private/js220_api.h` & `pyjoulescope_driver-1.3.3/include_private/js220_api.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/assert.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/assert.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/backend.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/backend.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/buffer.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/buffer.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/buffer_signal.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/buffer_signal.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/cdef.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/dbc.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/dbc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/device.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/device.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/devices.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/devices.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/downsample.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/downsample.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/event.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/event.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/frontend.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/frontend.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js110_cal.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_cal.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js110_sample_processor.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_sample_processor.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js110_stats.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js110_stats.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js220_i128.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js220_i128.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/js220_stats.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/js220_stats.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/json.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/json.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/list.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/list.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/log.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/log.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/msg_queue.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/msg_queue.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/mutex.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/mutex.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/platform.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/platform.h`

 * *Files 2% similar despite different names*

```diff
@@ -95,35 +95,27 @@
 }
 
 /**
  * \brief Function to deallocate memory provided by jsdrv_alloc() or jsdrv_alloc_clr().
  *
  * \param ptr The pointer to the memory to free.
  */
-JSDRV_INLINE_FN void jsdrv_free(void * ptr) {
-    free(ptr);
-}
+void jsdrv_free(void * ptr);
 
 /**
  * @brief Allocate memory from the heap.
  *
  * @param size_bytes The number of total_bytes to allocate.
  * @return The pointer to the allocated memory.
  *
  * This function will assert on out of memory conditions.
  * For platforms that support freeing memory, use jsdrv_free() to return the
  * memory to the heap.
  */
-JSDRV_COMPILER_ALLOC(jsdrv_free) JSDRV_INLINE_FN void * jsdrv_alloc(size_t size_bytes) {
-    void * ptr = malloc(size_bytes);
-    if (!ptr) {
-        JSDRV_FATAL("out of memory");
-    }
-    return ptr;
-}
+JSDRV_COMPILER_ALLOC(jsdrv_free) void * jsdrv_alloc(size_t size_bytes);
 
 /**
  * @brief Allocate memory from the heap and clear to 0.
  *
  * @param size_bytes The number of total_bytes to allocate.
  * @return The pointer to the allocated memory.
  *
```

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/pubsub.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/pubsub.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/sample_buffer_f32.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/sample_buffer_f32.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/statistics.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/thread.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/thread.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/usb_spec.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/usb_spec.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/include_private/jsdrv_prv/windows.h` & `pyjoulescope_driver-1.3.3/include_private/jsdrv_prv/windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/__init__.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/__main__.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/binding.c` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/binding.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
         ],
         "include_dirs": [
             "C:\\repos\\Jetperch\\joulescope_driver\\include",
             "C:\\repos\\Jetperch\\joulescope_driver\\include_private",
             "C:\\repos\\Jetperch\\joulescope_driver\\third-party\\tinyprintf",
-            "C:\\bin\\Python3_11_2\\Lib\\site-packages\\numpy\\core\\include"
+            "C:\\bin\\Python3_10_11\\lib\\site-packages\\numpy\\core\\include"
         ],
         "libraries": [
             "Setupapi",
             "Winusb",
             "user32"
         ],
         "name": "pyjoulescope_driver.binding",
@@ -1161,195 +1161,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":689
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":690
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":691
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":692
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":696
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":697
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":698
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":699
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":703
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":704
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":713
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":714
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":715
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":717
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":718
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":719
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":721
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":722
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":724
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":725
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":726
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1381,64 +1381,64 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_19pyjoulescope_driver_7binding_Driver;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":728
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":729
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":730
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":732
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 struct __pyx_opt_args_19pyjoulescope_driver_7binding__timeout_validate;
 
-/* "pyjoulescope_driver/binding.pyx":569
+/* "pyjoulescope_driver/binding.pyx":571
  * 
  * 
  * cdef int32_t _timeout_validate(value, default=None):             # <<<<<<<<<<<<<<
  *     if default is None:
  *         default = _TIMEOUT_MS_DEFAULT
  */
 struct __pyx_opt_args_19pyjoulescope_driver_7binding__timeout_validate {
   int __pyx_n;
   PyObject *__pyx_default;
 };
 
-/* "pyjoulescope_driver/binding.pyx":589
+/* "pyjoulescope_driver/binding.pyx":591
  * 
  * 
  * cdef class Driver:             # <<<<<<<<<<<<<<
  *     cdef c_jsdrv.jsdrv_context_s * _context
  *     cdef object _subscribers
  */
 struct __pyx_obj_19pyjoulescope_driver_7binding_Driver {
@@ -2573,16 +2573,15 @@
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
 static PyObject *__pyx_f_19pyjoulescope_driver_7binding__i128_to_int(uint64_t, uint64_t); /*proto*/
 static PyObject *__pyx_f_19pyjoulescope_driver_7binding__parse_buffer_info(struct jsdrv_buffer_info_s *); /*proto*/
 static PyObject *__pyx_f_19pyjoulescope_driver_7binding__parse_buffer_rsp(struct jsdrv_buffer_response_s *); /*proto*/
 static PyObject *__pyx_f_19pyjoulescope_driver_7binding__pack_buffer_req(PyObject *); /*proto*/
 static PyObject *__pyx_f_19pyjoulescope_driver_7binding__jsdrv_union_to_py(struct jsdrv_union_s const *); /*proto*/
 static int32_t __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(PyObject *, struct __pyx_opt_args_19pyjoulescope_driver_7binding__timeout_validate *__pyx_optional_args); /*proto*/
-static void __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish2_cbk(void *, char const *, struct jsdrv_union_s const *); /*proto*/
-static void __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish1_cbk(void *, char const *, struct jsdrv_union_s const *); /*proto*/
+static void __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish_cbk(void *, char const *, struct jsdrv_union_s const *); /*proto*/
 static void __pyx_f_19pyjoulescope_driver_7binding__on_log_recv(void *, struct jsdrv_log_header_s const *, char const *, char const *); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static void *__pyx_align_pointer(void *, size_t); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
 static PyObject *assert_direct_dimensions(Py_ssize_t *, int); /*proto*/
@@ -3603,15 +3602,15 @@
 static PyObject *__pyx_tuple__76;
 static PyObject *__pyx_codeobj__66;
 static PyObject *__pyx_codeobj__68;
 static PyObject *__pyx_codeobj__70;
 static PyObject *__pyx_codeobj__77;
 /* Late includes */
 
-/* "pyjoulescope_driver/binding.pyx":81
+/* "pyjoulescope_driver/binding.pyx":83
  * 
  * 
  * cdef object _i128_to_int(uint64_t high, uint64_t low):             # <<<<<<<<<<<<<<
  *     i = int(high) << 64
  *     i |= int(low)
  */
 
@@ -3623,103 +3622,103 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_i128_to_int", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":82
+  /* "pyjoulescope_driver/binding.pyx":84
  * 
  * cdef object _i128_to_int(uint64_t high, uint64_t low):
  *     i = int(high) << 64             # <<<<<<<<<<<<<<
  *     i |= int(low)
  *     if i & 0x8000_0000_0000_0000:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_v_high); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_v_high); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Lshift(__pyx_t_2, __pyx_int_64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Lshift(__pyx_t_2, __pyx_int_64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_i = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":83
+  /* "pyjoulescope_driver/binding.pyx":85
  * cdef object _i128_to_int(uint64_t high, uint64_t low):
  *     i = int(high) << 64
  *     i |= int(low)             # <<<<<<<<<<<<<<
  *     if i & 0x8000_0000_0000_0000:
  *         i = ((~i) & 0xffff_ffff_ffff_ffff) - 1
  */
-  __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_v_low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_v_low); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_i, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_i, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":84
+  /* "pyjoulescope_driver/binding.pyx":86
  *     i = int(high) << 64
  *     i |= int(low)
  *     if i & 0x8000_0000_0000_0000:             # <<<<<<<<<<<<<<
  *         i = ((~i) & 0xffff_ffff_ffff_ffff) - 1
  *     return i
  */
-  __pyx_t_1 = PyNumber_And(__pyx_v_i, __pyx_int_9223372036854775808); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_And(__pyx_v_i, __pyx_int_9223372036854775808); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_3) {
 
-    /* "pyjoulescope_driver/binding.pyx":85
+    /* "pyjoulescope_driver/binding.pyx":87
  *     i |= int(low)
  *     if i & 0x8000_0000_0000_0000:
  *         i = ((~i) & 0xffff_ffff_ffff_ffff) - 1             # <<<<<<<<<<<<<<
  *     return i
  * 
  */
-    __pyx_t_1 = PyNumber_Invert(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Invert(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyNumber_And(__pyx_t_1, __pyx_int_18446744073709551615); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_And(__pyx_t_1, __pyx_int_18446744073709551615); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":84
+    /* "pyjoulescope_driver/binding.pyx":86
  *     i = int(high) << 64
  *     i |= int(low)
  *     if i & 0x8000_0000_0000_0000:             # <<<<<<<<<<<<<<
  *         i = ((~i) & 0xffff_ffff_ffff_ffff) - 1
  *     return i
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":86
+  /* "pyjoulescope_driver/binding.pyx":88
  *     if i & 0x8000_0000_0000_0000:
  *         i = ((~i) & 0xffff_ffff_ffff_ffff) - 1
  *     return i             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_i);
   __pyx_r = __pyx_v_i;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":81
+  /* "pyjoulescope_driver/binding.pyx":83
  * 
  * 
  * cdef object _i128_to_int(uint64_t high, uint64_t low):             # <<<<<<<<<<<<<<
  *     i = int(high) << 64
  *     i |= int(low)
  */
 
@@ -3732,15 +3731,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":89
+/* "pyjoulescope_driver/binding.pyx":91
  * 
  * 
  * cdef object _parse_buffer_info(c_jsdrv.jsdrv_buffer_info_s * info):             # <<<<<<<<<<<<<<
  *     element_prefix = _element_type_to_prefix[info[0].element_type]
  *     name, field_name, units, use_index = _field_to_meta[info[0].field_id]
  */
 
@@ -3765,48 +3764,48 @@
   Py_UCS4 __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parse_buffer_info", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":90
+  /* "pyjoulescope_driver/binding.pyx":92
  * 
  * cdef object _parse_buffer_info(c_jsdrv.jsdrv_buffer_info_s * info):
  *     element_prefix = _element_type_to_prefix[info[0].element_type]             # <<<<<<<<<<<<<<
  *     name, field_name, units, use_index = _field_to_meta[info[0].field_id]
  *     if use_index:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_element_type_to_prefix); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_element_type_to_prefix); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, (__pyx_v_info[0]).element_type, uint8_t, 0, __Pyx_PyInt_From_uint8_t, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, (__pyx_v_info[0]).element_type, uint8_t, 0, __Pyx_PyInt_From_uint8_t, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_element_prefix = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":91
+  /* "pyjoulescope_driver/binding.pyx":93
  * cdef object _parse_buffer_info(c_jsdrv.jsdrv_buffer_info_s * info):
  *     element_prefix = _element_type_to_prefix[info[0].element_type]
  *     name, field_name, units, use_index = _field_to_meta[info[0].field_id]             # <<<<<<<<<<<<<<
  *     if use_index:
  *         name = f'{name}[{info[0].index:d}]'
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_field_to_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_field_to_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_2, (__pyx_v_info[0]).field_id, uint8_t, 0, __Pyx_PyInt_From_uint8_t, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_2, (__pyx_v_info[0]).field_id, uint8_t, 0, __Pyx_PyInt_From_uint8_t, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 4)) {
       if (size > 4) __Pyx_RaiseTooManyValuesError(4);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 91, __pyx_L1_error)
+      __PYX_ERR(0, 93, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
       __pyx_t_5 = PyTuple_GET_ITEM(sequence, 3); 
@@ -3821,476 +3820,476 @@
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     #else
     {
       Py_ssize_t i;
       PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_3,&__pyx_t_4,&__pyx_t_5};
       for (i=0; i < 4; i++) {
-        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 91, __pyx_L1_error)
+        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 93, __pyx_L1_error)
         __Pyx_GOTREF(item);
         *(temps[i]) = item;
       }
     }
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
     PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_3,&__pyx_t_4,&__pyx_t_5};
-    __pyx_t_6 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_6 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_7 = Py_TYPE(__pyx_t_6)->tp_iternext;
     for (index=0; index < 4; index++) {
       PyObject* item = __pyx_t_7(__pyx_t_6); if (unlikely(!item)) goto __pyx_L3_unpacking_failed;
       __Pyx_GOTREF(item);
       *(temps[index]) = item;
     }
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 4) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 4) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
     __pyx_t_7 = NULL;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 91, __pyx_L1_error)
+    __PYX_ERR(0, 93, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_name = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_field_name = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_units = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_use_index = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":92
+  /* "pyjoulescope_driver/binding.pyx":94
  *     element_prefix = _element_type_to_prefix[info[0].element_type]
  *     name, field_name, units, use_index = _field_to_meta[info[0].field_id]
  *     if use_index:             # <<<<<<<<<<<<<<
  *         name = f'{name}[{info[0].index:d}]'
  *         if not field_name:
  */
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_use_index); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_use_index); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 94, __pyx_L1_error)
   if (__pyx_t_8) {
 
-    /* "pyjoulescope_driver/binding.pyx":93
+    /* "pyjoulescope_driver/binding.pyx":95
  *     name, field_name, units, use_index = _field_to_meta[info[0].field_id]
  *     if use_index:
  *         name = f'{name}[{info[0].index:d}]'             # <<<<<<<<<<<<<<
  *         if not field_name:
  *             field_name = f'{info[0].index:d}'
  */
-    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_9 = 0;
     __pyx_t_10 = 127;
-    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_10;
     __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_INCREF(__pyx_kp_u_);
     __pyx_t_9 += 1;
     __Pyx_GIVEREF(__pyx_kp_u_);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u_);
-    __pyx_t_5 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_Format(__pyx_t_5, __pyx_n_u_d); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Format(__pyx_t_5, __pyx_n_u_d); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_10;
     __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_INCREF(__pyx_kp_u__2);
     __pyx_t_9 += 1;
     __Pyx_GIVEREF(__pyx_kp_u__2);
     PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__2);
-    __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_name, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":94
+    /* "pyjoulescope_driver/binding.pyx":96
  *     if use_index:
  *         name = f'{name}[{info[0].index:d}]'
  *         if not field_name:             # <<<<<<<<<<<<<<
  *             field_name = f'{info[0].index:d}'
  *         else:
  */
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_field_name); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_field_name); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
     __pyx_t_11 = ((!__pyx_t_8) != 0);
     if (__pyx_t_11) {
 
-      /* "pyjoulescope_driver/binding.pyx":95
+      /* "pyjoulescope_driver/binding.pyx":97
  *         name = f'{name}[{info[0].index:d}]'
  *         if not field_name:
  *             field_name = f'{info[0].index:d}'             # <<<<<<<<<<<<<<
  *         else:
  *             field_name = f'{field_name}[{info[0].index:d}]'
  */
-      __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyObject_Format(__pyx_t_4, __pyx_n_u_d); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Format(__pyx_t_4, __pyx_n_u_d); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF_SET(__pyx_v_field_name, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "pyjoulescope_driver/binding.pyx":94
+      /* "pyjoulescope_driver/binding.pyx":96
  *     if use_index:
  *         name = f'{name}[{info[0].index:d}]'
  *         if not field_name:             # <<<<<<<<<<<<<<
  *             field_name = f'{info[0].index:d}'
  *         else:
  */
       goto __pyx_L6;
     }
 
-    /* "pyjoulescope_driver/binding.pyx":97
+    /* "pyjoulescope_driver/binding.pyx":99
  *             field_name = f'{info[0].index:d}'
  *         else:
  *             field_name = f'{field_name}[{info[0].index:d}]'             # <<<<<<<<<<<<<<
  *     v = {
  *         'version': info[0].version,
  */
     /*else*/ {
-      __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_9 = 0;
       __pyx_t_10 = 127;
-      __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_field_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_field_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_10;
       __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
       __pyx_t_4 = 0;
       __Pyx_INCREF(__pyx_kp_u_);
       __pyx_t_9 += 1;
       __Pyx_GIVEREF(__pyx_kp_u_);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u_);
-      __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_Format(__pyx_t_4, __pyx_n_u_d); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Format(__pyx_t_4, __pyx_n_u_d); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_10;
       __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
       __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_kp_u__2);
       __pyx_t_9 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__2);
       PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__2);
-      __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF_SET(__pyx_v_field_name, __pyx_t_5);
       __pyx_t_5 = 0;
     }
     __pyx_L6:;
 
-    /* "pyjoulescope_driver/binding.pyx":92
+    /* "pyjoulescope_driver/binding.pyx":94
  *     element_prefix = _element_type_to_prefix[info[0].element_type]
  *     name, field_name, units, use_index = _field_to_meta[info[0].field_id]
  *     if use_index:             # <<<<<<<<<<<<<<
  *         name = f'{name}[{info[0].index:d}]'
  *         if not field_name:
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":99
+  /* "pyjoulescope_driver/binding.pyx":101
  *             field_name = f'{field_name}[{info[0].index:d}]'
  *     v = {
  *         'version': info[0].version,             # <<<<<<<<<<<<<<
  *         'name': name,
  *         'field': field_name,
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(15); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(15); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_version, __pyx_t_1) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_version, __pyx_t_1) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":100
+  /* "pyjoulescope_driver/binding.pyx":102
  *     v = {
  *         'version': info[0].version,
  *         'name': name,             # <<<<<<<<<<<<<<
  *         'field': field_name,
  *         'field_id': info[0].field_id,
  */
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_name, __pyx_v_name) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_name, __pyx_v_name) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":101
+  /* "pyjoulescope_driver/binding.pyx":103
  *         'version': info[0].version,
  *         'name': name,
  *         'field': field_name,             # <<<<<<<<<<<<<<
  *         'field_id': info[0].field_id,
  *         'index': info[0].index,
  */
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_field, __pyx_v_field_name) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_field, __pyx_v_field_name) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":102
+  /* "pyjoulescope_driver/binding.pyx":104
  *         'name': name,
  *         'field': field_name,
  *         'field_id': info[0].field_id,             # <<<<<<<<<<<<<<
  *         'index': info[0].index,
  *         'element_type': f'{element_prefix}{info[0].element_size_bits:d}',
  */
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).field_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).field_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_field_id, __pyx_t_1) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_field_id, __pyx_t_1) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":103
+  /* "pyjoulescope_driver/binding.pyx":105
  *         'field': field_name,
  *         'field_id': info[0].field_id,
  *         'index': info[0].index,             # <<<<<<<<<<<<<<
  *         'element_type': f'{element_prefix}{info[0].element_size_bits:d}',
  *         'element_type_enum': info[0].element_type,
  */
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_index, __pyx_t_1) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_index, __pyx_t_1) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":104
+  /* "pyjoulescope_driver/binding.pyx":106
  *         'field_id': info[0].field_id,
  *         'index': info[0].index,
  *         'element_type': f'{element_prefix}{info[0].element_size_bits:d}',             # <<<<<<<<<<<<<<
  *         'element_type_enum': info[0].element_type,
  *         'element_size_bits': info[0].element_size_bits,
  */
-  __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_element_prefix, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_element_prefix, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).element_size_bits); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).element_size_bits); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_Format(__pyx_t_4, __pyx_n_u_d); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Format(__pyx_t_4, __pyx_n_u_d); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_element_type, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_element_type, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":105
+  /* "pyjoulescope_driver/binding.pyx":107
  *         'index': info[0].index,
  *         'element_type': f'{element_prefix}{info[0].element_size_bits:d}',
  *         'element_type_enum': info[0].element_type,             # <<<<<<<<<<<<<<
  *         'element_size_bits': info[0].element_size_bits,
  *         'units': units,
  */
-  __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).element_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).element_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_element_type_enum, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_element_type_enum, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":106
+  /* "pyjoulescope_driver/binding.pyx":108
  *         'element_type': f'{element_prefix}{info[0].element_size_bits:d}',
  *         'element_type_enum': info[0].element_type,
  *         'element_size_bits': info[0].element_size_bits,             # <<<<<<<<<<<<<<
  *         'units': units,
  *         'topic': info[0].topic,
  */
-  __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).element_size_bits); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_info[0]).element_size_bits); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_element_size_bits, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_element_size_bits, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":107
+  /* "pyjoulescope_driver/binding.pyx":109
  *         'element_type_enum': info[0].element_type,
  *         'element_size_bits': info[0].element_size_bits,
  *         'units': units,             # <<<<<<<<<<<<<<
  *         'topic': info[0].topic,
  *         'size_in_utc': info[0].size_in_utc,
  */
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_units, __pyx_v_units) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_units, __pyx_v_units) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":108
+  /* "pyjoulescope_driver/binding.pyx":110
  *         'element_size_bits': info[0].element_size_bits,
  *         'units': units,
  *         'topic': info[0].topic,             # <<<<<<<<<<<<<<
  *         'size_in_utc': info[0].size_in_utc,
  *         'size_in_samples': info[0].size_in_samples,
  */
-  __pyx_t_4 = __Pyx_PyObject_FromString((__pyx_v_info[0]).topic); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FromString((__pyx_v_info[0]).topic); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_topic, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_topic, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":109
+  /* "pyjoulescope_driver/binding.pyx":111
  *         'units': units,
  *         'topic': info[0].topic,
  *         'size_in_utc': info[0].size_in_utc,             # <<<<<<<<<<<<<<
  *         'size_in_samples': info[0].size_in_samples,
  *         'time_range_utc': {
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int64_t((__pyx_v_info[0]).size_in_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int64_t((__pyx_v_info[0]).size_in_utc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_size_in_utc, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_size_in_utc, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":110
+  /* "pyjoulescope_driver/binding.pyx":112
  *         'topic': info[0].topic,
  *         'size_in_utc': info[0].size_in_utc,
  *         'size_in_samples': info[0].size_in_samples,             # <<<<<<<<<<<<<<
  *         'time_range_utc': {
  *             'start': info[0].time_range_utc.start,
  */
-  __pyx_t_4 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).size_in_samples); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).size_in_samples); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_size_in_samples, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_size_in_samples, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":112
+  /* "pyjoulescope_driver/binding.pyx":114
  *         'size_in_samples': info[0].size_in_samples,
  *         'time_range_utc': {
  *             'start': info[0].time_range_utc.start,             # <<<<<<<<<<<<<<
  *             'end': info[0].time_range_utc.end,
  *             'length': info[0].time_range_utc.length,
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_int64_t((__pyx_v_info[0]).time_range_utc.start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t((__pyx_v_info[0]).time_range_utc.start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_start, __pyx_t_3) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_start, __pyx_t_3) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":113
+  /* "pyjoulescope_driver/binding.pyx":115
  *         'time_range_utc': {
  *             'start': info[0].time_range_utc.start,
  *             'end': info[0].time_range_utc.end,             # <<<<<<<<<<<<<<
  *             'length': info[0].time_range_utc.length,
  *         },
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int64_t((__pyx_v_info[0]).time_range_utc.end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t((__pyx_v_info[0]).time_range_utc.end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_end, __pyx_t_3) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_end, __pyx_t_3) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":114
+  /* "pyjoulescope_driver/binding.pyx":116
  *             'start': info[0].time_range_utc.start,
  *             'end': info[0].time_range_utc.end,
  *             'length': info[0].time_range_utc.length,             # <<<<<<<<<<<<<<
  *         },
  *         'time_range_samples': {
  */
-  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_range_utc.length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_range_utc.length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_length, __pyx_t_3) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_length, __pyx_t_3) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_time_range_utc, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_time_range_utc, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":117
+  /* "pyjoulescope_driver/binding.pyx":119
  *         },
  *         'time_range_samples': {
  *             'start': info[0].time_range_samples.start,             # <<<<<<<<<<<<<<
  *             'end': info[0].time_range_samples.end,
  *             'length': info[0].time_range_samples.length,
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_range_samples.start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_range_samples.start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_start, __pyx_t_3) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_start, __pyx_t_3) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":118
+  /* "pyjoulescope_driver/binding.pyx":120
  *         'time_range_samples': {
  *             'start': info[0].time_range_samples.start,
  *             'end': info[0].time_range_samples.end,             # <<<<<<<<<<<<<<
  *             'length': info[0].time_range_samples.length,
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_range_samples.end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_range_samples.end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_end, __pyx_t_3) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_end, __pyx_t_3) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":119
+  /* "pyjoulescope_driver/binding.pyx":121
  *             'start': info[0].time_range_samples.start,
  *             'end': info[0].time_range_samples.end,
  *             'length': info[0].time_range_samples.length,             # <<<<<<<<<<<<<<
  * 
  *         },
  */
-  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_range_samples.length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_range_samples.length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_length, __pyx_t_3) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_length, __pyx_t_3) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_time_range_samples, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_time_range_samples, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":123
+  /* "pyjoulescope_driver/binding.pyx":125
  *         },
  *         'time_map': {
  *             'offset_time': info[0].time_map.offset_time,             # <<<<<<<<<<<<<<
  *             'offset_counter': info[0].time_map.offset_counter,
  *             'counter_rate': info[0].time_map.counter_rate,
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_int64_t((__pyx_v_info[0]).time_map.offset_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t((__pyx_v_info[0]).time_map.offset_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_offset_time, __pyx_t_3) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_offset_time, __pyx_t_3) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":124
+  /* "pyjoulescope_driver/binding.pyx":126
  *         'time_map': {
  *             'offset_time': info[0].time_map.offset_time,
  *             'offset_counter': info[0].time_map.offset_counter,             # <<<<<<<<<<<<<<
  *             'counter_rate': info[0].time_map.counter_rate,
  *         },
  */
-  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_map.offset_counter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint64_t((__pyx_v_info[0]).time_map.offset_counter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_offset_counter, __pyx_t_3) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_offset_counter, __pyx_t_3) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":125
+  /* "pyjoulescope_driver/binding.pyx":127
  *             'offset_time': info[0].time_map.offset_time,
  *             'offset_counter': info[0].time_map.offset_counter,
  *             'counter_rate': info[0].time_map.counter_rate,             # <<<<<<<<<<<<<<
  *         },
  *     }
  */
-  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_info[0]).time_map.counter_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_info[0]).time_map.counter_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_counter_rate, __pyx_t_3) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_counter_rate, __pyx_t_3) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_time_map, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_time_map, __pyx_t_4) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_v = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":128
+  /* "pyjoulescope_driver/binding.pyx":130
  *         },
  *     }
  *     return v             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_v);
   __pyx_r = __pyx_v_v;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":89
+  /* "pyjoulescope_driver/binding.pyx":91
  * 
  * 
  * cdef object _parse_buffer_info(c_jsdrv.jsdrv_buffer_info_s * info):             # <<<<<<<<<<<<<<
  *     element_prefix = _element_type_to_prefix[info[0].element_type]
  *     name, field_name, units, use_index = _field_to_meta[info[0].field_id]
  */
 
@@ -4312,15 +4311,15 @@
   __Pyx_XDECREF(__pyx_v_use_index);
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":131
+/* "pyjoulescope_driver/binding.pyx":133
  * 
  * 
  * cdef object _parse_buffer_rsp(c_jsdrv.jsdrv_buffer_response_s * r):             # <<<<<<<<<<<<<<
  *     cdef np.npy_intp shape[2]
  *     v = {
  */
 
@@ -4340,451 +4339,451 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parse_buffer_rsp", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":134
+  /* "pyjoulescope_driver/binding.pyx":136
  *     cdef np.npy_intp shape[2]
  *     v = {
  *         'version': r[0].version,             # <<<<<<<<<<<<<<
  *         'rsp_id': r[0].rsp_id,
  *         'info': _parse_buffer_info(&r[0].info),
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_uint8_t((__pyx_v_r[0]).version); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint8_t((__pyx_v_r[0]).version); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_version, __pyx_t_2) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_version, __pyx_t_2) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":135
+  /* "pyjoulescope_driver/binding.pyx":137
  *     v = {
  *         'version': r[0].version,
  *         'rsp_id': r[0].rsp_id,             # <<<<<<<<<<<<<<
  *         'info': _parse_buffer_info(&r[0].info),
  *     }
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int64_t((__pyx_v_r[0]).rsp_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int64_t((__pyx_v_r[0]).rsp_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_rsp_id, __pyx_t_2) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_rsp_id, __pyx_t_2) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":136
+  /* "pyjoulescope_driver/binding.pyx":138
  *         'version': r[0].version,
  *         'rsp_id': r[0].rsp_id,
  *         'info': _parse_buffer_info(&r[0].info),             # <<<<<<<<<<<<<<
  *     }
  *     length = v['info']['time_range_samples']['length']
  */
-  __pyx_t_2 = __pyx_f_19pyjoulescope_driver_7binding__parse_buffer_info((&(__pyx_v_r[0]).info)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_19pyjoulescope_driver_7binding__parse_buffer_info((&(__pyx_v_r[0]).info)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_info, __pyx_t_2) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_info, __pyx_t_2) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_v = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":138
+  /* "pyjoulescope_driver/binding.pyx":140
  *         'info': _parse_buffer_info(&r[0].info),
  *     }
  *     length = v['info']['time_range_samples']['length']             # <<<<<<<<<<<<<<
  *     if r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SAMPLES:
  *         v['response_type'] = 'samples'
  */
-  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_v, __pyx_n_u_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_v, __pyx_n_u_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_time_range_samples); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_time_range_samples); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_length = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":139
+  /* "pyjoulescope_driver/binding.pyx":141
  *     }
  *     length = v['info']['time_range_samples']['length']
  *     if r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SAMPLES:             # <<<<<<<<<<<<<<
  *         v['response_type'] = 'samples'
  *         info = v['info']
  */
   __pyx_t_3 = (((__pyx_v_r[0]).response_type == JSDRV_BUFFER_RESPONSE_SAMPLES) != 0);
   if (__pyx_t_3) {
 
-    /* "pyjoulescope_driver/binding.pyx":140
+    /* "pyjoulescope_driver/binding.pyx":142
  *     length = v['info']['time_range_samples']['length']
  *     if r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SAMPLES:
  *         v['response_type'] = 'samples'             # <<<<<<<<<<<<<<
  *         info = v['info']
  *         element_type = info['element_type']
  */
-    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_response_type, __pyx_n_u_samples) < 0)) __PYX_ERR(0, 140, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_response_type, __pyx_n_u_samples) < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
 
-    /* "pyjoulescope_driver/binding.pyx":141
+    /* "pyjoulescope_driver/binding.pyx":143
  *     if r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SAMPLES:
  *         v['response_type'] = 'samples'
  *         info = v['info']             # <<<<<<<<<<<<<<
  *         element_type = info['element_type']
  *         if element_type == 'f32':
  */
-    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_v, __pyx_n_u_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_v, __pyx_n_u_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_info = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":142
+    /* "pyjoulescope_driver/binding.pyx":144
  *         v['response_type'] = 'samples'
  *         info = v['info']
  *         element_type = info['element_type']             # <<<<<<<<<<<<<<
  *         if element_type == 'f32':
  *             shape[0] = <np.npy_intp> length
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_info, __pyx_n_u_element_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_info, __pyx_n_u_element_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_element_type = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":143
+    /* "pyjoulescope_driver/binding.pyx":145
  *         info = v['info']
  *         element_type = info['element_type']
  *         if element_type == 'f32':             # <<<<<<<<<<<<<<
  *             shape[0] = <np.npy_intp> length
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])
  */
-    __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_v_element_type, __pyx_n_u_f32, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_v_element_type, __pyx_n_u_f32, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
     if (__pyx_t_3) {
 
-      /* "pyjoulescope_driver/binding.pyx":144
+      /* "pyjoulescope_driver/binding.pyx":146
  *         element_type = info['element_type']
  *         if element_type == 'f32':
  *             shape[0] = <np.npy_intp> length             # <<<<<<<<<<<<<<
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])
  *         elif element_type == 'u1':
  */
-      __pyx_t_4 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_length); if (unlikely((__pyx_t_4 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 144, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_length); if (unlikely((__pyx_t_4 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 146, __pyx_L1_error)
       (__pyx_v_shape[0]) = ((npy_intp)__pyx_t_4);
 
-      /* "pyjoulescope_driver/binding.pyx":145
+      /* "pyjoulescope_driver/binding.pyx":147
  *         if element_type == 'f32':
  *             shape[0] = <np.npy_intp> length
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])             # <<<<<<<<<<<<<<
  *         elif element_type == 'u1':
  *             shape[0] = <np.npy_intp> ((length + 7) // 8)
  */
-      __pyx_t_1 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_FLOAT32, ((void *)(&((__pyx_v_r[0]).data[0])))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
+      __pyx_t_1 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_FLOAT32, ((void *)(&((__pyx_v_r[0]).data[0])))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_ndarray = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "pyjoulescope_driver/binding.pyx":143
+      /* "pyjoulescope_driver/binding.pyx":145
  *         info = v['info']
  *         element_type = info['element_type']
  *         if element_type == 'f32':             # <<<<<<<<<<<<<<
  *             shape[0] = <np.npy_intp> length
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])
  */
       goto __pyx_L4;
     }
 
-    /* "pyjoulescope_driver/binding.pyx":146
+    /* "pyjoulescope_driver/binding.pyx":148
  *             shape[0] = <np.npy_intp> length
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])
  *         elif element_type == 'u1':             # <<<<<<<<<<<<<<
  *             shape[0] = <np.npy_intp> ((length + 7) // 8)
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  */
-    __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_v_element_type, __pyx_n_u_u1, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_v_element_type, __pyx_n_u_u1, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 148, __pyx_L1_error)
     if (__pyx_t_3) {
 
-      /* "pyjoulescope_driver/binding.pyx":147
+      /* "pyjoulescope_driver/binding.pyx":149
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])
  *         elif element_type == 'u1':
  *             shape[0] = <np.npy_intp> ((length + 7) // 8)             # <<<<<<<<<<<<<<
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  *         elif element_type == 'u4':
  */
-      __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_7, 7, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_7, 7, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_1, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_1, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_4 = __Pyx_PyInt_As_Py_intptr_t(__pyx_t_2); if (unlikely((__pyx_t_4 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 147, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_As_Py_intptr_t(__pyx_t_2); if (unlikely((__pyx_t_4 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 149, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       (__pyx_v_shape[0]) = ((npy_intp)__pyx_t_4);
 
-      /* "pyjoulescope_driver/binding.pyx":148
+      /* "pyjoulescope_driver/binding.pyx":150
  *         elif element_type == 'u1':
  *             shape[0] = <np.npy_intp> ((length + 7) // 8)
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])             # <<<<<<<<<<<<<<
  *         elif element_type == 'u4':
  *             shape[0] = <np.npy_intp> ((length + 1) // 2)
  */
-      __pyx_t_2 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_UINT8, ((void *)(&((__pyx_v_r[0]).data[0])))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+      __pyx_t_2 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_UINT8, ((void *)(&((__pyx_v_r[0]).data[0])))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_v_ndarray = __pyx_t_2;
       __pyx_t_2 = 0;
 
-      /* "pyjoulescope_driver/binding.pyx":146
+      /* "pyjoulescope_driver/binding.pyx":148
  *             shape[0] = <np.npy_intp> length
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])
  *         elif element_type == 'u1':             # <<<<<<<<<<<<<<
  *             shape[0] = <np.npy_intp> ((length + 7) // 8)
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  */
       goto __pyx_L4;
     }
 
-    /* "pyjoulescope_driver/binding.pyx":149
+    /* "pyjoulescope_driver/binding.pyx":151
  *             shape[0] = <np.npy_intp> ((length + 7) // 8)
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  *         elif element_type == 'u4':             # <<<<<<<<<<<<<<
  *             shape[0] = <np.npy_intp> ((length + 1) // 2)
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  */
-    __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_v_element_type, __pyx_n_u_u4, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_v_element_type, __pyx_n_u_u4, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 151, __pyx_L1_error)
     if (__pyx_t_3) {
 
-      /* "pyjoulescope_driver/binding.pyx":150
+      /* "pyjoulescope_driver/binding.pyx":152
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  *         elif element_type == 'u4':
  *             shape[0] = <np.npy_intp> ((length + 1) // 2)             # <<<<<<<<<<<<<<
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  *         else:
  */
-      __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_2, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_2, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_4 = __Pyx_PyInt_As_Py_intptr_t(__pyx_t_1); if (unlikely((__pyx_t_4 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 150, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_As_Py_intptr_t(__pyx_t_1); if (unlikely((__pyx_t_4 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 152, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       (__pyx_v_shape[0]) = ((npy_intp)__pyx_t_4);
 
-      /* "pyjoulescope_driver/binding.pyx":151
+      /* "pyjoulescope_driver/binding.pyx":153
  *         elif element_type == 'u4':
  *             shape[0] = <np.npy_intp> ((length + 1) // 2)
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])             # <<<<<<<<<<<<<<
  *         else:
  *             _log_c.error('unsupported sample format')
  */
-      __pyx_t_1 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_UINT8, ((void *)(&((__pyx_v_r[0]).data[0])))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __pyx_t_1 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_UINT8, ((void *)(&((__pyx_v_r[0]).data[0])))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_ndarray = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "pyjoulescope_driver/binding.pyx":149
+      /* "pyjoulescope_driver/binding.pyx":151
  *             shape[0] = <np.npy_intp> ((length + 7) // 8)
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  *         elif element_type == 'u4':             # <<<<<<<<<<<<<<
  *             shape[0] = <np.npy_intp> ((length + 1) // 2)
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  */
       goto __pyx_L4;
     }
 
-    /* "pyjoulescope_driver/binding.pyx":153
+    /* "pyjoulescope_driver/binding.pyx":155
  *             ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> &r[0].data[0])
  *         else:
  *             _log_c.error('unsupported sample format')             # <<<<<<<<<<<<<<
  *             return
  *         v['data_type'] = info['element_type']
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log_c); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log_c); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 155, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_2)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_kp_u_unsupported_sample_format) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u_unsupported_sample_format);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyjoulescope_driver/binding.pyx":154
+      /* "pyjoulescope_driver/binding.pyx":156
  *         else:
  *             _log_c.error('unsupported sample format')
  *             return             # <<<<<<<<<<<<<<
  *         v['data_type'] = info['element_type']
  *         v['data'] = ndarray.copy()
  */
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L0;
     }
     __pyx_L4:;
 
-    /* "pyjoulescope_driver/binding.pyx":155
+    /* "pyjoulescope_driver/binding.pyx":157
  *             _log_c.error('unsupported sample format')
  *             return
  *         v['data_type'] = info['element_type']             # <<<<<<<<<<<<<<
  *         v['data'] = ndarray.copy()
  *     elif r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SUMMARY:
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_info, __pyx_n_u_element_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_info, __pyx_n_u_element_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_data_type, __pyx_t_1) < 0)) __PYX_ERR(0, 155, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_data_type, __pyx_t_1) < 0)) __PYX_ERR(0, 157, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":156
+    /* "pyjoulescope_driver/binding.pyx":158
  *             return
  *         v['data_type'] = info['element_type']
  *         v['data'] = ndarray.copy()             # <<<<<<<<<<<<<<
  *     elif r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SUMMARY:
  *         v['response_type'] = 'summary'
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_1) < 0)) __PYX_ERR(0, 156, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_1) < 0)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":139
+    /* "pyjoulescope_driver/binding.pyx":141
  *     }
  *     length = v['info']['time_range_samples']['length']
  *     if r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SAMPLES:             # <<<<<<<<<<<<<<
  *         v['response_type'] = 'samples'
  *         info = v['info']
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":157
+  /* "pyjoulescope_driver/binding.pyx":159
  *         v['data_type'] = info['element_type']
  *         v['data'] = ndarray.copy()
  *     elif r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SUMMARY:             # <<<<<<<<<<<<<<
  *         v['response_type'] = 'summary'
  *         shape[0] = <np.npy_intp> length
  */
   __pyx_t_3 = (((__pyx_v_r[0]).response_type == JSDRV_BUFFER_RESPONSE_SUMMARY) != 0);
   if (__pyx_t_3) {
 
-    /* "pyjoulescope_driver/binding.pyx":158
+    /* "pyjoulescope_driver/binding.pyx":160
  *         v['data'] = ndarray.copy()
  *     elif r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SUMMARY:
  *         v['response_type'] = 'summary'             # <<<<<<<<<<<<<<
  *         shape[0] = <np.npy_intp> length
  *         shape[1] = <np.npy_intp> 4
  */
-    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_response_type, __pyx_n_u_summary) < 0)) __PYX_ERR(0, 158, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_response_type, __pyx_n_u_summary) < 0)) __PYX_ERR(0, 160, __pyx_L1_error)
 
-    /* "pyjoulescope_driver/binding.pyx":159
+    /* "pyjoulescope_driver/binding.pyx":161
  *     elif r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SUMMARY:
  *         v['response_type'] = 'summary'
  *         shape[0] = <np.npy_intp> length             # <<<<<<<<<<<<<<
  *         shape[1] = <np.npy_intp> 4
  *         ndarray = np.PyArray_SimpleNewFromData(2, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])
  */
-    __pyx_t_4 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_length); if (unlikely((__pyx_t_4 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 159, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_Py_intptr_t(__pyx_v_length); if (unlikely((__pyx_t_4 == ((npy_intp)-1)) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L1_error)
     (__pyx_v_shape[0]) = ((npy_intp)__pyx_t_4);
 
-    /* "pyjoulescope_driver/binding.pyx":160
+    /* "pyjoulescope_driver/binding.pyx":162
  *         v['response_type'] = 'summary'
  *         shape[0] = <np.npy_intp> length
  *         shape[1] = <np.npy_intp> 4             # <<<<<<<<<<<<<<
  *         ndarray = np.PyArray_SimpleNewFromData(2, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])
  *         v['data'] = ndarray.copy()
  */
     (__pyx_v_shape[1]) = ((npy_intp)4);
 
-    /* "pyjoulescope_driver/binding.pyx":161
+    /* "pyjoulescope_driver/binding.pyx":163
  *         shape[0] = <np.npy_intp> length
  *         shape[1] = <np.npy_intp> 4
  *         ndarray = np.PyArray_SimpleNewFromData(2, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])             # <<<<<<<<<<<<<<
  *         v['data'] = ndarray.copy()
  *     else:
  */
-    __pyx_t_1 = PyArray_SimpleNewFromData(2, __pyx_v_shape, NPY_FLOAT32, ((void *)(&((__pyx_v_r[0]).data[0])))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_1 = PyArray_SimpleNewFromData(2, __pyx_v_shape, NPY_FLOAT32, ((void *)(&((__pyx_v_r[0]).data[0])))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_ndarray = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":162
+    /* "pyjoulescope_driver/binding.pyx":164
  *         shape[1] = <np.npy_intp> 4
  *         ndarray = np.PyArray_SimpleNewFromData(2, shape, np.NPY_FLOAT32, <void *> &r[0].data[0])
  *         v['data'] = ndarray.copy()             # <<<<<<<<<<<<<<
  *     else:
  *         _log_c.error(f'unsupported response_type {r[0].response_type}')
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_1) < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_1) < 0)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":157
+    /* "pyjoulescope_driver/binding.pyx":159
  *         v['data_type'] = info['element_type']
  *         v['data'] = ndarray.copy()
  *     elif r[0].response_type == c_jsdrv.JSDRV_BUFFER_RESPONSE_SUMMARY:             # <<<<<<<<<<<<<<
  *         v['response_type'] = 'summary'
  *         shape[0] = <np.npy_intp> length
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":164
+  /* "pyjoulescope_driver/binding.pyx":166
  *         v['data'] = ndarray.copy()
  *     else:
  *         _log_c.error(f'unsupported response_type {r[0].response_type}')             # <<<<<<<<<<<<<<
  *     return v
  * 
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_log_c); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_log_c); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyInt_From_uint8_t((__pyx_v_r[0]).response_type); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint8_t((__pyx_v_r[0]).response_type); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_unsupported_response_type, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_unsupported_response_type, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4792,34 +4791,34 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "pyjoulescope_driver/binding.pyx":165
+  /* "pyjoulescope_driver/binding.pyx":167
  *     else:
  *         _log_c.error(f'unsupported response_type {r[0].response_type}')
  *     return v             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_v);
   __pyx_r = __pyx_v_v;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":131
+  /* "pyjoulescope_driver/binding.pyx":133
  * 
  * 
  * cdef object _parse_buffer_rsp(c_jsdrv.jsdrv_buffer_response_s * r):             # <<<<<<<<<<<<<<
  *     cdef np.npy_intp shape[2]
  *     v = {
  */
 
@@ -4838,15 +4837,15 @@
   __Pyx_XDECREF(__pyx_v_element_type);
   __Pyx_XDECREF(__pyx_v_ndarray);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":168
+/* "pyjoulescope_driver/binding.pyx":170
  * 
  * 
  * cdef object _pack_buffer_req(r):             # <<<<<<<<<<<<<<
  *     cdef const uint8_t[:] rsp_topic_str = r['rsp_topic'].encode('utf-8')
  *     cdef c_jsdrv.jsdrv_buffer_request_s s
  */
 
@@ -4867,345 +4866,345 @@
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_pack_buffer_req", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":169
+  /* "pyjoulescope_driver/binding.pyx":171
  * 
  * cdef object _pack_buffer_req(r):
  *     cdef const uint8_t[:] rsp_topic_str = r['rsp_topic'].encode('utf-8')             # <<<<<<<<<<<<<<
  *     cdef c_jsdrv.jsdrv_buffer_request_s s
  *     cdef uint8_t * u8_ptr
  */
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_rsp_topic); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_rsp_topic); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_rsp_topic_str = __pyx_t_4;
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
 
-  /* "pyjoulescope_driver/binding.pyx":173
+  /* "pyjoulescope_driver/binding.pyx":175
  *     cdef uint8_t * u8_ptr
  * 
  *     s.version = 1             # <<<<<<<<<<<<<<
  *     time_type = r['time_type'].lower()
  *     if time_type == 'utc':
  */
   __pyx_v_s.version = 1;
 
-  /* "pyjoulescope_driver/binding.pyx":174
+  /* "pyjoulescope_driver/binding.pyx":176
  * 
  *     s.version = 1
  *     time_type = r['time_type'].lower()             # <<<<<<<<<<<<<<
  *     if time_type == 'utc':
  *         s.time_type = c_jsdrv.JSDRV_TIME_UTC
  */
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_time_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_time_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_time_type = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":175
+  /* "pyjoulescope_driver/binding.pyx":177
  *     s.version = 1
  *     time_type = r['time_type'].lower()
  *     if time_type == 'utc':             # <<<<<<<<<<<<<<
  *         s.time_type = c_jsdrv.JSDRV_TIME_UTC
  *         s.time.utc.start = r['start']
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_time_type, __pyx_n_u_utc, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_time_type, __pyx_n_u_utc, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "pyjoulescope_driver/binding.pyx":176
+    /* "pyjoulescope_driver/binding.pyx":178
  *     time_type = r['time_type'].lower()
  *     if time_type == 'utc':
  *         s.time_type = c_jsdrv.JSDRV_TIME_UTC             # <<<<<<<<<<<<<<
  *         s.time.utc.start = r['start']
  *         s.time.utc.end = r.get('end', 0)
  */
     __pyx_v_s.time_type = JSDRV_TIME_UTC;
 
-    /* "pyjoulescope_driver/binding.pyx":177
+    /* "pyjoulescope_driver/binding.pyx":179
  *     if time_type == 'utc':
  *         s.time_type = c_jsdrv.JSDRV_TIME_UTC
  *         s.time.utc.start = r['start']             # <<<<<<<<<<<<<<
  *         s.time.utc.end = r.get('end', 0)
  *         s.time.utc.length = r.get('length', 0)
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_t_1); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_t_1); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_s.time.utc.start = __pyx_t_6;
 
-    /* "pyjoulescope_driver/binding.pyx":178
+    /* "pyjoulescope_driver/binding.pyx":180
  *         s.time_type = c_jsdrv.JSDRV_TIME_UTC
  *         s.time.utc.start = r['start']
  *         s.time.utc.end = r.get('end', 0)             # <<<<<<<<<<<<<<
  *         s.time.utc.length = r.get('length', 0)
  *     elif time_type == 'samples':
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_r, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_r, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_t_2); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_t_2); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_s.time.utc.end = __pyx_t_6;
 
-    /* "pyjoulescope_driver/binding.pyx":179
+    /* "pyjoulescope_driver/binding.pyx":181
  *         s.time.utc.start = r['start']
  *         s.time.utc.end = r.get('end', 0)
  *         s.time.utc.length = r.get('length', 0)             # <<<<<<<<<<<<<<
  *     elif time_type == 'samples':
  *         s.time_type = c_jsdrv.JSDRV_TIME_SAMPLES
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_r, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_r, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_t_1); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_t_1); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_s.time.utc.length = __pyx_t_7;
 
-    /* "pyjoulescope_driver/binding.pyx":175
+    /* "pyjoulescope_driver/binding.pyx":177
  *     s.version = 1
  *     time_type = r['time_type'].lower()
  *     if time_type == 'utc':             # <<<<<<<<<<<<<<
  *         s.time_type = c_jsdrv.JSDRV_TIME_UTC
  *         s.time.utc.start = r['start']
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":180
+  /* "pyjoulescope_driver/binding.pyx":182
  *         s.time.utc.end = r.get('end', 0)
  *         s.time.utc.length = r.get('length', 0)
  *     elif time_type == 'samples':             # <<<<<<<<<<<<<<
  *         s.time_type = c_jsdrv.JSDRV_TIME_SAMPLES
  *         s.time.samples.start = r['start']
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_time_type, __pyx_n_u_samples, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_time_type, __pyx_n_u_samples, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 182, __pyx_L1_error)
   if (likely(__pyx_t_5)) {
 
-    /* "pyjoulescope_driver/binding.pyx":181
+    /* "pyjoulescope_driver/binding.pyx":183
  *         s.time.utc.length = r.get('length', 0)
  *     elif time_type == 'samples':
  *         s.time_type = c_jsdrv.JSDRV_TIME_SAMPLES             # <<<<<<<<<<<<<<
  *         s.time.samples.start = r['start']
  *         s.time.samples.end = r.get('end', 0)
  */
     __pyx_v_s.time_type = JSDRV_TIME_SAMPLES;
 
-    /* "pyjoulescope_driver/binding.pyx":182
+    /* "pyjoulescope_driver/binding.pyx":184
  *     elif time_type == 'samples':
  *         s.time_type = c_jsdrv.JSDRV_TIME_SAMPLES
  *         s.time.samples.start = r['start']             # <<<<<<<<<<<<<<
  *         s.time.samples.end = r.get('end', 0)
  *         s.time.samples.length = r.get('length', 0)
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_t_1); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_t_1); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_s.time.samples.start = __pyx_t_7;
 
-    /* "pyjoulescope_driver/binding.pyx":183
+    /* "pyjoulescope_driver/binding.pyx":185
  *         s.time_type = c_jsdrv.JSDRV_TIME_SAMPLES
  *         s.time.samples.start = r['start']
  *         s.time.samples.end = r.get('end', 0)             # <<<<<<<<<<<<<<
  *         s.time.samples.length = r.get('length', 0)
  *     else:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_r, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_r, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_t_2); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_t_2); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_s.time.samples.end = __pyx_t_7;
 
-    /* "pyjoulescope_driver/binding.pyx":184
+    /* "pyjoulescope_driver/binding.pyx":186
  *         s.time.samples.start = r['start']
  *         s.time.samples.end = r.get('end', 0)
  *         s.time.samples.length = r.get('length', 0)             # <<<<<<<<<<<<<<
  *     else:
  *         raise ValueError(f'invalid time type: {time_type}')
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_r, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_r, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_t_1); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_As_uint64_t(__pyx_t_1); if (unlikely((__pyx_t_7 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_s.time.samples.length = __pyx_t_7;
 
-    /* "pyjoulescope_driver/binding.pyx":180
+    /* "pyjoulescope_driver/binding.pyx":182
  *         s.time.utc.end = r.get('end', 0)
  *         s.time.utc.length = r.get('length', 0)
  *     elif time_type == 'samples':             # <<<<<<<<<<<<<<
  *         s.time_type = c_jsdrv.JSDRV_TIME_SAMPLES
  *         s.time.samples.start = r['start']
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":186
+  /* "pyjoulescope_driver/binding.pyx":188
  *         s.time.samples.length = r.get('length', 0)
  *     else:
  *         raise ValueError(f'invalid time type: {time_type}')             # <<<<<<<<<<<<<<
  *     s.rsv1_u8 = 0
  *     s.rsv2_u8 = 0
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_time_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_time_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_time_type, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_time_type, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 186, __pyx_L1_error)
+    __PYX_ERR(0, 188, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "pyjoulescope_driver/binding.pyx":187
+  /* "pyjoulescope_driver/binding.pyx":189
  *     else:
  *         raise ValueError(f'invalid time type: {time_type}')
  *     s.rsv1_u8 = 0             # <<<<<<<<<<<<<<
  *     s.rsv2_u8 = 0
  *     s.rsv3_u32 = 0
  */
   __pyx_v_s.rsv1_u8 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":188
+  /* "pyjoulescope_driver/binding.pyx":190
  *         raise ValueError(f'invalid time type: {time_type}')
  *     s.rsv1_u8 = 0
  *     s.rsv2_u8 = 0             # <<<<<<<<<<<<<<
  *     s.rsv3_u32 = 0
  *     strcpy(s.rsp_topic, <const char *> &rsp_topic_str[0])
  */
   __pyx_v_s.rsv2_u8 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":189
+  /* "pyjoulescope_driver/binding.pyx":191
  *     s.rsv1_u8 = 0
  *     s.rsv2_u8 = 0
  *     s.rsv3_u32 = 0             # <<<<<<<<<<<<<<
  *     strcpy(s.rsp_topic, <const char *> &rsp_topic_str[0])
  *     s.rsp_id = int(r['rsp_id'])
  */
   __pyx_v_s.rsv3_u32 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":190
+  /* "pyjoulescope_driver/binding.pyx":192
  *     s.rsv2_u8 = 0
  *     s.rsv3_u32 = 0
  *     strcpy(s.rsp_topic, <const char *> &rsp_topic_str[0])             # <<<<<<<<<<<<<<
  *     s.rsp_id = int(r['rsp_id'])
  * 
  */
   __pyx_t_8 = 0;
   __pyx_t_9 = -1;
   if (__pyx_t_8 < 0) {
     __pyx_t_8 += __pyx_v_rsp_topic_str.shape[0];
     if (unlikely(__pyx_t_8 < 0)) __pyx_t_9 = 0;
   } else if (unlikely(__pyx_t_8 >= __pyx_v_rsp_topic_str.shape[0])) __pyx_t_9 = 0;
   if (unlikely(__pyx_t_9 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_9);
-    __PYX_ERR(0, 190, __pyx_L1_error)
+    __PYX_ERR(0, 192, __pyx_L1_error)
   }
   (void)(strcpy(__pyx_v_s.rsp_topic, ((char const *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_rsp_topic_str.data + __pyx_t_8 * __pyx_v_rsp_topic_str.strides[0]) )))))));
 
-  /* "pyjoulescope_driver/binding.pyx":191
+  /* "pyjoulescope_driver/binding.pyx":193
  *     s.rsv3_u32 = 0
  *     strcpy(s.rsp_topic, <const char *> &rsp_topic_str[0])
  *     s.rsp_id = int(r['rsp_id'])             # <<<<<<<<<<<<<<
  * 
  *     u8_ptr = <uint8_t *> &s;
  */
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_rsp_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r, __pyx_n_u_rsp_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_t_2); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_t_2); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_s.rsp_id = __pyx_t_6;
 
-  /* "pyjoulescope_driver/binding.pyx":193
+  /* "pyjoulescope_driver/binding.pyx":195
  *     s.rsp_id = int(r['rsp_id'])
  * 
  *     u8_ptr = <uint8_t *> &s;             # <<<<<<<<<<<<<<
  *     return bytes(u8_ptr[:sizeof(s)])
  * 
  */
   __pyx_v_u8_ptr = ((uint8_t *)(&__pyx_v_s));
 
-  /* "pyjoulescope_driver/binding.pyx":194
+  /* "pyjoulescope_driver/binding.pyx":196
  * 
  *     u8_ptr = <uint8_t *> &s;
  *     return bytes(u8_ptr[:sizeof(s)])             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_v_u8_ptr) + 0, (sizeof(__pyx_v_s)) - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_v_u8_ptr) + 0, (sizeof(__pyx_v_s)) - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":168
+  /* "pyjoulescope_driver/binding.pyx":170
  * 
  * 
  * cdef object _pack_buffer_req(r):             # <<<<<<<<<<<<<<
  *     cdef const uint8_t[:] rsp_topic_str = r['rsp_topic'].encode('utf-8')
  *     cdef c_jsdrv.jsdrv_buffer_request_s s
  */
 
@@ -5221,15 +5220,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_rsp_topic_str, 1);
   __Pyx_XDECREF(__pyx_v_time_type);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":198
+/* "pyjoulescope_driver/binding.pyx":200
  * 
  * 
  * cdef object _jsdrv_union_to_py(const c_jsdrv.jsdrv_union_s * value):             # <<<<<<<<<<<<<<
  *     cdef c_jsdrv.jsdrv_stream_signal_s * stream;
  *     cdef np.npy_intp shape[1]
  */
 
@@ -5282,25 +5281,25 @@
   PyObject *__pyx_t_26 = NULL;
   PyObject *__pyx_t_27 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_jsdrv_union_to_py", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":203
+  /* "pyjoulescope_driver/binding.pyx":205
  *     cdef uint8_t[:] u8_mem
  *     cdef int32_t idx
  *     t = value[0].type             # <<<<<<<<<<<<<<
  *     try:
  *         if t == c_jsdrv.JSDRV_UNION_STR:
  */
   __pyx_t_1 = (__pyx_v_value[0]).type;
   __pyx_v_t = __pyx_t_1;
 
-  /* "pyjoulescope_driver/binding.pyx":204
+  /* "pyjoulescope_driver/binding.pyx":206
  *     cdef int32_t idx
  *     t = value[0].type
  *     try:             # <<<<<<<<<<<<<<
  *         if t == c_jsdrv.JSDRV_UNION_STR:
  *             v = value[0].value.str.decode('utf-8')
  */
   {
@@ -5308,63 +5307,63 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pyjoulescope_driver/binding.pyx":205
+      /* "pyjoulescope_driver/binding.pyx":207
  *     t = value[0].type
  *     try:
  *         if t == c_jsdrv.JSDRV_UNION_STR:             # <<<<<<<<<<<<<<
  *             v = value[0].value.str.decode('utf-8')
  *         elif t == c_jsdrv.JSDRV_UNION_JSON:
  */
       switch (__pyx_v_t) {
         case JSDRV_UNION_STR:
 
-        /* "pyjoulescope_driver/binding.pyx":206
+        /* "pyjoulescope_driver/binding.pyx":208
  *     try:
  *         if t == c_jsdrv.JSDRV_UNION_STR:
  *             v = value[0].value.str.decode('utf-8')             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_JSON:
  *             v = value[0].value.str.decode('utf-8')
  */
         __pyx_t_5 = (__pyx_v_value[0]).value.str;
-        __pyx_t_6 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 206, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 208, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":205
+        /* "pyjoulescope_driver/binding.pyx":207
  *     t = value[0].type
  *     try:
  *         if t == c_jsdrv.JSDRV_UNION_STR:             # <<<<<<<<<<<<<<
  *             v = value[0].value.str.decode('utf-8')
  *         elif t == c_jsdrv.JSDRV_UNION_JSON:
  */
         break;
         case JSDRV_UNION_JSON:
 
-        /* "pyjoulescope_driver/binding.pyx":208
+        /* "pyjoulescope_driver/binding.pyx":210
  *             v = value[0].value.str.decode('utf-8')
  *         elif t == c_jsdrv.JSDRV_UNION_JSON:
  *             v = value[0].value.str.decode('utf-8')             # <<<<<<<<<<<<<<
  *             try:
  *                 v = json.loads(v)
  */
         __pyx_t_5 = (__pyx_v_value[0]).value.str;
-        __pyx_t_6 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 208, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 210, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":209
+        /* "pyjoulescope_driver/binding.pyx":211
  *         elif t == c_jsdrv.JSDRV_UNION_JSON:
  *             v = value[0].value.str.decode('utf-8')
  *             try:             # <<<<<<<<<<<<<<
  *                 v = json.loads(v)
  *             except Exception:
  */
         {
@@ -5372,45 +5371,45 @@
           __Pyx_PyThreadState_assign
           __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
           __Pyx_XGOTREF(__pyx_t_7);
           __Pyx_XGOTREF(__pyx_t_8);
           __Pyx_XGOTREF(__pyx_t_9);
           /*try:*/ {
 
-            /* "pyjoulescope_driver/binding.pyx":210
+            /* "pyjoulescope_driver/binding.pyx":212
  *             v = value[0].value.str.decode('utf-8')
  *             try:
  *                 v = json.loads(v)             # <<<<<<<<<<<<<<
  *             except Exception:
  *                 v = None
  */
-            __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_json); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 210, __pyx_L9_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_json); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 212, __pyx_L9_error)
             __Pyx_GOTREF(__pyx_t_10);
-            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_loads); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 210, __pyx_L9_error)
+            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_loads); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 212, __pyx_L9_error)
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
             __pyx_t_10 = NULL;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
               __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
               if (likely(__pyx_t_10)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
                 __Pyx_INCREF(__pyx_t_10);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_11, function);
               }
             }
             __pyx_t_6 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_10, __pyx_v_v) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_v_v);
             __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 210, __pyx_L9_error)
+            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 212, __pyx_L9_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
             __Pyx_DECREF_SET(__pyx_v_v, __pyx_t_6);
             __pyx_t_6 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":209
+            /* "pyjoulescope_driver/binding.pyx":211
  *         elif t == c_jsdrv.JSDRV_UNION_JSON:
  *             v = value[0].value.str.decode('utf-8')
  *             try:             # <<<<<<<<<<<<<<
  *                 v = json.loads(v)
  *             except Exception:
  */
           }
@@ -5419,30 +5418,30 @@
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           goto __pyx_L14_try_end;
           __pyx_L9_error:;
           __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":211
+          /* "pyjoulescope_driver/binding.pyx":213
  *             try:
  *                 v = json.loads(v)
  *             except Exception:             # <<<<<<<<<<<<<<
  *                 v = None
  *         elif t == c_jsdrv.JSDRV_UNION_BIN:
  */
           __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
           if (__pyx_t_12) {
             __Pyx_AddTraceback("pyjoulescope_driver.binding._jsdrv_union_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
-            if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_11, &__pyx_t_10) < 0) __PYX_ERR(0, 211, __pyx_L11_except_error)
+            if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_11, &__pyx_t_10) < 0) __PYX_ERR(0, 213, __pyx_L11_except_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_GOTREF(__pyx_t_10);
 
-            /* "pyjoulescope_driver/binding.pyx":212
+            /* "pyjoulescope_driver/binding.pyx":214
  *                 v = json.loads(v)
  *             except Exception:
  *                 v = None             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_BIN:
  *             if value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STREAM:
  */
             __Pyx_INCREF(Py_None);
@@ -5451,15 +5450,15 @@
             __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
             __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
             goto __pyx_L10_exception_handled;
           }
           goto __pyx_L11_except_error;
           __pyx_L11_except_error:;
 
-          /* "pyjoulescope_driver/binding.pyx":209
+          /* "pyjoulescope_driver/binding.pyx":211
  *         elif t == c_jsdrv.JSDRV_UNION_JSON:
  *             v = value[0].value.str.decode('utf-8')
  *             try:             # <<<<<<<<<<<<<<
  *                 v = json.loads(v)
  *             except Exception:
  */
           __Pyx_XGIVEREF(__pyx_t_7);
@@ -5471,1781 +5470,1781 @@
           __Pyx_XGIVEREF(__pyx_t_7);
           __Pyx_XGIVEREF(__pyx_t_8);
           __Pyx_XGIVEREF(__pyx_t_9);
           __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
           __pyx_L14_try_end:;
         }
 
-        /* "pyjoulescope_driver/binding.pyx":207
+        /* "pyjoulescope_driver/binding.pyx":209
  *         if t == c_jsdrv.JSDRV_UNION_STR:
  *             v = value[0].value.str.decode('utf-8')
  *         elif t == c_jsdrv.JSDRV_UNION_JSON:             # <<<<<<<<<<<<<<
  *             v = value[0].value.str.decode('utf-8')
  *             try:
  */
         break;
         case JSDRV_UNION_BIN:
 
-        /* "pyjoulescope_driver/binding.pyx":214
+        /* "pyjoulescope_driver/binding.pyx":216
  *                 v = None
  *         elif t == c_jsdrv.JSDRV_UNION_BIN:
  *             if value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STREAM:             # <<<<<<<<<<<<<<
  *                 stream = <c_jsdrv.jsdrv_stream_signal_s *> &(value[0].value.bin[0])
  *                 el = (stream[0].element_type, stream[0].element_size_bits)
  */
         __pyx_t_13 = (((__pyx_v_value[0]).app == JSDRV_PAYLOAD_TYPE_STREAM) != 0);
         if (__pyx_t_13) {
 
-          /* "pyjoulescope_driver/binding.pyx":215
+          /* "pyjoulescope_driver/binding.pyx":217
  *         elif t == c_jsdrv.JSDRV_UNION_BIN:
  *             if value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STREAM:
  *                 stream = <c_jsdrv.jsdrv_stream_signal_s *> &(value[0].value.bin[0])             # <<<<<<<<<<<<<<
  *                 el = (stream[0].element_type, stream[0].element_size_bits)
  *                 v = {
  */
           __pyx_v_stream = ((struct jsdrv_stream_signal_s *)(&((__pyx_v_value[0]).value.bin[0])));
 
-          /* "pyjoulescope_driver/binding.pyx":216
+          /* "pyjoulescope_driver/binding.pyx":218
  *             if value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STREAM:
  *                 stream = <c_jsdrv.jsdrv_stream_signal_s *> &(value[0].value.bin[0])
  *                 el = (stream[0].element_type, stream[0].element_size_bits)             # <<<<<<<<<<<<<<
  *                 v = {
  *                     'sample_id': stream[0].sample_id,
  */
-          __pyx_t_10 = __Pyx_PyInt_From_uint8_t((__pyx_v_stream[0]).element_type); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 216, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyInt_From_uint8_t((__pyx_v_stream[0]).element_type); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 218, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_11 = __Pyx_PyInt_From_uint8_t((__pyx_v_stream[0]).element_size_bits); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 216, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyInt_From_uint8_t((__pyx_v_stream[0]).element_size_bits); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 218, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 216, __pyx_L3_error)
+          __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 218, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_GIVEREF(__pyx_t_10);
           PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_10);
           __Pyx_GIVEREF(__pyx_t_11);
           PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_11);
           __pyx_t_10 = 0;
           __pyx_t_11 = 0;
           __pyx_v_el = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":218
+          /* "pyjoulescope_driver/binding.pyx":220
  *                 el = (stream[0].element_type, stream[0].element_size_bits)
  *                 v = {
  *                     'sample_id': stream[0].sample_id,             # <<<<<<<<<<<<<<
  *                     'utc': c_jsdrv.jsdrv_time_from_counter(&stream[0].time_map, stream[0].sample_id),
  *                     'field_id': stream[0].field_id,
  */
-          __pyx_t_6 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 218, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_11 = __Pyx_PyInt_From_uint64_t((__pyx_v_stream[0]).sample_id); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 218, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyInt_From_uint64_t((__pyx_v_stream[0]).sample_id); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 220, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_sample_id, __pyx_t_11) < 0) __PYX_ERR(0, 218, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_sample_id, __pyx_t_11) < 0) __PYX_ERR(0, 220, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":219
+          /* "pyjoulescope_driver/binding.pyx":221
  *                 v = {
  *                     'sample_id': stream[0].sample_id,
  *                     'utc': c_jsdrv.jsdrv_time_from_counter(&stream[0].time_map, stream[0].sample_id),             # <<<<<<<<<<<<<<
  *                     'field_id': stream[0].field_id,
  *                     'index': stream[0].index,
  */
-          __pyx_t_11 = __Pyx_PyInt_From_int64_t(jsdrv_time_from_counter((&(__pyx_v_stream[0]).time_map), (__pyx_v_stream[0]).sample_id)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 219, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyInt_From_int64_t(jsdrv_time_from_counter((&(__pyx_v_stream[0]).time_map), (__pyx_v_stream[0]).sample_id)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 221, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_utc, __pyx_t_11) < 0) __PYX_ERR(0, 218, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_utc, __pyx_t_11) < 0) __PYX_ERR(0, 220, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":220
+          /* "pyjoulescope_driver/binding.pyx":222
  *                     'sample_id': stream[0].sample_id,
  *                     'utc': c_jsdrv.jsdrv_time_from_counter(&stream[0].time_map, stream[0].sample_id),
  *                     'field_id': stream[0].field_id,             # <<<<<<<<<<<<<<
  *                     'index': stream[0].index,
  *                     'sample_rate': stream[0].sample_rate,
  */
-          __pyx_t_11 = __Pyx_PyInt_From_uint8_t((__pyx_v_stream[0]).field_id); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 220, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyInt_From_uint8_t((__pyx_v_stream[0]).field_id); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 222, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_field_id, __pyx_t_11) < 0) __PYX_ERR(0, 218, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_field_id, __pyx_t_11) < 0) __PYX_ERR(0, 220, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":221
+          /* "pyjoulescope_driver/binding.pyx":223
  *                     'utc': c_jsdrv.jsdrv_time_from_counter(&stream[0].time_map, stream[0].sample_id),
  *                     'field_id': stream[0].field_id,
  *                     'index': stream[0].index,             # <<<<<<<<<<<<<<
  *                     'sample_rate': stream[0].sample_rate,
  *                     'decimate_factor': stream[0].decimate_factor,
  */
-          __pyx_t_11 = __Pyx_PyInt_From_uint8_t((__pyx_v_stream[0]).index); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 221, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyInt_From_uint8_t((__pyx_v_stream[0]).index); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 223, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_index, __pyx_t_11) < 0) __PYX_ERR(0, 218, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_index, __pyx_t_11) < 0) __PYX_ERR(0, 220, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":222
+          /* "pyjoulescope_driver/binding.pyx":224
  *                     'field_id': stream[0].field_id,
  *                     'index': stream[0].index,
  *                     'sample_rate': stream[0].sample_rate,             # <<<<<<<<<<<<<<
  *                     'decimate_factor': stream[0].decimate_factor,
  *                     'time_map': {
  */
-          __pyx_t_11 = __Pyx_PyInt_From_uint32_t((__pyx_v_stream[0]).sample_rate); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 222, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyInt_From_uint32_t((__pyx_v_stream[0]).sample_rate); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 224, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_sample_rate, __pyx_t_11) < 0) __PYX_ERR(0, 218, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_sample_rate, __pyx_t_11) < 0) __PYX_ERR(0, 220, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":223
+          /* "pyjoulescope_driver/binding.pyx":225
  *                     'index': stream[0].index,
  *                     'sample_rate': stream[0].sample_rate,
  *                     'decimate_factor': stream[0].decimate_factor,             # <<<<<<<<<<<<<<
  *                     'time_map': {
  *                         'offset_time': stream[0].time_map.offset_time,
  */
-          __pyx_t_11 = __Pyx_PyInt_From_uint32_t((__pyx_v_stream[0]).decimate_factor); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 223, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyInt_From_uint32_t((__pyx_v_stream[0]).decimate_factor); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 225, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_decimate_factor, __pyx_t_11) < 0) __PYX_ERR(0, 218, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_decimate_factor, __pyx_t_11) < 0) __PYX_ERR(0, 220, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":225
+          /* "pyjoulescope_driver/binding.pyx":227
  *                     'decimate_factor': stream[0].decimate_factor,
  *                     'time_map': {
  *                         'offset_time': stream[0].time_map.offset_time,             # <<<<<<<<<<<<<<
  *                         'offset_counter': stream[0].time_map.offset_counter,
  *                         'counter_rate': stream[0].time_map.counter_rate,
  */
-          __pyx_t_11 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 225, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 227, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_10 = __Pyx_PyInt_From_int64_t((__pyx_v_stream[0]).time_map.offset_time); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 225, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyInt_From_int64_t((__pyx_v_stream[0]).time_map.offset_time); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 227, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_offset_time, __pyx_t_10) < 0) __PYX_ERR(0, 225, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_offset_time, __pyx_t_10) < 0) __PYX_ERR(0, 227, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":226
+          /* "pyjoulescope_driver/binding.pyx":228
  *                     'time_map': {
  *                         'offset_time': stream[0].time_map.offset_time,
  *                         'offset_counter': stream[0].time_map.offset_counter,             # <<<<<<<<<<<<<<
  *                         'counter_rate': stream[0].time_map.counter_rate,
  *                     }
  */
-          __pyx_t_10 = __Pyx_PyInt_From_uint64_t((__pyx_v_stream[0]).time_map.offset_counter); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 226, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyInt_From_uint64_t((__pyx_v_stream[0]).time_map.offset_counter); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 228, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_offset_counter, __pyx_t_10) < 0) __PYX_ERR(0, 225, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_offset_counter, __pyx_t_10) < 0) __PYX_ERR(0, 227, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":227
+          /* "pyjoulescope_driver/binding.pyx":229
  *                         'offset_time': stream[0].time_map.offset_time,
  *                         'offset_counter': stream[0].time_map.offset_counter,
  *                         'counter_rate': stream[0].time_map.counter_rate,             # <<<<<<<<<<<<<<
  *                     }
  *                 }
  */
-          __pyx_t_10 = PyFloat_FromDouble((__pyx_v_stream[0]).time_map.counter_rate); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 227, __pyx_L3_error)
+          __pyx_t_10 = PyFloat_FromDouble((__pyx_v_stream[0]).time_map.counter_rate); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 229, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_counter_rate, __pyx_t_10) < 0) __PYX_ERR(0, 225, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_counter_rate, __pyx_t_10) < 0) __PYX_ERR(0, 227, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_time_map, __pyx_t_11) < 0) __PYX_ERR(0, 218, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_time_map, __pyx_t_11) < 0) __PYX_ERR(0, 220, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           __pyx_v_v = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":230
+          /* "pyjoulescope_driver/binding.pyx":232
  *                     }
  *                 }
  *                 if el == (c_jsdrv.JSDRV_DATA_TYPE_FLOAT, 32):  # float32             # <<<<<<<<<<<<<<
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> stream[0].data)
  */
-          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_FLOAT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 230, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_FLOAT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 230, __pyx_L3_error)
+          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 232, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_6);
           PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_6);
           __Pyx_INCREF(__pyx_int_32);
           __Pyx_GIVEREF(__pyx_int_32);
           PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_int_32);
           __pyx_t_6 = 0;
-          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 230, __pyx_L3_error)
+          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 230, __pyx_L3_error)
+          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 232, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           if (__pyx_t_13) {
 
-            /* "pyjoulescope_driver/binding.pyx":231
+            /* "pyjoulescope_driver/binding.pyx":233
  *                 }
  *                 if el == (c_jsdrv.JSDRV_DATA_TYPE_FLOAT, 32):  # float32
  *                     shape[0] = <np.npy_intp> stream[0].element_count             # <<<<<<<<<<<<<<
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  */
             (__pyx_v_shape[0]) = ((npy_intp)(__pyx_v_stream[0]).element_count);
 
-            /* "pyjoulescope_driver/binding.pyx":232
+            /* "pyjoulescope_driver/binding.pyx":234
  *                 if el == (c_jsdrv.JSDRV_DATA_TYPE_FLOAT, 32):  # float32
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> stream[0].data)             # <<<<<<<<<<<<<<
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 1):  # uint1, 8 per uint8
  */
-            __pyx_t_6 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_FLOAT32, ((void *)(__pyx_v_stream[0]).data)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 232, __pyx_L3_error)
+            __pyx_t_6 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_FLOAT32, ((void *)(__pyx_v_stream[0]).data)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
             __pyx_v_ndarray = __pyx_t_6;
             __pyx_t_6 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":233
+            /* "pyjoulescope_driver/binding.pyx":235
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()             # <<<<<<<<<<<<<<
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 1):  # uint1, 8 per uint8
  *                     shape[0] = <np.npy_intp> ((stream[0].element_count + 7) / 8)
  */
-            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 233, __pyx_L3_error)
+            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 235, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_11);
             __pyx_t_10 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
               __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
               if (likely(__pyx_t_10)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
                 __Pyx_INCREF(__pyx_t_10);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_11, function);
               }
             }
             __pyx_t_6 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
             __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 233, __pyx_L3_error)
+            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_6) < 0)) __PYX_ERR(0, 233, __pyx_L3_error)
+            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_6) < 0)) __PYX_ERR(0, 235, __pyx_L3_error)
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":230
+            /* "pyjoulescope_driver/binding.pyx":232
  *                     }
  *                 }
  *                 if el == (c_jsdrv.JSDRV_DATA_TYPE_FLOAT, 32):  # float32             # <<<<<<<<<<<<<<
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> stream[0].data)
  */
             goto __pyx_L18;
           }
 
-          /* "pyjoulescope_driver/binding.pyx":234
+          /* "pyjoulescope_driver/binding.pyx":236
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 1):  # uint1, 8 per uint8             # <<<<<<<<<<<<<<
  *                     shape[0] = <np.npy_intp> ((stream[0].element_count + 7) / 8)
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  */
-          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_UINT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_UINT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 236, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 234, __pyx_L3_error)
+          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 236, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_6);
           PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_6);
           __Pyx_INCREF(__pyx_int_1);
           __Pyx_GIVEREF(__pyx_int_1);
           PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_int_1);
           __pyx_t_6 = 0;
-          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L3_error)
+          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 236, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 234, __pyx_L3_error)
+          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 236, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           if (__pyx_t_13) {
 
-            /* "pyjoulescope_driver/binding.pyx":235
+            /* "pyjoulescope_driver/binding.pyx":237
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 1):  # uint1, 8 per uint8
  *                     shape[0] = <np.npy_intp> ((stream[0].element_count + 7) / 8)             # <<<<<<<<<<<<<<
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  */
             (__pyx_v_shape[0]) = ((npy_intp)(((double)((__pyx_v_stream[0]).element_count + 7)) / 8.0));
 
-            /* "pyjoulescope_driver/binding.pyx":236
+            /* "pyjoulescope_driver/binding.pyx":238
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 1):  # uint1, 8 per uint8
  *                     shape[0] = <np.npy_intp> ((stream[0].element_count + 7) / 8)
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)             # <<<<<<<<<<<<<<
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_INT, 16):  # int16
  */
-            __pyx_t_6 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_UINT8, ((void *)(__pyx_v_stream[0]).data)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 236, __pyx_L3_error)
+            __pyx_t_6 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_UINT8, ((void *)(__pyx_v_stream[0]).data)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
             __pyx_v_ndarray = __pyx_t_6;
             __pyx_t_6 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":237
+            /* "pyjoulescope_driver/binding.pyx":239
  *                     shape[0] = <np.npy_intp> ((stream[0].element_count + 7) / 8)
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()             # <<<<<<<<<<<<<<
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_INT, 16):  # int16
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  */
-            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 237, __pyx_L3_error)
+            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 239, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_11);
             __pyx_t_10 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
               __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
               if (likely(__pyx_t_10)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
                 __Pyx_INCREF(__pyx_t_10);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_11, function);
               }
             }
             __pyx_t_6 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
             __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 237, __pyx_L3_error)
+            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 239, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_6) < 0)) __PYX_ERR(0, 237, __pyx_L3_error)
+            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_6) < 0)) __PYX_ERR(0, 239, __pyx_L3_error)
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":234
+            /* "pyjoulescope_driver/binding.pyx":236
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_FLOAT32, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 1):  # uint1, 8 per uint8             # <<<<<<<<<<<<<<
  *                     shape[0] = <np.npy_intp> ((stream[0].element_count + 7) / 8)
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  */
             goto __pyx_L18;
           }
 
-          /* "pyjoulescope_driver/binding.pyx":238
+          /* "pyjoulescope_driver/binding.pyx":240
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_INT, 16):  # int16             # <<<<<<<<<<<<<<
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_INT16, <void *> stream[0].data)
  */
-          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_INT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_INT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 240, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 238, __pyx_L3_error)
+          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 240, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_6);
           PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_6);
           __Pyx_INCREF(__pyx_int_16);
           __Pyx_GIVEREF(__pyx_int_16);
           PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_int_16);
           __pyx_t_6 = 0;
-          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L3_error)
+          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 240, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 238, __pyx_L3_error)
+          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 240, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           if (__pyx_t_13) {
 
-            /* "pyjoulescope_driver/binding.pyx":239
+            /* "pyjoulescope_driver/binding.pyx":241
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_INT, 16):  # int16
  *                     shape[0] = <np.npy_intp> stream[0].element_count             # <<<<<<<<<<<<<<
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_INT16, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  */
             (__pyx_v_shape[0]) = ((npy_intp)(__pyx_v_stream[0]).element_count);
 
-            /* "pyjoulescope_driver/binding.pyx":240
+            /* "pyjoulescope_driver/binding.pyx":242
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_INT, 16):  # int16
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_INT16, <void *> stream[0].data)             # <<<<<<<<<<<<<<
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 8):  # uint8
  */
-            __pyx_t_6 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_INT16, ((void *)(__pyx_v_stream[0]).data)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 240, __pyx_L3_error)
+            __pyx_t_6 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_INT16, ((void *)(__pyx_v_stream[0]).data)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
             __pyx_v_ndarray = __pyx_t_6;
             __pyx_t_6 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":241
+            /* "pyjoulescope_driver/binding.pyx":243
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_INT16, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()             # <<<<<<<<<<<<<<
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 8):  # uint8
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  */
-            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 241, __pyx_L3_error)
+            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 243, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_11);
             __pyx_t_10 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
               __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
               if (likely(__pyx_t_10)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
                 __Pyx_INCREF(__pyx_t_10);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_11, function);
               }
             }
             __pyx_t_6 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
             __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 241, __pyx_L3_error)
+            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_6) < 0)) __PYX_ERR(0, 241, __pyx_L3_error)
+            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_6) < 0)) __PYX_ERR(0, 243, __pyx_L3_error)
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":238
+            /* "pyjoulescope_driver/binding.pyx":240
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_INT, 16):  # int16             # <<<<<<<<<<<<<<
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_INT16, <void *> stream[0].data)
  */
             goto __pyx_L18;
           }
 
-          /* "pyjoulescope_driver/binding.pyx":242
+          /* "pyjoulescope_driver/binding.pyx":244
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_INT16, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 8):  # uint8             # <<<<<<<<<<<<<<
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  */
-          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_UINT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_UINT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 242, __pyx_L3_error)
+          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 244, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_6);
           PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_6);
           __Pyx_INCREF(__pyx_int_8);
           __Pyx_GIVEREF(__pyx_int_8);
           PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_int_8);
           __pyx_t_6 = 0;
-          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L3_error)
+          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 242, __pyx_L3_error)
+          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 244, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           if (__pyx_t_13) {
 
-            /* "pyjoulescope_driver/binding.pyx":243
+            /* "pyjoulescope_driver/binding.pyx":245
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 8):  # uint8
  *                     shape[0] = <np.npy_intp> stream[0].element_count             # <<<<<<<<<<<<<<
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  */
             (__pyx_v_shape[0]) = ((npy_intp)(__pyx_v_stream[0]).element_count);
 
-            /* "pyjoulescope_driver/binding.pyx":244
+            /* "pyjoulescope_driver/binding.pyx":246
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 8):  # uint8
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)             # <<<<<<<<<<<<<<
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 4):  # uint4 -> uint8
  */
-            __pyx_t_6 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_UINT8, ((void *)(__pyx_v_stream[0]).data)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L3_error)
+            __pyx_t_6 = PyArray_SimpleNewFromData(1, __pyx_v_shape, NPY_UINT8, ((void *)(__pyx_v_stream[0]).data)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
             __pyx_v_ndarray = __pyx_t_6;
             __pyx_t_6 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":245
+            /* "pyjoulescope_driver/binding.pyx":247
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()             # <<<<<<<<<<<<<<
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 4):  # uint4 -> uint8
  *                     # unpack to make i/range support easy
  */
-            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 245, __pyx_L3_error)
+            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ndarray, __pyx_n_s_copy); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 247, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_11);
             __pyx_t_10 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
               __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
               if (likely(__pyx_t_10)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
                 __Pyx_INCREF(__pyx_t_10);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_11, function);
               }
             }
             __pyx_t_6 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
             __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 245, __pyx_L3_error)
+            if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_6) < 0)) __PYX_ERR(0, 245, __pyx_L3_error)
+            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_t_6) < 0)) __PYX_ERR(0, 247, __pyx_L3_error)
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":242
+            /* "pyjoulescope_driver/binding.pyx":244
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_INT16, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 8):  # uint8             # <<<<<<<<<<<<<<
  *                     shape[0] = <np.npy_intp> stream[0].element_count
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  */
             goto __pyx_L18;
           }
 
-          /* "pyjoulescope_driver/binding.pyx":246
+          /* "pyjoulescope_driver/binding.pyx":248
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 4):  # uint4 -> uint8             # <<<<<<<<<<<<<<
  *                     # unpack to make i/range support easy
  *                     # future uses may want to leave packed, so may need to check JSDRV_FIELD_RANGE
  */
-          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_UINT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyInt_From_enum__jsdrv_element_type_e(JSDRV_DATA_TYPE_UINT); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 246, __pyx_L3_error)
+          __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 248, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_6);
           PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_6);
           __Pyx_INCREF(__pyx_int_4);
           __Pyx_GIVEREF(__pyx_int_4);
           PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_int_4);
           __pyx_t_6 = 0;
-          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L3_error)
+          __pyx_t_6 = PyObject_RichCompare(__pyx_v_el, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 246, __pyx_L3_error)
+          __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 248, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           if (__pyx_t_13) {
 
-            /* "pyjoulescope_driver/binding.pyx":249
+            /* "pyjoulescope_driver/binding.pyx":251
  *                     # unpack to make i/range support easy
  *                     # future uses may want to leave packed, so may need to check JSDRV_FIELD_RANGE
  *                     ndarray = np.empty(stream[0].element_count, dtype=np.uint8)             # <<<<<<<<<<<<<<
  *                     u8_mem = ndarray
  *                     for idx in range(0, stream[0].element_count >> 1):
  */
-            __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L3_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 251, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
-            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 249, __pyx_L3_error)
+            __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 251, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-            __pyx_t_6 = __Pyx_PyInt_From_uint32_t((__pyx_v_stream[0]).element_count); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L3_error)
+            __pyx_t_6 = __Pyx_PyInt_From_uint32_t((__pyx_v_stream[0]).element_count); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 251, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
-            __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 249, __pyx_L3_error)
+            __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 251, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_10);
             __Pyx_GIVEREF(__pyx_t_6);
             PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_6);
             __pyx_t_6 = 0;
-            __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L3_error)
+            __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 251, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_6);
-            __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 249, __pyx_L3_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 251, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_14);
-            __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_uint8); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 249, __pyx_L3_error)
+            __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_uint8); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 251, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_15);
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-            if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_15) < 0) __PYX_ERR(0, 249, __pyx_L3_error)
+            if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_15) < 0) __PYX_ERR(0, 251, __pyx_L3_error)
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-            __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_10, __pyx_t_6); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 249, __pyx_L3_error)
+            __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_10, __pyx_t_6); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 251, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_15);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
             __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
             __pyx_v_ndarray = __pyx_t_15;
             __pyx_t_15 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":250
+            /* "pyjoulescope_driver/binding.pyx":252
  *                     # future uses may want to leave packed, so may need to check JSDRV_FIELD_RANGE
  *                     ndarray = np.empty(stream[0].element_count, dtype=np.uint8)
  *                     u8_mem = ndarray             # <<<<<<<<<<<<<<
  *                     for idx in range(0, stream[0].element_count >> 1):
  *                         u8_mem[2 * idx] = stream[0].data[idx] & 0x0f
  */
-            __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t(__pyx_v_ndarray, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 250, __pyx_L3_error)
+            __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t(__pyx_v_ndarray, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 252, __pyx_L3_error)
             __pyx_v_u8_mem = __pyx_t_16;
             __pyx_t_16.memview = NULL;
             __pyx_t_16.data = NULL;
 
-            /* "pyjoulescope_driver/binding.pyx":251
+            /* "pyjoulescope_driver/binding.pyx":253
  *                     ndarray = np.empty(stream[0].element_count, dtype=np.uint8)
  *                     u8_mem = ndarray
  *                     for idx in range(0, stream[0].element_count >> 1):             # <<<<<<<<<<<<<<
  *                         u8_mem[2 * idx] = stream[0].data[idx] & 0x0f
  *                         u8_mem[2 * idx + 1] = (stream[0].data[idx] >> 4) & 0x0f
  */
             __pyx_t_17 = ((__pyx_v_stream[0]).element_count >> 1);
             __pyx_t_18 = __pyx_t_17;
             for (__pyx_t_19 = 0; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
               __pyx_v_idx = __pyx_t_19;
 
-              /* "pyjoulescope_driver/binding.pyx":252
+              /* "pyjoulescope_driver/binding.pyx":254
  *                     u8_mem = ndarray
  *                     for idx in range(0, stream[0].element_count >> 1):
  *                         u8_mem[2 * idx] = stream[0].data[idx] & 0x0f             # <<<<<<<<<<<<<<
  *                         u8_mem[2 * idx + 1] = (stream[0].data[idx] >> 4) & 0x0f
  *                     v['data'] = ndarray
  */
               __pyx_t_20 = (2 * __pyx_v_idx);
               __pyx_t_12 = -1;
               if (__pyx_t_20 < 0) {
                 __pyx_t_20 += __pyx_v_u8_mem.shape[0];
                 if (unlikely(__pyx_t_20 < 0)) __pyx_t_12 = 0;
               } else if (unlikely(__pyx_t_20 >= __pyx_v_u8_mem.shape[0])) __pyx_t_12 = 0;
               if (unlikely(__pyx_t_12 != -1)) {
                 __Pyx_RaiseBufferIndexError(__pyx_t_12);
-                __PYX_ERR(0, 252, __pyx_L3_error)
+                __PYX_ERR(0, 254, __pyx_L3_error)
               }
               *((uint8_t *) ( /* dim=0 */ (__pyx_v_u8_mem.data + __pyx_t_20 * __pyx_v_u8_mem.strides[0]) )) = (((__pyx_v_stream[0]).data[__pyx_v_idx]) & 0x0f);
 
-              /* "pyjoulescope_driver/binding.pyx":253
+              /* "pyjoulescope_driver/binding.pyx":255
  *                     for idx in range(0, stream[0].element_count >> 1):
  *                         u8_mem[2 * idx] = stream[0].data[idx] & 0x0f
  *                         u8_mem[2 * idx + 1] = (stream[0].data[idx] >> 4) & 0x0f             # <<<<<<<<<<<<<<
  *                     v['data'] = ndarray
  *                 else:
  */
               __pyx_t_20 = ((2 * __pyx_v_idx) + 1);
               __pyx_t_12 = -1;
               if (__pyx_t_20 < 0) {
                 __pyx_t_20 += __pyx_v_u8_mem.shape[0];
                 if (unlikely(__pyx_t_20 < 0)) __pyx_t_12 = 0;
               } else if (unlikely(__pyx_t_20 >= __pyx_v_u8_mem.shape[0])) __pyx_t_12 = 0;
               if (unlikely(__pyx_t_12 != -1)) {
                 __Pyx_RaiseBufferIndexError(__pyx_t_12);
-                __PYX_ERR(0, 253, __pyx_L3_error)
+                __PYX_ERR(0, 255, __pyx_L3_error)
               }
               *((uint8_t *) ( /* dim=0 */ (__pyx_v_u8_mem.data + __pyx_t_20 * __pyx_v_u8_mem.strides[0]) )) = ((((__pyx_v_stream[0]).data[__pyx_v_idx]) >> 4) & 0x0f);
             }
 
-            /* "pyjoulescope_driver/binding.pyx":254
+            /* "pyjoulescope_driver/binding.pyx":256
  *                         u8_mem[2 * idx] = stream[0].data[idx] & 0x0f
  *                         u8_mem[2 * idx + 1] = (stream[0].data[idx] >> 4) & 0x0f
  *                     v['data'] = ndarray             # <<<<<<<<<<<<<<
  *                 else:
  *                     print('jsdrv._jsdrv_union_to_py: unsupported data type')
  */
-            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_v_ndarray) < 0)) __PYX_ERR(0, 254, __pyx_L3_error)
+            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, __pyx_v_ndarray) < 0)) __PYX_ERR(0, 256, __pyx_L3_error)
 
-            /* "pyjoulescope_driver/binding.pyx":246
+            /* "pyjoulescope_driver/binding.pyx":248
  *                     ndarray = np.PyArray_SimpleNewFromData(1, shape, np.NPY_UINT8, <void *> stream[0].data)
  *                     v['data'] = ndarray.copy()
  *                 elif el == (c_jsdrv.JSDRV_DATA_TYPE_UINT, 4):  # uint4 -> uint8             # <<<<<<<<<<<<<<
  *                     # unpack to make i/range support easy
  *                     # future uses may want to leave packed, so may need to check JSDRV_FIELD_RANGE
  */
             goto __pyx_L18;
           }
 
-          /* "pyjoulescope_driver/binding.pyx":256
+          /* "pyjoulescope_driver/binding.pyx":258
  *                     v['data'] = ndarray
  *                 else:
  *                     print('jsdrv._jsdrv_union_to_py: unsupported data type')             # <<<<<<<<<<<<<<
  *                     v['data'] = None
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STATISTICS:
  */
           /*else*/ {
-            __pyx_t_15 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 256, __pyx_L3_error)
+            __pyx_t_15 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 258, __pyx_L3_error)
             __Pyx_GOTREF(__pyx_t_15);
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-            /* "pyjoulescope_driver/binding.pyx":257
+            /* "pyjoulescope_driver/binding.pyx":259
  *                 else:
  *                     print('jsdrv._jsdrv_union_to_py: unsupported data type')
  *                     v['data'] = None             # <<<<<<<<<<<<<<
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STATISTICS:
  *                 stats = <c_jsdrv.jsdrv_statistics_s *> &(value[0].value.bin[0])
  */
-            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, Py_None) < 0)) __PYX_ERR(0, 257, __pyx_L3_error)
+            if (unlikely(PyObject_SetItem(__pyx_v_v, __pyx_n_u_data, Py_None) < 0)) __PYX_ERR(0, 259, __pyx_L3_error)
           }
           __pyx_L18:;
 
-          /* "pyjoulescope_driver/binding.pyx":214
+          /* "pyjoulescope_driver/binding.pyx":216
  *                 v = None
  *         elif t == c_jsdrv.JSDRV_UNION_BIN:
  *             if value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STREAM:             # <<<<<<<<<<<<<<
  *                 stream = <c_jsdrv.jsdrv_stream_signal_s *> &(value[0].value.bin[0])
  *                 el = (stream[0].element_type, stream[0].element_size_bits)
  */
           goto __pyx_L17;
         }
 
-        /* "pyjoulescope_driver/binding.pyx":258
+        /* "pyjoulescope_driver/binding.pyx":260
  *                     print('jsdrv._jsdrv_union_to_py: unsupported data type')
  *                     v['data'] = None
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STATISTICS:             # <<<<<<<<<<<<<<
  *                 stats = <c_jsdrv.jsdrv_statistics_s *> &(value[0].value.bin[0])
  *                 sample_freq = stats[0].sample_freq
  */
         __pyx_t_13 = (((__pyx_v_value[0]).app == JSDRV_PAYLOAD_TYPE_STATISTICS) != 0);
         if (__pyx_t_13) {
 
-          /* "pyjoulescope_driver/binding.pyx":259
+          /* "pyjoulescope_driver/binding.pyx":261
  *                     v['data'] = None
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STATISTICS:
  *                 stats = <c_jsdrv.jsdrv_statistics_s *> &(value[0].value.bin[0])             # <<<<<<<<<<<<<<
  *                 sample_freq = stats[0].sample_freq
  *                 samples_full_rate = stats[0].block_sample_count * stats[0].decimate_factor
  */
           __pyx_v_stats = ((struct jsdrv_statistics_s *)(&((__pyx_v_value[0]).value.bin[0])));
 
-          /* "pyjoulescope_driver/binding.pyx":260
+          /* "pyjoulescope_driver/binding.pyx":262
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STATISTICS:
  *                 stats = <c_jsdrv.jsdrv_statistics_s *> &(value[0].value.bin[0])
  *                 sample_freq = stats[0].sample_freq             # <<<<<<<<<<<<<<
  *                 samples_full_rate = stats[0].block_sample_count * stats[0].decimate_factor
  *                 sample_id_start = stats[0].block_sample_id
  */
-          __pyx_t_15 = __Pyx_PyInt_From_uint32_t((__pyx_v_stats[0]).sample_freq); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 260, __pyx_L3_error)
+          __pyx_t_15 = __Pyx_PyInt_From_uint32_t((__pyx_v_stats[0]).sample_freq); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 262, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_15);
           __pyx_v_sample_freq = __pyx_t_15;
           __pyx_t_15 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":261
+          /* "pyjoulescope_driver/binding.pyx":263
  *                 stats = <c_jsdrv.jsdrv_statistics_s *> &(value[0].value.bin[0])
  *                 sample_freq = stats[0].sample_freq
  *                 samples_full_rate = stats[0].block_sample_count * stats[0].decimate_factor             # <<<<<<<<<<<<<<
  *                 sample_id_start = stats[0].block_sample_id
  *                 sample_id_end = stats[0].block_sample_id + samples_full_rate
  */
-          __pyx_t_15 = __Pyx_PyInt_From_uint32_t(((__pyx_v_stats[0]).block_sample_count * (__pyx_v_stats[0]).decimate_factor)); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 261, __pyx_L3_error)
+          __pyx_t_15 = __Pyx_PyInt_From_uint32_t(((__pyx_v_stats[0]).block_sample_count * (__pyx_v_stats[0]).decimate_factor)); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 263, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_15);
           __pyx_v_samples_full_rate = __pyx_t_15;
           __pyx_t_15 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":262
+          /* "pyjoulescope_driver/binding.pyx":264
  *                 sample_freq = stats[0].sample_freq
  *                 samples_full_rate = stats[0].block_sample_count * stats[0].decimate_factor
  *                 sample_id_start = stats[0].block_sample_id             # <<<<<<<<<<<<<<
  *                 sample_id_end = stats[0].block_sample_id + samples_full_rate
  *                 t_start = sample_id_start / sample_freq
  */
-          __pyx_t_15 = __Pyx_PyInt_From_uint64_t((__pyx_v_stats[0]).block_sample_id); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 262, __pyx_L3_error)
+          __pyx_t_15 = __Pyx_PyInt_From_uint64_t((__pyx_v_stats[0]).block_sample_id); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 264, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_15);
           __pyx_v_sample_id_start = __pyx_t_15;
           __pyx_t_15 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":263
+          /* "pyjoulescope_driver/binding.pyx":265
  *                 samples_full_rate = stats[0].block_sample_count * stats[0].decimate_factor
  *                 sample_id_start = stats[0].block_sample_id
  *                 sample_id_end = stats[0].block_sample_id + samples_full_rate             # <<<<<<<<<<<<<<
  *                 t_start = sample_id_start / sample_freq
  *                 t_delta = samples_full_rate / sample_freq
  */
-          __pyx_t_15 = __Pyx_PyInt_From_uint64_t((__pyx_v_stats[0]).block_sample_id); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 263, __pyx_L3_error)
+          __pyx_t_15 = __Pyx_PyInt_From_uint64_t((__pyx_v_stats[0]).block_sample_id); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 265, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_15);
-          __pyx_t_6 = PyNumber_Add(__pyx_t_15, __pyx_v_samples_full_rate); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 263, __pyx_L3_error)
+          __pyx_t_6 = PyNumber_Add(__pyx_t_15, __pyx_v_samples_full_rate); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
           __pyx_v_sample_id_end = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":264
+          /* "pyjoulescope_driver/binding.pyx":266
  *                 sample_id_start = stats[0].block_sample_id
  *                 sample_id_end = stats[0].block_sample_id + samples_full_rate
  *                 t_start = sample_id_start / sample_freq             # <<<<<<<<<<<<<<
  *                 t_delta = samples_full_rate / sample_freq
  *                 charge = _i128_to_int(stats[0].charge_i128[1], stats[0].charge_i128[0])
  */
-          __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_v_sample_id_start, __pyx_v_sample_freq); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 264, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_v_sample_id_start, __pyx_v_sample_freq); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_t_start = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":265
+          /* "pyjoulescope_driver/binding.pyx":267
  *                 sample_id_end = stats[0].block_sample_id + samples_full_rate
  *                 t_start = sample_id_start / sample_freq
  *                 t_delta = samples_full_rate / sample_freq             # <<<<<<<<<<<<<<
  *                 charge = _i128_to_int(stats[0].charge_i128[1], stats[0].charge_i128[0])
  *                 energy = _i128_to_int(stats[0].energy_i128[1], stats[0].energy_i128[0])
  */
-          __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_v_samples_full_rate, __pyx_v_sample_freq); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_v_samples_full_rate, __pyx_v_sample_freq); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 267, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_t_delta = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":266
+          /* "pyjoulescope_driver/binding.pyx":268
  *                 t_start = sample_id_start / sample_freq
  *                 t_delta = samples_full_rate / sample_freq
  *                 charge = _i128_to_int(stats[0].charge_i128[1], stats[0].charge_i128[0])             # <<<<<<<<<<<<<<
  *                 energy = _i128_to_int(stats[0].energy_i128[1], stats[0].energy_i128[0])
  *                 v = {
  */
-          __pyx_t_6 = __pyx_f_19pyjoulescope_driver_7binding__i128_to_int(((__pyx_v_stats[0]).charge_i128[1]), ((__pyx_v_stats[0]).charge_i128[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L3_error)
+          __pyx_t_6 = __pyx_f_19pyjoulescope_driver_7binding__i128_to_int(((__pyx_v_stats[0]).charge_i128[1]), ((__pyx_v_stats[0]).charge_i128[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 268, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_charge = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":267
+          /* "pyjoulescope_driver/binding.pyx":269
  *                 t_delta = samples_full_rate / sample_freq
  *                 charge = _i128_to_int(stats[0].charge_i128[1], stats[0].charge_i128[0])
  *                 energy = _i128_to_int(stats[0].energy_i128[1], stats[0].energy_i128[0])             # <<<<<<<<<<<<<<
  *                 v = {
  *                     'time': {
  */
-          __pyx_t_6 = __pyx_f_19pyjoulescope_driver_7binding__i128_to_int(((__pyx_v_stats[0]).energy_i128[1]), ((__pyx_v_stats[0]).energy_i128[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 267, __pyx_L3_error)
+          __pyx_t_6 = __pyx_f_19pyjoulescope_driver_7binding__i128_to_int(((__pyx_v_stats[0]).energy_i128[1]), ((__pyx_v_stats[0]).energy_i128[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 269, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_energy = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":269
+          /* "pyjoulescope_driver/binding.pyx":271
  *                 energy = _i128_to_int(stats[0].energy_i128[1], stats[0].energy_i128[0])
  *                 v = {
  *                     'time': {             # <<<<<<<<<<<<<<
  *                         'samples': {'value': [sample_id_start, sample_id_end], 'units': 'samples'},
  *                         'utc': {
  */
-          __pyx_t_6 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 269, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 271, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
 
-          /* "pyjoulescope_driver/binding.pyx":270
+          /* "pyjoulescope_driver/binding.pyx":272
  *                 v = {
  *                     'time': {
  *                         'samples': {'value': [sample_id_start, sample_id_end], 'units': 'samples'},             # <<<<<<<<<<<<<<
  *                         'utc': {
  *                             'value': [
  */
-          __pyx_t_15 = __Pyx_PyDict_NewPresized(9); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 270, __pyx_L3_error)
+          __pyx_t_15 = __Pyx_PyDict_NewPresized(9); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_15);
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 270, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_11 = PyList_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 270, __pyx_L3_error)
+          __pyx_t_11 = PyList_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_INCREF(__pyx_v_sample_id_start);
           __Pyx_GIVEREF(__pyx_v_sample_id_start);
           PyList_SET_ITEM(__pyx_t_11, 0, __pyx_v_sample_id_start);
           __Pyx_INCREF(__pyx_v_sample_id_end);
           __Pyx_GIVEREF(__pyx_v_sample_id_end);
           PyList_SET_ITEM(__pyx_t_11, 1, __pyx_v_sample_id_end);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_samples) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_samples, __pyx_t_10) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_samples) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_samples, __pyx_t_10) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":272
+          /* "pyjoulescope_driver/binding.pyx":274
  *                         'samples': {'value': [sample_id_start, sample_id_end], 'units': 'samples'},
  *                         'utc': {
  *                             'value': [             # <<<<<<<<<<<<<<
  *                                 c_jsdrv.jsdrv_time_from_counter(&stats[0].time_map, sample_id_start),
  *                                 c_jsdrv.jsdrv_time_from_counter(&stats[0].time_map, sample_id_end),
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 272, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 274, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
 
-          /* "pyjoulescope_driver/binding.pyx":273
+          /* "pyjoulescope_driver/binding.pyx":275
  *                         'utc': {
  *                             'value': [
  *                                 c_jsdrv.jsdrv_time_from_counter(&stats[0].time_map, sample_id_start),             # <<<<<<<<<<<<<<
  *                                 c_jsdrv.jsdrv_time_from_counter(&stats[0].time_map, sample_id_end),
  *                             ],
  */
-          __pyx_t_21 = __Pyx_PyInt_As_uint64_t(__pyx_v_sample_id_start); if (unlikely((__pyx_t_21 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 273, __pyx_L3_error)
-          __pyx_t_11 = __Pyx_PyInt_From_int64_t(jsdrv_time_from_counter((&(__pyx_v_stats[0]).time_map), __pyx_t_21)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 273, __pyx_L3_error)
+          __pyx_t_21 = __Pyx_PyInt_As_uint64_t(__pyx_v_sample_id_start); if (unlikely((__pyx_t_21 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyInt_From_int64_t(jsdrv_time_from_counter((&(__pyx_v_stats[0]).time_map), __pyx_t_21)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 275, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
 
-          /* "pyjoulescope_driver/binding.pyx":274
+          /* "pyjoulescope_driver/binding.pyx":276
  *                             'value': [
  *                                 c_jsdrv.jsdrv_time_from_counter(&stats[0].time_map, sample_id_start),
  *                                 c_jsdrv.jsdrv_time_from_counter(&stats[0].time_map, sample_id_end),             # <<<<<<<<<<<<<<
  *                             ],
  *                             'units': 'time64',
  */
-          __pyx_t_21 = __Pyx_PyInt_As_uint64_t(__pyx_v_sample_id_end); if (unlikely((__pyx_t_21 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 274, __pyx_L3_error)
-          __pyx_t_14 = __Pyx_PyInt_From_int64_t(jsdrv_time_from_counter((&(__pyx_v_stats[0]).time_map), __pyx_t_21)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 274, __pyx_L3_error)
+          __pyx_t_21 = __Pyx_PyInt_As_uint64_t(__pyx_v_sample_id_end); if (unlikely((__pyx_t_21 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 276, __pyx_L3_error)
+          __pyx_t_14 = __Pyx_PyInt_From_int64_t(jsdrv_time_from_counter((&(__pyx_v_stats[0]).time_map), __pyx_t_21)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 276, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
 
-          /* "pyjoulescope_driver/binding.pyx":272
+          /* "pyjoulescope_driver/binding.pyx":274
  *                         'samples': {'value': [sample_id_start, sample_id_end], 'units': 'samples'},
  *                         'utc': {
  *                             'value': [             # <<<<<<<<<<<<<<
  *                                 c_jsdrv.jsdrv_time_from_counter(&stats[0].time_map, sample_id_start),
  *                                 c_jsdrv.jsdrv_time_from_counter(&stats[0].time_map, sample_id_end),
  */
-          __pyx_t_22 = PyList_New(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 272, __pyx_L3_error)
+          __pyx_t_22 = PyList_New(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 274, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_GIVEREF(__pyx_t_11);
           PyList_SET_ITEM(__pyx_t_22, 0, __pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_14);
           PyList_SET_ITEM(__pyx_t_22, 1, __pyx_t_14);
           __pyx_t_11 = 0;
           __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_22) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_22) < 0) __PYX_ERR(0, 274, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_time64) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_utc, __pyx_t_10) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_time64) < 0) __PYX_ERR(0, 274, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_utc, __pyx_t_10) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":278
+          /* "pyjoulescope_driver/binding.pyx":280
  *                             'units': 'time64',
  *                         },
  *                         'sample_freq': {'value': sample_freq, 'units': 'Hz'},             # <<<<<<<<<<<<<<
  *                         'range': {'value': [t_start, t_start + t_delta], 'units': 's'},
  *                         'delta': {'value': t_delta, 'units': 's'},
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 278, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 280, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_v_sample_freq) < 0) __PYX_ERR(0, 278, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_Hz) < 0) __PYX_ERR(0, 278, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_sample_freq, __pyx_t_10) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_v_sample_freq) < 0) __PYX_ERR(0, 280, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_Hz) < 0) __PYX_ERR(0, 280, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_sample_freq, __pyx_t_10) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":279
+          /* "pyjoulescope_driver/binding.pyx":281
  *                         },
  *                         'sample_freq': {'value': sample_freq, 'units': 'Hz'},
  *                         'range': {'value': [t_start, t_start + t_delta], 'units': 's'},             # <<<<<<<<<<<<<<
  *                         'delta': {'value': t_delta, 'units': 's'},
  *                         'decimate_factor': {'value': stats[0].decimate_factor, 'units': 'samples'},
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 279, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 281, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_22 = PyNumber_Add(__pyx_v_t_start, __pyx_v_t_delta); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 279, __pyx_L3_error)
+          __pyx_t_22 = PyNumber_Add(__pyx_v_t_start, __pyx_v_t_delta); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 281, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_14 = PyList_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 279, __pyx_L3_error)
+          __pyx_t_14 = PyList_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 281, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
           __Pyx_INCREF(__pyx_v_t_start);
           __Pyx_GIVEREF(__pyx_v_t_start);
           PyList_SET_ITEM(__pyx_t_14, 0, __pyx_v_t_start);
           __Pyx_GIVEREF(__pyx_t_22);
           PyList_SET_ITEM(__pyx_t_14, 1, __pyx_t_22);
           __pyx_t_22 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 279, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 281, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_s) < 0) __PYX_ERR(0, 279, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_range, __pyx_t_10) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_s) < 0) __PYX_ERR(0, 281, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_range, __pyx_t_10) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":280
+          /* "pyjoulescope_driver/binding.pyx":282
  *                         'sample_freq': {'value': sample_freq, 'units': 'Hz'},
  *                         'range': {'value': [t_start, t_start + t_delta], 'units': 's'},
  *                         'delta': {'value': t_delta, 'units': 's'},             # <<<<<<<<<<<<<<
  *                         'decimate_factor': {'value': stats[0].decimate_factor, 'units': 'samples'},
  *                         'decimate_sample_count': {'value': stats[0].block_sample_count, 'units': 'samples'},
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 280, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 282, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_v_t_delta) < 0) __PYX_ERR(0, 280, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_s) < 0) __PYX_ERR(0, 280, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_delta, __pyx_t_10) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_v_t_delta) < 0) __PYX_ERR(0, 282, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_s) < 0) __PYX_ERR(0, 282, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_delta, __pyx_t_10) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":281
+          /* "pyjoulescope_driver/binding.pyx":283
  *                         'range': {'value': [t_start, t_start + t_delta], 'units': 's'},
  *                         'delta': {'value': t_delta, 'units': 's'},
  *                         'decimate_factor': {'value': stats[0].decimate_factor, 'units': 'samples'},             # <<<<<<<<<<<<<<
  *                         'decimate_sample_count': {'value': stats[0].block_sample_count, 'units': 'samples'},
  *                         'accum_samples': {'value': [stats[0].accum_sample_id, sample_id_end], 'units': 'samples'},
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 281, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 283, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_14 = __Pyx_PyInt_From_uint8_t((__pyx_v_stats[0]).decimate_factor); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 281, __pyx_L3_error)
+          __pyx_t_14 = __Pyx_PyInt_From_uint8_t((__pyx_v_stats[0]).decimate_factor); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 283, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 281, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 283, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_samples) < 0) __PYX_ERR(0, 281, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_decimate_factor, __pyx_t_10) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_samples) < 0) __PYX_ERR(0, 283, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_decimate_factor, __pyx_t_10) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":282
+          /* "pyjoulescope_driver/binding.pyx":284
  *                         'delta': {'value': t_delta, 'units': 's'},
  *                         'decimate_factor': {'value': stats[0].decimate_factor, 'units': 'samples'},
  *                         'decimate_sample_count': {'value': stats[0].block_sample_count, 'units': 'samples'},             # <<<<<<<<<<<<<<
  *                         'accum_samples': {'value': [stats[0].accum_sample_id, sample_id_end], 'units': 'samples'},
  *                         'time_map': {
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 282, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 284, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_14 = __Pyx_PyInt_From_uint32_t((__pyx_v_stats[0]).block_sample_count); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 282, __pyx_L3_error)
+          __pyx_t_14 = __Pyx_PyInt_From_uint32_t((__pyx_v_stats[0]).block_sample_count); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 284, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 282, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 284, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_samples) < 0) __PYX_ERR(0, 282, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_decimate_sample_count, __pyx_t_10) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_samples) < 0) __PYX_ERR(0, 284, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_decimate_sample_count, __pyx_t_10) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":283
+          /* "pyjoulescope_driver/binding.pyx":285
  *                         'decimate_factor': {'value': stats[0].decimate_factor, 'units': 'samples'},
  *                         'decimate_sample_count': {'value': stats[0].block_sample_count, 'units': 'samples'},
  *                         'accum_samples': {'value': [stats[0].accum_sample_id, sample_id_end], 'units': 'samples'},             # <<<<<<<<<<<<<<
  *                         'time_map': {
  *                             'offset_time': stats[0].time_map.offset_time,
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 283, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 285, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_14 = __Pyx_PyInt_From_uint64_t((__pyx_v_stats[0]).accum_sample_id); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 283, __pyx_L3_error)
+          __pyx_t_14 = __Pyx_PyInt_From_uint64_t((__pyx_v_stats[0]).accum_sample_id); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 285, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
-          __pyx_t_22 = PyList_New(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 283, __pyx_L3_error)
+          __pyx_t_22 = PyList_New(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 285, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_GIVEREF(__pyx_t_14);
           PyList_SET_ITEM(__pyx_t_22, 0, __pyx_t_14);
           __Pyx_INCREF(__pyx_v_sample_id_end);
           __Pyx_GIVEREF(__pyx_v_sample_id_end);
           PyList_SET_ITEM(__pyx_t_22, 1, __pyx_v_sample_id_end);
           __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_22) < 0) __PYX_ERR(0, 283, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_22) < 0) __PYX_ERR(0, 285, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_samples) < 0) __PYX_ERR(0, 283, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_accum_samples, __pyx_t_10) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_samples) < 0) __PYX_ERR(0, 285, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_accum_samples, __pyx_t_10) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":285
+          /* "pyjoulescope_driver/binding.pyx":287
  *                         'accum_samples': {'value': [stats[0].accum_sample_id, sample_id_end], 'units': 'samples'},
  *                         'time_map': {
  *                             'offset_time': stats[0].time_map.offset_time,             # <<<<<<<<<<<<<<
  *                             'offset_counter': stats[0].time_map.offset_counter,
  *                             'counter_rate': stats[0].time_map.counter_rate,
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 285, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 287, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_22 = __Pyx_PyInt_From_int64_t((__pyx_v_stats[0]).time_map.offset_time); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 285, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyInt_From_int64_t((__pyx_v_stats[0]).time_map.offset_time); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 287, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_offset_time, __pyx_t_22) < 0) __PYX_ERR(0, 285, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_offset_time, __pyx_t_22) < 0) __PYX_ERR(0, 287, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":286
+          /* "pyjoulescope_driver/binding.pyx":288
  *                         'time_map': {
  *                             'offset_time': stats[0].time_map.offset_time,
  *                             'offset_counter': stats[0].time_map.offset_counter,             # <<<<<<<<<<<<<<
  *                             'counter_rate': stats[0].time_map.counter_rate,
  *                         }
  */
-          __pyx_t_22 = __Pyx_PyInt_From_uint64_t((__pyx_v_stats[0]).time_map.offset_counter); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 286, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyInt_From_uint64_t((__pyx_v_stats[0]).time_map.offset_counter); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 288, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_offset_counter, __pyx_t_22) < 0) __PYX_ERR(0, 285, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_offset_counter, __pyx_t_22) < 0) __PYX_ERR(0, 287, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":287
+          /* "pyjoulescope_driver/binding.pyx":289
  *                             'offset_time': stats[0].time_map.offset_time,
  *                             'offset_counter': stats[0].time_map.offset_counter,
  *                             'counter_rate': stats[0].time_map.counter_rate,             # <<<<<<<<<<<<<<
  *                         }
  *                     },
  */
-          __pyx_t_22 = PyFloat_FromDouble((__pyx_v_stats[0]).time_map.counter_rate); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 287, __pyx_L3_error)
+          __pyx_t_22 = PyFloat_FromDouble((__pyx_v_stats[0]).time_map.counter_rate); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 289, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_counter_rate, __pyx_t_22) < 0) __PYX_ERR(0, 285, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_counter_rate, __pyx_t_22) < 0) __PYX_ERR(0, 287, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_time_map, __pyx_t_10) < 0) __PYX_ERR(0, 270, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_time_map, __pyx_t_10) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_time, __pyx_t_15) < 0) __PYX_ERR(0, 269, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_time, __pyx_t_15) < 0) __PYX_ERR(0, 271, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":291
+          /* "pyjoulescope_driver/binding.pyx":293
  *                     },
  *                     'signals': {
  *                         'current': {             # <<<<<<<<<<<<<<
  *                             'avg': {'value': stats[0].i_avg, 'units': 'A'},
  *                             'std': {'value': stats[0].i_std, 'units': 'A'},
  */
-          __pyx_t_15 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 291, __pyx_L3_error)
+          __pyx_t_15 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 293, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_15);
 
-          /* "pyjoulescope_driver/binding.pyx":292
+          /* "pyjoulescope_driver/binding.pyx":294
  *                     'signals': {
  *                         'current': {
  *                             'avg': {'value': stats[0].i_avg, 'units': 'A'},             # <<<<<<<<<<<<<<
  *                             'std': {'value': stats[0].i_std, 'units': 'A'},
  *                             'min': {'value': stats[0].i_min, 'units': 'A'},
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 292, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 292, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_avg); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 292, __pyx_L3_error)
+          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_avg); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 292, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 292, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_avg, __pyx_t_22) < 0) __PYX_ERR(0, 292, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_avg, __pyx_t_22) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":293
+          /* "pyjoulescope_driver/binding.pyx":295
  *                         'current': {
  *                             'avg': {'value': stats[0].i_avg, 'units': 'A'},
  *                             'std': {'value': stats[0].i_std, 'units': 'A'},             # <<<<<<<<<<<<<<
  *                             'min': {'value': stats[0].i_min, 'units': 'A'},
  *                             'max': {'value': stats[0].i_max, 'units': 'A'},
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 293, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 295, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_std); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 293, __pyx_L3_error)
+          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_std); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 295, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 293, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 295, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 293, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_std, __pyx_t_22) < 0) __PYX_ERR(0, 292, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 295, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_std, __pyx_t_22) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":294
+          /* "pyjoulescope_driver/binding.pyx":296
  *                             'avg': {'value': stats[0].i_avg, 'units': 'A'},
  *                             'std': {'value': stats[0].i_std, 'units': 'A'},
  *                             'min': {'value': stats[0].i_min, 'units': 'A'},             # <<<<<<<<<<<<<<
  *                             'max': {'value': stats[0].i_max, 'units': 'A'},
  *                             'p2p': {'value': stats[0].i_max - stats[0].i_min, 'units': 'A'},
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 294, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 296, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_min); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 294, __pyx_L3_error)
+          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_min); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 296, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 296, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_min, __pyx_t_22) < 0) __PYX_ERR(0, 292, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 296, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_min, __pyx_t_22) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":295
+          /* "pyjoulescope_driver/binding.pyx":297
  *                             'std': {'value': stats[0].i_std, 'units': 'A'},
  *                             'min': {'value': stats[0].i_min, 'units': 'A'},
  *                             'max': {'value': stats[0].i_max, 'units': 'A'},             # <<<<<<<<<<<<<<
  *                             'p2p': {'value': stats[0].i_max - stats[0].i_min, 'units': 'A'},
  *                             'integral': {'value': stats[0].i_avg * t_delta, 'units': 'C'},
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 295, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 297, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_max); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 295, __pyx_L3_error)
+          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_max); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 297, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 295, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 297, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 295, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_max, __pyx_t_22) < 0) __PYX_ERR(0, 292, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 297, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_max, __pyx_t_22) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":296
+          /* "pyjoulescope_driver/binding.pyx":298
  *                             'min': {'value': stats[0].i_min, 'units': 'A'},
  *                             'max': {'value': stats[0].i_max, 'units': 'A'},
  *                             'p2p': {'value': stats[0].i_max - stats[0].i_min, 'units': 'A'},             # <<<<<<<<<<<<<<
  *                             'integral': {'value': stats[0].i_avg * t_delta, 'units': 'C'},
  *                         },
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 296, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 298, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_14 = PyFloat_FromDouble(((__pyx_v_stats[0]).i_max - (__pyx_v_stats[0]).i_min)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 296, __pyx_L3_error)
+          __pyx_t_14 = PyFloat_FromDouble(((__pyx_v_stats[0]).i_max - (__pyx_v_stats[0]).i_min)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 298, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 296, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 298, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 296, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_p2p, __pyx_t_22) < 0) __PYX_ERR(0, 292, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_A) < 0) __PYX_ERR(0, 298, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_p2p, __pyx_t_22) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":297
+          /* "pyjoulescope_driver/binding.pyx":299
  *                             'max': {'value': stats[0].i_max, 'units': 'A'},
  *                             'p2p': {'value': stats[0].i_max - stats[0].i_min, 'units': 'A'},
  *                             'integral': {'value': stats[0].i_avg * t_delta, 'units': 'C'},             # <<<<<<<<<<<<<<
  *                         },
  *                         'voltage': {
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 297, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 299, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_avg); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 297, __pyx_L3_error)
+          __pyx_t_14 = PyFloat_FromDouble((__pyx_v_stats[0]).i_avg); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 299, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
-          __pyx_t_11 = PyNumber_Multiply(__pyx_t_14, __pyx_v_t_delta); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 297, __pyx_L3_error)
+          __pyx_t_11 = PyNumber_Multiply(__pyx_t_14, __pyx_v_t_delta); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 299, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 297, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 299, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_C) < 0) __PYX_ERR(0, 297, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_integral, __pyx_t_22) < 0) __PYX_ERR(0, 292, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_C) < 0) __PYX_ERR(0, 299, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_integral, __pyx_t_22) < 0) __PYX_ERR(0, 294, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_current, __pyx_t_10) < 0) __PYX_ERR(0, 291, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_current, __pyx_t_10) < 0) __PYX_ERR(0, 293, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":300
+          /* "pyjoulescope_driver/binding.pyx":302
  *                         },
  *                         'voltage': {
  *                             'avg': {'value': stats[0].v_avg, 'units': 'V'},             # <<<<<<<<<<<<<<
  *                             'std': {'value': stats[0].v_std, 'units': 'V'},
  *                             'min': {'value': stats[0].v_min, 'units': 'V'},
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 300, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 302, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 300, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 302, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).v_avg); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 300, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).v_avg); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 302, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 300, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 302, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 300, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_avg, __pyx_t_22) < 0) __PYX_ERR(0, 300, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 302, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_avg, __pyx_t_22) < 0) __PYX_ERR(0, 302, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":301
+          /* "pyjoulescope_driver/binding.pyx":303
  *                         'voltage': {
  *                             'avg': {'value': stats[0].v_avg, 'units': 'V'},
  *                             'std': {'value': stats[0].v_std, 'units': 'V'},             # <<<<<<<<<<<<<<
  *                             'min': {'value': stats[0].v_min, 'units': 'V'},
  *                             'max': {'value': stats[0].v_max, 'units': 'V'},
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 301, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 303, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).v_std); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 301, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).v_std); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 303, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 301, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 303, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 301, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_std, __pyx_t_22) < 0) __PYX_ERR(0, 300, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 303, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_std, __pyx_t_22) < 0) __PYX_ERR(0, 302, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":302
+          /* "pyjoulescope_driver/binding.pyx":304
  *                             'avg': {'value': stats[0].v_avg, 'units': 'V'},
  *                             'std': {'value': stats[0].v_std, 'units': 'V'},
  *                             'min': {'value': stats[0].v_min, 'units': 'V'},             # <<<<<<<<<<<<<<
  *                             'max': {'value': stats[0].v_max, 'units': 'V'},
  *                             'p2p': {'value': stats[0].v_max - stats[0].v_min, 'units': 'V'},
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 302, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 304, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).v_min); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 302, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).v_min); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 304, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 302, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 304, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 302, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_min, __pyx_t_22) < 0) __PYX_ERR(0, 300, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 304, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_min, __pyx_t_22) < 0) __PYX_ERR(0, 302, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":303
+          /* "pyjoulescope_driver/binding.pyx":305
  *                             'std': {'value': stats[0].v_std, 'units': 'V'},
  *                             'min': {'value': stats[0].v_min, 'units': 'V'},
  *                             'max': {'value': stats[0].v_max, 'units': 'V'},             # <<<<<<<<<<<<<<
  *                             'p2p': {'value': stats[0].v_max - stats[0].v_min, 'units': 'V'},
  *                         },
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 303, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 305, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).v_max); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 303, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).v_max); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 305, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 303, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 305, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 303, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_max, __pyx_t_22) < 0) __PYX_ERR(0, 300, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 305, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_max, __pyx_t_22) < 0) __PYX_ERR(0, 302, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":304
+          /* "pyjoulescope_driver/binding.pyx":306
  *                             'min': {'value': stats[0].v_min, 'units': 'V'},
  *                             'max': {'value': stats[0].v_max, 'units': 'V'},
  *                             'p2p': {'value': stats[0].v_max - stats[0].v_min, 'units': 'V'},             # <<<<<<<<<<<<<<
  *                         },
  *                         'power': {
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 304, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 306, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble(((__pyx_v_stats[0]).v_max - (__pyx_v_stats[0]).v_min)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 304, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble(((__pyx_v_stats[0]).v_max - (__pyx_v_stats[0]).v_min)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 306, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 304, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 306, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 304, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_p2p, __pyx_t_22) < 0) __PYX_ERR(0, 300, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_V) < 0) __PYX_ERR(0, 306, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_p2p, __pyx_t_22) < 0) __PYX_ERR(0, 302, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_voltage, __pyx_t_10) < 0) __PYX_ERR(0, 291, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_voltage, __pyx_t_10) < 0) __PYX_ERR(0, 293, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":307
+          /* "pyjoulescope_driver/binding.pyx":309
  *                         },
  *                         'power': {
  *                             'avg': {'value': stats[0].p_avg, 'units': 'W'},             # <<<<<<<<<<<<<<
  *                             'std': {'value': stats[0].p_std, 'units': 'W'},
  *                             'min': {'value': stats[0].p_min, 'units': 'W'},
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 307, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 307, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_avg); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 307, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_avg); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 307, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 307, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_avg, __pyx_t_22) < 0) __PYX_ERR(0, 307, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_avg, __pyx_t_22) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":308
+          /* "pyjoulescope_driver/binding.pyx":310
  *                         'power': {
  *                             'avg': {'value': stats[0].p_avg, 'units': 'W'},
  *                             'std': {'value': stats[0].p_std, 'units': 'W'},             # <<<<<<<<<<<<<<
  *                             'min': {'value': stats[0].p_min, 'units': 'W'},
  *                             'max': {'value': stats[0].p_max, 'units': 'W'},
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 308, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 310, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_std); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 308, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_std); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 310, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 308, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 310, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 308, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_std, __pyx_t_22) < 0) __PYX_ERR(0, 307, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 310, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_std, __pyx_t_22) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":309
+          /* "pyjoulescope_driver/binding.pyx":311
  *                             'avg': {'value': stats[0].p_avg, 'units': 'W'},
  *                             'std': {'value': stats[0].p_std, 'units': 'W'},
  *                             'min': {'value': stats[0].p_min, 'units': 'W'},             # <<<<<<<<<<<<<<
  *                             'max': {'value': stats[0].p_max, 'units': 'W'},
  *                             'p2p': {'value': stats[0].p_max - stats[0].p_min, 'units': 'W'},
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 309, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 311, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_min); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 309, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_min); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 311, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 311, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_min, __pyx_t_22) < 0) __PYX_ERR(0, 307, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 311, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_min, __pyx_t_22) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":310
+          /* "pyjoulescope_driver/binding.pyx":312
  *                             'std': {'value': stats[0].p_std, 'units': 'W'},
  *                             'min': {'value': stats[0].p_min, 'units': 'W'},
  *                             'max': {'value': stats[0].p_max, 'units': 'W'},             # <<<<<<<<<<<<<<
  *                             'p2p': {'value': stats[0].p_max - stats[0].p_min, 'units': 'W'},
  *                             'integral': {'value': stats[0].p_avg * t_delta, 'units': 'J'},
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 310, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 312, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_max); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 310, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_max); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 312, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 310, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 312, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 310, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_max, __pyx_t_22) < 0) __PYX_ERR(0, 307, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 312, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_max, __pyx_t_22) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":311
+          /* "pyjoulescope_driver/binding.pyx":313
  *                             'min': {'value': stats[0].p_min, 'units': 'W'},
  *                             'max': {'value': stats[0].p_max, 'units': 'W'},
  *                             'p2p': {'value': stats[0].p_max - stats[0].p_min, 'units': 'W'},             # <<<<<<<<<<<<<<
  *                             'integral': {'value': stats[0].p_avg * t_delta, 'units': 'J'},
  *                         },
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 311, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 313, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble(((__pyx_v_stats[0]).p_max - (__pyx_v_stats[0]).p_min)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 311, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble(((__pyx_v_stats[0]).p_max - (__pyx_v_stats[0]).p_min)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 313, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 311, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_11) < 0) __PYX_ERR(0, 313, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 311, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_p2p, __pyx_t_22) < 0) __PYX_ERR(0, 307, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_W) < 0) __PYX_ERR(0, 313, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_p2p, __pyx_t_22) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":312
+          /* "pyjoulescope_driver/binding.pyx":314
  *                             'max': {'value': stats[0].p_max, 'units': 'W'},
  *                             'p2p': {'value': stats[0].p_max - stats[0].p_min, 'units': 'W'},
  *                             'integral': {'value': stats[0].p_avg * t_delta, 'units': 'J'},             # <<<<<<<<<<<<<<
  *                         },
  *                     },
  */
-          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 312, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 314, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_avg); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 312, __pyx_L3_error)
+          __pyx_t_11 = PyFloat_FromDouble((__pyx_v_stats[0]).p_avg); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 314, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_14 = PyNumber_Multiply(__pyx_t_11, __pyx_v_t_delta); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 312, __pyx_L3_error)
+          __pyx_t_14 = PyNumber_Multiply(__pyx_t_11, __pyx_v_t_delta); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 314, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 312, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_value, __pyx_t_14) < 0) __PYX_ERR(0, 314, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_J) < 0) __PYX_ERR(0, 312, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_integral, __pyx_t_22) < 0) __PYX_ERR(0, 307, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_22, __pyx_n_u_units, __pyx_n_u_J) < 0) __PYX_ERR(0, 314, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_integral, __pyx_t_22) < 0) __PYX_ERR(0, 309, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_power, __pyx_t_10) < 0) __PYX_ERR(0, 291, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_power, __pyx_t_10) < 0) __PYX_ERR(0, 293, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_signals, __pyx_t_15) < 0) __PYX_ERR(0, 269, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_signals, __pyx_t_15) < 0) __PYX_ERR(0, 271, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":316
+          /* "pyjoulescope_driver/binding.pyx":318
  *                     },
  *                     'accumulators': {
  *                         'charge': {             # <<<<<<<<<<<<<<
  *                             'value': stats[0].charge_f64,
  *                             'int_value': charge,
  */
-          __pyx_t_15 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 316, __pyx_L3_error)
+          __pyx_t_15 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 318, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_15);
 
-          /* "pyjoulescope_driver/binding.pyx":317
+          /* "pyjoulescope_driver/binding.pyx":319
  *                     'accumulators': {
  *                         'charge': {
  *                             'value': stats[0].charge_f64,             # <<<<<<<<<<<<<<
  *                             'int_value': charge,
  *                             'int_scale': 2 ** -31,
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 317, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 319, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_22 = PyFloat_FromDouble((__pyx_v_stats[0]).charge_f64); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 317, __pyx_L3_error)
+          __pyx_t_22 = PyFloat_FromDouble((__pyx_v_stats[0]).charge_f64); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 319, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_22) < 0) __PYX_ERR(0, 317, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_22) < 0) __PYX_ERR(0, 319, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":318
+          /* "pyjoulescope_driver/binding.pyx":320
  *                         'charge': {
  *                             'value': stats[0].charge_f64,
  *                             'int_value': charge,             # <<<<<<<<<<<<<<
  *                             'int_scale': 2 ** -31,
  *                             'units': 'C',
  */
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_int_value, __pyx_v_charge) < 0) __PYX_ERR(0, 317, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_int_value, __pyx_v_charge) < 0) __PYX_ERR(0, 319, __pyx_L3_error)
 
-          /* "pyjoulescope_driver/binding.pyx":319
+          /* "pyjoulescope_driver/binding.pyx":321
  *                             'value': stats[0].charge_f64,
  *                             'int_value': charge,
  *                             'int_scale': 2 ** -31,             # <<<<<<<<<<<<<<
  *                             'units': 'C',
  *                         },
  */
-          __pyx_t_22 = __Pyx_PyInt_From_long(__Pyx_pow_long(2, -31L)); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 319, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyInt_From_long(__Pyx_pow_long(2, -31L)); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 321, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_int_scale, __pyx_t_22) < 0) __PYX_ERR(0, 317, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_int_scale, __pyx_t_22) < 0) __PYX_ERR(0, 319, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_C) < 0) __PYX_ERR(0, 317, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_charge, __pyx_t_10) < 0) __PYX_ERR(0, 316, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_C) < 0) __PYX_ERR(0, 319, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_charge, __pyx_t_10) < 0) __PYX_ERR(0, 318, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":323
+          /* "pyjoulescope_driver/binding.pyx":325
  *                         },
  *                         'energy': {
  *                             'value': stats[0].energy_f64,             # <<<<<<<<<<<<<<
  *                             'int_value': energy,
  *                             'int_scale': 2 ** -27,
  */
-          __pyx_t_10 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 323, __pyx_L3_error)
+          __pyx_t_10 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 325, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_22 = PyFloat_FromDouble((__pyx_v_stats[0]).energy_f64); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 323, __pyx_L3_error)
+          __pyx_t_22 = PyFloat_FromDouble((__pyx_v_stats[0]).energy_f64); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 325, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_22) < 0) __PYX_ERR(0, 323, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_value, __pyx_t_22) < 0) __PYX_ERR(0, 325, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":324
+          /* "pyjoulescope_driver/binding.pyx":326
  *                         'energy': {
  *                             'value': stats[0].energy_f64,
  *                             'int_value': energy,             # <<<<<<<<<<<<<<
  *                             'int_scale': 2 ** -27,
  *                             'units': 'J',
  */
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_int_value, __pyx_v_energy) < 0) __PYX_ERR(0, 323, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_int_value, __pyx_v_energy) < 0) __PYX_ERR(0, 325, __pyx_L3_error)
 
-          /* "pyjoulescope_driver/binding.pyx":325
+          /* "pyjoulescope_driver/binding.pyx":327
  *                             'value': stats[0].energy_f64,
  *                             'int_value': energy,
  *                             'int_scale': 2 ** -27,             # <<<<<<<<<<<<<<
  *                             'units': 'J',
  *                         },
  */
-          __pyx_t_22 = __Pyx_PyInt_From_long(__Pyx_pow_long(2, -27L)); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 325, __pyx_L3_error)
+          __pyx_t_22 = __Pyx_PyInt_From_long(__Pyx_pow_long(2, -27L)); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 327, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_22);
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_int_scale, __pyx_t_22) < 0) __PYX_ERR(0, 323, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_int_scale, __pyx_t_22) < 0) __PYX_ERR(0, 325, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_J) < 0) __PYX_ERR(0, 323, __pyx_L3_error)
-          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_energy, __pyx_t_10) < 0) __PYX_ERR(0, 316, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_units, __pyx_n_u_J) < 0) __PYX_ERR(0, 325, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_15, __pyx_n_u_energy, __pyx_t_10) < 0) __PYX_ERR(0, 318, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_accumulators, __pyx_t_15) < 0) __PYX_ERR(0, 269, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_accumulators, __pyx_t_15) < 0) __PYX_ERR(0, 271, __pyx_L3_error)
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_source, __pyx_n_u_sensor) < 0) __PYX_ERR(0, 269, __pyx_L3_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_source, __pyx_n_u_sensor) < 0) __PYX_ERR(0, 271, __pyx_L3_error)
           __pyx_v_v = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":258
+          /* "pyjoulescope_driver/binding.pyx":260
  *                     print('jsdrv._jsdrv_union_to_py: unsupported data type')
  *                     v['data'] = None
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STATISTICS:             # <<<<<<<<<<<<<<
  *                 stats = <c_jsdrv.jsdrv_statistics_s *> &(value[0].value.bin[0])
  *                 sample_freq = stats[0].sample_freq
  */
           goto __pyx_L17;
         }
 
-        /* "pyjoulescope_driver/binding.pyx":331
+        /* "pyjoulescope_driver/binding.pyx":333
  *                     'source': 'sensor',
  *                 }
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_INFO:             # <<<<<<<<<<<<<<
  *                 v = _parse_buffer_info(<c_jsdrv.jsdrv_buffer_info_s *> &(value[0].value.bin[0]))
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_RSP:
  */
         __pyx_t_13 = (((__pyx_v_value[0]).app == JSDRV_PAYLOAD_TYPE_BUFFER_INFO) != 0);
         if (__pyx_t_13) {
 
-          /* "pyjoulescope_driver/binding.pyx":332
+          /* "pyjoulescope_driver/binding.pyx":334
  *                 }
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_INFO:
  *                 v = _parse_buffer_info(<c_jsdrv.jsdrv_buffer_info_s *> &(value[0].value.bin[0]))             # <<<<<<<<<<<<<<
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_RSP:
  *                 v = _parse_buffer_rsp(<c_jsdrv.jsdrv_buffer_response_s *> &(value[0].value.bin[0]))
  */
-          __pyx_t_6 = __pyx_f_19pyjoulescope_driver_7binding__parse_buffer_info(((struct jsdrv_buffer_info_s *)(&((__pyx_v_value[0]).value.bin[0])))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 332, __pyx_L3_error)
+          __pyx_t_6 = __pyx_f_19pyjoulescope_driver_7binding__parse_buffer_info(((struct jsdrv_buffer_info_s *)(&((__pyx_v_value[0]).value.bin[0])))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 334, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_v = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":331
+          /* "pyjoulescope_driver/binding.pyx":333
  *                     'source': 'sensor',
  *                 }
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_INFO:             # <<<<<<<<<<<<<<
  *                 v = _parse_buffer_info(<c_jsdrv.jsdrv_buffer_info_s *> &(value[0].value.bin[0]))
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_RSP:
  */
           goto __pyx_L17;
         }
 
-        /* "pyjoulescope_driver/binding.pyx":333
+        /* "pyjoulescope_driver/binding.pyx":335
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_INFO:
  *                 v = _parse_buffer_info(<c_jsdrv.jsdrv_buffer_info_s *> &(value[0].value.bin[0]))
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_RSP:             # <<<<<<<<<<<<<<
  *                 v = _parse_buffer_rsp(<c_jsdrv.jsdrv_buffer_response_s *> &(value[0].value.bin[0]))
  *             else:
  */
         __pyx_t_13 = (((__pyx_v_value[0]).app == JSDRV_PAYLOAD_TYPE_BUFFER_RSP) != 0);
         if (__pyx_t_13) {
 
-          /* "pyjoulescope_driver/binding.pyx":334
+          /* "pyjoulescope_driver/binding.pyx":336
  *                 v = _parse_buffer_info(<c_jsdrv.jsdrv_buffer_info_s *> &(value[0].value.bin[0]))
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_RSP:
  *                 v = _parse_buffer_rsp(<c_jsdrv.jsdrv_buffer_response_s *> &(value[0].value.bin[0]))             # <<<<<<<<<<<<<<
  *             else:
  *                 v = value[0].value.bin[:value[0].size]
  */
-          __pyx_t_6 = __pyx_f_19pyjoulescope_driver_7binding__parse_buffer_rsp(((struct jsdrv_buffer_response_s *)(&((__pyx_v_value[0]).value.bin[0])))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 334, __pyx_L3_error)
+          __pyx_t_6 = __pyx_f_19pyjoulescope_driver_7binding__parse_buffer_rsp(((struct jsdrv_buffer_response_s *)(&((__pyx_v_value[0]).value.bin[0])))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_v = __pyx_t_6;
           __pyx_t_6 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":333
+          /* "pyjoulescope_driver/binding.pyx":335
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_INFO:
  *                 v = _parse_buffer_info(<c_jsdrv.jsdrv_buffer_info_s *> &(value[0].value.bin[0]))
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_RSP:             # <<<<<<<<<<<<<<
  *                 v = _parse_buffer_rsp(<c_jsdrv.jsdrv_buffer_response_s *> &(value[0].value.bin[0]))
  *             else:
  */
           goto __pyx_L17;
         }
 
-        /* "pyjoulescope_driver/binding.pyx":336
+        /* "pyjoulescope_driver/binding.pyx":338
  *                 v = _parse_buffer_rsp(<c_jsdrv.jsdrv_buffer_response_s *> &(value[0].value.bin[0]))
  *             else:
  *                 v = value[0].value.bin[:value[0].size]             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_F32:
  *             v = value[0].value.f32
  */
         /*else*/ {
-          __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_value[0]).value.bin) + 0, (__pyx_v_value[0]).size - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L3_error)
+          __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_value[0]).value.bin) + 0, (__pyx_v_value[0]).size - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 338, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_v = __pyx_t_6;
           __pyx_t_6 = 0;
         }
         __pyx_L17:;
 
-        /* "pyjoulescope_driver/binding.pyx":213
+        /* "pyjoulescope_driver/binding.pyx":215
  *             except Exception:
  *                 v = None
  *         elif t == c_jsdrv.JSDRV_UNION_BIN:             # <<<<<<<<<<<<<<
  *             if value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STREAM:
  *                 stream = <c_jsdrv.jsdrv_stream_signal_s *> &(value[0].value.bin[0])
  */
         break;
         case JSDRV_UNION_F32:
 
-        /* "pyjoulescope_driver/binding.pyx":338
+        /* "pyjoulescope_driver/binding.pyx":340
  *                 v = value[0].value.bin[:value[0].size]
  *         elif t == c_jsdrv.JSDRV_UNION_F32:
  *             v = value[0].value.f32             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_F64:
  *             v = value[0].value.f64
  */
-        __pyx_t_6 = PyFloat_FromDouble((__pyx_v_value[0]).value.f32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 338, __pyx_L3_error)
+        __pyx_t_6 = PyFloat_FromDouble((__pyx_v_value[0]).value.f32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 340, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":337
+        /* "pyjoulescope_driver/binding.pyx":339
  *             else:
  *                 v = value[0].value.bin[:value[0].size]
  *         elif t == c_jsdrv.JSDRV_UNION_F32:             # <<<<<<<<<<<<<<
  *             v = value[0].value.f32
  *         elif t == c_jsdrv.JSDRV_UNION_F64:
  */
         break;
         case JSDRV_UNION_F64:
 
-        /* "pyjoulescope_driver/binding.pyx":340
+        /* "pyjoulescope_driver/binding.pyx":342
  *             v = value[0].value.f32
  *         elif t == c_jsdrv.JSDRV_UNION_F64:
  *             v = value[0].value.f64             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_U8:
  *             v = value[0].value.u8
  */
-        __pyx_t_6 = PyFloat_FromDouble((__pyx_v_value[0]).value.f64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 340, __pyx_L3_error)
+        __pyx_t_6 = PyFloat_FromDouble((__pyx_v_value[0]).value.f64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 342, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":339
+        /* "pyjoulescope_driver/binding.pyx":341
  *         elif t == c_jsdrv.JSDRV_UNION_F32:
  *             v = value[0].value.f32
  *         elif t == c_jsdrv.JSDRV_UNION_F64:             # <<<<<<<<<<<<<<
  *             v = value[0].value.f64
  *         elif t == c_jsdrv.JSDRV_UNION_U8:
  */
         break;
         case JSDRV_UNION_U8:
 
-        /* "pyjoulescope_driver/binding.pyx":342
+        /* "pyjoulescope_driver/binding.pyx":344
  *             v = value[0].value.f64
  *         elif t == c_jsdrv.JSDRV_UNION_U8:
  *             v = value[0].value.u8             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_U16:
  *             v = value[0].value.u16
  */
-        __pyx_t_6 = __Pyx_PyInt_From_uint8_t((__pyx_v_value[0]).value.u8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 342, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyInt_From_uint8_t((__pyx_v_value[0]).value.u8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 344, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":341
+        /* "pyjoulescope_driver/binding.pyx":343
  *         elif t == c_jsdrv.JSDRV_UNION_F64:
  *             v = value[0].value.f64
  *         elif t == c_jsdrv.JSDRV_UNION_U8:             # <<<<<<<<<<<<<<
  *             v = value[0].value.u8
  *         elif t == c_jsdrv.JSDRV_UNION_U16:
  */
         break;
         case JSDRV_UNION_U16:
 
-        /* "pyjoulescope_driver/binding.pyx":344
+        /* "pyjoulescope_driver/binding.pyx":346
  *             v = value[0].value.u8
  *         elif t == c_jsdrv.JSDRV_UNION_U16:
  *             v = value[0].value.u16             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_U32:
  *             v = value[0].value.u32
  */
-        __pyx_t_6 = __Pyx_PyInt_From_uint16_t((__pyx_v_value[0]).value.u16); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 344, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyInt_From_uint16_t((__pyx_v_value[0]).value.u16); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 346, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":343
+        /* "pyjoulescope_driver/binding.pyx":345
  *         elif t == c_jsdrv.JSDRV_UNION_U8:
  *             v = value[0].value.u8
  *         elif t == c_jsdrv.JSDRV_UNION_U16:             # <<<<<<<<<<<<<<
  *             v = value[0].value.u16
  *         elif t == c_jsdrv.JSDRV_UNION_U32:
  */
         break;
         case JSDRV_UNION_U32:
 
-        /* "pyjoulescope_driver/binding.pyx":346
+        /* "pyjoulescope_driver/binding.pyx":348
  *             v = value[0].value.u16
  *         elif t == c_jsdrv.JSDRV_UNION_U32:
  *             v = value[0].value.u32             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_U64:
  *             v = value[0].value.u64
  */
-        __pyx_t_6 = __Pyx_PyInt_From_uint32_t((__pyx_v_value[0]).value.u32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 346, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyInt_From_uint32_t((__pyx_v_value[0]).value.u32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":345
+        /* "pyjoulescope_driver/binding.pyx":347
  *         elif t == c_jsdrv.JSDRV_UNION_U16:
  *             v = value[0].value.u16
  *         elif t == c_jsdrv.JSDRV_UNION_U32:             # <<<<<<<<<<<<<<
  *             v = value[0].value.u32
  *         elif t == c_jsdrv.JSDRV_UNION_U64:
  */
         break;
         case JSDRV_UNION_U64:
 
-        /* "pyjoulescope_driver/binding.pyx":348
+        /* "pyjoulescope_driver/binding.pyx":350
  *             v = value[0].value.u32
  *         elif t == c_jsdrv.JSDRV_UNION_U64:
  *             v = value[0].value.u64             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_I8:
  *             v = value[0].value.i8
  */
-        __pyx_t_6 = __Pyx_PyInt_From_uint64_t((__pyx_v_value[0]).value.u64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyInt_From_uint64_t((__pyx_v_value[0]).value.u64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 350, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":347
+        /* "pyjoulescope_driver/binding.pyx":349
  *         elif t == c_jsdrv.JSDRV_UNION_U32:
  *             v = value[0].value.u32
  *         elif t == c_jsdrv.JSDRV_UNION_U64:             # <<<<<<<<<<<<<<
  *             v = value[0].value.u64
  *         elif t == c_jsdrv.JSDRV_UNION_I8:
  */
         break;
         case JSDRV_UNION_I8:
 
-        /* "pyjoulescope_driver/binding.pyx":350
+        /* "pyjoulescope_driver/binding.pyx":352
  *             v = value[0].value.u64
  *         elif t == c_jsdrv.JSDRV_UNION_I8:
  *             v = value[0].value.i8             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_I16:
  *             v = value[0].value.i16
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int8_t((__pyx_v_value[0]).value.i8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 350, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int8_t((__pyx_v_value[0]).value.i8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 352, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":349
+        /* "pyjoulescope_driver/binding.pyx":351
  *         elif t == c_jsdrv.JSDRV_UNION_U64:
  *             v = value[0].value.u64
  *         elif t == c_jsdrv.JSDRV_UNION_I8:             # <<<<<<<<<<<<<<
  *             v = value[0].value.i8
  *         elif t == c_jsdrv.JSDRV_UNION_I16:
  */
         break;
         case JSDRV_UNION_I16:
 
-        /* "pyjoulescope_driver/binding.pyx":352
+        /* "pyjoulescope_driver/binding.pyx":354
  *             v = value[0].value.i8
  *         elif t == c_jsdrv.JSDRV_UNION_I16:
  *             v = value[0].value.i16             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_I32:
  *             v = value[0].value.i32
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int16_t((__pyx_v_value[0]).value.i16); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 352, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int16_t((__pyx_v_value[0]).value.i16); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 354, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":351
+        /* "pyjoulescope_driver/binding.pyx":353
  *         elif t == c_jsdrv.JSDRV_UNION_I8:
  *             v = value[0].value.i8
  *         elif t == c_jsdrv.JSDRV_UNION_I16:             # <<<<<<<<<<<<<<
  *             v = value[0].value.i16
  *         elif t == c_jsdrv.JSDRV_UNION_I32:
  */
         break;
         case JSDRV_UNION_I32:
 
-        /* "pyjoulescope_driver/binding.pyx":354
+        /* "pyjoulescope_driver/binding.pyx":356
  *             v = value[0].value.i16
  *         elif t == c_jsdrv.JSDRV_UNION_I32:
  *             v = value[0].value.i32             # <<<<<<<<<<<<<<
  *         elif t == c_jsdrv.JSDRV_UNION_I64:
  *             v = value[0].value.i64
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int32_t((__pyx_v_value[0]).value.i32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 354, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int32_t((__pyx_v_value[0]).value.i32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 356, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":353
+        /* "pyjoulescope_driver/binding.pyx":355
  *         elif t == c_jsdrv.JSDRV_UNION_I16:
  *             v = value[0].value.i16
  *         elif t == c_jsdrv.JSDRV_UNION_I32:             # <<<<<<<<<<<<<<
  *             v = value[0].value.i32
  *         elif t == c_jsdrv.JSDRV_UNION_I64:
  */
         break;
         case JSDRV_UNION_I64:
 
-        /* "pyjoulescope_driver/binding.pyx":356
+        /* "pyjoulescope_driver/binding.pyx":358
  *             v = value[0].value.i32
  *         elif t == c_jsdrv.JSDRV_UNION_I64:
  *             v = value[0].value.i64             # <<<<<<<<<<<<<<
  *         else:
  *             v = None
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int64_t((__pyx_v_value[0]).value.i64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 356, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int64_t((__pyx_v_value[0]).value.i64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 358, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_v = __pyx_t_6;
         __pyx_t_6 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":355
+        /* "pyjoulescope_driver/binding.pyx":357
  *         elif t == c_jsdrv.JSDRV_UNION_I32:
  *             v = value[0].value.i32
  *         elif t == c_jsdrv.JSDRV_UNION_I64:             # <<<<<<<<<<<<<<
  *             v = value[0].value.i64
  *         else:
  */
         break;
         default:
 
-        /* "pyjoulescope_driver/binding.pyx":358
+        /* "pyjoulescope_driver/binding.pyx":360
  *             v = value[0].value.i64
  *         else:
  *             v = None             # <<<<<<<<<<<<<<
  *     except Exception as ex:
  *         _log_c.exception(ex)
  */
         __Pyx_INCREF(Py_None);
         __pyx_v_v = Py_None;
         break;
       }
 
-      /* "pyjoulescope_driver/binding.pyx":204
+      /* "pyjoulescope_driver/binding.pyx":206
  *     cdef int32_t idx
  *     t = value[0].type
  *     try:             # <<<<<<<<<<<<<<
  *         if t == c_jsdrv.JSDRV_UNION_STR:
  *             v = value[0].value.str.decode('utf-8')
  */
     }
@@ -7258,73 +7257,73 @@
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
     __PYX_XDEC_MEMVIEW(&__pyx_t_16, 1);
     __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":359
+    /* "pyjoulescope_driver/binding.pyx":361
  *         else:
  *             v = None
  *     except Exception as ex:             # <<<<<<<<<<<<<<
  *         _log_c.exception(ex)
  *         v = None
  */
     __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_12) {
       __Pyx_AddTraceback("pyjoulescope_driver.binding._jsdrv_union_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_15, &__pyx_t_10) < 0) __PYX_ERR(0, 359, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_15, &__pyx_t_10) < 0) __PYX_ERR(0, 361, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_15);
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_15);
       __pyx_v_ex = __pyx_t_15;
       /*try:*/ {
 
-        /* "pyjoulescope_driver/binding.pyx":360
+        /* "pyjoulescope_driver/binding.pyx":362
  *             v = None
  *     except Exception as ex:
  *         _log_c.exception(ex)             # <<<<<<<<<<<<<<
  *         v = None
  *     return v
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_log_c); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 360, __pyx_L26_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_log_c); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 362, __pyx_L26_error)
         __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_exception); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 360, __pyx_L26_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_exception); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 362, __pyx_L26_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_t_14 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_14)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
             __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
         __pyx_t_22 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_14, __pyx_v_ex) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_v_ex);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 360, __pyx_L26_error)
+        if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 362, __pyx_L26_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":361
+        /* "pyjoulescope_driver/binding.pyx":363
  *     except Exception as ex:
  *         _log_c.exception(ex)
  *         v = None             # <<<<<<<<<<<<<<
  *     return v
  * 
  */
         __Pyx_INCREF(Py_None);
         __Pyx_XDECREF_SET(__pyx_v_v, Py_None);
       }
 
-      /* "pyjoulescope_driver/binding.pyx":359
+      /* "pyjoulescope_driver/binding.pyx":361
  *         else:
  *             v = None
  *     except Exception as ex:             # <<<<<<<<<<<<<<
  *         _log_c.exception(ex)
  *         v = None
  */
       /*finally:*/ {
@@ -7375,15 +7374,15 @@
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       goto __pyx_L4_exception_handled;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "pyjoulescope_driver/binding.pyx":204
+    /* "pyjoulescope_driver/binding.pyx":206
  *     cdef int32_t idx
  *     t = value[0].type
  *     try:             # <<<<<<<<<<<<<<
  *         if t == c_jsdrv.JSDRV_UNION_STR:
  *             v = value[0].value.str.decode('utf-8')
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -7395,27 +7394,27 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     __pyx_L8_try_end:;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":362
+  /* "pyjoulescope_driver/binding.pyx":364
  *         _log_c.exception(ex)
  *         v = None
  *     return v             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_v);
   __pyx_r = __pyx_v_v;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":198
+  /* "pyjoulescope_driver/binding.pyx":200
  * 
  * 
  * cdef object _jsdrv_union_to_py(const c_jsdrv.jsdrv_union_s * value):             # <<<<<<<<<<<<<<
  *     cdef c_jsdrv.jsdrv_stream_signal_s * stream;
  *     cdef np.npy_intp shape[1]
  */
 
@@ -7445,15 +7444,15 @@
   __Pyx_XDECREF(__pyx_v_energy);
   __Pyx_XDECREF(__pyx_v_ex);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":456
+/* "pyjoulescope_driver/binding.pyx":458
  * 
  * 
  * def error_code_to_str(ec):             # <<<<<<<<<<<<<<
  *     """Get the string representation for an error code.
  * 
  */
 
@@ -7488,24 +7487,24 @@
   Py_ssize_t __pyx_t_8;
   Py_UCS4 __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("error_code_to_str", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":462
+  /* "pyjoulescope_driver/binding.pyx":464
  *     :return: The error code's name
  *     """
  *     v, name, rv = _error_code_to_meta.get(ec, (-1, "unknown", "unknown"))             # <<<<<<<<<<<<<<
  *     return f'{v} {name} : {rv}'
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_error_code_to_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 462, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_error_code_to_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 462, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -7515,51 +7514,51 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_ec, __pyx_tuple__6};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_ec, __pyx_tuple__6};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_v_ec);
     __Pyx_GIVEREF(__pyx_v_ec);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_ec);
     __Pyx_INCREF(__pyx_tuple__6);
     __Pyx_GIVEREF(__pyx_tuple__6);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_tuple__6);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 462, __pyx_L1_error)
+      __PYX_ERR(0, 464, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -7567,101 +7566,101 @@
       __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_2 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_t_2);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_6 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_6 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_7 = Py_TYPE(__pyx_t_6)->tp_iternext;
     index = 0; __pyx_t_3 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 1; __pyx_t_5 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_5)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_5);
     index = 2; __pyx_t_2 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 3) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 3) < 0) __PYX_ERR(0, 464, __pyx_L1_error)
     __pyx_t_7 = NULL;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 462, __pyx_L1_error)
+    __PYX_ERR(0, 464, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_v = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_name = __pyx_t_5;
   __pyx_t_5 = 0;
   __pyx_v_rv = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":463
+  /* "pyjoulescope_driver/binding.pyx":465
  *     """
  *     v, name, rv = _error_code_to_meta.get(ec, (-1, "unknown", "unknown"))
  *     return f'{v} {name} : {rv}'             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 465, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_8 = 0;
   __pyx_t_9 = 127;
-  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_v, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_v, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_9;
   __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
   __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_kp_u__7);
   __pyx_t_8 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__7);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u__7);
-  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_9;
   __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_2);
   __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_kp_u__8);
   __pyx_t_8 += 3;
   __Pyx_GIVEREF(__pyx_kp_u__8);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__8);
-  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_rv, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_rv, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_9;
   __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":456
+  /* "pyjoulescope_driver/binding.pyx":458
  * 
  * 
  * def error_code_to_str(ec):             # <<<<<<<<<<<<<<
  *     """Get the string representation for an error code.
  * 
  */
 
@@ -7679,15 +7678,15 @@
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XDECREF(__pyx_v_rv);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":524
+/* "pyjoulescope_driver/binding.pyx":526
  * 
  * 
  * def log_level_c_to_py(lvl):             # <<<<<<<<<<<<<<
  *     return _log_level_c_to_py.get(int(lvl))
  * 
  */
 
@@ -7713,50 +7712,50 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("log_level_c_to_py", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":525
+  /* "pyjoulescope_driver/binding.pyx":527
  * 
  * def log_level_c_to_py(lvl):
  *     return _log_level_c_to_py.get(int(lvl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log_level_c_to_py); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log_level_c_to_py); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 527, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 527, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_v_lvl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_v_lvl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 527, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 527, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":524
+  /* "pyjoulescope_driver/binding.pyx":526
  * 
  * 
  * def log_level_c_to_py(lvl):             # <<<<<<<<<<<<<<
  *     return _log_level_c_to_py.get(int(lvl))
  * 
  */
 
@@ -7770,15 +7769,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":569
+/* "pyjoulescope_driver/binding.pyx":571
  * 
  * 
  * cdef int32_t _timeout_validate(value, default=None):             # <<<<<<<<<<<<<<
  *     if default is None:
  *         default = _TIMEOUT_MS_DEFAULT
  */
 
@@ -7798,89 +7797,89 @@
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_default = __pyx_optional_args->__pyx_default;
     }
   }
   __Pyx_INCREF(__pyx_v_default);
 
-  /* "pyjoulescope_driver/binding.pyx":570
+  /* "pyjoulescope_driver/binding.pyx":572
  * 
  * cdef int32_t _timeout_validate(value, default=None):
  *     if default is None:             # <<<<<<<<<<<<<<
  *         default = _TIMEOUT_MS_DEFAULT
  *     if value is None:
  */
   __pyx_t_1 = (__pyx_v_default == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "pyjoulescope_driver/binding.pyx":571
+    /* "pyjoulescope_driver/binding.pyx":573
  * cdef int32_t _timeout_validate(value, default=None):
  *     if default is None:
  *         default = _TIMEOUT_MS_DEFAULT             # <<<<<<<<<<<<<<
  *     if value is None:
  *         return default
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_TIMEOUT_MS_DEFAULT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 571, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_TIMEOUT_MS_DEFAULT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_default, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":570
+    /* "pyjoulescope_driver/binding.pyx":572
  * 
  * cdef int32_t _timeout_validate(value, default=None):
  *     if default is None:             # <<<<<<<<<<<<<<
  *         default = _TIMEOUT_MS_DEFAULT
  *     if value is None:
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":572
+  /* "pyjoulescope_driver/binding.pyx":574
  *     if default is None:
  *         default = _TIMEOUT_MS_DEFAULT
  *     if value is None:             # <<<<<<<<<<<<<<
  *         return default
  *     return <int32_t> (float(value) * 1000)
  */
   __pyx_t_2 = (__pyx_v_value == Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "pyjoulescope_driver/binding.pyx":573
+    /* "pyjoulescope_driver/binding.pyx":575
  *         default = _TIMEOUT_MS_DEFAULT
  *     if value is None:
  *         return default             # <<<<<<<<<<<<<<
  *     return <int32_t> (float(value) * 1000)
  * 
  */
-    __pyx_t_4 = __Pyx_PyInt_As_int32_t(__pyx_v_default); if (unlikely((__pyx_t_4 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 573, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_int32_t(__pyx_v_default); if (unlikely((__pyx_t_4 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 575, __pyx_L1_error)
     __pyx_r = __pyx_t_4;
     goto __pyx_L0;
 
-    /* "pyjoulescope_driver/binding.pyx":572
+    /* "pyjoulescope_driver/binding.pyx":574
  *     if default is None:
  *         default = _TIMEOUT_MS_DEFAULT
  *     if value is None:             # <<<<<<<<<<<<<<
  *         return default
  *     return <int32_t> (float(value) * 1000)
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":574
+  /* "pyjoulescope_driver/binding.pyx":576
  *     if value is None:
  *         return default
  *     return <int32_t> (float(value) * 1000)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_AsDouble(__pyx_v_value); if (unlikely(__pyx_t_5 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsDouble(__pyx_v_value); if (unlikely(__pyx_t_5 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 576, __pyx_L1_error)
   __pyx_r = ((int32_t)(__pyx_t_5 * 1000.0));
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":569
+  /* "pyjoulescope_driver/binding.pyx":571
  * 
  * 
  * cdef int32_t _timeout_validate(value, default=None):             # <<<<<<<<<<<<<<
  *     if default is None:
  *         default = _TIMEOUT_MS_DEFAULT
  */
 
@@ -7891,15 +7890,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_default);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":577
+/* "pyjoulescope_driver/binding.pyx":579
  * 
  * 
  * def _handle_rc(rc, src, cause=None):             # <<<<<<<<<<<<<<
  *     if rc:
  *         if cause:
  */
 
@@ -7938,25 +7937,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rc)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_src)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_handle_rc", 0, 2, 3, 1); __PYX_ERR(0, 577, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_handle_rc", 0, 2, 3, 1); __PYX_ERR(0, 579, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cause);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_handle_rc") < 0)) __PYX_ERR(0, 577, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_handle_rc") < 0)) __PYX_ERR(0, 579, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -7966,15 +7965,15 @@
     }
     __pyx_v_rc = values[0];
     __pyx_v_src = values[1];
     __pyx_v_cause = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_handle_rc", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 577, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_handle_rc", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 579, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding._handle_rc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_4_handle_rc(__pyx_self, __pyx_v_rc, __pyx_v_src, __pyx_v_cause);
 
@@ -7994,197 +7993,197 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_rc", 0);
   __Pyx_INCREF(__pyx_v_cause);
 
-  /* "pyjoulescope_driver/binding.pyx":578
+  /* "pyjoulescope_driver/binding.pyx":580
  * 
  * def _handle_rc(rc, src, cause=None):
  *     if rc:             # <<<<<<<<<<<<<<
  *         if cause:
  *             cause = f' | {cause}'
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 578, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 580, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pyjoulescope_driver/binding.pyx":579
+    /* "pyjoulescope_driver/binding.pyx":581
  * def _handle_rc(rc, src, cause=None):
  *     if rc:
  *         if cause:             # <<<<<<<<<<<<<<
  *             cause = f' | {cause}'
  *         else:
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_cause); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_cause); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 581, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "pyjoulescope_driver/binding.pyx":580
+      /* "pyjoulescope_driver/binding.pyx":582
  *     if rc:
  *         if cause:
  *             cause = f' | {cause}'             # <<<<<<<<<<<<<<
  *         else:
  *             ''
  */
-      __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_cause, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_cause, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u__9, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 580, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u__9, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF_SET(__pyx_v_cause, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "pyjoulescope_driver/binding.pyx":579
+      /* "pyjoulescope_driver/binding.pyx":581
  * def _handle_rc(rc, src, cause=None):
  *     if rc:
  *         if cause:             # <<<<<<<<<<<<<<
  *             cause = f' | {cause}'
  *         else:
  */
       goto __pyx_L4;
     }
 
-    /* "pyjoulescope_driver/binding.pyx":582
+    /* "pyjoulescope_driver/binding.pyx":584
  *             cause = f' | {cause}'
  *         else:
  *             ''             # <<<<<<<<<<<<<<
  *         if rc == ErrorCode.TIMED_OUT:
  *             raise TimeoutError(f'{src} timed out{cause}')
  */
     /*else*/ {
     }
     __pyx_L4:;
 
-    /* "pyjoulescope_driver/binding.pyx":583
+    /* "pyjoulescope_driver/binding.pyx":585
  *         else:
  *             ''
  *         if rc == ErrorCode.TIMED_OUT:             # <<<<<<<<<<<<<<
  *             raise TimeoutError(f'{src} timed out{cause}')
  *         else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ErrorCode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 583, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ErrorCode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 585, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_TIMED_OUT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 583, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_TIMED_OUT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 585, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_rc, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 583, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_v_rc, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 585, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 583, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 585, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(__pyx_t_1)) {
 
-      /* "pyjoulescope_driver/binding.pyx":584
+      /* "pyjoulescope_driver/binding.pyx":586
  *             ''
  *         if rc == ErrorCode.TIMED_OUT:
  *             raise TimeoutError(f'{src} timed out{cause}')             # <<<<<<<<<<<<<<
  *         else:
  *             raise RuntimeError(f'{src} failed {rc}{cause}')
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_TimeoutError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 584, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_TimeoutError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 586, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 584, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = 0;
       __pyx_t_5 = 127;
-      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_src, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 584, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_src, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 586, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_5;
       __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_INCREF(__pyx_kp_u_timed_out);
       __pyx_t_4 += 10;
       __Pyx_GIVEREF(__pyx_kp_u_timed_out);
       PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_kp_u_timed_out);
-      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_cause, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 584, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_cause, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 586, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_5;
       __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_6);
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 584, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 586, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 584, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 584, __pyx_L1_error)
+      __PYX_ERR(0, 586, __pyx_L1_error)
 
-      /* "pyjoulescope_driver/binding.pyx":583
+      /* "pyjoulescope_driver/binding.pyx":585
  *         else:
  *             ''
  *         if rc == ErrorCode.TIMED_OUT:             # <<<<<<<<<<<<<<
  *             raise TimeoutError(f'{src} timed out{cause}')
  *         else:
  */
     }
 
-    /* "pyjoulescope_driver/binding.pyx":586
+    /* "pyjoulescope_driver/binding.pyx":588
  *             raise TimeoutError(f'{src} timed out{cause}')
  *         else:
  *             raise RuntimeError(f'{src} failed {rc}{cause}')             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = 0;
       __pyx_t_5 = 127;
-      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_src, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 586, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_src, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 588, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_5;
       __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_INCREF(__pyx_kp_u_failed);
       __pyx_t_4 += 8;
       __Pyx_GIVEREF(__pyx_kp_u_failed);
       PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_kp_u_failed);
-      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_rc, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 586, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_rc, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 588, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_5;
       __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_6);
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_cause, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 586, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_cause, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 588, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_5;
       __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_6);
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_2, 4, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 586, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_2, 4, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 588, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 586, __pyx_L1_error)
+      __PYX_ERR(0, 588, __pyx_L1_error)
     }
 
-    /* "pyjoulescope_driver/binding.pyx":578
+    /* "pyjoulescope_driver/binding.pyx":580
  * 
  * def _handle_rc(rc, src, cause=None):
  *     if rc:             # <<<<<<<<<<<<<<
  *         if cause:
  *             cause = f' | {cause}'
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":577
+  /* "pyjoulescope_driver/binding.pyx":579
  * 
  * 
  * def _handle_rc(rc, src, cause=None):             # <<<<<<<<<<<<<<
  *     if rc:
  *         if cause:
  */
 
@@ -8200,15 +8199,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_cause);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":593
+/* "pyjoulescope_driver/binding.pyx":595
  *     cdef object _subscribers
  * 
  *     def __init__(self, timeout=None):             # <<<<<<<<<<<<<<
  *         global _driver_count
  *         self._context = NULL
  */
 
@@ -8240,29 +8239,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 593, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 595, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_timeout = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 593, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 595, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver___init__(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_timeout);
 
@@ -8286,64 +8285,64 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":595
+  /* "pyjoulescope_driver/binding.pyx":597
  *     def __init__(self, timeout=None):
  *         global _driver_count
  *         self._context = NULL             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         timeout_ms = _timeout_validate(timeout, _TIMEOUT_MS_INIT)
  */
   __pyx_v_self->_context = NULL;
 
-  /* "pyjoulescope_driver/binding.pyx":597
+  /* "pyjoulescope_driver/binding.pyx":599
  *         self._context = NULL
  *         cdef int32_t rc
  *         timeout_ms = _timeout_validate(timeout, _TIMEOUT_MS_INIT)             # <<<<<<<<<<<<<<
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_initialize(&self._context, NULL, timeout_ms)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TIMEOUT_MS_INIT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 597, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TIMEOUT_MS_INIT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3.__pyx_n = 1;
   __pyx_t_3.__pyx_default = __pyx_t_1;
   __pyx_t_2 = __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(__pyx_v_timeout, &__pyx_t_3); 
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_timeout_ms = __pyx_t_2;
 
-  /* "pyjoulescope_driver/binding.pyx":598
+  /* "pyjoulescope_driver/binding.pyx":600
  *         cdef int32_t rc
  *         timeout_ms = _timeout_validate(timeout, _TIMEOUT_MS_INIT)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_initialize(&self._context, NULL, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_initialize')
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjoulescope_driver/binding.pyx":599
+        /* "pyjoulescope_driver/binding.pyx":601
  *         timeout_ms = _timeout_validate(timeout, _TIMEOUT_MS_INIT)
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_initialize(&self._context, NULL, timeout_ms)             # <<<<<<<<<<<<<<
  *         _handle_rc(rc, 'jsdrv_initialize')
  *         self._subscribers = set()  # (topic, fn)
  */
         __pyx_v_rc = jsdrv_initialize((&__pyx_v_self->_context), NULL, __pyx_v_timeout_ms);
       }
 
-      /* "pyjoulescope_driver/binding.pyx":598
+      /* "pyjoulescope_driver/binding.pyx":600
  *         cdef int32_t rc
  *         timeout_ms = _timeout_validate(timeout, _TIMEOUT_MS_INIT)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_initialize(&self._context, NULL, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_initialize')
  */
       /*finally:*/ {
@@ -8354,24 +8353,24 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyjoulescope_driver/binding.pyx":600
+  /* "pyjoulescope_driver/binding.pyx":602
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_initialize(&self._context, NULL, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_initialize')             # <<<<<<<<<<<<<<
  *         self._subscribers = set()  # (topic, fn)
  *         if _driver_count == 0:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -8380,110 +8379,110 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_5, __pyx_n_u_jsdrv_initialize};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_5, __pyx_n_u_jsdrv_initialize};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 602, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_5);
     __Pyx_INCREF(__pyx_n_u_jsdrv_initialize);
     __Pyx_GIVEREF(__pyx_n_u_jsdrv_initialize);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_n_u_jsdrv_initialize);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":601
+  /* "pyjoulescope_driver/binding.pyx":603
  *             rc = c_jsdrv.jsdrv_initialize(&self._context, NULL, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_initialize')
  *         self._subscribers = set()  # (topic, fn)             # <<<<<<<<<<<<<<
  *         if _driver_count == 0:
  *             c_jsdrv.jsdrv_log_initialize()
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_subscribers);
   __Pyx_DECREF(__pyx_v_self->_subscribers);
   __pyx_v_self->_subscribers = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":602
+  /* "pyjoulescope_driver/binding.pyx":604
  *         _handle_rc(rc, 'jsdrv_initialize')
  *         self._subscribers = set()  # (topic, fn)
  *         if _driver_count == 0:             # <<<<<<<<<<<<<<
  *             c_jsdrv.jsdrv_log_initialize()
  *             c_jsdrv.jsdrv_log_register(_on_log_recv, NULL)
  */
   __pyx_t_9 = ((__pyx_v_19pyjoulescope_driver_7binding__driver_count == 0) != 0);
   if (__pyx_t_9) {
 
-    /* "pyjoulescope_driver/binding.pyx":603
+    /* "pyjoulescope_driver/binding.pyx":605
  *         self._subscribers = set()  # (topic, fn)
  *         if _driver_count == 0:
  *             c_jsdrv.jsdrv_log_initialize()             # <<<<<<<<<<<<<<
  *             c_jsdrv.jsdrv_log_register(_on_log_recv, NULL)
  *         _driver_count += 1
  */
     jsdrv_log_initialize();
 
-    /* "pyjoulescope_driver/binding.pyx":604
+    /* "pyjoulescope_driver/binding.pyx":606
  *         if _driver_count == 0:
  *             c_jsdrv.jsdrv_log_initialize()
  *             c_jsdrv.jsdrv_log_register(_on_log_recv, NULL)             # <<<<<<<<<<<<<<
  *         _driver_count += 1
  * 
  */
     (void)(jsdrv_log_register(__pyx_f_19pyjoulescope_driver_7binding__on_log_recv, NULL));
 
-    /* "pyjoulescope_driver/binding.pyx":602
+    /* "pyjoulescope_driver/binding.pyx":604
  *         _handle_rc(rc, 'jsdrv_initialize')
  *         self._subscribers = set()  # (topic, fn)
  *         if _driver_count == 0:             # <<<<<<<<<<<<<<
  *             c_jsdrv.jsdrv_log_initialize()
  *             c_jsdrv.jsdrv_log_register(_on_log_recv, NULL)
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":605
+  /* "pyjoulescope_driver/binding.pyx":607
  *             c_jsdrv.jsdrv_log_initialize()
  *             c_jsdrv.jsdrv_log_register(_on_log_recv, NULL)
  *         _driver_count += 1             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
   __pyx_v_19pyjoulescope_driver_7binding__driver_count = (__pyx_v_19pyjoulescope_driver_7binding__driver_count + 1);
 
-  /* "pyjoulescope_driver/binding.pyx":593
+  /* "pyjoulescope_driver/binding.pyx":595
  *     cdef object _subscribers
  * 
  *     def __init__(self, timeout=None):             # <<<<<<<<<<<<<<
  *         global _driver_count
  *         self._context = NULL
  */
 
@@ -8499,15 +8498,15 @@
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":607
+/* "pyjoulescope_driver/binding.pyx":609
  *         _driver_count += 1
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -8525,42 +8524,42 @@
 }
 
 static PyObject *__pyx_pf_19pyjoulescope_driver_7binding_6Driver_2__enter__(struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":608
+  /* "pyjoulescope_driver/binding.pyx":610
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, type, value, traceback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":607
+  /* "pyjoulescope_driver/binding.pyx":609
  *         _driver_count += 1
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":610
+/* "pyjoulescope_driver/binding.pyx":612
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.finalize()
  * 
  */
 
@@ -8597,40 +8596,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 610, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 612, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_traceback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 610, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 612, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 610, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 612, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_type = values[0];
     __pyx_v_value = values[1];
     __pyx_v_traceback = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 610, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 612, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_4__exit__(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_type, __pyx_v_value, __pyx_v_traceback);
 
@@ -8646,41 +8645,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":611
+  /* "pyjoulescope_driver/binding.pyx":613
  * 
  *     def __exit__(self, type, value, traceback):
  *         self.finalize()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_finalize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 611, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_finalize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 611, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":610
+  /* "pyjoulescope_driver/binding.pyx":612
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.finalize()
  * 
  */
 
@@ -8695,15 +8694,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":614
+/* "pyjoulescope_driver/binding.pyx":616
  * 
  *     @property
  *     def log_level(self):             # <<<<<<<<<<<<<<
  *         """Get the current log level."""
  *         return c_jsdrv.jsdrv_log_level_get()
  */
 
@@ -8725,29 +8724,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":616
+  /* "pyjoulescope_driver/binding.pyx":618
  *     def log_level(self):
  *         """Get the current log level."""
  *         return c_jsdrv.jsdrv_log_level_get()             # <<<<<<<<<<<<<<
  * 
  *     @log_level.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int8_t(jsdrv_log_level_get()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int8_t(jsdrv_log_level_get()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":614
+  /* "pyjoulescope_driver/binding.pyx":616
  * 
  *     @property
  *     def log_level(self):             # <<<<<<<<<<<<<<
  *         """Get the current log level."""
  *         return c_jsdrv.jsdrv_log_level_get()
  */
 
@@ -8758,15 +8757,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":619
+/* "pyjoulescope_driver/binding.pyx":621
  * 
  *     @log_level.setter
  *     def log_level(self, level):             # <<<<<<<<<<<<<<
  *         """Set the current log level.
  * 
  */
 
@@ -8798,57 +8797,57 @@
   int8_t __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
   __Pyx_INCREF(__pyx_v_level);
 
-  /* "pyjoulescope_driver/binding.pyx":624
+  /* "pyjoulescope_driver/binding.pyx":626
  *         :param level: The log level.
  *         """
  *         if isinstance(level, str):             # <<<<<<<<<<<<<<
  *             level = _log_level_str_to_int.get(level.lower(), LogLevel.OFF)
  *         c_jsdrv.jsdrv_log_level_set(level)
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_level); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "pyjoulescope_driver/binding.pyx":625
+    /* "pyjoulescope_driver/binding.pyx":627
  *         """
  *         if isinstance(level, str):
  *             level = _log_level_str_to_int.get(level.lower(), LogLevel.OFF)             # <<<<<<<<<<<<<<
  *         c_jsdrv.jsdrv_log_level_set(level)
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_log_level_str_to_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 625, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_log_level_str_to_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 625, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_level, __pyx_n_s_lower); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 625, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_level, __pyx_n_s_lower); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 625, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 625, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_OFF); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 625, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_OFF); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
@@ -8858,71 +8857,71 @@
         __Pyx_DECREF_SET(__pyx_t_5, function);
         __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_5)) {
       PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_4, __pyx_t_7};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 627, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
       PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_4, __pyx_t_7};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 627, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     } else
     #endif
     {
-      __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 625, __pyx_L1_error)
+      __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (__pyx_t_6) {
         __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_6); __pyx_t_6 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_7);
       __pyx_t_4 = 0;
       __pyx_t_7 = 0;
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_level, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":624
+    /* "pyjoulescope_driver/binding.pyx":626
  *         :param level: The log level.
  *         """
  *         if isinstance(level, str):             # <<<<<<<<<<<<<<
  *             level = _log_level_str_to_int.get(level.lower(), LogLevel.OFF)
  *         c_jsdrv.jsdrv_log_level_set(level)
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":626
+  /* "pyjoulescope_driver/binding.pyx":628
  *         if isinstance(level, str):
  *             level = _log_level_str_to_int.get(level.lower(), LogLevel.OFF)
  *         c_jsdrv.jsdrv_log_level_set(level)             # <<<<<<<<<<<<<<
  * 
  *     def finalize(self, timeout=None):
  */
-  __pyx_t_10 = __Pyx_PyInt_As_int8_t(__pyx_v_level); if (unlikely((__pyx_t_10 == ((int8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 626, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_int8_t(__pyx_v_level); if (unlikely((__pyx_t_10 == ((int8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 628, __pyx_L1_error)
   jsdrv_log_level_set(__pyx_t_10);
 
-  /* "pyjoulescope_driver/binding.pyx":619
+  /* "pyjoulescope_driver/binding.pyx":621
  * 
  *     @log_level.setter
  *     def log_level(self, level):             # <<<<<<<<<<<<<<
  *         """Set the current log level.
  * 
  */
 
@@ -8940,15 +8939,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_level);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":628
+/* "pyjoulescope_driver/binding.pyx":630
  *         c_jsdrv.jsdrv_log_level_set(level)
  * 
  *     def finalize(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """Finalize the driver.
  * 
  */
 
@@ -8981,29 +8980,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "finalize") < 0)) __PYX_ERR(0, 628, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "finalize") < 0)) __PYX_ERR(0, 630, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_timeout = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("finalize", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 628, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("finalize", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 630, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.finalize", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_6finalize(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_timeout);
 
@@ -9016,68 +9015,68 @@
   struct jsdrv_context_s *__pyx_v_context;
   int32_t __pyx_v_timeout_ms;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   struct jsdrv_context_s *__pyx_t_1;
   __Pyx_RefNannySetupContext("finalize", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":635
+  /* "pyjoulescope_driver/binding.pyx":637
  *         """
  *         global _driver_count
  *         cdef c_jsdrv.jsdrv_context_s * context = self._context             # <<<<<<<<<<<<<<
  *         timeout_ms = _timeout_validate(timeout)
  *         with nogil:
  */
   __pyx_t_1 = __pyx_v_self->_context;
   __pyx_v_context = __pyx_t_1;
 
-  /* "pyjoulescope_driver/binding.pyx":636
+  /* "pyjoulescope_driver/binding.pyx":638
  *         global _driver_count
  *         cdef c_jsdrv.jsdrv_context_s * context = self._context
  *         timeout_ms = _timeout_validate(timeout)             # <<<<<<<<<<<<<<
  *         with nogil:
  *             c_jsdrv.jsdrv_finalize(context, timeout_ms)
  */
   __pyx_v_timeout_ms = __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(__pyx_v_timeout, NULL);
 
-  /* "pyjoulescope_driver/binding.pyx":637
+  /* "pyjoulescope_driver/binding.pyx":639
  *         cdef c_jsdrv.jsdrv_context_s * context = self._context
  *         timeout_ms = _timeout_validate(timeout)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_jsdrv.jsdrv_finalize(context, timeout_ms)
  *             c_jsdrv.jsdrv_log_finalize()
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjoulescope_driver/binding.pyx":638
+        /* "pyjoulescope_driver/binding.pyx":640
  *         timeout_ms = _timeout_validate(timeout)
  *         with nogil:
  *             c_jsdrv.jsdrv_finalize(context, timeout_ms)             # <<<<<<<<<<<<<<
  *             c_jsdrv.jsdrv_log_finalize()
  *         _driver_count -= 1
  */
         jsdrv_finalize(__pyx_v_context, __pyx_v_timeout_ms);
 
-        /* "pyjoulescope_driver/binding.pyx":639
+        /* "pyjoulescope_driver/binding.pyx":641
  *         with nogil:
  *             c_jsdrv.jsdrv_finalize(context, timeout_ms)
  *             c_jsdrv.jsdrv_log_finalize()             # <<<<<<<<<<<<<<
  *         _driver_count -= 1
  * 
  */
         jsdrv_log_finalize();
       }
 
-      /* "pyjoulescope_driver/binding.pyx":637
+      /* "pyjoulescope_driver/binding.pyx":639
  *         cdef c_jsdrv.jsdrv_context_s * context = self._context
  *         timeout_ms = _timeout_validate(timeout)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_jsdrv.jsdrv_finalize(context, timeout_ms)
  *             c_jsdrv.jsdrv_log_finalize()
  */
       /*finally:*/ {
@@ -9088,39 +9087,39 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyjoulescope_driver/binding.pyx":640
+  /* "pyjoulescope_driver/binding.pyx":642
  *             c_jsdrv.jsdrv_finalize(context, timeout_ms)
  *             c_jsdrv.jsdrv_log_finalize()
  *         _driver_count -= 1             # <<<<<<<<<<<<<<
  * 
  *     def publish(self, topic: str, value, timeout=None):
  */
   __pyx_v_19pyjoulescope_driver_7binding__driver_count = (__pyx_v_19pyjoulescope_driver_7binding__driver_count - 1);
 
-  /* "pyjoulescope_driver/binding.pyx":628
+  /* "pyjoulescope_driver/binding.pyx":630
  *         c_jsdrv.jsdrv_log_level_set(level)
  * 
  *     def finalize(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """Finalize the driver.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":642
+/* "pyjoulescope_driver/binding.pyx":644
  *         _driver_count -= 1
  * 
  *     def publish(self, topic: str, value, timeout=None):             # <<<<<<<<<<<<<<
  *         """Publish a value to a topic.
  * 
  */
 
@@ -9159,25 +9158,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_topic)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("publish", 0, 2, 3, 1); __PYX_ERR(0, 642, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("publish", 0, 2, 3, 1); __PYX_ERR(0, 644, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "publish") < 0)) __PYX_ERR(0, 642, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "publish") < 0)) __PYX_ERR(0, 644, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -9187,21 +9186,21 @@
     }
     __pyx_v_topic = ((PyObject*)values[0]);
     __pyx_v_value = values[1];
     __pyx_v_timeout = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("publish", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 642, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("publish", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 644, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.publish", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_topic), (&PyUnicode_Type), 1, "topic", 1))) __PYX_ERR(0, 642, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_topic), (&PyUnicode_Type), 1, "topic", 1))) __PYX_ERR(0, 644, __pyx_L1_error)
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_8publish(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_topic, __pyx_v_value, __pyx_v_timeout);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9234,548 +9233,548 @@
   PyObject *__pyx_t_14 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("publish", 0);
   __Pyx_INCREF(__pyx_v_value);
 
-  /* "pyjoulescope_driver/binding.pyx":653
+  /* "pyjoulescope_driver/binding.pyx":655
  *         cdef c_jsdrv.jsdrv_union_s v
  *         cdef char * byte_str
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')             # <<<<<<<<<<<<<<
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  * 
  */
   if (unlikely(__pyx_v_topic == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 653, __pyx_L1_error)
+    __PYX_ERR(0, 655, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_topic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_topic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 653, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 655, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_topic_str = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "pyjoulescope_driver/binding.pyx":654
+  /* "pyjoulescope_driver/binding.pyx":656
  *         cdef char * byte_str
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)             # <<<<<<<<<<<<<<
  * 
  *         memset(&v, 0, sizeof(v))
  */
   __pyx_v_timeout_ms = __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(__pyx_v_timeout, NULL);
 
-  /* "pyjoulescope_driver/binding.pyx":656
+  /* "pyjoulescope_driver/binding.pyx":658
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  * 
  *         memset(&v, 0, sizeof(v))             # <<<<<<<<<<<<<<
  *         if isinstance(value, str):
  *             py_byte_str = value.encode('utf-8')
  */
   (void)(memset((&__pyx_v_v), 0, (sizeof(__pyx_v_v))));
 
-  /* "pyjoulescope_driver/binding.pyx":657
+  /* "pyjoulescope_driver/binding.pyx":659
  * 
  *         memset(&v, 0, sizeof(v))
  *         if isinstance(value, str):             # <<<<<<<<<<<<<<
  *             py_byte_str = value.encode('utf-8')
  *             byte_str = py_byte_str
  */
   __pyx_t_3 = PyUnicode_Check(__pyx_v_value); 
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "pyjoulescope_driver/binding.pyx":658
+    /* "pyjoulescope_driver/binding.pyx":660
  *         memset(&v, 0, sizeof(v))
  *         if isinstance(value, str):
  *             py_byte_str = value.encode('utf-8')             # <<<<<<<<<<<<<<
  *             byte_str = py_byte_str
  *             v.type = c_jsdrv.JSDRV_UNION_STR
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 658, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 660, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u_utf_8);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 658, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_py_byte_str = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":659
+    /* "pyjoulescope_driver/binding.pyx":661
  *         if isinstance(value, str):
  *             py_byte_str = value.encode('utf-8')
  *             byte_str = py_byte_str             # <<<<<<<<<<<<<<
  *             v.type = c_jsdrv.JSDRV_UNION_STR
  *             v.value.str = &byte_str[0]
  */
-    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_v_py_byte_str); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 659, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_v_py_byte_str); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 661, __pyx_L1_error)
     __pyx_v_byte_str = __pyx_t_7;
 
-    /* "pyjoulescope_driver/binding.pyx":660
+    /* "pyjoulescope_driver/binding.pyx":662
  *             py_byte_str = value.encode('utf-8')
  *             byte_str = py_byte_str
  *             v.type = c_jsdrv.JSDRV_UNION_STR             # <<<<<<<<<<<<<<
  *             v.value.str = &byte_str[0]
  *         elif isinstance(value, int):
  */
     __pyx_v_v.type = JSDRV_UNION_STR;
 
-    /* "pyjoulescope_driver/binding.pyx":661
+    /* "pyjoulescope_driver/binding.pyx":663
  *             byte_str = py_byte_str
  *             v.type = c_jsdrv.JSDRV_UNION_STR
  *             v.value.str = &byte_str[0]             # <<<<<<<<<<<<<<
  *         elif isinstance(value, int):
  *             if (value >= 0) and (value < 4294967296LL):
  */
     __pyx_v_v.value.str = (&(__pyx_v_byte_str[0]));
 
-    /* "pyjoulescope_driver/binding.pyx":657
+    /* "pyjoulescope_driver/binding.pyx":659
  * 
  *         memset(&v, 0, sizeof(v))
  *         if isinstance(value, str):             # <<<<<<<<<<<<<<
  *             py_byte_str = value.encode('utf-8')
  *             byte_str = py_byte_str
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":662
+  /* "pyjoulescope_driver/binding.pyx":664
  *             v.type = c_jsdrv.JSDRV_UNION_STR
  *             v.value.str = &byte_str[0]
  *         elif isinstance(value, int):             # <<<<<<<<<<<<<<
  *             if (value >= 0) and (value < 4294967296LL):
  *                 v.type = c_jsdrv.JSDRV_UNION_U32
  */
   __pyx_t_4 = PyInt_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_4 != 0);
   if (__pyx_t_3) {
 
-    /* "pyjoulescope_driver/binding.pyx":663
+    /* "pyjoulescope_driver/binding.pyx":665
  *             v.value.str = &byte_str[0]
  *         elif isinstance(value, int):
  *             if (value >= 0) and (value < 4294967296LL):             # <<<<<<<<<<<<<<
  *                 v.type = c_jsdrv.JSDRV_UNION_U32
  *                 v.value.u64 = value
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_0, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 663, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 663, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_0, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 665, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 665, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_4) {
     } else {
       __pyx_t_3 = __pyx_t_4;
       goto __pyx_L5_bool_binop_done;
     }
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_4294967296L, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 663, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 663, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_4294967296L, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 665, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 665, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_3 = __pyx_t_4;
     __pyx_L5_bool_binop_done:;
     if (__pyx_t_3) {
 
-      /* "pyjoulescope_driver/binding.pyx":664
+      /* "pyjoulescope_driver/binding.pyx":666
  *         elif isinstance(value, int):
  *             if (value >= 0) and (value < 4294967296LL):
  *                 v.type = c_jsdrv.JSDRV_UNION_U32             # <<<<<<<<<<<<<<
  *                 v.value.u64 = value
  *             elif value >= 0:
  */
       __pyx_v_v.type = JSDRV_UNION_U32;
 
-      /* "pyjoulescope_driver/binding.pyx":665
+      /* "pyjoulescope_driver/binding.pyx":667
  *             if (value >= 0) and (value < 4294967296LL):
  *                 v.type = c_jsdrv.JSDRV_UNION_U32
  *                 v.value.u64 = value             # <<<<<<<<<<<<<<
  *             elif value >= 0:
  *                 v.type = c_jsdrv.JSDRV_UNION_U64
  */
-      __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_value); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 665, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_value); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 667, __pyx_L1_error)
       __pyx_v_v.value.u64 = __pyx_t_8;
 
-      /* "pyjoulescope_driver/binding.pyx":663
+      /* "pyjoulescope_driver/binding.pyx":665
  *             v.value.str = &byte_str[0]
  *         elif isinstance(value, int):
  *             if (value >= 0) and (value < 4294967296LL):             # <<<<<<<<<<<<<<
  *                 v.type = c_jsdrv.JSDRV_UNION_U32
  *                 v.value.u64 = value
  */
       goto __pyx_L4;
     }
 
-    /* "pyjoulescope_driver/binding.pyx":666
+    /* "pyjoulescope_driver/binding.pyx":668
  *                 v.type = c_jsdrv.JSDRV_UNION_U32
  *                 v.value.u64 = value
  *             elif value >= 0:             # <<<<<<<<<<<<<<
  *                 v.type = c_jsdrv.JSDRV_UNION_U64
  *                 v.value.u64 = value
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_0, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 666, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 666, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_0, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 668, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 668, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_3) {
 
-      /* "pyjoulescope_driver/binding.pyx":667
+      /* "pyjoulescope_driver/binding.pyx":669
  *                 v.value.u64 = value
  *             elif value >= 0:
  *                 v.type = c_jsdrv.JSDRV_UNION_U64             # <<<<<<<<<<<<<<
  *                 v.value.u64 = value
  *             elif value >= -2147483648LL:
  */
       __pyx_v_v.type = JSDRV_UNION_U64;
 
-      /* "pyjoulescope_driver/binding.pyx":668
+      /* "pyjoulescope_driver/binding.pyx":670
  *             elif value >= 0:
  *                 v.type = c_jsdrv.JSDRV_UNION_U64
  *                 v.value.u64 = value             # <<<<<<<<<<<<<<
  *             elif value >= -2147483648LL:
  *                 v.type = c_jsdrv.JSDRV_UNION_I32
  */
-      __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_value); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 668, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_v_value); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 670, __pyx_L1_error)
       __pyx_v_v.value.u64 = __pyx_t_8;
 
-      /* "pyjoulescope_driver/binding.pyx":666
+      /* "pyjoulescope_driver/binding.pyx":668
  *                 v.type = c_jsdrv.JSDRV_UNION_U32
  *                 v.value.u64 = value
  *             elif value >= 0:             # <<<<<<<<<<<<<<
  *                 v.type = c_jsdrv.JSDRV_UNION_U64
  *                 v.value.u64 = value
  */
       goto __pyx_L4;
     }
 
-    /* "pyjoulescope_driver/binding.pyx":669
+    /* "pyjoulescope_driver/binding.pyx":671
  *                 v.type = c_jsdrv.JSDRV_UNION_U64
  *                 v.value.u64 = value
  *             elif value >= -2147483648LL:             # <<<<<<<<<<<<<<
  *                 v.type = c_jsdrv.JSDRV_UNION_I32
  *                 v.value.i64 = value
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_neg_2147483648L, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 669, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_neg_2147483648L, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 671, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 671, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_3) {
 
-      /* "pyjoulescope_driver/binding.pyx":670
+      /* "pyjoulescope_driver/binding.pyx":672
  *                 v.value.u64 = value
  *             elif value >= -2147483648LL:
  *                 v.type = c_jsdrv.JSDRV_UNION_I32             # <<<<<<<<<<<<<<
  *                 v.value.i64 = value
  *             else:
  */
       __pyx_v_v.type = JSDRV_UNION_I32;
 
-      /* "pyjoulescope_driver/binding.pyx":671
+      /* "pyjoulescope_driver/binding.pyx":673
  *             elif value >= -2147483648LL:
  *                 v.type = c_jsdrv.JSDRV_UNION_I32
  *                 v.value.i64 = value             # <<<<<<<<<<<<<<
  *             else:
  *                 v.type = c_jsdrv.JSDRV_UNION_I64
  */
-      __pyx_t_9 = __Pyx_PyInt_As_int64_t(__pyx_v_value); if (unlikely((__pyx_t_9 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 671, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyInt_As_int64_t(__pyx_v_value); if (unlikely((__pyx_t_9 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 673, __pyx_L1_error)
       __pyx_v_v.value.i64 = __pyx_t_9;
 
-      /* "pyjoulescope_driver/binding.pyx":669
+      /* "pyjoulescope_driver/binding.pyx":671
  *                 v.type = c_jsdrv.JSDRV_UNION_U64
  *                 v.value.u64 = value
  *             elif value >= -2147483648LL:             # <<<<<<<<<<<<<<
  *                 v.type = c_jsdrv.JSDRV_UNION_I32
  *                 v.value.i64 = value
  */
       goto __pyx_L4;
     }
 
-    /* "pyjoulescope_driver/binding.pyx":673
+    /* "pyjoulescope_driver/binding.pyx":675
  *                 v.value.i64 = value
  *             else:
  *                 v.type = c_jsdrv.JSDRV_UNION_I64             # <<<<<<<<<<<<<<
  *                 v.value.i64 = value
  *         elif topic.startswith('m/') and topic.endswith('/!req'):
  */
     /*else*/ {
       __pyx_v_v.type = JSDRV_UNION_I64;
 
-      /* "pyjoulescope_driver/binding.pyx":674
+      /* "pyjoulescope_driver/binding.pyx":676
  *             else:
  *                 v.type = c_jsdrv.JSDRV_UNION_I64
  *                 v.value.i64 = value             # <<<<<<<<<<<<<<
  *         elif topic.startswith('m/') and topic.endswith('/!req'):
  *             value = _pack_buffer_req(value)
  */
-      __pyx_t_9 = __Pyx_PyInt_As_int64_t(__pyx_v_value); if (unlikely((__pyx_t_9 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 674, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyInt_As_int64_t(__pyx_v_value); if (unlikely((__pyx_t_9 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 676, __pyx_L1_error)
       __pyx_v_v.value.i64 = __pyx_t_9;
     }
     __pyx_L4:;
 
-    /* "pyjoulescope_driver/binding.pyx":662
+    /* "pyjoulescope_driver/binding.pyx":664
  *             v.type = c_jsdrv.JSDRV_UNION_STR
  *             v.value.str = &byte_str[0]
  *         elif isinstance(value, int):             # <<<<<<<<<<<<<<
  *             if (value >= 0) and (value < 4294967296LL):
  *                 v.type = c_jsdrv.JSDRV_UNION_U32
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":675
+  /* "pyjoulescope_driver/binding.pyx":677
  *                 v.type = c_jsdrv.JSDRV_UNION_I64
  *                 v.value.i64 = value
  *         elif topic.startswith('m/') and topic.endswith('/!req'):             # <<<<<<<<<<<<<<
  *             value = _pack_buffer_req(value)
  *             byte_str = value
  */
   if (unlikely(__pyx_v_topic == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "startswith");
-    __PYX_ERR(0, 675, __pyx_L1_error)
+    __PYX_ERR(0, 677, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyUnicode_Tailmatch(__pyx_v_topic, __pyx_kp_u_m, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Tailmatch(__pyx_v_topic, __pyx_kp_u_m, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 677, __pyx_L1_error)
   if ((__pyx_t_4 != 0)) {
   } else {
     __pyx_t_3 = (__pyx_t_4 != 0);
     goto __pyx_L7_bool_binop_done;
   }
   if (unlikely(__pyx_v_topic == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "endswith");
-    __PYX_ERR(0, 675, __pyx_L1_error)
+    __PYX_ERR(0, 677, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyUnicode_Tailmatch(__pyx_v_topic, __pyx_kp_u_req, 0, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Tailmatch(__pyx_v_topic, __pyx_kp_u_req, 0, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 677, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_3) {
 
-    /* "pyjoulescope_driver/binding.pyx":676
+    /* "pyjoulescope_driver/binding.pyx":678
  *                 v.value.i64 = value
  *         elif topic.startswith('m/') and topic.endswith('/!req'):
  *             value = _pack_buffer_req(value)             # <<<<<<<<<<<<<<
  *             byte_str = value
  *             v.type = c_jsdrv.JSDRV_UNION_BIN
  */
-    __pyx_t_1 = __pyx_f_19pyjoulescope_driver_7binding__pack_buffer_req(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 676, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_19pyjoulescope_driver_7binding__pack_buffer_req(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 678, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":677
+    /* "pyjoulescope_driver/binding.pyx":679
  *         elif topic.startswith('m/') and topic.endswith('/!req'):
  *             value = _pack_buffer_req(value)
  *             byte_str = value             # <<<<<<<<<<<<<<
  *             v.type = c_jsdrv.JSDRV_UNION_BIN
  *             v.value.bin = <const uint8_t *> byte_str
  */
-    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_v_value); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 677, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_v_value); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 679, __pyx_L1_error)
     __pyx_v_byte_str = __pyx_t_7;
 
-    /* "pyjoulescope_driver/binding.pyx":678
+    /* "pyjoulescope_driver/binding.pyx":680
  *             value = _pack_buffer_req(value)
  *             byte_str = value
  *             v.type = c_jsdrv.JSDRV_UNION_BIN             # <<<<<<<<<<<<<<
  *             v.value.bin = <const uint8_t *> byte_str
  *             v.app = c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_REQ
  */
     __pyx_v_v.type = JSDRV_UNION_BIN;
 
-    /* "pyjoulescope_driver/binding.pyx":679
+    /* "pyjoulescope_driver/binding.pyx":681
  *             byte_str = value
  *             v.type = c_jsdrv.JSDRV_UNION_BIN
  *             v.value.bin = <const uint8_t *> byte_str             # <<<<<<<<<<<<<<
  *             v.app = c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_REQ
  *             v.size = <uint32_t> len(value)
  */
     __pyx_v_v.value.bin = ((uint8_t const *)__pyx_v_byte_str);
 
-    /* "pyjoulescope_driver/binding.pyx":680
+    /* "pyjoulescope_driver/binding.pyx":682
  *             v.type = c_jsdrv.JSDRV_UNION_BIN
  *             v.value.bin = <const uint8_t *> byte_str
  *             v.app = c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_REQ             # <<<<<<<<<<<<<<
  *             v.size = <uint32_t> len(value)
  *         elif isinstance(value, bytes):
  */
     __pyx_v_v.app = JSDRV_PAYLOAD_TYPE_BUFFER_REQ;
 
-    /* "pyjoulescope_driver/binding.pyx":681
+    /* "pyjoulescope_driver/binding.pyx":683
  *             v.value.bin = <const uint8_t *> byte_str
  *             v.app = c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_REQ
  *             v.size = <uint32_t> len(value)             # <<<<<<<<<<<<<<
  *         elif isinstance(value, bytes):
  *             byte_str = value
  */
-    __pyx_t_10 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 681, __pyx_L1_error)
+    __pyx_t_10 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 683, __pyx_L1_error)
     __pyx_v_v.size = ((uint32_t)__pyx_t_10);
 
-    /* "pyjoulescope_driver/binding.pyx":675
+    /* "pyjoulescope_driver/binding.pyx":677
  *                 v.type = c_jsdrv.JSDRV_UNION_I64
  *                 v.value.i64 = value
  *         elif topic.startswith('m/') and topic.endswith('/!req'):             # <<<<<<<<<<<<<<
  *             value = _pack_buffer_req(value)
  *             byte_str = value
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":682
+  /* "pyjoulescope_driver/binding.pyx":684
  *             v.app = c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_REQ
  *             v.size = <uint32_t> len(value)
  *         elif isinstance(value, bytes):             # <<<<<<<<<<<<<<
  *             byte_str = value
  *             v.type = c_jsdrv.JSDRV_UNION_BIN
  */
   __pyx_t_3 = PyBytes_Check(__pyx_v_value); 
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (likely(__pyx_t_4)) {
 
-    /* "pyjoulescope_driver/binding.pyx":683
+    /* "pyjoulescope_driver/binding.pyx":685
  *             v.size = <uint32_t> len(value)
  *         elif isinstance(value, bytes):
  *             byte_str = value             # <<<<<<<<<<<<<<
  *             v.type = c_jsdrv.JSDRV_UNION_BIN
  *             v.value.bin = <const uint8_t *> byte_str
  */
-    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_v_value); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 683, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_v_value); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 685, __pyx_L1_error)
     __pyx_v_byte_str = __pyx_t_7;
 
-    /* "pyjoulescope_driver/binding.pyx":684
+    /* "pyjoulescope_driver/binding.pyx":686
  *         elif isinstance(value, bytes):
  *             byte_str = value
  *             v.type = c_jsdrv.JSDRV_UNION_BIN             # <<<<<<<<<<<<<<
  *             v.value.bin = <const uint8_t *> byte_str
  *             v.size = <uint32_t> len(value)
  */
     __pyx_v_v.type = JSDRV_UNION_BIN;
 
-    /* "pyjoulescope_driver/binding.pyx":685
+    /* "pyjoulescope_driver/binding.pyx":687
  *             byte_str = value
  *             v.type = c_jsdrv.JSDRV_UNION_BIN
  *             v.value.bin = <const uint8_t *> byte_str             # <<<<<<<<<<<<<<
  *             v.size = <uint32_t> len(value)
  *         else:
  */
     __pyx_v_v.value.bin = ((uint8_t const *)__pyx_v_byte_str);
 
-    /* "pyjoulescope_driver/binding.pyx":686
+    /* "pyjoulescope_driver/binding.pyx":688
  *             v.type = c_jsdrv.JSDRV_UNION_BIN
  *             v.value.bin = <const uint8_t *> byte_str
  *             v.size = <uint32_t> len(value)             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError(f'Unsupported value type: {type(value)}')
  */
-    __pyx_t_10 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 686, __pyx_L1_error)
+    __pyx_t_10 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 688, __pyx_L1_error)
     __pyx_v_v.size = ((uint32_t)__pyx_t_10);
 
-    /* "pyjoulescope_driver/binding.pyx":682
+    /* "pyjoulescope_driver/binding.pyx":684
  *             v.app = c_jsdrv.JSDRV_PAYLOAD_TYPE_BUFFER_REQ
  *             v.size = <uint32_t> len(value)
  *         elif isinstance(value, bytes):             # <<<<<<<<<<<<<<
  *             byte_str = value
  *             v.type = c_jsdrv.JSDRV_UNION_BIN
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":688
+  /* "pyjoulescope_driver/binding.pyx":690
  *             v.size = <uint32_t> len(value)
  *         else:
  *             raise ValueError(f'Unsupported value type: {type(value)}')             # <<<<<<<<<<<<<<
  *         if '!' not in topic:
  *             v.flags = c_jsdrv.JSDRV_UNION_FLAG_RETAIN
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(((PyObject *)Py_TYPE(__pyx_v_value)), __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 688, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(((PyObject *)Py_TYPE(__pyx_v_value)), __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 690, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unsupported_value_type, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 688, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unsupported_value_type, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 690, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 688, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 690, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 688, __pyx_L1_error)
+    __PYX_ERR(0, 690, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "pyjoulescope_driver/binding.pyx":689
+  /* "pyjoulescope_driver/binding.pyx":691
  *         else:
  *             raise ValueError(f'Unsupported value type: {type(value)}')
  *         if '!' not in topic:             # <<<<<<<<<<<<<<
  *             v.flags = c_jsdrv.JSDRV_UNION_FLAG_RETAIN
  *         with nogil:
  */
   if (unlikely(__pyx_v_topic == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 689, __pyx_L1_error)
+    __PYX_ERR(0, 691, __pyx_L1_error)
   }
-  __pyx_t_4 = (__Pyx_PyUnicode_ContainsTF(__pyx_kp_u__10, __pyx_v_topic, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_ContainsTF(__pyx_kp_u__10, __pyx_v_topic, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 691, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   if (__pyx_t_3) {
 
-    /* "pyjoulescope_driver/binding.pyx":690
+    /* "pyjoulescope_driver/binding.pyx":692
  *             raise ValueError(f'Unsupported value type: {type(value)}')
  *         if '!' not in topic:
  *             v.flags = c_jsdrv.JSDRV_UNION_FLAG_RETAIN             # <<<<<<<<<<<<<<
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms)
  */
     __pyx_v_v.flags = JSDRV_UNION_FLAG_RETAIN;
 
-    /* "pyjoulescope_driver/binding.pyx":689
+    /* "pyjoulescope_driver/binding.pyx":691
  *         else:
  *             raise ValueError(f'Unsupported value type: {type(value)}')
  *         if '!' not in topic:             # <<<<<<<<<<<<<<
  *             v.flags = c_jsdrv.JSDRV_UNION_FLAG_RETAIN
  *         with nogil:
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":691
+  /* "pyjoulescope_driver/binding.pyx":693
  *         if '!' not in topic:
  *             v.flags = c_jsdrv.JSDRV_UNION_FLAG_RETAIN
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_publish', topic)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjoulescope_driver/binding.pyx":692
+        /* "pyjoulescope_driver/binding.pyx":694
  *             v.flags = c_jsdrv.JSDRV_UNION_FLAG_RETAIN
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms)             # <<<<<<<<<<<<<<
  *         _handle_rc(rc, 'jsdrv_publish', topic)
  * 
  */
         __pyx_t_11 = 0;
         __pyx_t_12 = -1;
         if (__pyx_t_11 < 0) {
           __pyx_t_11 += __pyx_v_topic_str.shape[0];
           if (unlikely(__pyx_t_11 < 0)) __pyx_t_12 = 0;
         } else if (unlikely(__pyx_t_11 >= __pyx_v_topic_str.shape[0])) __pyx_t_12 = 0;
         if (unlikely(__pyx_t_12 != -1)) {
           __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_12);
-          __PYX_ERR(0, 692, __pyx_L11_error)
+          __PYX_ERR(0, 694, __pyx_L11_error)
         }
         __pyx_v_rc = jsdrv_publish(__pyx_v_self->_context, ((char *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_topic_str.data + __pyx_t_11 * __pyx_v_topic_str.strides[0]) ))))), (&__pyx_v_v), __pyx_v_timeout_ms);
       }
 
-      /* "pyjoulescope_driver/binding.pyx":691
+      /* "pyjoulescope_driver/binding.pyx":693
  *         if '!' not in topic:
  *             v.flags = c_jsdrv.JSDRV_UNION_FLAG_RETAIN
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_publish', topic)
  */
       /*finally:*/ {
@@ -9793,24 +9792,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L12:;
       }
   }
 
-  /* "pyjoulescope_driver/binding.pyx":693
+  /* "pyjoulescope_driver/binding.pyx":695
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_publish', topic)             # <<<<<<<<<<<<<<
  * 
  *     def query(self, topic: str, timeout=None):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 693, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 693, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_13 = NULL;
   __pyx_t_12 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_13)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -9819,52 +9818,52 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_12 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_13, __pyx_t_6, __pyx_n_u_jsdrv_publish, __pyx_v_topic};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_12, 3+__pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_12, 3+__pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_13, __pyx_t_6, __pyx_n_u_jsdrv_publish, __pyx_v_topic};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_12, 3+__pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_12, 3+__pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_14 = PyTuple_New(3+__pyx_t_12); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 693, __pyx_L1_error)
+    __pyx_t_14 = PyTuple_New(3+__pyx_t_12); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 695, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     if (__pyx_t_13) {
       __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13); __pyx_t_13 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_12, __pyx_t_6);
     __Pyx_INCREF(__pyx_n_u_jsdrv_publish);
     __Pyx_GIVEREF(__pyx_n_u_jsdrv_publish);
     PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_12, __pyx_n_u_jsdrv_publish);
     __Pyx_INCREF(__pyx_v_topic);
     __Pyx_GIVEREF(__pyx_v_topic);
     PyTuple_SET_ITEM(__pyx_t_14, 2+__pyx_t_12, __pyx_v_topic);
     __pyx_t_6 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":642
+  /* "pyjoulescope_driver/binding.pyx":644
  *         _driver_count -= 1
  * 
  *     def publish(self, topic: str, value, timeout=None):             # <<<<<<<<<<<<<<
  *         """Publish a value to a topic.
  * 
  */
 
@@ -9885,15 +9884,15 @@
   __Pyx_XDECREF(__pyx_v_py_byte_str);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":695
+/* "pyjoulescope_driver/binding.pyx":697
  *         _handle_rc(rc, 'jsdrv_publish', topic)
  * 
  *     def query(self, topic: str, timeout=None):             # <<<<<<<<<<<<<<
  *         """Query the value for a topic.
  * 
  */
 
@@ -9933,15 +9932,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "query") < 0)) __PYX_ERR(0, 695, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "query") < 0)) __PYX_ERR(0, 697, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -9949,21 +9948,21 @@
       }
     }
     __pyx_v_topic = ((PyObject*)values[0]);
     __pyx_v_timeout = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("query", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 695, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("query", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 697, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.query", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_topic), (&PyUnicode_Type), 1, "topic", 1))) __PYX_ERR(0, 695, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_topic), (&PyUnicode_Type), 1, "topic", 1))) __PYX_ERR(0, 697, __pyx_L1_error)
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_10query(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_topic, __pyx_v_timeout);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9988,105 +9987,105 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("query", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":706
+  /* "pyjoulescope_driver/binding.pyx":708
  *         cdef c_jsdrv.jsdrv_union_s v
  *         cdef char byte_str[1024]
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')             # <<<<<<<<<<<<<<
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  * 
  */
   if (unlikely(__pyx_v_topic == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 706, __pyx_L1_error)
+    __PYX_ERR(0, 708, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_topic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 706, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_topic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 708, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 706, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 708, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_topic_str = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "pyjoulescope_driver/binding.pyx":707
+  /* "pyjoulescope_driver/binding.pyx":709
  *         cdef char byte_str[1024]
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)             # <<<<<<<<<<<<<<
  * 
  *         v.type = c_jsdrv.JSDRV_UNION_BIN
  */
   __pyx_v_timeout_ms = __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(__pyx_v_timeout, NULL);
 
-  /* "pyjoulescope_driver/binding.pyx":709
+  /* "pyjoulescope_driver/binding.pyx":711
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  * 
  *         v.type = c_jsdrv.JSDRV_UNION_BIN             # <<<<<<<<<<<<<<
  *         v.size = 1024
  *         v.value.str = byte_str
  */
   __pyx_v_v.type = JSDRV_UNION_BIN;
 
-  /* "pyjoulescope_driver/binding.pyx":710
+  /* "pyjoulescope_driver/binding.pyx":712
  * 
  *         v.type = c_jsdrv.JSDRV_UNION_BIN
  *         v.size = 1024             # <<<<<<<<<<<<<<
  *         v.value.str = byte_str
  *         with nogil:
  */
   __pyx_v_v.size = 0x400;
 
-  /* "pyjoulescope_driver/binding.pyx":711
+  /* "pyjoulescope_driver/binding.pyx":713
  *         v.type = c_jsdrv.JSDRV_UNION_BIN
  *         v.size = 1024
  *         v.value.str = byte_str             # <<<<<<<<<<<<<<
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_query(self._context, <char *> &topic_str[0], &v, timeout_ms)
  */
   __pyx_v_v.value.str = __pyx_v_byte_str;
 
-  /* "pyjoulescope_driver/binding.pyx":712
+  /* "pyjoulescope_driver/binding.pyx":714
  *         v.size = 1024
  *         v.value.str = byte_str
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_query(self._context, <char *> &topic_str[0], &v, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_query', topic)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjoulescope_driver/binding.pyx":713
+        /* "pyjoulescope_driver/binding.pyx":715
  *         v.value.str = byte_str
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_query(self._context, <char *> &topic_str[0], &v, timeout_ms)             # <<<<<<<<<<<<<<
  *         _handle_rc(rc, 'jsdrv_query', topic)
  *         return _jsdrv_union_to_py(&v)
  */
         __pyx_t_3 = 0;
         __pyx_t_4 = -1;
         if (__pyx_t_3 < 0) {
           __pyx_t_3 += __pyx_v_topic_str.shape[0];
           if (unlikely(__pyx_t_3 < 0)) __pyx_t_4 = 0;
         } else if (unlikely(__pyx_t_3 >= __pyx_v_topic_str.shape[0])) __pyx_t_4 = 0;
         if (unlikely(__pyx_t_4 != -1)) {
           __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_4);
-          __PYX_ERR(0, 713, __pyx_L4_error)
+          __PYX_ERR(0, 715, __pyx_L4_error)
         }
         __pyx_v_rc = jsdrv_query(__pyx_v_self->_context, ((char *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_topic_str.data + __pyx_t_3 * __pyx_v_topic_str.strides[0]) ))))), (&__pyx_v_v), __pyx_v_timeout_ms);
       }
 
-      /* "pyjoulescope_driver/binding.pyx":712
+      /* "pyjoulescope_driver/binding.pyx":714
  *         v.size = 1024
  *         v.value.str = byte_str
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_query(self._context, <char *> &topic_str[0], &v, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_query', topic)
  */
       /*finally:*/ {
@@ -10104,24 +10103,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyjoulescope_driver/binding.pyx":714
+  /* "pyjoulescope_driver/binding.pyx":716
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_query(self._context, <char *> &topic_str[0], &v, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_query', topic)             # <<<<<<<<<<<<<<
  *         return _jsdrv_union_to_py(&v)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 714, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 716, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 714, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 716, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -10130,66 +10129,66 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_6, __pyx_n_u_jsdrv_query, __pyx_v_topic};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 714, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_6, __pyx_n_u_jsdrv_query, __pyx_v_topic};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 714, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 714, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 716, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_4, __pyx_t_6);
     __Pyx_INCREF(__pyx_n_u_jsdrv_query);
     __Pyx_GIVEREF(__pyx_n_u_jsdrv_query);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_4, __pyx_n_u_jsdrv_query);
     __Pyx_INCREF(__pyx_v_topic);
     __Pyx_GIVEREF(__pyx_v_topic);
     PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_4, __pyx_v_topic);
     __pyx_t_6 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 714, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":715
+  /* "pyjoulescope_driver/binding.pyx":717
  *             rc = c_jsdrv.jsdrv_query(self._context, <char *> &topic_str[0], &v, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_query', topic)
  *         return _jsdrv_union_to_py(&v)             # <<<<<<<<<<<<<<
  * 
  *     def device_paths(self, timeout=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_19pyjoulescope_driver_7binding__jsdrv_union_to_py((&__pyx_v_v)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_19pyjoulescope_driver_7binding__jsdrv_union_to_py((&__pyx_v_v)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":695
+  /* "pyjoulescope_driver/binding.pyx":697
  *         _handle_rc(rc, 'jsdrv_publish', topic)
  * 
  *     def query(self, topic: str, timeout=None):             # <<<<<<<<<<<<<<
  *         """Query the value for a topic.
  * 
  */
 
@@ -10206,15 +10205,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_topic_str, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":717
+/* "pyjoulescope_driver/binding.pyx":719
  *         return _jsdrv_union_to_py(&v)
  * 
  *     def device_paths(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """List the currently connected devices.
  * 
  */
 
@@ -10247,29 +10246,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "device_paths") < 0)) __PYX_ERR(0, 717, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "device_paths") < 0)) __PYX_ERR(0, 719, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_timeout = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("device_paths", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 717, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("device_paths", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 719, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.device_paths", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_12device_paths(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_timeout);
 
@@ -10291,22 +10290,22 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("device_paths", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":724
+  /* "pyjoulescope_driver/binding.pyx":726
  *         :return: The list of device path strings.
  *         """
  *         s = self.query('@/list', timeout)             # <<<<<<<<<<<<<<
  *         if not len(s):
  *             return []
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 724, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -10315,117 +10314,117 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_kp_u_list, __pyx_v_timeout};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 724, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_kp_u_list, __pyx_v_timeout};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 724, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 724, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 726, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_kp_u_list);
     __Pyx_GIVEREF(__pyx_kp_u_list);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_kp_u_list);
     __Pyx_INCREF(__pyx_v_timeout);
     __Pyx_GIVEREF(__pyx_v_timeout);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_timeout);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 724, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":725
+  /* "pyjoulescope_driver/binding.pyx":727
  *         """
  *         s = self.query('@/list', timeout)
  *         if not len(s):             # <<<<<<<<<<<<<<
  *             return []
  *         return sorted(s.split(','))
  */
-  __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 727, __pyx_L1_error)
   __pyx_t_7 = ((!(__pyx_t_6 != 0)) != 0);
   if (__pyx_t_7) {
 
-    /* "pyjoulescope_driver/binding.pyx":726
+    /* "pyjoulescope_driver/binding.pyx":728
  *         s = self.query('@/list', timeout)
  *         if not len(s):
  *             return []             # <<<<<<<<<<<<<<
  *         return sorted(s.split(','))
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 728, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "pyjoulescope_driver/binding.pyx":725
+    /* "pyjoulescope_driver/binding.pyx":727
  *         """
  *         s = self.query('@/list', timeout)
  *         if not len(s):             # <<<<<<<<<<<<<<
  *             return []
  *         return sorted(s.split(','))
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":727
+  /* "pyjoulescope_driver/binding.pyx":729
  *         if not len(s):
  *             return []
  *         return sorted(s.split(','))             # <<<<<<<<<<<<<<
  * 
  *     def subscribe(self, topic: str, flags, fn, timeout=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_split); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_split); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_kp_u__11) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__11);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 727, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_5 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_1 = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_8 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_8 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 729, __pyx_L1_error)
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyjoulescope_driver/binding.pyx":717
+  /* "pyjoulescope_driver/binding.pyx":719
  *         return _jsdrv_union_to_py(&v)
  * 
  *     def device_paths(self, timeout=None):             # <<<<<<<<<<<<<<
  *         """List the currently connected devices.
  * 
  */
 
@@ -10440,15 +10439,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":729
+/* "pyjoulescope_driver/binding.pyx":731
  *         return sorted(s.split(','))
  * 
  *     def subscribe(self, topic: str, flags, fn, timeout=None):             # <<<<<<<<<<<<<<
  *         """Subscribe to receive topic updates.
  * 
  */
 
@@ -10490,31 +10489,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_topic)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("subscribe", 0, 3, 4, 1); __PYX_ERR(0, 729, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("subscribe", 0, 3, 4, 1); __PYX_ERR(0, 731, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fn)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("subscribe", 0, 3, 4, 2); __PYX_ERR(0, 729, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("subscribe", 0, 3, 4, 2); __PYX_ERR(0, 731, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "subscribe") < 0)) __PYX_ERR(0, 729, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "subscribe") < 0)) __PYX_ERR(0, 731, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -10526,21 +10525,21 @@
     __pyx_v_topic = ((PyObject*)values[0]);
     __pyx_v_flags = values[1];
     __pyx_v_fn = values[2];
     __pyx_v_timeout = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("subscribe", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 729, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("subscribe", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 731, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.subscribe", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_topic), (&PyUnicode_Type), 1, "topic", 1))) __PYX_ERR(0, 729, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_topic), (&PyUnicode_Type), 1, "topic", 1))) __PYX_ERR(0, 731, __pyx_L1_error)
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_14subscribe(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_topic, __pyx_v_flags, __pyx_v_fn, __pyx_v_timeout);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -10574,116 +10573,116 @@
   Py_ssize_t __pyx_t_15;
   int __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("subscribe", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":759
+  /* "pyjoulescope_driver/binding.pyx":761
  *         :raise RuntimeError: on subscribe failure.
  *         """
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')             # <<<<<<<<<<<<<<
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  *         cdef int32_t c_flags = 0
  */
   if (unlikely(__pyx_v_topic == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 759, __pyx_L1_error)
+    __PYX_ERR(0, 761, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_topic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_topic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 761, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 761, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_topic_str = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "pyjoulescope_driver/binding.pyx":760
+  /* "pyjoulescope_driver/binding.pyx":762
  *         """
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)             # <<<<<<<<<<<<<<
  *         cdef int32_t c_flags = 0
  *         cdef void * fn_ptr = <void *> fn
  */
   __pyx_v_timeout_ms = __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(__pyx_v_timeout, NULL);
 
-  /* "pyjoulescope_driver/binding.pyx":761
+  /* "pyjoulescope_driver/binding.pyx":763
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  *         cdef int32_t c_flags = 0             # <<<<<<<<<<<<<<
  *         cdef void * fn_ptr = <void *> fn
  * 
  */
   __pyx_v_c_flags = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":762
+  /* "pyjoulescope_driver/binding.pyx":764
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  *         cdef int32_t c_flags = 0
  *         cdef void * fn_ptr = <void *> fn             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(flags, str):
  */
   __pyx_v_fn_ptr = ((void *)__pyx_v_fn);
 
-  /* "pyjoulescope_driver/binding.pyx":764
+  /* "pyjoulescope_driver/binding.pyx":766
  *         cdef void * fn_ptr = <void *> fn
  * 
  *         if isinstance(flags, str):             # <<<<<<<<<<<<<<
  *             c_flags = _SUBSCRIBE_FLAG_LOOKUP[flags.lower()]
  *         elif isinstance(flags, (list, tuple)) and isinstance(flags[0], str):
  */
   __pyx_t_3 = PyUnicode_Check(__pyx_v_flags); 
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "pyjoulescope_driver/binding.pyx":765
+    /* "pyjoulescope_driver/binding.pyx":767
  * 
  *         if isinstance(flags, str):
  *             c_flags = _SUBSCRIBE_FLAG_LOOKUP[flags.lower()]             # <<<<<<<<<<<<<<
  *         elif isinstance(flags, (list, tuple)) and isinstance(flags[0], str):
  *             for f in flags:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SUBSCRIBE_FLAG_LOOKUP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 765, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SUBSCRIBE_FLAG_LOOKUP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_flags, __pyx_n_s_lower); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 765, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_flags, __pyx_n_s_lower); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 765, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 765, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_8 = __Pyx_PyInt_As_int32_t(__pyx_t_6); if (unlikely((__pyx_t_8 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 765, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_int32_t(__pyx_t_6); if (unlikely((__pyx_t_8 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 767, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_c_flags = __pyx_t_8;
 
-    /* "pyjoulescope_driver/binding.pyx":764
+    /* "pyjoulescope_driver/binding.pyx":766
  *         cdef void * fn_ptr = <void *> fn
  * 
  *         if isinstance(flags, str):             # <<<<<<<<<<<<<<
  *             c_flags = _SUBSCRIBE_FLAG_LOOKUP[flags.lower()]
  *         elif isinstance(flags, (list, tuple)) and isinstance(flags[0], str):
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":766
+  /* "pyjoulescope_driver/binding.pyx":768
  *         if isinstance(flags, str):
  *             c_flags = _SUBSCRIBE_FLAG_LOOKUP[flags.lower()]
  *         elif isinstance(flags, (list, tuple)) and isinstance(flags[0], str):             # <<<<<<<<<<<<<<
  *             for f in flags:
  *                 c_flags |= _SUBSCRIBE_FLAG_LOOKUP[f.lower()]
  */
   __pyx_t_9 = PyList_Check(__pyx_v_flags); 
@@ -10699,158 +10698,158 @@
   __pyx_L6_bool_binop_done:;
   __pyx_t_9 = (__pyx_t_3 != 0);
   if (__pyx_t_9) {
   } else {
     __pyx_t_4 = __pyx_t_9;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_flags, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 766, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_flags, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 768, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_9 = PyUnicode_Check(__pyx_t_6); 
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_3 = (__pyx_t_9 != 0);
   __pyx_t_4 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_4) {
 
-    /* "pyjoulescope_driver/binding.pyx":767
+    /* "pyjoulescope_driver/binding.pyx":769
  *             c_flags = _SUBSCRIBE_FLAG_LOOKUP[flags.lower()]
  *         elif isinstance(flags, (list, tuple)) and isinstance(flags[0], str):
  *             for f in flags:             # <<<<<<<<<<<<<<
  *                 c_flags |= _SUBSCRIBE_FLAG_LOOKUP[f.lower()]
  *         else:
  */
     if (likely(PyList_CheckExact(__pyx_v_flags)) || PyTuple_CheckExact(__pyx_v_flags)) {
       __pyx_t_6 = __pyx_v_flags; __Pyx_INCREF(__pyx_t_6); __pyx_t_11 = 0;
       __pyx_t_12 = NULL;
     } else {
-      __pyx_t_11 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_flags); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 767, __pyx_L1_error)
+      __pyx_t_11 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_flags); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 769, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_12 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 767, __pyx_L1_error)
+      __pyx_t_12 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 769, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_12)) {
         if (likely(PyList_CheckExact(__pyx_t_6))) {
           if (__pyx_t_11 >= PyList_GET_SIZE(__pyx_t_6)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 767, __pyx_L1_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 769, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_6, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 767, __pyx_L1_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_6, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 769, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_11 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 767, __pyx_L1_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely(0 < 0)) __PYX_ERR(0, 769, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_6, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 767, __pyx_L1_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_6, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 769, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_12(__pyx_t_6);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 767, __pyx_L1_error)
+            else __PYX_ERR(0, 769, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_v_f, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "pyjoulescope_driver/binding.pyx":768
+      /* "pyjoulescope_driver/binding.pyx":770
  *         elif isinstance(flags, (list, tuple)) and isinstance(flags[0], str):
  *             for f in flags:
  *                 c_flags |= _SUBSCRIBE_FLAG_LOOKUP[f.lower()]             # <<<<<<<<<<<<<<
  *         else:
  *             c_flags = <int32_t> int(flags)
  */
-      __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_c_flags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 768, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_c_flags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 770, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SUBSCRIBE_FLAG_LOOKUP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 768, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SUBSCRIBE_FLAG_LOOKUP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 770, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_lower); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 768, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_lower); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 770, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __pyx_t_14 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
         __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_13);
         if (likely(__pyx_t_14)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
           __Pyx_INCREF(__pyx_t_14);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_13, function);
         }
       }
       __pyx_t_7 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_13);
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 768, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 770, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __pyx_t_13 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 768, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_7); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 770, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_7 = PyNumber_InPlaceOr(__pyx_t_5, __pyx_t_13); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 768, __pyx_L1_error)
+      __pyx_t_7 = PyNumber_InPlaceOr(__pyx_t_5, __pyx_t_13); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 770, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __pyx_t_8 = __Pyx_PyInt_As_int32_t(__pyx_t_7); if (unlikely((__pyx_t_8 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 768, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_As_int32_t(__pyx_t_7); if (unlikely((__pyx_t_8 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 770, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_v_c_flags = __pyx_t_8;
 
-      /* "pyjoulescope_driver/binding.pyx":767
+      /* "pyjoulescope_driver/binding.pyx":769
  *             c_flags = _SUBSCRIBE_FLAG_LOOKUP[flags.lower()]
  *         elif isinstance(flags, (list, tuple)) and isinstance(flags[0], str):
  *             for f in flags:             # <<<<<<<<<<<<<<
  *                 c_flags |= _SUBSCRIBE_FLAG_LOOKUP[f.lower()]
  *         else:
  */
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":766
+    /* "pyjoulescope_driver/binding.pyx":768
  *         if isinstance(flags, str):
  *             c_flags = _SUBSCRIBE_FLAG_LOOKUP[flags.lower()]
  *         elif isinstance(flags, (list, tuple)) and isinstance(flags[0], str):             # <<<<<<<<<<<<<<
  *             for f in flags:
  *                 c_flags |= _SUBSCRIBE_FLAG_LOOKUP[f.lower()]
  */
     goto __pyx_L3;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":770
+  /* "pyjoulescope_driver/binding.pyx":772
  *                 c_flags |= _SUBSCRIBE_FLAG_LOOKUP[f.lower()]
  *         else:
  *             c_flags = <int32_t> int(flags)             # <<<<<<<<<<<<<<
  *         self._subscribers.add((topic, fn))
  *         with nogil:
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyNumber_Int(__pyx_v_flags); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 770, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyNumber_Int(__pyx_v_flags); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 772, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_8 = __Pyx_PyInt_As_int32_t(__pyx_t_6); if (unlikely((__pyx_t_8 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 770, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_int32_t(__pyx_t_6); if (unlikely((__pyx_t_8 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 772, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_c_flags = ((int32_t)__pyx_t_8);
   }
   __pyx_L3:;
 
-  /* "pyjoulescope_driver/binding.pyx":771
+  /* "pyjoulescope_driver/binding.pyx":773
  *         else:
  *             c_flags = <int32_t> int(flags)
  *         self._subscribers.add((topic, fn))             # <<<<<<<<<<<<<<
  *         with nogil:
- *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish1_cbk, fn_ptr, timeout_ms)
+ *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish_cbk, fn_ptr, timeout_ms)
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_subscribers, __pyx_n_s_add); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 771, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_subscribers, __pyx_n_s_add); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 773, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_13 = PyTuple_New(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 771, __pyx_L1_error)
+  __pyx_t_13 = PyTuple_New(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 773, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_INCREF(__pyx_v_topic);
   __Pyx_GIVEREF(__pyx_v_topic);
   PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_v_topic);
   __Pyx_INCREF(__pyx_v_fn);
   __Pyx_GIVEREF(__pyx_v_fn);
   PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_v_fn);
@@ -10863,59 +10862,59 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_6 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_5, __pyx_t_13) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_13);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 771, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 773, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":772
+  /* "pyjoulescope_driver/binding.pyx":774
  *             c_flags = <int32_t> int(flags)
  *         self._subscribers.add((topic, fn))
  *         with nogil:             # <<<<<<<<<<<<<<
- *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish1_cbk, fn_ptr, timeout_ms)
+ *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish_cbk, fn_ptr, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_subscribe', topic)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjoulescope_driver/binding.pyx":773
+        /* "pyjoulescope_driver/binding.pyx":775
  *         self._subscribers.add((topic, fn))
  *         with nogil:
- *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish1_cbk, fn_ptr, timeout_ms)             # <<<<<<<<<<<<<<
+ *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish_cbk, fn_ptr, timeout_ms)             # <<<<<<<<<<<<<<
  *         _handle_rc(rc, 'jsdrv_subscribe', topic)
  * 
  */
         __pyx_t_15 = 0;
         __pyx_t_16 = -1;
         if (__pyx_t_15 < 0) {
           __pyx_t_15 += __pyx_v_topic_str.shape[0];
           if (unlikely(__pyx_t_15 < 0)) __pyx_t_16 = 0;
         } else if (unlikely(__pyx_t_15 >= __pyx_v_topic_str.shape[0])) __pyx_t_16 = 0;
         if (unlikely(__pyx_t_16 != -1)) {
           __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_16);
-          __PYX_ERR(0, 773, __pyx_L11_error)
+          __PYX_ERR(0, 775, __pyx_L11_error)
         }
-        __pyx_v_rc = jsdrv_subscribe(__pyx_v_self->_context, ((char *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_topic_str.data + __pyx_t_15 * __pyx_v_topic_str.strides[0]) ))))), __pyx_v_c_flags, __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish1_cbk, __pyx_v_fn_ptr, __pyx_v_timeout_ms);
+        __pyx_v_rc = jsdrv_subscribe(__pyx_v_self->_context, ((char *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_topic_str.data + __pyx_t_15 * __pyx_v_topic_str.strides[0]) ))))), __pyx_v_c_flags, __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish_cbk, __pyx_v_fn_ptr, __pyx_v_timeout_ms);
       }
 
-      /* "pyjoulescope_driver/binding.pyx":772
+      /* "pyjoulescope_driver/binding.pyx":774
  *             c_flags = <int32_t> int(flags)
  *         self._subscribers.add((topic, fn))
  *         with nogil:             # <<<<<<<<<<<<<<
- *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish1_cbk, fn_ptr, timeout_ms)
+ *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish_cbk, fn_ptr, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_subscribe', topic)
  */
       /*finally:*/ {
         /*normal exit:*/{
           #ifdef WITH_THREAD
           __Pyx_FastGIL_Forget();
           Py_BLOCK_THREADS
@@ -10929,24 +10928,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L12:;
       }
   }
 
-  /* "pyjoulescope_driver/binding.pyx":774
+  /* "pyjoulescope_driver/binding.pyx":776
  *         with nogil:
- *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish1_cbk, fn_ptr, timeout_ms)
+ *             rc = c_jsdrv.jsdrv_subscribe(self._context, <char *> &topic_str[0], c_flags, _on_cmd_publish_cbk, fn_ptr, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_subscribe', topic)             # <<<<<<<<<<<<<<
  * 
  *     def unsubscribe(self, topic, fn, timeout=None):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 774, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 776, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_13 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 774, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 776, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_5 = NULL;
   __pyx_t_16 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -10955,52 +10954,52 @@
       __Pyx_DECREF_SET(__pyx_t_7, function);
       __pyx_t_16 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_13, __pyx_n_u_jsdrv_subscribe, __pyx_v_topic};
-    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 774, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_13, __pyx_n_u_jsdrv_subscribe, __pyx_v_topic};
-    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 774, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   } else
   #endif
   {
-    __pyx_t_1 = PyTuple_New(3+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 774, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_13);
     PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_16, __pyx_t_13);
     __Pyx_INCREF(__pyx_n_u_jsdrv_subscribe);
     __Pyx_GIVEREF(__pyx_n_u_jsdrv_subscribe);
     PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_16, __pyx_n_u_jsdrv_subscribe);
     __Pyx_INCREF(__pyx_v_topic);
     __Pyx_GIVEREF(__pyx_v_topic);
     PyTuple_SET_ITEM(__pyx_t_1, 2+__pyx_t_16, __pyx_v_topic);
     __pyx_t_13 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 774, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":729
+  /* "pyjoulescope_driver/binding.pyx":731
  *         return sorted(s.split(','))
  * 
  *     def subscribe(self, topic: str, flags, fn, timeout=None):             # <<<<<<<<<<<<<<
  *         """Subscribe to receive topic updates.
  * 
  */
 
@@ -11021,15 +11020,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_topic_str, 1);
   __Pyx_XDECREF(__pyx_v_f);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":776
+/* "pyjoulescope_driver/binding.pyx":778
  *         _handle_rc(rc, 'jsdrv_subscribe', topic)
  * 
  *     def unsubscribe(self, topic, fn, timeout=None):             # <<<<<<<<<<<<<<
  *         """Unsubscribe from a topic.
  * 
  */
 
@@ -11068,25 +11067,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_topic)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fn)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("unsubscribe", 0, 2, 3, 1); __PYX_ERR(0, 776, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("unsubscribe", 0, 2, 3, 1); __PYX_ERR(0, 778, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "unsubscribe") < 0)) __PYX_ERR(0, 776, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "unsubscribe") < 0)) __PYX_ERR(0, 778, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -11096,15 +11095,15 @@
     }
     __pyx_v_topic = values[0];
     __pyx_v_fn = values[1];
     __pyx_v_timeout = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("unsubscribe", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 776, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("unsubscribe", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 778, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.unsubscribe", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_16unsubscribe(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_topic, __pyx_v_fn, __pyx_v_timeout);
 
@@ -11120,147 +11119,112 @@
   int32_t __pyx_v_rc;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_memviewslice __pyx_t_4 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  PyObject *__pyx_t_5 = NULL;
-  Py_ssize_t __pyx_t_6;
-  int __pyx_t_7;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unsubscribe", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":785
+  /* "pyjoulescope_driver/binding.pyx":787
  *         :raise: On error.
  *         """
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')             # <<<<<<<<<<<<<<
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  *         cdef void * fn_ptr = <void *> fn
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_topic, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 785, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_topic, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 787, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 785, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 787, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 785, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 787, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_topic_str = __pyx_t_4;
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
 
-  /* "pyjoulescope_driver/binding.pyx":786
+  /* "pyjoulescope_driver/binding.pyx":788
  *         """
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)             # <<<<<<<<<<<<<<
  *         cdef void * fn_ptr = <void *> fn
  * 
  */
   __pyx_v_timeout_ms = __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(__pyx_v_timeout, NULL);
 
-  /* "pyjoulescope_driver/binding.pyx":787
+  /* "pyjoulescope_driver/binding.pyx":789
  *         cdef const uint8_t[:] topic_str = topic.encode('utf-8')
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  *         cdef void * fn_ptr = <void *> fn             # <<<<<<<<<<<<<<
  * 
- *         self._subscribers.discard((topic, fn))
+ *         with nogil:
  */
   __pyx_v_fn_ptr = ((void *)__pyx_v_fn);
 
-  /* "pyjoulescope_driver/binding.pyx":789
+  /* "pyjoulescope_driver/binding.pyx":791
  *         cdef void * fn_ptr = <void *> fn
  * 
- *         self._subscribers.discard((topic, fn))             # <<<<<<<<<<<<<<
- *         with nogil:
- *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish1_cbk, fn_ptr, timeout_ms)
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_subscribers, __pyx_n_s_discard); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 789, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 789, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_INCREF(__pyx_v_topic);
-  __Pyx_GIVEREF(__pyx_v_topic);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_topic);
-  __Pyx_INCREF(__pyx_v_fn);
-  __Pyx_GIVEREF(__pyx_v_fn);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_fn);
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_5);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 789, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "pyjoulescope_driver/binding.pyx":790
- * 
- *         self._subscribers.discard((topic, fn))
  *         with nogil:             # <<<<<<<<<<<<<<
- *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish1_cbk, fn_ptr, timeout_ms)
- *         _handle_rc(rc, 'jsdrv_unsubscribe', topic)
+ *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish_cbk, fn_ptr, timeout_ms)
+ *         self._subscribers.discard((topic, fn))
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjoulescope_driver/binding.pyx":791
- *         self._subscribers.discard((topic, fn))
+        /* "pyjoulescope_driver/binding.pyx":792
+ * 
  *         with nogil:
- *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish1_cbk, fn_ptr, timeout_ms)             # <<<<<<<<<<<<<<
+ *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish_cbk, fn_ptr, timeout_ms)             # <<<<<<<<<<<<<<
+ *         self._subscribers.discard((topic, fn))
  *         _handle_rc(rc, 'jsdrv_unsubscribe', topic)
- * 
  */
-        __pyx_t_6 = 0;
-        __pyx_t_7 = -1;
-        if (__pyx_t_6 < 0) {
-          __pyx_t_6 += __pyx_v_topic_str.shape[0];
-          if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
-        } else if (unlikely(__pyx_t_6 >= __pyx_v_topic_str.shape[0])) __pyx_t_7 = 0;
-        if (unlikely(__pyx_t_7 != -1)) {
-          __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_7);
-          __PYX_ERR(0, 791, __pyx_L4_error)
+        __pyx_t_5 = 0;
+        __pyx_t_6 = -1;
+        if (__pyx_t_5 < 0) {
+          __pyx_t_5 += __pyx_v_topic_str.shape[0];
+          if (unlikely(__pyx_t_5 < 0)) __pyx_t_6 = 0;
+        } else if (unlikely(__pyx_t_5 >= __pyx_v_topic_str.shape[0])) __pyx_t_6 = 0;
+        if (unlikely(__pyx_t_6 != -1)) {
+          __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_6);
+          __PYX_ERR(0, 792, __pyx_L4_error)
         }
-        __pyx_v_rc = jsdrv_unsubscribe(__pyx_v_self->_context, ((char *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_topic_str.data + __pyx_t_6 * __pyx_v_topic_str.strides[0]) ))))), __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish1_cbk, __pyx_v_fn_ptr, __pyx_v_timeout_ms);
+        __pyx_v_rc = jsdrv_unsubscribe(__pyx_v_self->_context, ((char *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_topic_str.data + __pyx_t_5 * __pyx_v_topic_str.strides[0]) ))))), __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish_cbk, __pyx_v_fn_ptr, __pyx_v_timeout_ms);
       }
 
-      /* "pyjoulescope_driver/binding.pyx":790
+      /* "pyjoulescope_driver/binding.pyx":791
+ *         cdef void * fn_ptr = <void *> fn
  * 
- *         self._subscribers.discard((topic, fn))
  *         with nogil:             # <<<<<<<<<<<<<<
- *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish1_cbk, fn_ptr, timeout_ms)
- *         _handle_rc(rc, 'jsdrv_unsubscribe', topic)
+ *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish_cbk, fn_ptr, timeout_ms)
+ *         self._subscribers.discard((topic, fn))
  */
       /*finally:*/ {
         /*normal exit:*/{
           #ifdef WITH_THREAD
           __Pyx_FastGIL_Forget();
           Py_BLOCK_THREADS
           #endif
@@ -11273,78 +11237,113 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyjoulescope_driver/binding.pyx":792
+  /* "pyjoulescope_driver/binding.pyx":793
  *         with nogil:
- *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish1_cbk, fn_ptr, timeout_ms)
+ *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish_cbk, fn_ptr, timeout_ms)
+ *         self._subscribers.discard((topic, fn))             # <<<<<<<<<<<<<<
+ *         _handle_rc(rc, 'jsdrv_unsubscribe', topic)
+ * 
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_subscribers, __pyx_n_s_discard); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 793, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_INCREF(__pyx_v_topic);
+  __Pyx_GIVEREF(__pyx_v_topic);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_topic);
+  __Pyx_INCREF(__pyx_v_fn);
+  __Pyx_GIVEREF(__pyx_v_fn);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_fn);
+  __pyx_t_7 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_7)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_7);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_7, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 793, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "pyjoulescope_driver/binding.pyx":794
+ *             rc = c_jsdrv.jsdrv_unsubscribe(self._context, <char *> &topic_str[0], _on_cmd_publish_cbk, fn_ptr, timeout_ms)
+ *         self._subscribers.discard((topic, fn))
  *         _handle_rc(rc, 'jsdrv_unsubscribe', topic)             # <<<<<<<<<<<<<<
  * 
  *     def unsubscribe_all(self, fn, timeout=None):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 792, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 794, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 792, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 794, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = NULL;
-  __pyx_t_7 = 0;
+  __pyx_t_7 = NULL;
+  __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_5)) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_7 = 1;
+      __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_3, __pyx_n_u_jsdrv_unsubscribe, __pyx_v_topic};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_n_u_jsdrv_unsubscribe, __pyx_v_topic};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 794, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_3, __pyx_n_u_jsdrv_unsubscribe, __pyx_v_topic};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, __pyx_n_u_jsdrv_unsubscribe, __pyx_v_topic};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 794, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 792, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (__pyx_t_5) {
-      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
+    if (__pyx_t_7) {
+      __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_6, __pyx_t_3);
     __Pyx_INCREF(__pyx_n_u_jsdrv_unsubscribe);
     __Pyx_GIVEREF(__pyx_n_u_jsdrv_unsubscribe);
-    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_n_u_jsdrv_unsubscribe);
+    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_6, __pyx_n_u_jsdrv_unsubscribe);
     __Pyx_INCREF(__pyx_v_topic);
     __Pyx_GIVEREF(__pyx_v_topic);
-    PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_v_topic);
+    PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_6, __pyx_v_topic);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":776
+  /* "pyjoulescope_driver/binding.pyx":778
  *         _handle_rc(rc, 'jsdrv_subscribe', topic)
  * 
  *     def unsubscribe(self, topic, fn, timeout=None):             # <<<<<<<<<<<<<<
  *         """Unsubscribe from a topic.
  * 
  */
 
@@ -11352,26 +11351,26 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.unsubscribe", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_topic_str, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":794
+/* "pyjoulescope_driver/binding.pyx":796
  *         _handle_rc(rc, 'jsdrv_unsubscribe', topic)
  * 
  *     def unsubscribe_all(self, fn, timeout=None):             # <<<<<<<<<<<<<<
  *         """Unsubscribe a callback from all topics.
  * 
  */
 
@@ -11411,15 +11410,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "unsubscribe_all") < 0)) __PYX_ERR(0, 794, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "unsubscribe_all") < 0)) __PYX_ERR(0, 796, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -11427,32 +11426,32 @@
       }
     }
     __pyx_v_fn = values[0];
     __pyx_v_timeout = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("unsubscribe_all", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 794, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("unsubscribe_all", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 796, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.unsubscribe_all", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_18unsubscribe_all(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_fn, __pyx_v_timeout);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_19pyjoulescope_driver_7binding_6Driver_18unsubscribe_all(struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *__pyx_v_self, PyObject *__pyx_v_fn, PyObject *__pyx_v_timeout) {
   int32_t __pyx_v_timeout_ms;
+  int32_t __pyx_v_rc;
   PyObject *__pyx_v_remove_list = NULL;
   PyObject *__pyx_v_item = NULL;
-  int32_t __pyx_v_rc;
   PyObject *__pyx_7genexpr__pyx_v_t = NULL;
   PyObject *__pyx_7genexpr__pyx_v_f = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
@@ -11465,260 +11464,260 @@
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unsubscribe_all", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":802
+  /* "pyjoulescope_driver/binding.pyx":804
  *         :raise: On error.
  *         """
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)             # <<<<<<<<<<<<<<
  * 
- *         remove_list = [(t, f) for t, f in self._subscribers if f == fn]
+ *         with nogil:
  */
   __pyx_v_timeout_ms = __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(__pyx_v_timeout, NULL);
 
-  /* "pyjoulescope_driver/binding.pyx":804
+  /* "pyjoulescope_driver/binding.pyx":806
+ *         cdef int32_t timeout_ms = _timeout_validate(timeout)
+ * 
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish_cbk, <void *> fn, timeout_ms)
+ *         remove_list = [(t, f) for t, f in self._subscribers if f == fn]
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "pyjoulescope_driver/binding.pyx":807
+ * 
+ *         with nogil:
+ *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish_cbk, <void *> fn, timeout_ms)             # <<<<<<<<<<<<<<
+ *         remove_list = [(t, f) for t, f in self._subscribers if f == fn]
+ *         for item in remove_list:
+ */
+        __pyx_v_rc = jsdrv_unsubscribe_all(__pyx_v_self->_context, __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish_cbk, ((void *)__pyx_v_fn), __pyx_v_timeout_ms);
+      }
+
+      /* "pyjoulescope_driver/binding.pyx":806
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  * 
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish_cbk, <void *> fn, timeout_ms)
+ *         remove_list = [(t, f) for t, f in self._subscribers if f == fn]
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "pyjoulescope_driver/binding.pyx":808
+ *         with nogil:
+ *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish_cbk, <void *> fn, timeout_ms)
  *         remove_list = [(t, f) for t, f in self._subscribers if f == fn]             # <<<<<<<<<<<<<<
  *         for item in remove_list:
  *             self._subscribers.discard(item)
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 804, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 808, __pyx_L8_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(__pyx_v_self->_subscribers)) || PyTuple_CheckExact(__pyx_v_self->_subscribers)) {
       __pyx_t_2 = __pyx_v_self->_subscribers; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_self->_subscribers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 804, __pyx_L5_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_self->_subscribers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 808, __pyx_L8_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 804, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 808, __pyx_L8_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 804, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 808, __pyx_L8_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 804, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 808, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 804, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 808, __pyx_L8_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 804, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 808, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 804, __pyx_L5_error)
+            else __PYX_ERR(0, 808, __pyx_L8_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
         PyObject* sequence = __pyx_t_5;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 804, __pyx_L5_error)
+          __PYX_ERR(0, 808, __pyx_L8_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         #else
-        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 804, __pyx_L5_error)
+        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 808, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 804, __pyx_L5_error)
+        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 808, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_8 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 804, __pyx_L5_error)
+        __pyx_t_8 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 808, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
-        index = 0; __pyx_t_6 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_6)) goto __pyx_L8_unpacking_failed;
+        index = 0; __pyx_t_6 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_6)) goto __pyx_L11_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_6);
-        index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L8_unpacking_failed;
+        index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L11_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_7);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 804, __pyx_L5_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 808, __pyx_L8_error)
         __pyx_t_9 = NULL;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        goto __pyx_L9_unpacking_done;
-        __pyx_L8_unpacking_failed:;
+        goto __pyx_L12_unpacking_done;
+        __pyx_L11_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_t_9 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 804, __pyx_L5_error)
-        __pyx_L9_unpacking_done:;
+        __PYX_ERR(0, 808, __pyx_L8_error)
+        __pyx_L12_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_t, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_f, __pyx_t_7);
       __pyx_t_7 = 0;
-      __pyx_t_5 = PyObject_RichCompare(__pyx_7genexpr__pyx_v_f, __pyx_v_fn, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 804, __pyx_L5_error)
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 804, __pyx_L5_error)
+      __pyx_t_5 = PyObject_RichCompare(__pyx_7genexpr__pyx_v_f, __pyx_v_fn, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 808, __pyx_L8_error)
+      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 808, __pyx_L8_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (__pyx_t_10) {
-        __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 804, __pyx_L5_error)
+        __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 808, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_INCREF(__pyx_7genexpr__pyx_v_t);
         __Pyx_GIVEREF(__pyx_7genexpr__pyx_v_t);
         PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_7genexpr__pyx_v_t);
         __Pyx_INCREF(__pyx_7genexpr__pyx_v_f);
         __Pyx_GIVEREF(__pyx_7genexpr__pyx_v_f);
         PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_7genexpr__pyx_v_f);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 804, __pyx_L5_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 808, __pyx_L8_error)
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_f); __pyx_7genexpr__pyx_v_f = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_t); __pyx_7genexpr__pyx_v_t = 0;
-    goto __pyx_L11_exit_scope;
-    __pyx_L5_error:;
+    goto __pyx_L14_exit_scope;
+    __pyx_L8_error:;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_f); __pyx_7genexpr__pyx_v_f = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_t); __pyx_7genexpr__pyx_v_t = 0;
     goto __pyx_L1_error;
-    __pyx_L11_exit_scope:;
+    __pyx_L14_exit_scope:;
   } /* exit inner scope */
   __pyx_v_remove_list = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":805
- * 
+  /* "pyjoulescope_driver/binding.pyx":809
+ *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish_cbk, <void *> fn, timeout_ms)
  *         remove_list = [(t, f) for t, f in self._subscribers if f == fn]
  *         for item in remove_list:             # <<<<<<<<<<<<<<
  *             self._subscribers.discard(item)
- *         with nogil:
+ *         _handle_rc(rc, 'jsdrv_unsubscribe_all')
  */
   __pyx_t_1 = __pyx_v_remove_list; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
   for (;;) {
     if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 805, __pyx_L1_error)
+    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 809, __pyx_L1_error)
     #else
-    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 805, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 809, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":806
+    /* "pyjoulescope_driver/binding.pyx":810
  *         remove_list = [(t, f) for t, f in self._subscribers if f == fn]
  *         for item in remove_list:
  *             self._subscribers.discard(item)             # <<<<<<<<<<<<<<
- *         with nogil:
- *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish1_cbk, <void *> fn, timeout_ms)
+ *         _handle_rc(rc, 'jsdrv_unsubscribe_all')
+ * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_subscribers, __pyx_n_s_discard); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 806, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_subscribers, __pyx_n_s_discard); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 810, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_v_item) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_item);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 806, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 810, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":805
- * 
+    /* "pyjoulescope_driver/binding.pyx":809
+ *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish_cbk, <void *> fn, timeout_ms)
  *         remove_list = [(t, f) for t, f in self._subscribers if f == fn]
  *         for item in remove_list:             # <<<<<<<<<<<<<<
  *             self._subscribers.discard(item)
- *         with nogil:
+ *         _handle_rc(rc, 'jsdrv_unsubscribe_all')
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":807
- *         for item in remove_list:
- *             self._subscribers.discard(item)
- *         with nogil:             # <<<<<<<<<<<<<<
- *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish1_cbk, <void *> fn, timeout_ms)
- *         _handle_rc(rc, 'jsdrv_unsubscribe_all')
- */
-  {
-      #ifdef WITH_THREAD
-      PyThreadState *_save;
-      Py_UNBLOCK_THREADS
-      __Pyx_FastGIL_Remember();
-      #endif
-      /*try:*/ {
-
-        /* "pyjoulescope_driver/binding.pyx":808
- *             self._subscribers.discard(item)
- *         with nogil:
- *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish1_cbk, <void *> fn, timeout_ms)             # <<<<<<<<<<<<<<
- *         _handle_rc(rc, 'jsdrv_unsubscribe_all')
- * 
- */
-        __pyx_v_rc = jsdrv_unsubscribe_all(__pyx_v_self->_context, __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish1_cbk, ((void *)__pyx_v_fn), __pyx_v_timeout_ms);
-      }
-
-      /* "pyjoulescope_driver/binding.pyx":807
+  /* "pyjoulescope_driver/binding.pyx":811
  *         for item in remove_list:
  *             self._subscribers.discard(item)
- *         with nogil:             # <<<<<<<<<<<<<<
- *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish1_cbk, <void *> fn, timeout_ms)
- *         _handle_rc(rc, 'jsdrv_unsubscribe_all')
- */
-      /*finally:*/ {
-        /*normal exit:*/{
-          #ifdef WITH_THREAD
-          __Pyx_FastGIL_Forget();
-          Py_BLOCK_THREADS
-          #endif
-          goto __pyx_L16;
-        }
-        __pyx_L16:;
-      }
-  }
-
-  /* "pyjoulescope_driver/binding.pyx":809
- *         with nogil:
- *             rc = c_jsdrv.jsdrv_unsubscribe_all(self._context, _on_cmd_publish1_cbk, <void *> fn, timeout_ms)
  *         _handle_rc(rc, 'jsdrv_unsubscribe_all')             # <<<<<<<<<<<<<<
  * 
  *     def open(self, device_prefix, mode=None, timeout=None):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 809, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 811, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 809, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 811, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -11727,49 +11726,49 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_11 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_n_u_jsdrv_unsubscribe_all};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 811, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_n_u_jsdrv_unsubscribe_all};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 811, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 811, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_11, __pyx_t_5);
     __Pyx_INCREF(__pyx_n_u_jsdrv_unsubscribe_all);
     __Pyx_GIVEREF(__pyx_n_u_jsdrv_unsubscribe_all);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_11, __pyx_n_u_jsdrv_unsubscribe_all);
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 811, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":794
+  /* "pyjoulescope_driver/binding.pyx":796
  *         _handle_rc(rc, 'jsdrv_unsubscribe', topic)
  * 
  *     def unsubscribe_all(self, fn, timeout=None):             # <<<<<<<<<<<<<<
  *         """Unsubscribe a callback from all topics.
  * 
  */
 
@@ -11791,15 +11790,15 @@
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_t);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_f);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":811
+/* "pyjoulescope_driver/binding.pyx":813
  *         _handle_rc(rc, 'jsdrv_unsubscribe_all')
  * 
  *     def open(self, device_prefix, mode=None, timeout=None):             # <<<<<<<<<<<<<<
  *         """Open an attached device.
  * 
  */
 
@@ -11849,15 +11848,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 811, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 813, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -11868,15 +11867,15 @@
     }
     __pyx_v_device_prefix = values[0];
     __pyx_v_mode = values[1];
     __pyx_v_timeout = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 811, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 813, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_20open(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_device_prefix, __pyx_v_mode, __pyx_v_timeout);
 
@@ -11907,218 +11906,218 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
   __Pyx_INCREF(__pyx_v_device_prefix);
   __Pyx_INCREF(__pyx_v_mode);
 
-  /* "pyjoulescope_driver/binding.pyx":824
+  /* "pyjoulescope_driver/binding.pyx":826
  * 
  *         cdef const uint8_t[:] topic_str
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)             # <<<<<<<<<<<<<<
  *         cdef c_jsdrv.jsdrv_union_s v
  *         memset(&v, 0, sizeof(v))
  */
   __pyx_v_timeout_ms = __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(__pyx_v_timeout, NULL);
 
-  /* "pyjoulescope_driver/binding.pyx":826
+  /* "pyjoulescope_driver/binding.pyx":828
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)
  *         cdef c_jsdrv.jsdrv_union_s v
  *         memset(&v, 0, sizeof(v))             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(mode, str):
  */
   (void)(memset((&__pyx_v_v), 0, (sizeof(__pyx_v_v))));
 
-  /* "pyjoulescope_driver/binding.pyx":828
+  /* "pyjoulescope_driver/binding.pyx":830
  *         memset(&v, 0, sizeof(v))
  * 
  *         if isinstance(mode, str):             # <<<<<<<<<<<<<<
  *             mode = mode.lower()
  *         mode = _DEVICE_OPEN_MODES[mode]
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_mode); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "pyjoulescope_driver/binding.pyx":829
+    /* "pyjoulescope_driver/binding.pyx":831
  * 
  *         if isinstance(mode, str):
  *             mode = mode.lower()             # <<<<<<<<<<<<<<
  *         mode = _DEVICE_OPEN_MODES[mode]
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_lower); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 829, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_lower); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 831, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 829, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 831, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_mode, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "pyjoulescope_driver/binding.pyx":828
+    /* "pyjoulescope_driver/binding.pyx":830
  *         memset(&v, 0, sizeof(v))
  * 
  *         if isinstance(mode, str):             # <<<<<<<<<<<<<<
  *             mode = mode.lower()
  *         mode = _DEVICE_OPEN_MODES[mode]
  */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":830
+  /* "pyjoulescope_driver/binding.pyx":832
  *         if isinstance(mode, str):
  *             mode = mode.lower()
  *         mode = _DEVICE_OPEN_MODES[mode]             # <<<<<<<<<<<<<<
  * 
  *         while device_prefix[-1] == '/':
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DEVICE_OPEN_MODES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 830, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DEVICE_OPEN_MODES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 832, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_v_mode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 830, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_v_mode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 832, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_mode, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":832
+  /* "pyjoulescope_driver/binding.pyx":834
  *         mode = _DEVICE_OPEN_MODES[mode]
  * 
  *         while device_prefix[-1] == '/':             # <<<<<<<<<<<<<<
  *             device_prefix = device_prefix[:-1]
  *         topic = device_prefix + "/@/!open"
  */
   while (1) {
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_device_prefix, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 832, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_device_prefix, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 834, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_kp_u__12, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 832, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_kp_u__12, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 834, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (!__pyx_t_2) break;
 
-    /* "pyjoulescope_driver/binding.pyx":833
+    /* "pyjoulescope_driver/binding.pyx":835
  * 
  *         while device_prefix[-1] == '/':
  *             device_prefix = device_prefix[:-1]             # <<<<<<<<<<<<<<
  *         topic = device_prefix + "/@/!open"
  *         topic_str = topic.encode('utf-8')
  */
-    __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_device_prefix, 0, -1L, NULL, NULL, &__pyx_slice__13, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 833, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_device_prefix, 0, -1L, NULL, NULL, &__pyx_slice__13, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 835, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF_SET(__pyx_v_device_prefix, __pyx_t_4);
     __pyx_t_4 = 0;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":834
+  /* "pyjoulescope_driver/binding.pyx":836
  *         while device_prefix[-1] == '/':
  *             device_prefix = device_prefix[:-1]
  *         topic = device_prefix + "/@/!open"             # <<<<<<<<<<<<<<
  *         topic_str = topic.encode('utf-8')
  * 
  */
-  __pyx_t_4 = PyNumber_Add(__pyx_v_device_prefix, __pyx_kp_u_open); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 834, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Add(__pyx_v_device_prefix, __pyx_kp_u_open); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 836, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_topic = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":835
+  /* "pyjoulescope_driver/binding.pyx":837
  *             device_prefix = device_prefix[:-1]
  *         topic = device_prefix + "/@/!open"
  *         topic_str = topic.encode('utf-8')             # <<<<<<<<<<<<<<
  * 
  *         v.type = c_jsdrv.JSDRV_UNION_I32
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_topic, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 835, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_topic, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 835, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_4, 0); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 835, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_4, 0); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_topic_str = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "pyjoulescope_driver/binding.pyx":837
+  /* "pyjoulescope_driver/binding.pyx":839
  *         topic_str = topic.encode('utf-8')
  * 
  *         v.type = c_jsdrv.JSDRV_UNION_I32             # <<<<<<<<<<<<<<
  *         v.value.i32 = mode
  * 
  */
   __pyx_v_v.type = JSDRV_UNION_I32;
 
-  /* "pyjoulescope_driver/binding.pyx":838
+  /* "pyjoulescope_driver/binding.pyx":840
  * 
  *         v.type = c_jsdrv.JSDRV_UNION_I32
  *         v.value.i32 = mode             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __pyx_t_7 = __Pyx_PyInt_As_int32_t(__pyx_v_mode); if (unlikely((__pyx_t_7 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 838, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int32_t(__pyx_v_mode); if (unlikely((__pyx_t_7 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 840, __pyx_L1_error)
   __pyx_v_v.value.i32 = __pyx_t_7;
 
-  /* "pyjoulescope_driver/binding.pyx":840
+  /* "pyjoulescope_driver/binding.pyx":842
  *         v.value.i32 = mode
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms);
  *         _handle_rc(rc, 'jsdrv_open', device_prefix)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjoulescope_driver/binding.pyx":841
+        /* "pyjoulescope_driver/binding.pyx":843
  * 
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms);             # <<<<<<<<<<<<<<
  *         _handle_rc(rc, 'jsdrv_open', device_prefix)
  * 
  */
         __pyx_t_8 = 0;
         __pyx_t_9 = -1;
         if (__pyx_t_8 < 0) {
           __pyx_t_8 += __pyx_v_topic_str.shape[0];
           if (unlikely(__pyx_t_8 < 0)) __pyx_t_9 = 0;
         } else if (unlikely(__pyx_t_8 >= __pyx_v_topic_str.shape[0])) __pyx_t_9 = 0;
         if (unlikely(__pyx_t_9 != -1)) {
           __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_9);
-          __PYX_ERR(0, 841, __pyx_L7_error)
+          __PYX_ERR(0, 843, __pyx_L7_error)
         }
         __pyx_v_rc = jsdrv_publish(__pyx_v_self->_context, ((char *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_topic_str.data + __pyx_t_8 * __pyx_v_topic_str.strides[0]) ))))), (&__pyx_v_v), __pyx_v_timeout_ms);
       }
 
-      /* "pyjoulescope_driver/binding.pyx":840
+      /* "pyjoulescope_driver/binding.pyx":842
  *         v.value.i32 = mode
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms);
  *         _handle_rc(rc, 'jsdrv_open', device_prefix)
  */
       /*finally:*/ {
@@ -12136,24 +12135,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L8:;
       }
   }
 
-  /* "pyjoulescope_driver/binding.pyx":842
+  /* "pyjoulescope_driver/binding.pyx":844
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms);
  *         _handle_rc(rc, 'jsdrv_open', device_prefix)             # <<<<<<<<<<<<<<
  * 
  *     def close(self, device_prefix, timeout=None):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 842, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 844, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 842, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 844, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_10 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -12162,52 +12161,52 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_t_5, __pyx_n_u_jsdrv_open, __pyx_v_device_prefix};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 842, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 844, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_t_5, __pyx_n_u_jsdrv_open, __pyx_v_device_prefix};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 842, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 844, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_11 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 842, __pyx_L1_error)
+    __pyx_t_11 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 844, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     if (__pyx_t_10) {
       __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_10); __pyx_t_10 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_9, __pyx_t_5);
     __Pyx_INCREF(__pyx_n_u_jsdrv_open);
     __Pyx_GIVEREF(__pyx_n_u_jsdrv_open);
     PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_9, __pyx_n_u_jsdrv_open);
     __Pyx_INCREF(__pyx_v_device_prefix);
     __Pyx_GIVEREF(__pyx_v_device_prefix);
     PyTuple_SET_ITEM(__pyx_t_11, 2+__pyx_t_9, __pyx_v_device_prefix);
     __pyx_t_5 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_11, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 842, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_11, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 844, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":811
+  /* "pyjoulescope_driver/binding.pyx":813
  *         _handle_rc(rc, 'jsdrv_unsubscribe_all')
  * 
  *     def open(self, device_prefix, mode=None, timeout=None):             # <<<<<<<<<<<<<<
  *         """Open an attached device.
  * 
  */
 
@@ -12229,15 +12228,15 @@
   __Pyx_XDECREF(__pyx_v_device_prefix);
   __Pyx_XDECREF(__pyx_v_mode);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":844
+/* "pyjoulescope_driver/binding.pyx":846
  *         _handle_rc(rc, 'jsdrv_open', device_prefix)
  * 
  *     def close(self, device_prefix, timeout=None):             # <<<<<<<<<<<<<<
  *         """Close an attached device.
  * 
  */
 
@@ -12277,15 +12276,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "close") < 0)) __PYX_ERR(0, 844, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "close") < 0)) __PYX_ERR(0, 846, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -12293,15 +12292,15 @@
       }
     }
     __pyx_v_device_prefix = values[0];
     __pyx_v_timeout = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("close", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 844, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("close", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 846, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.close", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_19pyjoulescope_driver_7binding_6Driver_22close(((struct __pyx_obj_19pyjoulescope_driver_7binding_Driver *)__pyx_v_self), __pyx_v_device_prefix, __pyx_v_timeout);
 
@@ -12329,146 +12328,146 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
   __Pyx_INCREF(__pyx_v_device_prefix);
 
-  /* "pyjoulescope_driver/binding.pyx":851
+  /* "pyjoulescope_driver/binding.pyx":853
  *         """
  *         cdef const uint8_t[:] topic_str
  *         cdef int32_t timeout_ms = _timeout_validate(timeout)             # <<<<<<<<<<<<<<
  *         cdef c_jsdrv.jsdrv_union_s v
  * 
  */
   __pyx_v_timeout_ms = __pyx_f_19pyjoulescope_driver_7binding__timeout_validate(__pyx_v_timeout, NULL);
 
-  /* "pyjoulescope_driver/binding.pyx":854
+  /* "pyjoulescope_driver/binding.pyx":856
  *         cdef c_jsdrv.jsdrv_union_s v
  * 
  *         while device_prefix[-1] == '/':             # <<<<<<<<<<<<<<
  *             device_prefix = device_prefix[:-1]
  *         topic = device_prefix + "/@/!close"
  */
   while (1) {
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_device_prefix, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 854, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_device_prefix, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 856, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u__12, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 854, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u__12, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 856, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!__pyx_t_2) break;
 
-    /* "pyjoulescope_driver/binding.pyx":855
+    /* "pyjoulescope_driver/binding.pyx":857
  * 
  *         while device_prefix[-1] == '/':
  *             device_prefix = device_prefix[:-1]             # <<<<<<<<<<<<<<
  *         topic = device_prefix + "/@/!close"
  *         topic_str = topic.encode('utf-8')
  */
-    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_device_prefix, 0, -1L, NULL, NULL, &__pyx_slice__13, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 855, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_device_prefix, 0, -1L, NULL, NULL, &__pyx_slice__13, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 857, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_device_prefix, __pyx_t_1);
     __pyx_t_1 = 0;
   }
 
-  /* "pyjoulescope_driver/binding.pyx":856
+  /* "pyjoulescope_driver/binding.pyx":858
  *         while device_prefix[-1] == '/':
  *             device_prefix = device_prefix[:-1]
  *         topic = device_prefix + "/@/!close"             # <<<<<<<<<<<<<<
  *         topic_str = topic.encode('utf-8')
  *         v.type = c_jsdrv.JSDRV_UNION_I32
  */
-  __pyx_t_1 = PyNumber_Add(__pyx_v_device_prefix, __pyx_kp_u_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 856, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_device_prefix, __pyx_kp_u_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 858, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_topic = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":857
+  /* "pyjoulescope_driver/binding.pyx":859
  *             device_prefix = device_prefix[:-1]
  *         topic = device_prefix + "/@/!close"
  *         topic_str = topic.encode('utf-8')             # <<<<<<<<<<<<<<
  *         v.type = c_jsdrv.JSDRV_UNION_I32
  *         v.value.i32 = 0
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_topic, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 857, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_topic, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 859, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 857, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 859, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 857, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 859, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_topic_str = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
-  /* "pyjoulescope_driver/binding.pyx":858
+  /* "pyjoulescope_driver/binding.pyx":860
  *         topic = device_prefix + "/@/!close"
  *         topic_str = topic.encode('utf-8')
  *         v.type = c_jsdrv.JSDRV_UNION_I32             # <<<<<<<<<<<<<<
  *         v.value.i32 = 0
  *         with nogil:
  */
   __pyx_v_v.type = JSDRV_UNION_I32;
 
-  /* "pyjoulescope_driver/binding.pyx":859
+  /* "pyjoulescope_driver/binding.pyx":861
  *         topic_str = topic.encode('utf-8')
  *         v.type = c_jsdrv.JSDRV_UNION_I32
  *         v.value.i32 = 0             # <<<<<<<<<<<<<<
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms);
  */
   __pyx_v_v.value.i32 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":860
+  /* "pyjoulescope_driver/binding.pyx":862
  *         v.type = c_jsdrv.JSDRV_UNION_I32
  *         v.value.i32 = 0
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms);
  *         _handle_rc(rc, 'jsdrv_close', device_prefix)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjoulescope_driver/binding.pyx":861
+        /* "pyjoulescope_driver/binding.pyx":863
  *         v.value.i32 = 0
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms);             # <<<<<<<<<<<<<<
  *         _handle_rc(rc, 'jsdrv_close', device_prefix)
  * 
  */
         __pyx_t_6 = 0;
         __pyx_t_7 = -1;
         if (__pyx_t_6 < 0) {
           __pyx_t_6 += __pyx_v_topic_str.shape[0];
           if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
         } else if (unlikely(__pyx_t_6 >= __pyx_v_topic_str.shape[0])) __pyx_t_7 = 0;
         if (unlikely(__pyx_t_7 != -1)) {
           __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_7);
-          __PYX_ERR(0, 861, __pyx_L6_error)
+          __PYX_ERR(0, 863, __pyx_L6_error)
         }
         __pyx_v_rc = jsdrv_publish(__pyx_v_self->_context, ((char *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_topic_str.data + __pyx_t_6 * __pyx_v_topic_str.strides[0]) ))))), (&__pyx_v_v), __pyx_v_timeout_ms);
       }
 
-      /* "pyjoulescope_driver/binding.pyx":860
+      /* "pyjoulescope_driver/binding.pyx":862
  *         v.type = c_jsdrv.JSDRV_UNION_I32
  *         v.value.i32 = 0
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms);
  *         _handle_rc(rc, 'jsdrv_close', device_prefix)
  */
       /*finally:*/ {
@@ -12486,24 +12485,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L7:;
       }
   }
 
-  /* "pyjoulescope_driver/binding.pyx":862
+  /* "pyjoulescope_driver/binding.pyx":864
  *         with nogil:
  *             rc = c_jsdrv.jsdrv_publish(self._context, <char *> &topic_str[0], &v, timeout_ms);
  *         _handle_rc(rc, 'jsdrv_close', device_prefix)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 862, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 864, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 862, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 864, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_8 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -12512,52 +12511,52 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_t_4, __pyx_n_u_jsdrv_close, __pyx_v_device_prefix};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 862, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_t_4, __pyx_n_u_jsdrv_close, __pyx_v_device_prefix};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 862, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 862, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 864, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_8) {
       __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_8); __pyx_t_8 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_7, __pyx_t_4);
     __Pyx_INCREF(__pyx_n_u_jsdrv_close);
     __Pyx_GIVEREF(__pyx_n_u_jsdrv_close);
     PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_7, __pyx_n_u_jsdrv_close);
     __Pyx_INCREF(__pyx_v_device_prefix);
     __Pyx_GIVEREF(__pyx_v_device_prefix);
     PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_7, __pyx_v_device_prefix);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 862, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":844
+  /* "pyjoulescope_driver/binding.pyx":846
  *         _handle_rc(rc, 'jsdrv_open', device_prefix)
  * 
  *     def close(self, device_prefix, timeout=None):             # <<<<<<<<<<<<<<
  *         """Close an attached device.
  * 
  */
 
@@ -12691,23 +12690,23 @@
   __Pyx_AddTraceback("pyjoulescope_driver.binding.Driver.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjoulescope_driver/binding.pyx":865
+/* "pyjoulescope_driver/binding.pyx":867
  * 
  * 
- * cdef void _on_cmd_publish2_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) with gil:             # <<<<<<<<<<<<<<
+ * cdef void _on_cmd_publish_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) with gil:             # <<<<<<<<<<<<<<
  *     cdef object fn = <object> user_data
  *     topic_str = topic.decode('utf-8')
  */
 
-static void __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish2_cbk(void *__pyx_v_user_data, char const *__pyx_v_topic, struct jsdrv_union_s const *__pyx_v_value) {
+static void __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish_cbk(void *__pyx_v_user_data, char const *__pyx_v_topic, struct jsdrv_union_s const *__pyx_v_value) {
   PyObject *__pyx_v_fn = 0;
   PyObject *__pyx_v_topic_str = NULL;
   PyObject *__pyx_v_v = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -12715,53 +12714,53 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("_on_cmd_publish2_cbk", 0);
+  __Pyx_RefNannySetupContext("_on_cmd_publish_cbk", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":866
+  /* "pyjoulescope_driver/binding.pyx":868
  * 
- * cdef void _on_cmd_publish2_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) with gil:
+ * cdef void _on_cmd_publish_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) with gil:
  *     cdef object fn = <object> user_data             # <<<<<<<<<<<<<<
  *     topic_str = topic.decode('utf-8')
  *     v = _jsdrv_union_to_py(value)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_user_data);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_fn = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":867
- * cdef void _on_cmd_publish2_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) with gil:
+  /* "pyjoulescope_driver/binding.pyx":869
+ * cdef void _on_cmd_publish_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) with gil:
  *     cdef object fn = <object> user_data
  *     topic_str = topic.decode('utf-8')             # <<<<<<<<<<<<<<
  *     v = _jsdrv_union_to_py(value)
  *     # print(f'{topic_str} = {v}')
  */
-  __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_topic, 0, strlen(__pyx_v_topic), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 867, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_topic, 0, strlen(__pyx_v_topic), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 869, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_topic_str = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":868
+  /* "pyjoulescope_driver/binding.pyx":870
  *     cdef object fn = <object> user_data
  *     topic_str = topic.decode('utf-8')
  *     v = _jsdrv_union_to_py(value)             # <<<<<<<<<<<<<<
  *     # print(f'{topic_str} = {v}')
  *     fn(topic_str, v)
  */
-  __pyx_t_1 = __pyx_f_19pyjoulescope_driver_7binding__jsdrv_union_to_py(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 868, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_19pyjoulescope_driver_7binding__jsdrv_union_to_py(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 870, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_v = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":870
+  /* "pyjoulescope_driver/binding.pyx":872
  *     v = _jsdrv_union_to_py(value)
  *     # print(f'{topic_str} = {v}')
  *     fn(topic_str, v)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_INCREF(__pyx_v_fn);
@@ -12776,108 +12775,78 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_topic_str, __pyx_v_v};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 870, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 872, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_topic_str, __pyx_v_v};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 870, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 872, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 870, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 872, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_topic_str);
     __Pyx_GIVEREF(__pyx_v_topic_str);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_topic_str);
     __Pyx_INCREF(__pyx_v_v);
     __Pyx_GIVEREF(__pyx_v_v);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_v);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 870, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 872, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":865
+  /* "pyjoulescope_driver/binding.pyx":867
  * 
  * 
- * cdef void _on_cmd_publish2_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) with gil:             # <<<<<<<<<<<<<<
+ * cdef void _on_cmd_publish_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) with gil:             # <<<<<<<<<<<<<<
  *     cdef object fn = <object> user_data
  *     topic_str = topic.decode('utf-8')
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_WriteUnraisable("pyjoulescope_driver.binding._on_cmd_publish2_cbk", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("pyjoulescope_driver.binding._on_cmd_publish_cbk", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_fn);
   __Pyx_XDECREF(__pyx_v_topic_str);
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "pyjoulescope_driver/binding.pyx":873
- * 
- * 
- * cdef void _on_cmd_publish1_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) nogil:             # <<<<<<<<<<<<<<
- *     _on_cmd_publish2_cbk(user_data, topic, value)
- * 
- */
-
-static void __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish1_cbk(void *__pyx_v_user_data, char const *__pyx_v_topic, struct jsdrv_union_s const *__pyx_v_value) {
-
-  /* "pyjoulescope_driver/binding.pyx":874
- * 
- * cdef void _on_cmd_publish1_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) nogil:
- *     _on_cmd_publish2_cbk(user_data, topic, value)             # <<<<<<<<<<<<<<
- * 
- * # https://cython.readthedocs.io/en/latest/src/userguide/external_C_code.html#acquiring-and-releasing-the-gil
- */
-  __pyx_f_19pyjoulescope_driver_7binding__on_cmd_publish2_cbk(__pyx_v_user_data, __pyx_v_topic, __pyx_v_value);
-
-  /* "pyjoulescope_driver/binding.pyx":873
- * 
- * 
- * cdef void _on_cmd_publish1_cbk(void * user_data, const char * topic, const c_jsdrv.jsdrv_union_s * value) nogil:             # <<<<<<<<<<<<<<
- *     _on_cmd_publish2_cbk(user_data, topic, value)
+/* "pyjoulescope_driver/binding.pyx":875
  * 
- */
-
-  /* function exit code */
-}
-
-/* "pyjoulescope_driver/binding.pyx":877
  * 
- * # https://cython.readthedocs.io/en/latest/src/userguide/external_C_code.html#acquiring-and-releasing-the-gil
  * cdef void _on_log_recv(void * user_data, const c_jsdrv.jsdrv_log_header_s * header,             # <<<<<<<<<<<<<<
- *                        const char * filename, const char * message) nogil:
- *     with gil:
+ *                        const char * filename, const char * message) with gil:
+ *     fname = filename.decode('utf-8')
  */
 
 static void __pyx_f_19pyjoulescope_driver_7binding__on_log_recv(CYTHON_UNUSED void *__pyx_v_user_data, struct jsdrv_log_header_s const *__pyx_v_header, char const *__pyx_v_filename, char const *__pyx_v_message) {
   PyObject *__pyx_v_fname = NULL;
   PyObject *__pyx_v_msg = NULL;
   PyObject *__pyx_v_lvl = NULL;
   PyObject *__pyx_v_record = NULL;
@@ -12891,295 +12860,241 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
-  PyGILState_STATE __pyx_gilstate_save;
+  PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("_on_log_recv", 1);
+  __Pyx_RefNannySetupContext("_on_log_recv", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":879
+  /* "pyjoulescope_driver/binding.pyx":877
  * cdef void _on_log_recv(void * user_data, const c_jsdrv.jsdrv_log_header_s * header,
- *                        const char * filename, const char * message) nogil:
- *     with gil:             # <<<<<<<<<<<<<<
- *         fname = filename.decode('utf-8')
- *         msg = message.decode('utf-8')
+ *                        const char * filename, const char * message) with gil:
+ *     fname = filename.decode('utf-8')             # <<<<<<<<<<<<<<
+ *     msg = message.decode('utf-8')
+ *     lvl = _log_level_c_to_py[header[0].level]
  */
-  /*try:*/ {
-    {
-        #ifdef WITH_THREAD
-        PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
-        #endif
-        /*try:*/ {
+  __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_filename, 0, strlen(__pyx_v_filename), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 877, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_fname = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-          /* "pyjoulescope_driver/binding.pyx":880
- *                        const char * filename, const char * message) nogil:
- *     with gil:
- *         fname = filename.decode('utf-8')             # <<<<<<<<<<<<<<
- *         msg = message.decode('utf-8')
- *         lvl = _log_level_c_to_py[header[0].level]
- */
-          __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_filename, 0, strlen(__pyx_v_filename), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 880, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          __pyx_v_fname = __pyx_t_1;
-          __pyx_t_1 = 0;
-
-          /* "pyjoulescope_driver/binding.pyx":881
- *     with gil:
- *         fname = filename.decode('utf-8')
- *         msg = message.decode('utf-8')             # <<<<<<<<<<<<<<
- *         lvl = _log_level_c_to_py[header[0].level]
- *         if _log_c.isEnabledFor(lvl):
- */
-          __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_message, 0, strlen(__pyx_v_message), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 881, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          __pyx_v_msg = __pyx_t_1;
-          __pyx_t_1 = 0;
-
-          /* "pyjoulescope_driver/binding.pyx":882
- *         fname = filename.decode('utf-8')
- *         msg = message.decode('utf-8')
- *         lvl = _log_level_c_to_py[header[0].level]             # <<<<<<<<<<<<<<
- *         if _log_c.isEnabledFor(lvl):
- *             record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)
- */
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log_level_c_to_py); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, (__pyx_v_header[0]).level, uint8_t const , 0, __Pyx_PyInt_From_uint8_t, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 882, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_v_lvl = __pyx_t_2;
-          __pyx_t_2 = 0;
-
-          /* "pyjoulescope_driver/binding.pyx":883
- *         msg = message.decode('utf-8')
- *         lvl = _log_level_c_to_py[header[0].level]
- *         if _log_c.isEnabledFor(lvl):             # <<<<<<<<<<<<<<
- *             record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)
- *             _log_c.handle(record)
- */
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 883, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_isEnabledFor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 883, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = NULL;
-          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-            __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
-            if (likely(__pyx_t_1)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-              __Pyx_INCREF(__pyx_t_1);
-              __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_3, function);
-            }
-          }
-          __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_lvl) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_lvl);
-          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 883, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 883, __pyx_L7_error)
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (__pyx_t_4) {
-
-            /* "pyjoulescope_driver/binding.pyx":884
- *         lvl = _log_level_c_to_py[header[0].level]
- *         if _log_c.isEnabledFor(lvl):
- *             record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)             # <<<<<<<<<<<<<<
- *             _log_c.handle(record)
- */
-            __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_log_c); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 884, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_3);
-            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_makeRecord); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 884, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_1);
-            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-            __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_log_c_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 884, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_3);
-            __pyx_t_5 = __Pyx_PyInt_From_uint32_t((__pyx_v_header[0]).line); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 884, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_5);
-            __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 884, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_6);
-            __pyx_t_7 = NULL;
-            __pyx_t_8 = 0;
-            if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-              __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
-              if (likely(__pyx_t_7)) {
-                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-                __Pyx_INCREF(__pyx_t_7);
-                __Pyx_INCREF(function);
-                __Pyx_DECREF_SET(__pyx_t_1, function);
-                __pyx_t_8 = 1;
-              }
-            }
-            #if CYTHON_FAST_PYCALL
-            if (PyFunction_Check(__pyx_t_1)) {
-              PyObject *__pyx_temp[8] = {__pyx_t_7, __pyx_t_3, __pyx_v_lvl, __pyx_v_fname, __pyx_t_5, __pyx_v_msg, __pyx_t_6, Py_None};
-              __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 7+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 884, __pyx_L7_error)
-              __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-              __Pyx_GOTREF(__pyx_t_2);
-              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-              __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-            } else
-            #endif
-            #if CYTHON_FAST_PYCCALL
-            if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-              PyObject *__pyx_temp[8] = {__pyx_t_7, __pyx_t_3, __pyx_v_lvl, __pyx_v_fname, __pyx_t_5, __pyx_v_msg, __pyx_t_6, Py_None};
-              __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 7+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 884, __pyx_L7_error)
-              __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-              __Pyx_GOTREF(__pyx_t_2);
-              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-              __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-            } else
-            #endif
-            {
-              __pyx_t_9 = PyTuple_New(7+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 884, __pyx_L7_error)
-              __Pyx_GOTREF(__pyx_t_9);
-              if (__pyx_t_7) {
-                __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
-              }
-              __Pyx_GIVEREF(__pyx_t_3);
-              PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_3);
-              __Pyx_INCREF(__pyx_v_lvl);
-              __Pyx_GIVEREF(__pyx_v_lvl);
-              PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_lvl);
-              __Pyx_INCREF(__pyx_v_fname);
-              __Pyx_GIVEREF(__pyx_v_fname);
-              PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_v_fname);
-              __Pyx_GIVEREF(__pyx_t_5);
-              PyTuple_SET_ITEM(__pyx_t_9, 3+__pyx_t_8, __pyx_t_5);
-              __Pyx_INCREF(__pyx_v_msg);
-              __Pyx_GIVEREF(__pyx_v_msg);
-              PyTuple_SET_ITEM(__pyx_t_9, 4+__pyx_t_8, __pyx_v_msg);
-              __Pyx_GIVEREF(__pyx_t_6);
-              PyTuple_SET_ITEM(__pyx_t_9, 5+__pyx_t_8, __pyx_t_6);
-              __Pyx_INCREF(Py_None);
-              __Pyx_GIVEREF(Py_None);
-              PyTuple_SET_ITEM(__pyx_t_9, 6+__pyx_t_8, Py_None);
-              __pyx_t_3 = 0;
-              __pyx_t_5 = 0;
-              __pyx_t_6 = 0;
-              __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 884, __pyx_L7_error)
-              __Pyx_GOTREF(__pyx_t_2);
-              __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-            }
-            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __pyx_v_record = __pyx_t_2;
-            __pyx_t_2 = 0;
-
-            /* "pyjoulescope_driver/binding.pyx":885
- *         if _log_c.isEnabledFor(lvl):
- *             record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)
- *             _log_c.handle(record)             # <<<<<<<<<<<<<<
- */
-            __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 885, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_handle); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 885, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_9);
-            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __pyx_t_1 = NULL;
-            if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-              __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_9);
-              if (likely(__pyx_t_1)) {
-                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-                __Pyx_INCREF(__pyx_t_1);
-                __Pyx_INCREF(function);
-                __Pyx_DECREF_SET(__pyx_t_9, function);
-              }
-            }
-            __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_1, __pyx_v_record) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_record);
-            __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 885, __pyx_L7_error)
-            __Pyx_GOTREF(__pyx_t_2);
-            __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-            /* "pyjoulescope_driver/binding.pyx":883
- *         msg = message.decode('utf-8')
- *         lvl = _log_level_c_to_py[header[0].level]
- *         if _log_c.isEnabledFor(lvl):             # <<<<<<<<<<<<<<
- *             record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)
- *             _log_c.handle(record)
+  /* "pyjoulescope_driver/binding.pyx":878
+ *                        const char * filename, const char * message) with gil:
+ *     fname = filename.decode('utf-8')
+ *     msg = message.decode('utf-8')             # <<<<<<<<<<<<<<
+ *     lvl = _log_level_c_to_py[header[0].level]
+ *     if _log_c.isEnabledFor(lvl):
  */
-          }
-        }
+  __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_message, 0, strlen(__pyx_v_message), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 878, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_msg = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-        /* "pyjoulescope_driver/binding.pyx":879
- * cdef void _on_log_recv(void * user_data, const c_jsdrv.jsdrv_log_header_s * header,
- *                        const char * filename, const char * message) nogil:
- *     with gil:             # <<<<<<<<<<<<<<
- *         fname = filename.decode('utf-8')
- *         msg = message.decode('utf-8')
- */
-        /*finally:*/ {
-          /*normal exit:*/{
-            #ifdef WITH_THREAD
-            __Pyx_PyGILState_Release(__pyx_gilstate_save);
-            #endif
-            goto __pyx_L8;
-          }
-          __pyx_L7_error: {
-            #ifdef WITH_THREAD
-            __Pyx_PyGILState_Release(__pyx_gilstate_save);
-            #endif
-            goto __pyx_L4_error;
-          }
-          __pyx_L8:;
-        }
+  /* "pyjoulescope_driver/binding.pyx":879
+ *     fname = filename.decode('utf-8')
+ *     msg = message.decode('utf-8')
+ *     lvl = _log_level_c_to_py[header[0].level]             # <<<<<<<<<<<<<<
+ *     if _log_c.isEnabledFor(lvl):
+ *         record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log_level_c_to_py); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 879, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, (__pyx_v_header[0]).level, uint8_t const , 0, __Pyx_PyInt_From_uint8_t, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 879, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_lvl = __pyx_t_2;
+  __pyx_t_2 = 0;
+
+  /* "pyjoulescope_driver/binding.pyx":880
+ *     msg = message.decode('utf-8')
+ *     lvl = _log_level_c_to_py[header[0].level]
+ *     if _log_c.isEnabledFor(lvl):             # <<<<<<<<<<<<<<
+ *         record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)
+ *         _log_c.handle(record)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 880, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_isEnabledFor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 880, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  /*finally:*/ {
-    /*normal exit:*/{
-      #ifdef WITH_THREAD
-      __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
-      #endif
-      goto __pyx_L5;
+  __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_lvl) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_lvl);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 880, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 880, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__pyx_t_4) {
+
+    /* "pyjoulescope_driver/binding.pyx":881
+ *     lvl = _log_level_c_to_py[header[0].level]
+ *     if _log_c.isEnabledFor(lvl):
+ *         record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)             # <<<<<<<<<<<<<<
+ *         _log_c.handle(record)
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_log_c); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 881, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_makeRecord); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 881, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_log_c_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 881, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = __Pyx_PyInt_From_uint32_t((__pyx_v_header[0]).line); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 881, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 881, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = NULL;
+    __pyx_t_8 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
+        __pyx_t_8 = 1;
+      }
     }
-    __pyx_L4_error: {
-      #ifdef WITH_THREAD
-      __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
-      #endif
-      goto __pyx_L1_error;
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(__pyx_t_1)) {
+      PyObject *__pyx_temp[8] = {__pyx_t_7, __pyx_t_3, __pyx_v_lvl, __pyx_v_fname, __pyx_t_5, __pyx_v_msg, __pyx_t_6, Py_None};
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 7+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    } else
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
+      PyObject *__pyx_temp[8] = {__pyx_t_7, __pyx_t_3, __pyx_v_lvl, __pyx_v_fname, __pyx_t_5, __pyx_v_msg, __pyx_t_6, Py_None};
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 7+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    } else
+    #endif
+    {
+      __pyx_t_9 = PyTuple_New(7+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 881, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      if (__pyx_t_7) {
+        __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
+      }
+      __Pyx_GIVEREF(__pyx_t_3);
+      PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_3);
+      __Pyx_INCREF(__pyx_v_lvl);
+      __Pyx_GIVEREF(__pyx_v_lvl);
+      PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_lvl);
+      __Pyx_INCREF(__pyx_v_fname);
+      __Pyx_GIVEREF(__pyx_v_fname);
+      PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_v_fname);
+      __Pyx_GIVEREF(__pyx_t_5);
+      PyTuple_SET_ITEM(__pyx_t_9, 3+__pyx_t_8, __pyx_t_5);
+      __Pyx_INCREF(__pyx_v_msg);
+      __Pyx_GIVEREF(__pyx_v_msg);
+      PyTuple_SET_ITEM(__pyx_t_9, 4+__pyx_t_8, __pyx_v_msg);
+      __Pyx_GIVEREF(__pyx_t_6);
+      PyTuple_SET_ITEM(__pyx_t_9, 5+__pyx_t_8, __pyx_t_6);
+      __Pyx_INCREF(Py_None);
+      __Pyx_GIVEREF(Py_None);
+      PyTuple_SET_ITEM(__pyx_t_9, 6+__pyx_t_8, Py_None);
+      __pyx_t_3 = 0;
+      __pyx_t_5 = 0;
+      __pyx_t_6 = 0;
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
-    __pyx_L5:;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_v_record = __pyx_t_2;
+    __pyx_t_2 = 0;
+
+    /* "pyjoulescope_driver/binding.pyx":882
+ *     if _log_c.isEnabledFor(lvl):
+ *         record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)
+ *         _log_c.handle(record)             # <<<<<<<<<<<<<<
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_handle); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 882, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_9);
+      if (likely(__pyx_t_1)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+        __Pyx_INCREF(__pyx_t_1);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_9, function);
+      }
+    }
+    __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_1, __pyx_v_record) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_record);
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 882, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "pyjoulescope_driver/binding.pyx":880
+ *     msg = message.decode('utf-8')
+ *     lvl = _log_level_c_to_py[header[0].level]
+ *     if _log_c.isEnabledFor(lvl):             # <<<<<<<<<<<<<<
+ *         record = _log_c.makeRecord(_log_c_name, lvl, fname, header[0].line, msg, [], None)
+ *         _log_c.handle(record)
+ */
   }
 
-  /* "pyjoulescope_driver/binding.pyx":877
+  /* "pyjoulescope_driver/binding.pyx":875
+ * 
  * 
- * # https://cython.readthedocs.io/en/latest/src/userguide/external_C_code.html#acquiring-and-releasing-the-gil
  * cdef void _on_log_recv(void * user_data, const c_jsdrv.jsdrv_log_header_s * header,             # <<<<<<<<<<<<<<
- *                        const char * filename, const char * message) nogil:
- *     with gil:
+ *                        const char * filename, const char * message) with gil:
+ *     fname = filename.decode('utf-8')
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_WriteUnraisable("pyjoulescope_driver.binding._on_log_recv", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
+  __Pyx_WriteUnraisable("pyjoulescope_driver.binding._on_log_recv", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_fname);
   __Pyx_XDECREF(__pyx_v_msg);
   __Pyx_XDECREF(__pyx_v_lvl);
   __Pyx_XDECREF(__pyx_v_record);
+  __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":734
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13188,29 +13103,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13221,15 +13136,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":737
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13238,29 +13153,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13271,15 +13186,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":740
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13288,29 +13203,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13321,15 +13236,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":743
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13338,29 +13253,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13371,15 +13286,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":746
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13388,29 +13303,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13421,212 +13336,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":749
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":928
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":932
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":934
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":936
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":940
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13642,15 +13557,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -13658,53 +13573,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":941
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":943
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":944
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -13712,30 +13627,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":940
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -13750,15 +13665,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":946
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13774,15 +13689,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13790,53 +13705,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":947
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":949
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":950
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -13844,30 +13759,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":946
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13882,15 +13797,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":952
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -13906,15 +13821,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -13922,53 +13837,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":953
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":955
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":956
+      /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -13976,30 +13891,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":952
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14014,176 +13929,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":966
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":978
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":966
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":981
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":993
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":981
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":996
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":996
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1006
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1013
+/* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -28576,18 +28491,18 @@
   {&__pyx_n_u_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 1, 0, 1},
   {&__pyx_n_u_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 1, 0, 1},
   {&__pyx_n_u_warning, __pyx_k_warning, sizeof(__pyx_k_warning), 0, 1, 0, 1},
   {&__pyx_n_u_z, __pyx_k_z, sizeof(__pyx_k_z), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 186, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 251, __pyx_L1_error)
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 256, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 588, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 944, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
@@ -28596,66 +28511,66 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "pyjoulescope_driver/binding.pyx":178
+  /* "pyjoulescope_driver/binding.pyx":180
  *         s.time_type = c_jsdrv.JSDRV_TIME_UTC
  *         s.time.utc.start = r['start']
  *         s.time.utc.end = r.get('end', 0)             # <<<<<<<<<<<<<<
  *         s.time.utc.length = r.get('length', 0)
  *     elif time_type == 'samples':
  */
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_end, __pyx_int_0); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_end, __pyx_int_0); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "pyjoulescope_driver/binding.pyx":179
+  /* "pyjoulescope_driver/binding.pyx":181
  *         s.time.utc.start = r['start']
  *         s.time.utc.end = r.get('end', 0)
  *         s.time.utc.length = r.get('length', 0)             # <<<<<<<<<<<<<<
  *     elif time_type == 'samples':
  *         s.time_type = c_jsdrv.JSDRV_TIME_SAMPLES
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_length, __pyx_int_0); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_length, __pyx_int_0); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "pyjoulescope_driver/binding.pyx":256
+  /* "pyjoulescope_driver/binding.pyx":258
  *                     v['data'] = ndarray
  *                 else:
  *                     print('jsdrv._jsdrv_union_to_py: unsupported data type')             # <<<<<<<<<<<<<<
  *                     v['data'] = None
  *             elif value[0].app == c_jsdrv.JSDRV_PAYLOAD_TYPE_STATISTICS:
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_jsdrv__jsdrv_union_to_py_unsuppo); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_jsdrv__jsdrv_union_to_py_unsuppo); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "pyjoulescope_driver/binding.pyx":462
+  /* "pyjoulescope_driver/binding.pyx":464
  *     :return: The error code's name
  *     """
  *     v, name, rv = _error_code_to_meta.get(ec, (-1, "unknown", "unknown"))             # <<<<<<<<<<<<<<
  *     return f'{v} {name} : {rv}'
  * 
  */
-  __pyx_tuple__6 = PyTuple_Pack(3, __pyx_int_neg_1, __pyx_n_u_unknown, __pyx_n_u_unknown); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 462, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(3, __pyx_int_neg_1, __pyx_n_u_unknown, __pyx_n_u_unknown); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "pyjoulescope_driver/binding.pyx":833
+  /* "pyjoulescope_driver/binding.pyx":835
  * 
  *         while device_prefix[-1] == '/':
  *             device_prefix = device_prefix[:-1]             # <<<<<<<<<<<<<<
  *         topic = device_prefix + "/@/!open"
  *         topic_str = topic.encode('utf-8')
  */
-  __pyx_slice__13 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__13)) __PYX_ERR(0, 833, __pyx_L1_error)
+  __pyx_slice__13 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__13)) __PYX_ERR(0, 835, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__13);
   __Pyx_GIVEREF(__pyx_slice__13);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._context cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -28670,26 +28585,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._context cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_self__context_cannot_be_converte); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "../../../bin/Python3_11_2/Lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../bin/Python3_10_11/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -28887,335 +28802,335 @@
   __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
   __pyx_tuple__36 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
 
-  /* "pyjoulescope_driver/binding.pyx":400
+  /* "pyjoulescope_driver/binding.pyx":402
  *     # automatically maintained by error_code_update.py
  *     # ENUM_ERROR_CODE_META_START
  *     0: (0, 'SUCCESS', 'Success (no error)'),             # <<<<<<<<<<<<<<
  *     1: (1, 'UNSPECIFIED', 'Unspecified error'),
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  */
-  __pyx_tuple__39 = PyTuple_Pack(3, __pyx_int_0, __pyx_n_u_SUCCESS, __pyx_kp_u_Success_no_error); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(3, __pyx_int_0, __pyx_n_u_SUCCESS, __pyx_kp_u_Success_no_error); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
 
-  /* "pyjoulescope_driver/binding.pyx":401
+  /* "pyjoulescope_driver/binding.pyx":403
  *     # ENUM_ERROR_CODE_META_START
  *     0: (0, 'SUCCESS', 'Success (no error)'),
  *     1: (1, 'UNSPECIFIED', 'Unspecified error'),             # <<<<<<<<<<<<<<
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  */
-  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_int_1, __pyx_n_u_UNSPECIFIED, __pyx_kp_u_Unspecified_error); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_int_1, __pyx_n_u_UNSPECIFIED, __pyx_kp_u_Unspecified_error); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
 
-  /* "pyjoulescope_driver/binding.pyx":402
+  /* "pyjoulescope_driver/binding.pyx":404
  *     0: (0, 'SUCCESS', 'Success (no error)'),
  *     1: (1, 'UNSPECIFIED', 'Unspecified error'),
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),             # <<<<<<<<<<<<<<
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  *     4: (4, 'IO', 'Input/output error'),
  */
-  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_int_2, __pyx_n_u_NOT_ENOUGH_MEMORY, __pyx_kp_u_Insufficient_memory_to_complete); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_int_2, __pyx_n_u_NOT_ENOUGH_MEMORY, __pyx_kp_u_Insufficient_memory_to_complete); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
 
-  /* "pyjoulescope_driver/binding.pyx":403
+  /* "pyjoulescope_driver/binding.pyx":405
  *     1: (1, 'UNSPECIFIED', 'Unspecified error'),
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),             # <<<<<<<<<<<<<<
  *     4: (4, 'IO', 'Input/output error'),
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  */
-  __pyx_tuple__42 = PyTuple_Pack(3, __pyx_int_3, __pyx_n_u_NOT_SUPPORTED, __pyx_kp_u_Operation_is_not_supported); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_tuple__42 = PyTuple_Pack(3, __pyx_int_3, __pyx_n_u_NOT_SUPPORTED, __pyx_kp_u_Operation_is_not_supported); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__42);
   __Pyx_GIVEREF(__pyx_tuple__42);
 
-  /* "pyjoulescope_driver/binding.pyx":404
+  /* "pyjoulescope_driver/binding.pyx":406
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  *     4: (4, 'IO', 'Input/output error'),             # <<<<<<<<<<<<<<
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  */
-  __pyx_tuple__43 = PyTuple_Pack(3, __pyx_int_4, __pyx_n_u_IO, __pyx_kp_u_Input_output_error); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(3, __pyx_int_4, __pyx_n_u_IO, __pyx_kp_u_Input_output_error); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
 
-  /* "pyjoulescope_driver/binding.pyx":405
+  /* "pyjoulescope_driver/binding.pyx":407
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  *     4: (4, 'IO', 'Input/output error'),
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),             # <<<<<<<<<<<<<<
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),
  */
-  __pyx_tuple__44 = PyTuple_Pack(3, __pyx_int_5, __pyx_n_u_PARAMETER_INVALID, __pyx_kp_u_The_parameter_value_is_invalid); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_tuple__44 = PyTuple_Pack(3, __pyx_int_5, __pyx_n_u_PARAMETER_INVALID, __pyx_kp_u_The_parameter_value_is_invalid); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__44);
   __Pyx_GIVEREF(__pyx_tuple__44);
 
-  /* "pyjoulescope_driver/binding.pyx":406
+  /* "pyjoulescope_driver/binding.pyx":408
  *     4: (4, 'IO', 'Input/output error'),
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),             # <<<<<<<<<<<<<<
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  */
-  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_int_6, __pyx_n_u_INVALID_RETURN_CONDITION, __pyx_kp_u_The_function_return_condition_is); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_int_6, __pyx_n_u_INVALID_RETURN_CONDITION, __pyx_kp_u_The_function_return_condition_is); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
 
-  /* "pyjoulescope_driver/binding.pyx":407
+  /* "pyjoulescope_driver/binding.pyx":409
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),             # <<<<<<<<<<<<<<
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  */
-  __pyx_tuple__46 = PyTuple_Pack(3, __pyx_int_7, __pyx_n_u_INVALID_CONTEXT, __pyx_kp_u_The_context_is_invalid); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_tuple__46 = PyTuple_Pack(3, __pyx_int_7, __pyx_n_u_INVALID_CONTEXT, __pyx_kp_u_The_context_is_invalid); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__46);
   __Pyx_GIVEREF(__pyx_tuple__46);
 
-  /* "pyjoulescope_driver/binding.pyx":408
+  /* "pyjoulescope_driver/binding.pyx":410
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),             # <<<<<<<<<<<<<<
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  */
-  __pyx_tuple__47 = PyTuple_Pack(3, __pyx_int_8, __pyx_n_u_INVALID_MESSAGE_LENGTH, __pyx_kp_u_The_message_length_in_invalid); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(3, __pyx_int_8, __pyx_n_u_INVALID_MESSAGE_LENGTH, __pyx_kp_u_The_message_length_in_invalid); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__47);
   __Pyx_GIVEREF(__pyx_tuple__47);
 
-  /* "pyjoulescope_driver/binding.pyx":409
+  /* "pyjoulescope_driver/binding.pyx":411
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),             # <<<<<<<<<<<<<<
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),
  */
-  __pyx_tuple__48 = PyTuple_Pack(3, __pyx_int_9, __pyx_n_u_MESSAGE_INTEGRITY, __pyx_kp_u_The_message_integrity_check_fail); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_tuple__48 = PyTuple_Pack(3, __pyx_int_9, __pyx_n_u_MESSAGE_INTEGRITY, __pyx_kp_u_The_message_integrity_check_fail); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__48);
   __Pyx_GIVEREF(__pyx_tuple__48);
 
-  /* "pyjoulescope_driver/binding.pyx":410
+  /* "pyjoulescope_driver/binding.pyx":412
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),             # <<<<<<<<<<<<<<
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),
  *     12: (12, 'FULL', 'The target of the operation is full'),
  */
-  __pyx_tuple__49 = PyTuple_Pack(3, __pyx_int_10, __pyx_n_u_SYNTAX_ERROR, __pyx_kp_u_A_syntax_error_was_detected); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_tuple__49 = PyTuple_Pack(3, __pyx_int_10, __pyx_n_u_SYNTAX_ERROR, __pyx_kp_u_A_syntax_error_was_detected); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__49);
   __Pyx_GIVEREF(__pyx_tuple__49);
 
-  /* "pyjoulescope_driver/binding.pyx":411
+  /* "pyjoulescope_driver/binding.pyx":413
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),             # <<<<<<<<<<<<<<
  *     12: (12, 'FULL', 'The target of the operation is full'),
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),
  */
-  __pyx_tuple__50 = PyTuple_Pack(3, __pyx_int_11, __pyx_n_u_TIMED_OUT, __pyx_kp_u_The_operation_did_not_complete_i); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_tuple__50 = PyTuple_Pack(3, __pyx_int_11, __pyx_n_u_TIMED_OUT, __pyx_kp_u_The_operation_did_not_complete_i); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__50);
   __Pyx_GIVEREF(__pyx_tuple__50);
 
-  /* "pyjoulescope_driver/binding.pyx":412
+  /* "pyjoulescope_driver/binding.pyx":414
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),
  *     12: (12, 'FULL', 'The target of the operation is full'),             # <<<<<<<<<<<<<<
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),
  */
-  __pyx_tuple__51 = PyTuple_Pack(3, __pyx_int_12, __pyx_n_u_FULL, __pyx_kp_u_The_target_of_the_operation_is_f); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_tuple__51 = PyTuple_Pack(3, __pyx_int_12, __pyx_n_u_FULL, __pyx_kp_u_The_target_of_the_operation_is_f); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
 
-  /* "pyjoulescope_driver/binding.pyx":413
+  /* "pyjoulescope_driver/binding.pyx":415
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),
  *     12: (12, 'FULL', 'The target of the operation is full'),
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),             # <<<<<<<<<<<<<<
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),
  */
-  __pyx_tuple__52 = PyTuple_Pack(3, __pyx_int_13, __pyx_n_u_EMPTY, __pyx_kp_u_The_target_of_the_operation_is_e); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(3, __pyx_int_13, __pyx_n_u_EMPTY, __pyx_kp_u_The_target_of_the_operation_is_e); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__52);
   __Pyx_GIVEREF(__pyx_tuple__52);
 
-  /* "pyjoulescope_driver/binding.pyx":414
+  /* "pyjoulescope_driver/binding.pyx":416
  *     12: (12, 'FULL', 'The target of the operation is full'),
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),             # <<<<<<<<<<<<<<
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),
  */
-  __pyx_tuple__53 = PyTuple_Pack(3, __pyx_int_14, __pyx_n_u_TOO_SMALL, __pyx_kp_u_The_target_of_the_operation_is_t); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_tuple__53 = PyTuple_Pack(3, __pyx_int_14, __pyx_n_u_TOO_SMALL, __pyx_kp_u_The_target_of_the_operation_is_t); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__53);
   __Pyx_GIVEREF(__pyx_tuple__53);
 
-  /* "pyjoulescope_driver/binding.pyx":415
+  /* "pyjoulescope_driver/binding.pyx":417
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),             # <<<<<<<<<<<<<<
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  */
-  __pyx_tuple__54 = PyTuple_Pack(3, __pyx_int_15, __pyx_n_u_TOO_BIG, __pyx_kp_u_The_target_of_the_operation_is_t_2); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_tuple__54 = PyTuple_Pack(3, __pyx_int_15, __pyx_n_u_TOO_BIG, __pyx_kp_u_The_target_of_the_operation_is_t_2); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__54);
   __Pyx_GIVEREF(__pyx_tuple__54);
 
-  /* "pyjoulescope_driver/binding.pyx":416
+  /* "pyjoulescope_driver/binding.pyx":418
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),             # <<<<<<<<<<<<<<
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  */
-  __pyx_tuple__55 = PyTuple_Pack(3, __pyx_int_16, __pyx_n_u_NOT_FOUND, __pyx_kp_u_The_requested_resource_was_not_f); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_tuple__55 = PyTuple_Pack(3, __pyx_int_16, __pyx_n_u_NOT_FOUND, __pyx_kp_u_The_requested_resource_was_not_f); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__55);
   __Pyx_GIVEREF(__pyx_tuple__55);
 
-  /* "pyjoulescope_driver/binding.pyx":417
+  /* "pyjoulescope_driver/binding.pyx":419
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),             # <<<<<<<<<<<<<<
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),
  */
-  __pyx_tuple__56 = PyTuple_Pack(3, __pyx_int_17, __pyx_n_u_ALREADY_EXISTS, __pyx_kp_u_The_requested_resource_already_e); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(3, __pyx_int_17, __pyx_n_u_ALREADY_EXISTS, __pyx_kp_u_The_requested_resource_already_e); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__56);
   __Pyx_GIVEREF(__pyx_tuple__56);
 
-  /* "pyjoulescope_driver/binding.pyx":418
+  /* "pyjoulescope_driver/binding.pyx":420
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),             # <<<<<<<<<<<<<<
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  */
-  __pyx_tuple__57 = PyTuple_Pack(3, __pyx_int_18, __pyx_n_u_PERMISSIONS, __pyx_kp_u_Insufficient_permissions_to_perf); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_tuple__57 = PyTuple_Pack(3, __pyx_int_18, __pyx_n_u_PERMISSIONS, __pyx_kp_u_Insufficient_permissions_to_perf); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__57);
   __Pyx_GIVEREF(__pyx_tuple__57);
 
-  /* "pyjoulescope_driver/binding.pyx":419
+  /* "pyjoulescope_driver/binding.pyx":421
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),             # <<<<<<<<<<<<<<
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),
  */
-  __pyx_tuple__58 = PyTuple_Pack(3, __pyx_int_19, __pyx_n_u_BUSY, __pyx_kp_u_The_requested_resource_is_curren); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(3, __pyx_int_19, __pyx_n_u_BUSY, __pyx_kp_u_The_requested_resource_is_curren); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__58);
   __Pyx_GIVEREF(__pyx_tuple__58);
 
-  /* "pyjoulescope_driver/binding.pyx":420
+  /* "pyjoulescope_driver/binding.pyx":422
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),             # <<<<<<<<<<<<<<
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),
  */
-  __pyx_tuple__59 = PyTuple_Pack(3, __pyx_int_20, __pyx_n_u_UNAVAILABLE, __pyx_kp_u_The_requested_resource_is_curren_2); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_tuple__59 = PyTuple_Pack(3, __pyx_int_20, __pyx_n_u_UNAVAILABLE, __pyx_kp_u_The_requested_resource_is_curren_2); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__59);
   __Pyx_GIVEREF(__pyx_tuple__59);
 
-  /* "pyjoulescope_driver/binding.pyx":421
+  /* "pyjoulescope_driver/binding.pyx":423
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),             # <<<<<<<<<<<<<<
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  */
-  __pyx_tuple__60 = PyTuple_Pack(3, __pyx_int_21, __pyx_n_u_IN_USE, __pyx_kp_u_The_requested_resource_is_curren_3); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_tuple__60 = PyTuple_Pack(3, __pyx_int_21, __pyx_n_u_IN_USE, __pyx_kp_u_The_requested_resource_is_curren_3); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__60);
   __Pyx_GIVEREF(__pyx_tuple__60);
 
-  /* "pyjoulescope_driver/binding.pyx":422
+  /* "pyjoulescope_driver/binding.pyx":424
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),             # <<<<<<<<<<<<<<
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  *     24: (24, 'ABORTED', 'The requested operation was previously aborted.'),
  */
-  __pyx_tuple__61 = PyTuple_Pack(3, __pyx_int_22, __pyx_n_u_CLOSED, __pyx_kp_u_The_requested_resource_is_curren_4); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_tuple__61 = PyTuple_Pack(3, __pyx_int_22, __pyx_n_u_CLOSED, __pyx_kp_u_The_requested_resource_is_curren_4); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__61);
   __Pyx_GIVEREF(__pyx_tuple__61);
 
-  /* "pyjoulescope_driver/binding.pyx":423
+  /* "pyjoulescope_driver/binding.pyx":425
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),             # <<<<<<<<<<<<<<
  *     24: (24, 'ABORTED', 'The requested operation was previously aborted.'),
  *     25: (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),
  */
-  __pyx_tuple__62 = PyTuple_Pack(3, __pyx_int_23, __pyx_n_u_SEQUENCE, __pyx_kp_u_The_requested_operation_was_out); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_tuple__62 = PyTuple_Pack(3, __pyx_int_23, __pyx_n_u_SEQUENCE, __pyx_kp_u_The_requested_operation_was_out); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__62);
   __Pyx_GIVEREF(__pyx_tuple__62);
 
-  /* "pyjoulescope_driver/binding.pyx":424
+  /* "pyjoulescope_driver/binding.pyx":426
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  *     24: (24, 'ABORTED', 'The requested operation was previously aborted.'),             # <<<<<<<<<<<<<<
  *     25: (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),
  *     'SUCCESS': (0, 'SUCCESS', 'Success (no error)'),
  */
-  __pyx_tuple__63 = PyTuple_Pack(3, __pyx_int_24, __pyx_n_u_ABORTED, __pyx_kp_u_The_requested_operation_was_prev); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_tuple__63 = PyTuple_Pack(3, __pyx_int_24, __pyx_n_u_ABORTED, __pyx_kp_u_The_requested_operation_was_prev); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__63);
   __Pyx_GIVEREF(__pyx_tuple__63);
 
-  /* "pyjoulescope_driver/binding.pyx":425
+  /* "pyjoulescope_driver/binding.pyx":427
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  *     24: (24, 'ABORTED', 'The requested operation was previously aborted.'),
  *     25: (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),             # <<<<<<<<<<<<<<
  *     'SUCCESS': (0, 'SUCCESS', 'Success (no error)'),
  *     'UNSPECIFIED': (1, 'UNSPECIFIED', 'Unspecified error'),
  */
-  __pyx_tuple__64 = PyTuple_Pack(3, __pyx_int_25, __pyx_n_u_SYNCHRONIZATION, __pyx_kp_u_The_target_is_not_synchronized_w); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(3, __pyx_int_25, __pyx_n_u_SYNCHRONIZATION, __pyx_kp_u_The_target_is_not_synchronized_w); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__64);
   __Pyx_GIVEREF(__pyx_tuple__64);
 
-  /* "pyjoulescope_driver/binding.pyx":456
+  /* "pyjoulescope_driver/binding.pyx":458
  * 
  * 
  * def error_code_to_str(ec):             # <<<<<<<<<<<<<<
  *     """Get the string representation for an error code.
  * 
  */
-  __pyx_tuple__65 = PyTuple_Pack(4, __pyx_n_s_ec, __pyx_n_s_v, __pyx_n_s_name, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 456, __pyx_L1_error)
+  __pyx_tuple__65 = PyTuple_Pack(4, __pyx_n_s_ec, __pyx_n_s_v, __pyx_n_s_name, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__65);
   __Pyx_GIVEREF(__pyx_tuple__65);
-  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjoulescope_driver_binding_pyx, __pyx_n_s_error_code_to_str, 456, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 456, __pyx_L1_error)
+  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjoulescope_driver_binding_pyx, __pyx_n_s_error_code_to_str, 458, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 458, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":524
+  /* "pyjoulescope_driver/binding.pyx":526
  * 
  * 
  * def log_level_c_to_py(lvl):             # <<<<<<<<<<<<<<
  *     return _log_level_c_to_py.get(int(lvl))
  * 
  */
-  __pyx_tuple__67 = PyTuple_Pack(1, __pyx_n_s_lvl); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 524, __pyx_L1_error)
+  __pyx_tuple__67 = PyTuple_Pack(1, __pyx_n_s_lvl); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__67);
   __Pyx_GIVEREF(__pyx_tuple__67);
-  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjoulescope_driver_binding_pyx, __pyx_n_s_log_level_c_to_py_2, 524, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 524, __pyx_L1_error)
+  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjoulescope_driver_binding_pyx, __pyx_n_s_log_level_c_to_py_2, 526, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 526, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":577
+  /* "pyjoulescope_driver/binding.pyx":579
  * 
  * 
  * def _handle_rc(rc, src, cause=None):             # <<<<<<<<<<<<<<
  *     if rc:
  *         if cause:
  */
-  __pyx_tuple__69 = PyTuple_Pack(3, __pyx_n_s_rc, __pyx_n_s_src, __pyx_n_s_cause); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_tuple__69 = PyTuple_Pack(3, __pyx_n_s_rc, __pyx_n_s_src, __pyx_n_s_cause); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__69);
   __Pyx_GIVEREF(__pyx_tuple__69);
-  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjoulescope_driver_binding_pyx, __pyx_n_s_handle_rc, 577, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjoulescope_driver_binding_pyx, __pyx_n_s_handle_rc, 579, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 579, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -29370,23 +29285,23 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_19pyjoulescope_driver_7binding_Driver) < 0) __PYX_ERR(0, 589, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_19pyjoulescope_driver_7binding_Driver) < 0) __PYX_ERR(0, 591, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_19pyjoulescope_driver_7binding_Driver.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_19pyjoulescope_driver_7binding_Driver.tp_dictoffset && __pyx_type_19pyjoulescope_driver_7binding_Driver.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_19pyjoulescope_driver_7binding_Driver.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Driver, (PyObject *)&__pyx_type_19pyjoulescope_driver_7binding_Driver) < 0) __PYX_ERR(0, 589, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_19pyjoulescope_driver_7binding_Driver) < 0) __PYX_ERR(0, 589, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Driver, (PyObject *)&__pyx_type_19pyjoulescope_driver_7binding_Driver) < 0) __PYX_ERR(0, 591, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_19pyjoulescope_driver_7binding_Driver) < 0) __PYX_ERR(0, 591, __pyx_L1_error)
   __pyx_ptype_19pyjoulescope_driver_7binding_Driver = &__pyx_type_19pyjoulescope_driver_7binding_Driver;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
@@ -29734,69 +29649,69 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "pyjoulescope_driver/binding.pyx":28
+  /* "pyjoulescope_driver/binding.pyx":30
  * from libc.string cimport memset, strcpy
  * 
  * from collections.abc import Mapping             # <<<<<<<<<<<<<<
  * import json
  * import logging
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Mapping);
   __Pyx_GIVEREF(__pyx_n_s_Mapping);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Mapping);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_collections_abc, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_collections_abc, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Mapping, __pyx_t_1) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Mapping, __pyx_t_1) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":29
+  /* "pyjoulescope_driver/binding.pyx":31
  * 
  * from collections.abc import Mapping
  * import json             # <<<<<<<<<<<<<<
  * import logging
  * import numpy as np
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_json, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_json, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_json, __pyx_t_2) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_json, __pyx_t_2) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":30
+  /* "pyjoulescope_driver/binding.pyx":32
  * from collections.abc import Mapping
  * import json
  * import logging             # <<<<<<<<<<<<<<
  * import numpy as np
  * include "module.pxi"
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_logging, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_logging, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logging, __pyx_t_2) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logging, __pyx_t_2) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":31
+  /* "pyjoulescope_driver/binding.pyx":33
  * import json
  * import logging
  * import numpy as np             # <<<<<<<<<<<<<<
  * include "module.pxi"
  * import time
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyjoulescope_driver/module.pxi":22
  * from libc.stdint cimport intptr_t
  * from libc.stdlib cimport malloc, free
  * import logging             # <<<<<<<<<<<<<<
  * log = logging.getLogger(__name__)
@@ -29949,2329 +29864,2329 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_D, __pyx_t_2) < 0) __PYX_ERR(4, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u__37, __pyx_int_0) < 0) __PYX_ERR(4, 27, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_LOG_LEVEL_MAP, __pyx_t_3) < 0) __PYX_ERR(4, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":33
+  /* "pyjoulescope_driver/binding.pyx":35
  * import numpy as np
  * include "module.pxi"
  * import time             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * from . cimport c_jsdrv
  */
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_time, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_time, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_time, __pyx_t_3) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_time, __pyx_t_3) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":38
+  /* "pyjoulescope_driver/binding.pyx":40
  * 
  * 
  * __all__ = ['Driver']             # <<<<<<<<<<<<<<
  * np.import_array()                           # initialize numpy before use
  * _log_c_name = 'jsdrv'
  */
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_u_Driver);
   __Pyx_GIVEREF(__pyx_n_u_Driver);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_u_Driver);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_t_3) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_t_3) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":39
+  /* "pyjoulescope_driver/binding.pyx":41
  * 
  * __all__ = ['Driver']
  * np.import_array()                           # initialize numpy before use             # <<<<<<<<<<<<<<
  * _log_c_name = 'jsdrv'
  * _log_c = logging.getLogger(_log_c_name)
  */
-  __pyx_t_4 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 41, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":40
+  /* "pyjoulescope_driver/binding.pyx":42
  * __all__ = ['Driver']
  * np.import_array()                           # initialize numpy before use
  * _log_c_name = 'jsdrv'             # <<<<<<<<<<<<<<
  * _log_c = logging.getLogger(_log_c_name)
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_c_name, __pyx_n_u_jsdrv) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_c_name, __pyx_n_u_jsdrv) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":41
+  /* "pyjoulescope_driver/binding.pyx":43
  * np.import_array()                           # initialize numpy before use
  * _log_c_name = 'jsdrv'
  * _log_c = logging.getLogger(_log_c_name)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_log_c_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_log_c_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_c, __pyx_t_1) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_c, __pyx_t_1) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":44
+  /* "pyjoulescope_driver/binding.pyx":46
  * 
  * 
  * class ElementType:             # <<<<<<<<<<<<<<
  *     UNDEFINED = 0
  *     INT = 2
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_ElementType, __pyx_n_s_ElementType, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_ElementType, __pyx_n_s_ElementType, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pyjoulescope_driver/binding.pyx":45
+  /* "pyjoulescope_driver/binding.pyx":47
  * 
  * class ElementType:
  *     UNDEFINED = 0             # <<<<<<<<<<<<<<
  *     INT = 2
  *     UINT = 3
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UNDEFINED, __pyx_int_0) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UNDEFINED, __pyx_int_0) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":46
+  /* "pyjoulescope_driver/binding.pyx":48
  * class ElementType:
  *     UNDEFINED = 0
  *     INT = 2             # <<<<<<<<<<<<<<
  *     UINT = 3
  *     FLOAT = 4
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INT, __pyx_int_2) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INT, __pyx_int_2) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":47
+  /* "pyjoulescope_driver/binding.pyx":49
  *     UNDEFINED = 0
  *     INT = 2
  *     UINT = 3             # <<<<<<<<<<<<<<
  *     FLOAT = 4
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UINT, __pyx_int_3) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UINT, __pyx_int_3) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":48
+  /* "pyjoulescope_driver/binding.pyx":50
  *     INT = 2
  *     UINT = 3
  *     FLOAT = 4             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_FLOAT, __pyx_int_4) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_FLOAT, __pyx_int_4) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":44
+  /* "pyjoulescope_driver/binding.pyx":46
  * 
  * 
  * class ElementType:             # <<<<<<<<<<<<<<
  *     UNDEFINED = 0
  *     INT = 2
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_ElementType, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_ElementType, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ElementType, __pyx_t_3) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ElementType, __pyx_t_3) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":51
+  /* "pyjoulescope_driver/binding.pyx":53
  * 
  * 
  * class Field:             # <<<<<<<<<<<<<<
  *     UNDEFINED = 0
  *     CURRENT   = 1
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Field, __pyx_n_s_Field, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Field, __pyx_n_s_Field, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pyjoulescope_driver/binding.pyx":52
+  /* "pyjoulescope_driver/binding.pyx":54
  * 
  * class Field:
  *     UNDEFINED = 0             # <<<<<<<<<<<<<<
  *     CURRENT   = 1
  *     VOLTAGE   = 2
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UNDEFINED, __pyx_int_0) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UNDEFINED, __pyx_int_0) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":53
+  /* "pyjoulescope_driver/binding.pyx":55
  * class Field:
  *     UNDEFINED = 0
  *     CURRENT   = 1             # <<<<<<<<<<<<<<
  *     VOLTAGE   = 2
  *     POWER     = 3
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_CURRENT, __pyx_int_1) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_CURRENT, __pyx_int_1) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":54
+  /* "pyjoulescope_driver/binding.pyx":56
  *     UNDEFINED = 0
  *     CURRENT   = 1
  *     VOLTAGE   = 2             # <<<<<<<<<<<<<<
  *     POWER     = 3
  *     RANGE     = 4
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_VOLTAGE, __pyx_int_2) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_VOLTAGE, __pyx_int_2) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":55
+  /* "pyjoulescope_driver/binding.pyx":57
  *     CURRENT   = 1
  *     VOLTAGE   = 2
  *     POWER     = 3             # <<<<<<<<<<<<<<
  *     RANGE     = 4
  *     GPI       = 5
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_POWER, __pyx_int_3) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_POWER, __pyx_int_3) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":56
+  /* "pyjoulescope_driver/binding.pyx":58
  *     VOLTAGE   = 2
  *     POWER     = 3
  *     RANGE     = 4             # <<<<<<<<<<<<<<
  *     GPI       = 5
  *     UART      = 6
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_RANGE, __pyx_int_4) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_RANGE, __pyx_int_4) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":57
+  /* "pyjoulescope_driver/binding.pyx":59
  *     POWER     = 3
  *     RANGE     = 4
  *     GPI       = 5             # <<<<<<<<<<<<<<
  *     UART      = 6
  *     RAW       = 7
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_GPI, __pyx_int_5) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_GPI, __pyx_int_5) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":58
+  /* "pyjoulescope_driver/binding.pyx":60
  *     RANGE     = 4
  *     GPI       = 5
  *     UART      = 6             # <<<<<<<<<<<<<<
  *     RAW       = 7
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UART, __pyx_int_6) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UART, __pyx_int_6) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":59
+  /* "pyjoulescope_driver/binding.pyx":61
  *     GPI       = 5
  *     UART      = 6
  *     RAW       = 7             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_RAW, __pyx_int_7) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_RAW, __pyx_int_7) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":51
+  /* "pyjoulescope_driver/binding.pyx":53
  * 
  * 
  * class Field:             # <<<<<<<<<<<<<<
  *     UNDEFINED = 0
  *     CURRENT   = 1
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Field, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Field, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Field, __pyx_t_3) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Field, __pyx_t_3) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":63
+  /* "pyjoulescope_driver/binding.pyx":65
  * 
  * _element_type_to_prefix = {
  *     ElementType.INT: 'i',             # <<<<<<<<<<<<<<
  *     ElementType.UINT: 'u',
  *     ElementType.FLOAT: 'f',
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ElementType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ElementType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_INT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_INT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_2, __pyx_n_u_i) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_2, __pyx_n_u_i) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":64
+  /* "pyjoulescope_driver/binding.pyx":66
  * _element_type_to_prefix = {
  *     ElementType.INT: 'i',
  *     ElementType.UINT: 'u',             # <<<<<<<<<<<<<<
  *     ElementType.FLOAT: 'f',
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ElementType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ElementType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_n_u_u) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_n_u_u) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":65
+  /* "pyjoulescope_driver/binding.pyx":67
  *     ElementType.INT: 'i',
  *     ElementType.UINT: 'u',
  *     ElementType.FLOAT: 'f',             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ElementType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ElementType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_FLOAT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_FLOAT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_2, __pyx_n_u_f) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_2, __pyx_n_u_f) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_element_type_to_prefix, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_element_type_to_prefix, __pyx_t_1) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":71
+  /* "pyjoulescope_driver/binding.pyx":73
  * _field_to_meta = {
  *     #field         [name,            field, units, use_index]
  *     Field.CURRENT: ['current',       'i',   'A',   False],             # <<<<<<<<<<<<<<
  *     Field.VOLTAGE: ['voltage',       'v',   'V',   False],
  *     Field.POWER:   ['power',         'p',   'W',   False],
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CURRENT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CURRENT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_current);
   __Pyx_GIVEREF(__pyx_n_u_current);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_current);
   __Pyx_INCREF(__pyx_n_u_i);
   __Pyx_GIVEREF(__pyx_n_u_i);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_i);
   __Pyx_INCREF(__pyx_n_u_A);
   __Pyx_GIVEREF(__pyx_n_u_A);
   PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_u_A);
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   PyList_SET_ITEM(__pyx_t_2, 3, Py_False);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":72
+  /* "pyjoulescope_driver/binding.pyx":74
  *     #field         [name,            field, units, use_index]
  *     Field.CURRENT: ['current',       'i',   'A',   False],
  *     Field.VOLTAGE: ['voltage',       'v',   'V',   False],             # <<<<<<<<<<<<<<
  *     Field.POWER:   ['power',         'p',   'W',   False],
  *     Field.RANGE:   ['current_range', 'r',   None,  False],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_VOLTAGE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_VOLTAGE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_voltage);
   __Pyx_GIVEREF(__pyx_n_u_voltage);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_voltage);
   __Pyx_INCREF(__pyx_n_u_v);
   __Pyx_GIVEREF(__pyx_n_u_v);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_v);
   __Pyx_INCREF(__pyx_n_u_V);
   __Pyx_GIVEREF(__pyx_n_u_V);
   PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_u_V);
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   PyList_SET_ITEM(__pyx_t_2, 3, Py_False);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":73
+  /* "pyjoulescope_driver/binding.pyx":75
  *     Field.CURRENT: ['current',       'i',   'A',   False],
  *     Field.VOLTAGE: ['voltage',       'v',   'V',   False],
  *     Field.POWER:   ['power',         'p',   'W',   False],             # <<<<<<<<<<<<<<
  *     Field.RANGE:   ['current_range', 'r',   None,  False],
  *     Field.GPI:     ['gpi',           '',    None,  True],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_POWER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_POWER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_power);
   __Pyx_GIVEREF(__pyx_n_u_power);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_power);
   __Pyx_INCREF(__pyx_n_u_p);
   __Pyx_GIVEREF(__pyx_n_u_p);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_p);
   __Pyx_INCREF(__pyx_n_u_W);
   __Pyx_GIVEREF(__pyx_n_u_W);
   PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_u_W);
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   PyList_SET_ITEM(__pyx_t_2, 3, Py_False);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":74
+  /* "pyjoulescope_driver/binding.pyx":76
  *     Field.VOLTAGE: ['voltage',       'v',   'V',   False],
  *     Field.POWER:   ['power',         'p',   'W',   False],
  *     Field.RANGE:   ['current_range', 'r',   None,  False],             # <<<<<<<<<<<<<<
  *     Field.GPI:     ['gpi',           '',    None,  True],
  *     Field.UART:    ['uart',          'u',   None,  True],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RANGE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RANGE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_current_range);
   __Pyx_GIVEREF(__pyx_n_u_current_range);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_current_range);
   __Pyx_INCREF(__pyx_n_u_r);
   __Pyx_GIVEREF(__pyx_n_u_r);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_r);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyList_SET_ITEM(__pyx_t_2, 2, Py_None);
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   PyList_SET_ITEM(__pyx_t_2, 3, Py_False);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":75
+  /* "pyjoulescope_driver/binding.pyx":77
  *     Field.POWER:   ['power',         'p',   'W',   False],
  *     Field.RANGE:   ['current_range', 'r',   None,  False],
  *     Field.GPI:     ['gpi',           '',    None,  True],             # <<<<<<<<<<<<<<
  *     Field.UART:    ['uart',          'u',   None,  True],
  *     Field.RAW:     ['raw',           'z',   None,  True],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_GPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_GPI); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_gpi);
   __Pyx_GIVEREF(__pyx_n_u_gpi);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_gpi);
   __Pyx_INCREF(__pyx_kp_u__38);
   __Pyx_GIVEREF(__pyx_kp_u__38);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_kp_u__38);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyList_SET_ITEM(__pyx_t_2, 2, Py_None);
   __Pyx_INCREF(Py_True);
   __Pyx_GIVEREF(Py_True);
   PyList_SET_ITEM(__pyx_t_2, 3, Py_True);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":76
+  /* "pyjoulescope_driver/binding.pyx":78
  *     Field.RANGE:   ['current_range', 'r',   None,  False],
  *     Field.GPI:     ['gpi',           '',    None,  True],
  *     Field.UART:    ['uart',          'u',   None,  True],             # <<<<<<<<<<<<<<
  *     Field.RAW:     ['raw',           'z',   None,  True],
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_UART); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_UART); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_uart);
   __Pyx_GIVEREF(__pyx_n_u_uart);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_uart);
   __Pyx_INCREF(__pyx_n_u_u);
   __Pyx_GIVEREF(__pyx_n_u_u);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_u);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyList_SET_ITEM(__pyx_t_2, 2, Py_None);
   __Pyx_INCREF(Py_True);
   __Pyx_GIVEREF(Py_True);
   PyList_SET_ITEM(__pyx_t_2, 3, Py_True);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":77
+  /* "pyjoulescope_driver/binding.pyx":79
  *     Field.GPI:     ['gpi',           '',    None,  True],
  *     Field.UART:    ['uart',          'u',   None,  True],
  *     Field.RAW:     ['raw',           'z',   None,  True],             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Field); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RAW); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RAW); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_raw);
   __Pyx_GIVEREF(__pyx_n_u_raw);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_raw);
   __Pyx_INCREF(__pyx_n_u_z);
   __Pyx_GIVEREF(__pyx_n_u_z);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_z);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyList_SET_ITEM(__pyx_t_2, 2, Py_None);
   __Pyx_INCREF(Py_True);
   __Pyx_GIVEREF(Py_True);
   PyList_SET_ITEM(__pyx_t_2, 3, Py_True);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_field_to_meta, __pyx_t_1) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_field_to_meta, __pyx_t_1) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":365
+  /* "pyjoulescope_driver/binding.pyx":367
  * 
  * 
  * class ErrorCode:             # <<<<<<<<<<<<<<
  *     # automatically maintained by error_code_update.py
  *     # ENUM_ERROR_CODE_START
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_ErrorCode, __pyx_n_s_ErrorCode, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_ErrorCode, __pyx_n_s_ErrorCode, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pyjoulescope_driver/binding.pyx":368
+  /* "pyjoulescope_driver/binding.pyx":370
  *     # automatically maintained by error_code_update.py
  *     # ENUM_ERROR_CODE_START
  *     SUCCESS                     = 0             # <<<<<<<<<<<<<<
  *     UNSPECIFIED                 = 1
  *     NOT_ENOUGH_MEMORY           = 2
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_SUCCESS, __pyx_int_0) < 0) __PYX_ERR(0, 368, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_SUCCESS, __pyx_int_0) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":369
+  /* "pyjoulescope_driver/binding.pyx":371
  *     # ENUM_ERROR_CODE_START
  *     SUCCESS                     = 0
  *     UNSPECIFIED                 = 1             # <<<<<<<<<<<<<<
  *     NOT_ENOUGH_MEMORY           = 2
  *     NOT_SUPPORTED               = 3
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UNSPECIFIED, __pyx_int_1) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UNSPECIFIED, __pyx_int_1) < 0) __PYX_ERR(0, 371, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":370
+  /* "pyjoulescope_driver/binding.pyx":372
  *     SUCCESS                     = 0
  *     UNSPECIFIED                 = 1
  *     NOT_ENOUGH_MEMORY           = 2             # <<<<<<<<<<<<<<
  *     NOT_SUPPORTED               = 3
  *     IO                          = 4
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NOT_ENOUGH_MEMORY, __pyx_int_2) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NOT_ENOUGH_MEMORY, __pyx_int_2) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":371
+  /* "pyjoulescope_driver/binding.pyx":373
  *     UNSPECIFIED                 = 1
  *     NOT_ENOUGH_MEMORY           = 2
  *     NOT_SUPPORTED               = 3             # <<<<<<<<<<<<<<
  *     IO                          = 4
  *     PARAMETER_INVALID           = 5
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NOT_SUPPORTED, __pyx_int_3) < 0) __PYX_ERR(0, 371, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NOT_SUPPORTED, __pyx_int_3) < 0) __PYX_ERR(0, 373, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":372
+  /* "pyjoulescope_driver/binding.pyx":374
  *     NOT_ENOUGH_MEMORY           = 2
  *     NOT_SUPPORTED               = 3
  *     IO                          = 4             # <<<<<<<<<<<<<<
  *     PARAMETER_INVALID           = 5
  *     INVALID_RETURN_CONDITION    = 6
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_IO, __pyx_int_4) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_IO, __pyx_int_4) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":373
+  /* "pyjoulescope_driver/binding.pyx":375
  *     NOT_SUPPORTED               = 3
  *     IO                          = 4
  *     PARAMETER_INVALID           = 5             # <<<<<<<<<<<<<<
  *     INVALID_RETURN_CONDITION    = 6
  *     INVALID_CONTEXT             = 7
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_PARAMETER_INVALID, __pyx_int_5) < 0) __PYX_ERR(0, 373, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_PARAMETER_INVALID, __pyx_int_5) < 0) __PYX_ERR(0, 375, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":374
+  /* "pyjoulescope_driver/binding.pyx":376
  *     IO                          = 4
  *     PARAMETER_INVALID           = 5
  *     INVALID_RETURN_CONDITION    = 6             # <<<<<<<<<<<<<<
  *     INVALID_CONTEXT             = 7
  *     INVALID_MESSAGE_LENGTH      = 8
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INVALID_RETURN_CONDITION, __pyx_int_6) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INVALID_RETURN_CONDITION, __pyx_int_6) < 0) __PYX_ERR(0, 376, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":375
+  /* "pyjoulescope_driver/binding.pyx":377
  *     PARAMETER_INVALID           = 5
  *     INVALID_RETURN_CONDITION    = 6
  *     INVALID_CONTEXT             = 7             # <<<<<<<<<<<<<<
  *     INVALID_MESSAGE_LENGTH      = 8
  *     MESSAGE_INTEGRITY           = 9
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INVALID_CONTEXT, __pyx_int_7) < 0) __PYX_ERR(0, 375, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INVALID_CONTEXT, __pyx_int_7) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":376
+  /* "pyjoulescope_driver/binding.pyx":378
  *     INVALID_RETURN_CONDITION    = 6
  *     INVALID_CONTEXT             = 7
  *     INVALID_MESSAGE_LENGTH      = 8             # <<<<<<<<<<<<<<
  *     MESSAGE_INTEGRITY           = 9
  *     SYNTAX_ERROR                = 10
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INVALID_MESSAGE_LENGTH, __pyx_int_8) < 0) __PYX_ERR(0, 376, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INVALID_MESSAGE_LENGTH, __pyx_int_8) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":377
+  /* "pyjoulescope_driver/binding.pyx":379
  *     INVALID_CONTEXT             = 7
  *     INVALID_MESSAGE_LENGTH      = 8
  *     MESSAGE_INTEGRITY           = 9             # <<<<<<<<<<<<<<
  *     SYNTAX_ERROR                = 10
  *     TIMED_OUT                   = 11
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_MESSAGE_INTEGRITY, __pyx_int_9) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_MESSAGE_INTEGRITY, __pyx_int_9) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":378
+  /* "pyjoulescope_driver/binding.pyx":380
  *     INVALID_MESSAGE_LENGTH      = 8
  *     MESSAGE_INTEGRITY           = 9
  *     SYNTAX_ERROR                = 10             # <<<<<<<<<<<<<<
  *     TIMED_OUT                   = 11
  *     FULL                        = 12
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_SYNTAX_ERROR, __pyx_int_10) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_SYNTAX_ERROR, __pyx_int_10) < 0) __PYX_ERR(0, 380, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":379
+  /* "pyjoulescope_driver/binding.pyx":381
  *     MESSAGE_INTEGRITY           = 9
  *     SYNTAX_ERROR                = 10
  *     TIMED_OUT                   = 11             # <<<<<<<<<<<<<<
  *     FULL                        = 12
  *     EMPTY                       = 13
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_TIMED_OUT, __pyx_int_11) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_TIMED_OUT, __pyx_int_11) < 0) __PYX_ERR(0, 381, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":380
+  /* "pyjoulescope_driver/binding.pyx":382
  *     SYNTAX_ERROR                = 10
  *     TIMED_OUT                   = 11
  *     FULL                        = 12             # <<<<<<<<<<<<<<
  *     EMPTY                       = 13
  *     TOO_SMALL                   = 14
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_FULL, __pyx_int_12) < 0) __PYX_ERR(0, 380, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_FULL, __pyx_int_12) < 0) __PYX_ERR(0, 382, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":381
+  /* "pyjoulescope_driver/binding.pyx":383
  *     TIMED_OUT                   = 11
  *     FULL                        = 12
  *     EMPTY                       = 13             # <<<<<<<<<<<<<<
  *     TOO_SMALL                   = 14
  *     TOO_BIG                     = 15
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_EMPTY, __pyx_int_13) < 0) __PYX_ERR(0, 381, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_EMPTY, __pyx_int_13) < 0) __PYX_ERR(0, 383, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":382
+  /* "pyjoulescope_driver/binding.pyx":384
  *     FULL                        = 12
  *     EMPTY                       = 13
  *     TOO_SMALL                   = 14             # <<<<<<<<<<<<<<
  *     TOO_BIG                     = 15
  *     NOT_FOUND                   = 16
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_TOO_SMALL, __pyx_int_14) < 0) __PYX_ERR(0, 382, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_TOO_SMALL, __pyx_int_14) < 0) __PYX_ERR(0, 384, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":383
+  /* "pyjoulescope_driver/binding.pyx":385
  *     EMPTY                       = 13
  *     TOO_SMALL                   = 14
  *     TOO_BIG                     = 15             # <<<<<<<<<<<<<<
  *     NOT_FOUND                   = 16
  *     ALREADY_EXISTS              = 17
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_TOO_BIG, __pyx_int_15) < 0) __PYX_ERR(0, 383, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_TOO_BIG, __pyx_int_15) < 0) __PYX_ERR(0, 385, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":384
+  /* "pyjoulescope_driver/binding.pyx":386
  *     TOO_SMALL                   = 14
  *     TOO_BIG                     = 15
  *     NOT_FOUND                   = 16             # <<<<<<<<<<<<<<
  *     ALREADY_EXISTS              = 17
  *     PERMISSIONS                 = 18
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NOT_FOUND, __pyx_int_16) < 0) __PYX_ERR(0, 384, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NOT_FOUND, __pyx_int_16) < 0) __PYX_ERR(0, 386, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":385
+  /* "pyjoulescope_driver/binding.pyx":387
  *     TOO_BIG                     = 15
  *     NOT_FOUND                   = 16
  *     ALREADY_EXISTS              = 17             # <<<<<<<<<<<<<<
  *     PERMISSIONS                 = 18
  *     BUSY                        = 19
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ALREADY_EXISTS, __pyx_int_17) < 0) __PYX_ERR(0, 385, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ALREADY_EXISTS, __pyx_int_17) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":386
+  /* "pyjoulescope_driver/binding.pyx":388
  *     NOT_FOUND                   = 16
  *     ALREADY_EXISTS              = 17
  *     PERMISSIONS                 = 18             # <<<<<<<<<<<<<<
  *     BUSY                        = 19
  *     UNAVAILABLE                 = 20
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_PERMISSIONS, __pyx_int_18) < 0) __PYX_ERR(0, 386, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_PERMISSIONS, __pyx_int_18) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":387
+  /* "pyjoulescope_driver/binding.pyx":389
  *     ALREADY_EXISTS              = 17
  *     PERMISSIONS                 = 18
  *     BUSY                        = 19             # <<<<<<<<<<<<<<
  *     UNAVAILABLE                 = 20
  *     IN_USE                      = 21
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_BUSY, __pyx_int_19) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_BUSY, __pyx_int_19) < 0) __PYX_ERR(0, 389, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":388
+  /* "pyjoulescope_driver/binding.pyx":390
  *     PERMISSIONS                 = 18
  *     BUSY                        = 19
  *     UNAVAILABLE                 = 20             # <<<<<<<<<<<<<<
  *     IN_USE                      = 21
  *     CLOSED                      = 22
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UNAVAILABLE, __pyx_int_20) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_UNAVAILABLE, __pyx_int_20) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":389
+  /* "pyjoulescope_driver/binding.pyx":391
  *     BUSY                        = 19
  *     UNAVAILABLE                 = 20
  *     IN_USE                      = 21             # <<<<<<<<<<<<<<
  *     CLOSED                      = 22
  *     SEQUENCE                    = 23
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_IN_USE, __pyx_int_21) < 0) __PYX_ERR(0, 389, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_IN_USE, __pyx_int_21) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":390
+  /* "pyjoulescope_driver/binding.pyx":392
  *     UNAVAILABLE                 = 20
  *     IN_USE                      = 21
  *     CLOSED                      = 22             # <<<<<<<<<<<<<<
  *     SEQUENCE                    = 23
  *     ABORTED                     = 24
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_CLOSED, __pyx_int_22) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_CLOSED, __pyx_int_22) < 0) __PYX_ERR(0, 392, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":391
+  /* "pyjoulescope_driver/binding.pyx":393
  *     IN_USE                      = 21
  *     CLOSED                      = 22
  *     SEQUENCE                    = 23             # <<<<<<<<<<<<<<
  *     ABORTED                     = 24
  *     SYNCHRONIZATION             = 25
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_SEQUENCE, __pyx_int_23) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_SEQUENCE, __pyx_int_23) < 0) __PYX_ERR(0, 393, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":392
+  /* "pyjoulescope_driver/binding.pyx":394
  *     CLOSED                      = 22
  *     SEQUENCE                    = 23
  *     ABORTED                     = 24             # <<<<<<<<<<<<<<
  *     SYNCHRONIZATION             = 25
  *     # ENUM_ERROR_CODE_END
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ABORTED, __pyx_int_24) < 0) __PYX_ERR(0, 392, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ABORTED, __pyx_int_24) < 0) __PYX_ERR(0, 394, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":393
+  /* "pyjoulescope_driver/binding.pyx":395
  *     SEQUENCE                    = 23
  *     ABORTED                     = 24
  *     SYNCHRONIZATION             = 25             # <<<<<<<<<<<<<<
  *     # ENUM_ERROR_CODE_END
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_SYNCHRONIZATION, __pyx_int_25) < 0) __PYX_ERR(0, 393, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_SYNCHRONIZATION, __pyx_int_25) < 0) __PYX_ERR(0, 395, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":365
+  /* "pyjoulescope_driver/binding.pyx":367
  * 
  * 
  * class ErrorCode:             # <<<<<<<<<<<<<<
  *     # automatically maintained by error_code_update.py
  *     # ENUM_ERROR_CODE_START
  */
-  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_ErrorCode, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_ErrorCode, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ErrorCode, __pyx_t_2) < 0) __PYX_ERR(0, 365, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ErrorCode, __pyx_t_2) < 0) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":400
+  /* "pyjoulescope_driver/binding.pyx":402
  *     # automatically maintained by error_code_update.py
  *     # ENUM_ERROR_CODE_META_START
  *     0: (0, 'SUCCESS', 'Success (no error)'),             # <<<<<<<<<<<<<<
  *     1: (1, 'UNSPECIFIED', 'Unspecified error'),
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(52); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(52); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_0, __pyx_tuple__39) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_0, __pyx_tuple__39) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":401
+  /* "pyjoulescope_driver/binding.pyx":403
  *     # ENUM_ERROR_CODE_META_START
  *     0: (0, 'SUCCESS', 'Success (no error)'),
  *     1: (1, 'UNSPECIFIED', 'Unspecified error'),             # <<<<<<<<<<<<<<
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_1, __pyx_tuple__40) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_1, __pyx_tuple__40) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":402
+  /* "pyjoulescope_driver/binding.pyx":404
  *     0: (0, 'SUCCESS', 'Success (no error)'),
  *     1: (1, 'UNSPECIFIED', 'Unspecified error'),
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),             # <<<<<<<<<<<<<<
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  *     4: (4, 'IO', 'Input/output error'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_2, __pyx_tuple__41) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_2, __pyx_tuple__41) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":403
+  /* "pyjoulescope_driver/binding.pyx":405
  *     1: (1, 'UNSPECIFIED', 'Unspecified error'),
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),             # <<<<<<<<<<<<<<
  *     4: (4, 'IO', 'Input/output error'),
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_3, __pyx_tuple__42) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_3, __pyx_tuple__42) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":404
+  /* "pyjoulescope_driver/binding.pyx":406
  *     2: (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  *     4: (4, 'IO', 'Input/output error'),             # <<<<<<<<<<<<<<
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_4, __pyx_tuple__43) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_4, __pyx_tuple__43) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":405
+  /* "pyjoulescope_driver/binding.pyx":407
  *     3: (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  *     4: (4, 'IO', 'Input/output error'),
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),             # <<<<<<<<<<<<<<
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_5, __pyx_tuple__44) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_5, __pyx_tuple__44) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":406
+  /* "pyjoulescope_driver/binding.pyx":408
  *     4: (4, 'IO', 'Input/output error'),
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),             # <<<<<<<<<<<<<<
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_6, __pyx_tuple__45) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_6, __pyx_tuple__45) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":407
+  /* "pyjoulescope_driver/binding.pyx":409
  *     5: (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),             # <<<<<<<<<<<<<<
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_7, __pyx_tuple__46) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_7, __pyx_tuple__46) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":408
+  /* "pyjoulescope_driver/binding.pyx":410
  *     6: (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),             # <<<<<<<<<<<<<<
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_8, __pyx_tuple__47) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_8, __pyx_tuple__47) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":409
+  /* "pyjoulescope_driver/binding.pyx":411
  *     7: (7, 'INVALID_CONTEXT', 'The context is invalid'),
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),             # <<<<<<<<<<<<<<
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_9, __pyx_tuple__48) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_9, __pyx_tuple__48) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":410
+  /* "pyjoulescope_driver/binding.pyx":412
  *     8: (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),             # <<<<<<<<<<<<<<
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),
  *     12: (12, 'FULL', 'The target of the operation is full'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_10, __pyx_tuple__49) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_10, __pyx_tuple__49) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":411
+  /* "pyjoulescope_driver/binding.pyx":413
  *     9: (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),             # <<<<<<<<<<<<<<
  *     12: (12, 'FULL', 'The target of the operation is full'),
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_11, __pyx_tuple__50) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_11, __pyx_tuple__50) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":412
+  /* "pyjoulescope_driver/binding.pyx":414
  *     10: (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),
  *     12: (12, 'FULL', 'The target of the operation is full'),             # <<<<<<<<<<<<<<
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_12, __pyx_tuple__51) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_12, __pyx_tuple__51) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":413
+  /* "pyjoulescope_driver/binding.pyx":415
  *     11: (11, 'TIMED_OUT', 'The operation did not complete in time'),
  *     12: (12, 'FULL', 'The target of the operation is full'),
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),             # <<<<<<<<<<<<<<
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_13, __pyx_tuple__52) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_13, __pyx_tuple__52) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":414
+  /* "pyjoulescope_driver/binding.pyx":416
  *     12: (12, 'FULL', 'The target of the operation is full'),
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),             # <<<<<<<<<<<<<<
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_14, __pyx_tuple__53) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_14, __pyx_tuple__53) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":415
+  /* "pyjoulescope_driver/binding.pyx":417
  *     13: (13, 'EMPTY', 'The target of the operation is empty'),
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),             # <<<<<<<<<<<<<<
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_15, __pyx_tuple__54) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_15, __pyx_tuple__54) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":416
+  /* "pyjoulescope_driver/binding.pyx":418
  *     14: (14, 'TOO_SMALL', 'The target of the operation is too small'),
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),             # <<<<<<<<<<<<<<
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_16, __pyx_tuple__55) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_16, __pyx_tuple__55) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":417
+  /* "pyjoulescope_driver/binding.pyx":419
  *     15: (15, 'TOO_BIG', 'The target of the operation is too big'),
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),             # <<<<<<<<<<<<<<
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_17, __pyx_tuple__56) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_17, __pyx_tuple__56) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":418
+  /* "pyjoulescope_driver/binding.pyx":420
  *     16: (16, 'NOT_FOUND', 'The requested resource was not found'),
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),             # <<<<<<<<<<<<<<
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_18, __pyx_tuple__57) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_18, __pyx_tuple__57) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":419
+  /* "pyjoulescope_driver/binding.pyx":421
  *     17: (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),             # <<<<<<<<<<<<<<
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_19, __pyx_tuple__58) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_19, __pyx_tuple__58) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":420
+  /* "pyjoulescope_driver/binding.pyx":422
  *     18: (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),             # <<<<<<<<<<<<<<
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_20, __pyx_tuple__59) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_20, __pyx_tuple__59) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":421
+  /* "pyjoulescope_driver/binding.pyx":423
  *     19: (19, 'BUSY', 'The requested resource is currently busy.'),
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),             # <<<<<<<<<<<<<<
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_21, __pyx_tuple__60) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_21, __pyx_tuple__60) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":422
+  /* "pyjoulescope_driver/binding.pyx":424
  *     20: (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),             # <<<<<<<<<<<<<<
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  *     24: (24, 'ABORTED', 'The requested operation was previously aborted.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_22, __pyx_tuple__61) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_22, __pyx_tuple__61) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":423
+  /* "pyjoulescope_driver/binding.pyx":425
  *     21: (21, 'IN_USE', 'The requested resource is currently in use.'),
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),             # <<<<<<<<<<<<<<
  *     24: (24, 'ABORTED', 'The requested operation was previously aborted.'),
  *     25: (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_23, __pyx_tuple__62) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_23, __pyx_tuple__62) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":424
+  /* "pyjoulescope_driver/binding.pyx":426
  *     22: (22, 'CLOSED', 'The requested resource is currently closed.'),
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  *     24: (24, 'ABORTED', 'The requested operation was previously aborted.'),             # <<<<<<<<<<<<<<
  *     25: (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),
  *     'SUCCESS': (0, 'SUCCESS', 'Success (no error)'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_24, __pyx_tuple__63) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_24, __pyx_tuple__63) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":425
+  /* "pyjoulescope_driver/binding.pyx":427
  *     23: (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  *     24: (24, 'ABORTED', 'The requested operation was previously aborted.'),
  *     25: (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),             # <<<<<<<<<<<<<<
  *     'SUCCESS': (0, 'SUCCESS', 'Success (no error)'),
  *     'UNSPECIFIED': (1, 'UNSPECIFIED', 'Unspecified error'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_25, __pyx_tuple__64) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_25, __pyx_tuple__64) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":426
+  /* "pyjoulescope_driver/binding.pyx":428
  *     24: (24, 'ABORTED', 'The requested operation was previously aborted.'),
  *     25: (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),
  *     'SUCCESS': (0, 'SUCCESS', 'Success (no error)'),             # <<<<<<<<<<<<<<
  *     'UNSPECIFIED': (1, 'UNSPECIFIED', 'Unspecified error'),
  *     'NOT_ENOUGH_MEMORY': (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_SUCCESS, __pyx_tuple__39) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_SUCCESS, __pyx_tuple__39) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":427
+  /* "pyjoulescope_driver/binding.pyx":429
  *     25: (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),
  *     'SUCCESS': (0, 'SUCCESS', 'Success (no error)'),
  *     'UNSPECIFIED': (1, 'UNSPECIFIED', 'Unspecified error'),             # <<<<<<<<<<<<<<
  *     'NOT_ENOUGH_MEMORY': (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  *     'NOT_SUPPORTED': (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_UNSPECIFIED, __pyx_tuple__40) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_UNSPECIFIED, __pyx_tuple__40) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":428
+  /* "pyjoulescope_driver/binding.pyx":430
  *     'SUCCESS': (0, 'SUCCESS', 'Success (no error)'),
  *     'UNSPECIFIED': (1, 'UNSPECIFIED', 'Unspecified error'),
  *     'NOT_ENOUGH_MEMORY': (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),             # <<<<<<<<<<<<<<
  *     'NOT_SUPPORTED': (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  *     'IO': (4, 'IO', 'Input/output error'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_NOT_ENOUGH_MEMORY, __pyx_tuple__41) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_NOT_ENOUGH_MEMORY, __pyx_tuple__41) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":429
+  /* "pyjoulescope_driver/binding.pyx":431
  *     'UNSPECIFIED': (1, 'UNSPECIFIED', 'Unspecified error'),
  *     'NOT_ENOUGH_MEMORY': (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  *     'NOT_SUPPORTED': (3, 'NOT_SUPPORTED', 'Operation is not supported'),             # <<<<<<<<<<<<<<
  *     'IO': (4, 'IO', 'Input/output error'),
  *     'PARAMETER_INVALID': (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_NOT_SUPPORTED, __pyx_tuple__42) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_NOT_SUPPORTED, __pyx_tuple__42) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":430
+  /* "pyjoulescope_driver/binding.pyx":432
  *     'NOT_ENOUGH_MEMORY': (2, 'NOT_ENOUGH_MEMORY', 'Insufficient memory to complete the operation'),
  *     'NOT_SUPPORTED': (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  *     'IO': (4, 'IO', 'Input/output error'),             # <<<<<<<<<<<<<<
  *     'PARAMETER_INVALID': (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  *     'INVALID_RETURN_CONDITION': (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_IO, __pyx_tuple__43) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_IO, __pyx_tuple__43) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":431
+  /* "pyjoulescope_driver/binding.pyx":433
  *     'NOT_SUPPORTED': (3, 'NOT_SUPPORTED', 'Operation is not supported'),
  *     'IO': (4, 'IO', 'Input/output error'),
  *     'PARAMETER_INVALID': (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),             # <<<<<<<<<<<<<<
  *     'INVALID_RETURN_CONDITION': (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  *     'INVALID_CONTEXT': (7, 'INVALID_CONTEXT', 'The context is invalid'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_PARAMETER_INVALID, __pyx_tuple__44) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_PARAMETER_INVALID, __pyx_tuple__44) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":432
+  /* "pyjoulescope_driver/binding.pyx":434
  *     'IO': (4, 'IO', 'Input/output error'),
  *     'PARAMETER_INVALID': (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  *     'INVALID_RETURN_CONDITION': (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),             # <<<<<<<<<<<<<<
  *     'INVALID_CONTEXT': (7, 'INVALID_CONTEXT', 'The context is invalid'),
  *     'INVALID_MESSAGE_LENGTH': (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_INVALID_RETURN_CONDITION, __pyx_tuple__45) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_INVALID_RETURN_CONDITION, __pyx_tuple__45) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":433
+  /* "pyjoulescope_driver/binding.pyx":435
  *     'PARAMETER_INVALID': (5, 'PARAMETER_INVALID', 'The parameter value is invalid'),
  *     'INVALID_RETURN_CONDITION': (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  *     'INVALID_CONTEXT': (7, 'INVALID_CONTEXT', 'The context is invalid'),             # <<<<<<<<<<<<<<
  *     'INVALID_MESSAGE_LENGTH': (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  *     'MESSAGE_INTEGRITY': (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_INVALID_CONTEXT, __pyx_tuple__46) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_INVALID_CONTEXT, __pyx_tuple__46) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":434
+  /* "pyjoulescope_driver/binding.pyx":436
  *     'INVALID_RETURN_CONDITION': (6, 'INVALID_RETURN_CONDITION', 'The function return condition is invalid'),
  *     'INVALID_CONTEXT': (7, 'INVALID_CONTEXT', 'The context is invalid'),
  *     'INVALID_MESSAGE_LENGTH': (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),             # <<<<<<<<<<<<<<
  *     'MESSAGE_INTEGRITY': (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  *     'SYNTAX_ERROR': (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_INVALID_MESSAGE_LENGTH, __pyx_tuple__47) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_INVALID_MESSAGE_LENGTH, __pyx_tuple__47) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":435
+  /* "pyjoulescope_driver/binding.pyx":437
  *     'INVALID_CONTEXT': (7, 'INVALID_CONTEXT', 'The context is invalid'),
  *     'INVALID_MESSAGE_LENGTH': (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  *     'MESSAGE_INTEGRITY': (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),             # <<<<<<<<<<<<<<
  *     'SYNTAX_ERROR': (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  *     'TIMED_OUT': (11, 'TIMED_OUT', 'The operation did not complete in time'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_MESSAGE_INTEGRITY, __pyx_tuple__48) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_MESSAGE_INTEGRITY, __pyx_tuple__48) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":436
+  /* "pyjoulescope_driver/binding.pyx":438
  *     'INVALID_MESSAGE_LENGTH': (8, 'INVALID_MESSAGE_LENGTH', 'The message length in invalid'),
  *     'MESSAGE_INTEGRITY': (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  *     'SYNTAX_ERROR': (10, 'SYNTAX_ERROR', 'A syntax error was detected'),             # <<<<<<<<<<<<<<
  *     'TIMED_OUT': (11, 'TIMED_OUT', 'The operation did not complete in time'),
  *     'FULL': (12, 'FULL', 'The target of the operation is full'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_SYNTAX_ERROR, __pyx_tuple__49) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_SYNTAX_ERROR, __pyx_tuple__49) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":437
+  /* "pyjoulescope_driver/binding.pyx":439
  *     'MESSAGE_INTEGRITY': (9, 'MESSAGE_INTEGRITY', 'The message integrity check failed'),
  *     'SYNTAX_ERROR': (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  *     'TIMED_OUT': (11, 'TIMED_OUT', 'The operation did not complete in time'),             # <<<<<<<<<<<<<<
  *     'FULL': (12, 'FULL', 'The target of the operation is full'),
  *     'EMPTY': (13, 'EMPTY', 'The target of the operation is empty'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_TIMED_OUT, __pyx_tuple__50) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_TIMED_OUT, __pyx_tuple__50) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":438
+  /* "pyjoulescope_driver/binding.pyx":440
  *     'SYNTAX_ERROR': (10, 'SYNTAX_ERROR', 'A syntax error was detected'),
  *     'TIMED_OUT': (11, 'TIMED_OUT', 'The operation did not complete in time'),
  *     'FULL': (12, 'FULL', 'The target of the operation is full'),             # <<<<<<<<<<<<<<
  *     'EMPTY': (13, 'EMPTY', 'The target of the operation is empty'),
  *     'TOO_SMALL': (14, 'TOO_SMALL', 'The target of the operation is too small'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_FULL, __pyx_tuple__51) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_FULL, __pyx_tuple__51) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":439
+  /* "pyjoulescope_driver/binding.pyx":441
  *     'TIMED_OUT': (11, 'TIMED_OUT', 'The operation did not complete in time'),
  *     'FULL': (12, 'FULL', 'The target of the operation is full'),
  *     'EMPTY': (13, 'EMPTY', 'The target of the operation is empty'),             # <<<<<<<<<<<<<<
  *     'TOO_SMALL': (14, 'TOO_SMALL', 'The target of the operation is too small'),
  *     'TOO_BIG': (15, 'TOO_BIG', 'The target of the operation is too big'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_EMPTY, __pyx_tuple__52) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_EMPTY, __pyx_tuple__52) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":440
+  /* "pyjoulescope_driver/binding.pyx":442
  *     'FULL': (12, 'FULL', 'The target of the operation is full'),
  *     'EMPTY': (13, 'EMPTY', 'The target of the operation is empty'),
  *     'TOO_SMALL': (14, 'TOO_SMALL', 'The target of the operation is too small'),             # <<<<<<<<<<<<<<
  *     'TOO_BIG': (15, 'TOO_BIG', 'The target of the operation is too big'),
  *     'NOT_FOUND': (16, 'NOT_FOUND', 'The requested resource was not found'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_TOO_SMALL, __pyx_tuple__53) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_TOO_SMALL, __pyx_tuple__53) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":441
+  /* "pyjoulescope_driver/binding.pyx":443
  *     'EMPTY': (13, 'EMPTY', 'The target of the operation is empty'),
  *     'TOO_SMALL': (14, 'TOO_SMALL', 'The target of the operation is too small'),
  *     'TOO_BIG': (15, 'TOO_BIG', 'The target of the operation is too big'),             # <<<<<<<<<<<<<<
  *     'NOT_FOUND': (16, 'NOT_FOUND', 'The requested resource was not found'),
  *     'ALREADY_EXISTS': (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_TOO_BIG, __pyx_tuple__54) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_TOO_BIG, __pyx_tuple__54) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":442
+  /* "pyjoulescope_driver/binding.pyx":444
  *     'TOO_SMALL': (14, 'TOO_SMALL', 'The target of the operation is too small'),
  *     'TOO_BIG': (15, 'TOO_BIG', 'The target of the operation is too big'),
  *     'NOT_FOUND': (16, 'NOT_FOUND', 'The requested resource was not found'),             # <<<<<<<<<<<<<<
  *     'ALREADY_EXISTS': (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  *     'PERMISSIONS': (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_NOT_FOUND, __pyx_tuple__55) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_NOT_FOUND, __pyx_tuple__55) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":443
+  /* "pyjoulescope_driver/binding.pyx":445
  *     'TOO_BIG': (15, 'TOO_BIG', 'The target of the operation is too big'),
  *     'NOT_FOUND': (16, 'NOT_FOUND', 'The requested resource was not found'),
  *     'ALREADY_EXISTS': (17, 'ALREADY_EXISTS', 'The requested resource already exists'),             # <<<<<<<<<<<<<<
  *     'PERMISSIONS': (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  *     'BUSY': (19, 'BUSY', 'The requested resource is currently busy.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_ALREADY_EXISTS, __pyx_tuple__56) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_ALREADY_EXISTS, __pyx_tuple__56) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":444
+  /* "pyjoulescope_driver/binding.pyx":446
  *     'NOT_FOUND': (16, 'NOT_FOUND', 'The requested resource was not found'),
  *     'ALREADY_EXISTS': (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  *     'PERMISSIONS': (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),             # <<<<<<<<<<<<<<
  *     'BUSY': (19, 'BUSY', 'The requested resource is currently busy.'),
  *     'UNAVAILABLE': (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_PERMISSIONS, __pyx_tuple__57) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_PERMISSIONS, __pyx_tuple__57) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":445
+  /* "pyjoulescope_driver/binding.pyx":447
  *     'ALREADY_EXISTS': (17, 'ALREADY_EXISTS', 'The requested resource already exists'),
  *     'PERMISSIONS': (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  *     'BUSY': (19, 'BUSY', 'The requested resource is currently busy.'),             # <<<<<<<<<<<<<<
  *     'UNAVAILABLE': (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  *     'IN_USE': (21, 'IN_USE', 'The requested resource is currently in use.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_BUSY, __pyx_tuple__58) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_BUSY, __pyx_tuple__58) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":446
+  /* "pyjoulescope_driver/binding.pyx":448
  *     'PERMISSIONS': (18, 'PERMISSIONS', 'Insufficient permissions to perform the operation.'),
  *     'BUSY': (19, 'BUSY', 'The requested resource is currently busy.'),
  *     'UNAVAILABLE': (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),             # <<<<<<<<<<<<<<
  *     'IN_USE': (21, 'IN_USE', 'The requested resource is currently in use.'),
  *     'CLOSED': (22, 'CLOSED', 'The requested resource is currently closed.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_UNAVAILABLE, __pyx_tuple__59) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_UNAVAILABLE, __pyx_tuple__59) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":447
+  /* "pyjoulescope_driver/binding.pyx":449
  *     'BUSY': (19, 'BUSY', 'The requested resource is currently busy.'),
  *     'UNAVAILABLE': (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  *     'IN_USE': (21, 'IN_USE', 'The requested resource is currently in use.'),             # <<<<<<<<<<<<<<
  *     'CLOSED': (22, 'CLOSED', 'The requested resource is currently closed.'),
  *     'SEQUENCE': (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_IN_USE, __pyx_tuple__60) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_IN_USE, __pyx_tuple__60) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":448
+  /* "pyjoulescope_driver/binding.pyx":450
  *     'UNAVAILABLE': (20, 'UNAVAILABLE', 'The requested resource is currently unavailable.'),
  *     'IN_USE': (21, 'IN_USE', 'The requested resource is currently in use.'),
  *     'CLOSED': (22, 'CLOSED', 'The requested resource is currently closed.'),             # <<<<<<<<<<<<<<
  *     'SEQUENCE': (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  *     'ABORTED': (24, 'ABORTED', 'The requested operation was previously aborted.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_CLOSED, __pyx_tuple__61) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_CLOSED, __pyx_tuple__61) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":449
+  /* "pyjoulescope_driver/binding.pyx":451
  *     'IN_USE': (21, 'IN_USE', 'The requested resource is currently in use.'),
  *     'CLOSED': (22, 'CLOSED', 'The requested resource is currently closed.'),
  *     'SEQUENCE': (23, 'SEQUENCE', 'The requested operation was out of sequence.'),             # <<<<<<<<<<<<<<
  *     'ABORTED': (24, 'ABORTED', 'The requested operation was previously aborted.'),
  *     'SYNCHRONIZATION': (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_SEQUENCE, __pyx_tuple__62) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_SEQUENCE, __pyx_tuple__62) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":450
+  /* "pyjoulescope_driver/binding.pyx":452
  *     'CLOSED': (22, 'CLOSED', 'The requested resource is currently closed.'),
  *     'SEQUENCE': (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  *     'ABORTED': (24, 'ABORTED', 'The requested operation was previously aborted.'),             # <<<<<<<<<<<<<<
  *     'SYNCHRONIZATION': (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),
  *     # ENUM_ERROR_CODE_META_END
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_ABORTED, __pyx_tuple__63) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_ABORTED, __pyx_tuple__63) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":451
+  /* "pyjoulescope_driver/binding.pyx":453
  *     'SEQUENCE': (23, 'SEQUENCE', 'The requested operation was out of sequence.'),
  *     'ABORTED': (24, 'ABORTED', 'The requested operation was previously aborted.'),
  *     'SYNCHRONIZATION': (25, 'SYNCHRONIZATION', 'The target is not synchronized with the originator.'),             # <<<<<<<<<<<<<<
  *     # ENUM_ERROR_CODE_META_END
  * }
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_SYNCHRONIZATION, __pyx_tuple__64) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_error_code_to_meta, __pyx_t_1) < 0) __PYX_ERR(0, 397, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_SYNCHRONIZATION, __pyx_tuple__64) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_error_code_to_meta, __pyx_t_1) < 0) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":456
+  /* "pyjoulescope_driver/binding.pyx":458
  * 
  * 
  * def error_code_to_str(ec):             # <<<<<<<<<<<<<<
  *     """Get the string representation for an error code.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_19pyjoulescope_driver_7binding_1error_code_to_str, NULL, __pyx_n_s_pyjoulescope_driver_binding); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 456, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_19pyjoulescope_driver_7binding_1error_code_to_str, NULL, __pyx_n_s_pyjoulescope_driver_binding); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_error_code_to_str, __pyx_t_1) < 0) __PYX_ERR(0, 456, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_error_code_to_str, __pyx_t_1) < 0) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":466
+  /* "pyjoulescope_driver/binding.pyx":468
  * 
  * 
  * class LogLevel:             # <<<<<<<<<<<<<<
  *     OFF         = -1
  *     EMERGENCY   = 0
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_LogLevel, __pyx_n_s_LogLevel, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_LogLevel, __pyx_n_s_LogLevel, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pyjoulescope_driver/binding.pyx":467
+  /* "pyjoulescope_driver/binding.pyx":469
  * 
  * class LogLevel:
  *     OFF         = -1             # <<<<<<<<<<<<<<
  *     EMERGENCY   = 0
  *     ALERT       = 1
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_OFF, __pyx_int_neg_1) < 0) __PYX_ERR(0, 467, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_OFF, __pyx_int_neg_1) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":468
+  /* "pyjoulescope_driver/binding.pyx":470
  * class LogLevel:
  *     OFF         = -1
  *     EMERGENCY   = 0             # <<<<<<<<<<<<<<
  *     ALERT       = 1
  *     CRITICAL    = 2
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_EMERGENCY, __pyx_int_0) < 0) __PYX_ERR(0, 468, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_EMERGENCY, __pyx_int_0) < 0) __PYX_ERR(0, 470, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":469
+  /* "pyjoulescope_driver/binding.pyx":471
  *     OFF         = -1
  *     EMERGENCY   = 0
  *     ALERT       = 1             # <<<<<<<<<<<<<<
  *     CRITICAL    = 2
  *     ERROR       = 3
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ALERT, __pyx_int_1) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ALERT, __pyx_int_1) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":470
+  /* "pyjoulescope_driver/binding.pyx":472
  *     EMERGENCY   = 0
  *     ALERT       = 1
  *     CRITICAL    = 2             # <<<<<<<<<<<<<<
  *     ERROR       = 3
  *     WARNING     = 4
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_CRITICAL, __pyx_int_2) < 0) __PYX_ERR(0, 470, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_CRITICAL, __pyx_int_2) < 0) __PYX_ERR(0, 472, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":471
+  /* "pyjoulescope_driver/binding.pyx":473
  *     ALERT       = 1
  *     CRITICAL    = 2
  *     ERROR       = 3             # <<<<<<<<<<<<<<
  *     WARNING     = 4
  *     NOTICE      = 5
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ERROR, __pyx_int_3) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ERROR, __pyx_int_3) < 0) __PYX_ERR(0, 473, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":472
+  /* "pyjoulescope_driver/binding.pyx":474
  *     CRITICAL    = 2
  *     ERROR       = 3
  *     WARNING     = 4             # <<<<<<<<<<<<<<
  *     NOTICE      = 5
  *     INFO        = 6
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_WARNING, __pyx_int_4) < 0) __PYX_ERR(0, 472, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_WARNING, __pyx_int_4) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":473
+  /* "pyjoulescope_driver/binding.pyx":475
  *     ERROR       = 3
  *     WARNING     = 4
  *     NOTICE      = 5             # <<<<<<<<<<<<<<
  *     INFO        = 6
  *     DEBUG1      = 7
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NOTICE, __pyx_int_5) < 0) __PYX_ERR(0, 473, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NOTICE, __pyx_int_5) < 0) __PYX_ERR(0, 475, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":474
+  /* "pyjoulescope_driver/binding.pyx":476
  *     WARNING     = 4
  *     NOTICE      = 5
  *     INFO        = 6             # <<<<<<<<<<<<<<
  *     DEBUG1      = 7
  *     DEBUG2      = 8
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INFO, __pyx_int_6) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_INFO, __pyx_int_6) < 0) __PYX_ERR(0, 476, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":475
+  /* "pyjoulescope_driver/binding.pyx":477
  *     NOTICE      = 5
  *     INFO        = 6
  *     DEBUG1      = 7             # <<<<<<<<<<<<<<
  *     DEBUG2      = 8
  *     DEBUG3      = 9
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_DEBUG1, __pyx_int_7) < 0) __PYX_ERR(0, 475, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_DEBUG1, __pyx_int_7) < 0) __PYX_ERR(0, 477, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":476
+  /* "pyjoulescope_driver/binding.pyx":478
  *     INFO        = 6
  *     DEBUG1      = 7
  *     DEBUG2      = 8             # <<<<<<<<<<<<<<
  *     DEBUG3      = 9
  *     ALL         = 10
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_DEBUG2, __pyx_int_8) < 0) __PYX_ERR(0, 476, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_DEBUG2, __pyx_int_8) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":477
+  /* "pyjoulescope_driver/binding.pyx":479
  *     DEBUG1      = 7
  *     DEBUG2      = 8
  *     DEBUG3      = 9             # <<<<<<<<<<<<<<
  *     ALL         = 10
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_DEBUG3, __pyx_int_9) < 0) __PYX_ERR(0, 477, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_DEBUG3, __pyx_int_9) < 0) __PYX_ERR(0, 479, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":478
+  /* "pyjoulescope_driver/binding.pyx":480
  *     DEBUG2      = 8
  *     DEBUG3      = 9
  *     ALL         = 10             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ALL, __pyx_int_10) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_ALL, __pyx_int_10) < 0) __PYX_ERR(0, 480, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":466
+  /* "pyjoulescope_driver/binding.pyx":468
  * 
  * 
  * class LogLevel:             # <<<<<<<<<<<<<<
  *     OFF         = -1
  *     EMERGENCY   = 0
  */
-  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_LogLevel, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_LogLevel, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LogLevel, __pyx_t_2) < 0) __PYX_ERR(0, 466, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LogLevel, __pyx_t_2) < 0) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":482
+  /* "pyjoulescope_driver/binding.pyx":484
  * 
  * _log_level_str_to_int = {
  *     'off': LogLevel.OFF,             # <<<<<<<<<<<<<<
  *     None: LogLevel.OFF,
  *     'emergency': LogLevel.EMERGENCY,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(23); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(23); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_OFF); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_OFF); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_off, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_off, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":483
+  /* "pyjoulescope_driver/binding.pyx":485
  * _log_level_str_to_int = {
  *     'off': LogLevel.OFF,
  *     None: LogLevel.OFF,             # <<<<<<<<<<<<<<
  *     'emergency': LogLevel.EMERGENCY,
  *     'e': LogLevel.EMERGENCY,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OFF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OFF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, Py_None, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, Py_None, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":484
+  /* "pyjoulescope_driver/binding.pyx":486
  *     'off': LogLevel.OFF,
  *     None: LogLevel.OFF,
  *     'emergency': LogLevel.EMERGENCY,             # <<<<<<<<<<<<<<
  *     'e': LogLevel.EMERGENCY,
  *     'alert': LogLevel.ALERT,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_EMERGENCY); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_EMERGENCY); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_emergency, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_emergency, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":485
+  /* "pyjoulescope_driver/binding.pyx":487
  *     None: LogLevel.OFF,
  *     'emergency': LogLevel.EMERGENCY,
  *     'e': LogLevel.EMERGENCY,             # <<<<<<<<<<<<<<
  *     'alert': LogLevel.ALERT,
  *     'a': LogLevel.ALERT,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 485, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_EMERGENCY); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 485, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_EMERGENCY); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_e, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_e, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":486
+  /* "pyjoulescope_driver/binding.pyx":488
  *     'emergency': LogLevel.EMERGENCY,
  *     'e': LogLevel.EMERGENCY,
  *     'alert': LogLevel.ALERT,             # <<<<<<<<<<<<<<
  *     'a': LogLevel.ALERT,
  *     'critical': LogLevel.CRITICAL,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 486, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 488, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ALERT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 486, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ALERT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 488, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_alert, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_alert, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":487
+  /* "pyjoulescope_driver/binding.pyx":489
  *     'e': LogLevel.EMERGENCY,
  *     'alert': LogLevel.ALERT,
  *     'a': LogLevel.ALERT,             # <<<<<<<<<<<<<<
  *     'critical': LogLevel.CRITICAL,
  *     'c': LogLevel.CRITICAL,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ALERT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 487, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ALERT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 489, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_a, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_a, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":488
+  /* "pyjoulescope_driver/binding.pyx":490
  *     'alert': LogLevel.ALERT,
  *     'a': LogLevel.ALERT,
  *     'critical': LogLevel.CRITICAL,             # <<<<<<<<<<<<<<
  *     'c': LogLevel.CRITICAL,
  *     'error': LogLevel.ERROR,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 488, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_critical, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_critical, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":489
+  /* "pyjoulescope_driver/binding.pyx":491
  *     'a': LogLevel.ALERT,
  *     'critical': LogLevel.CRITICAL,
  *     'c': LogLevel.CRITICAL,             # <<<<<<<<<<<<<<
  *     'error': LogLevel.ERROR,
  *     'e': LogLevel.ERROR,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_c, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_c, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":490
+  /* "pyjoulescope_driver/binding.pyx":492
  *     'critical': LogLevel.CRITICAL,
  *     'c': LogLevel.CRITICAL,
  *     'error': LogLevel.ERROR,             # <<<<<<<<<<<<<<
  *     'e': LogLevel.ERROR,
  *     'warn': LogLevel.WARNING,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 490, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_error, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_error, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":491
+  /* "pyjoulescope_driver/binding.pyx":493
  *     'c': LogLevel.CRITICAL,
  *     'error': LogLevel.ERROR,
  *     'e': LogLevel.ERROR,             # <<<<<<<<<<<<<<
  *     'warn': LogLevel.WARNING,
  *     'warning': LogLevel.WARNING,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_e, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_e, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":492
+  /* "pyjoulescope_driver/binding.pyx":494
  *     'error': LogLevel.ERROR,
  *     'e': LogLevel.ERROR,
  *     'warn': LogLevel.WARNING,             # <<<<<<<<<<<<<<
  *     'warning': LogLevel.WARNING,
  *     'w': LogLevel.WARNING,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 492, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_warn, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_warn, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":493
+  /* "pyjoulescope_driver/binding.pyx":495
  *     'e': LogLevel.ERROR,
  *     'warn': LogLevel.WARNING,
  *     'warning': LogLevel.WARNING,             # <<<<<<<<<<<<<<
  *     'w': LogLevel.WARNING,
  *     'notice': LogLevel.NOTICE,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 495, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 495, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_warning, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_warning, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":494
+  /* "pyjoulescope_driver/binding.pyx":496
  *     'warn': LogLevel.WARNING,
  *     'warning': LogLevel.WARNING,
  *     'w': LogLevel.WARNING,             # <<<<<<<<<<<<<<
  *     'notice': LogLevel.NOTICE,
  *     'n': LogLevel.NOTICE,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_w, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_w, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":495
+  /* "pyjoulescope_driver/binding.pyx":497
  *     'warning': LogLevel.WARNING,
  *     'w': LogLevel.WARNING,
  *     'notice': LogLevel.NOTICE,             # <<<<<<<<<<<<<<
  *     'n': LogLevel.NOTICE,
  *     'info': LogLevel.INFO,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NOTICE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NOTICE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_notice, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_notice, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":496
+  /* "pyjoulescope_driver/binding.pyx":498
  *     'w': LogLevel.WARNING,
  *     'notice': LogLevel.NOTICE,
  *     'n': LogLevel.NOTICE,             # <<<<<<<<<<<<<<
  *     'info': LogLevel.INFO,
  *     'i': LogLevel.INFO,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 496, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NOTICE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 496, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NOTICE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_n, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_n, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":497
+  /* "pyjoulescope_driver/binding.pyx":499
  *     'notice': LogLevel.NOTICE,
  *     'n': LogLevel.NOTICE,
  *     'info': LogLevel.INFO,             # <<<<<<<<<<<<<<
  *     'i': LogLevel.INFO,
  *     'debug1': LogLevel.DEBUG1,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_INFO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 497, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_INFO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_info, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_info, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":498
+  /* "pyjoulescope_driver/binding.pyx":500
  *     'n': LogLevel.NOTICE,
  *     'info': LogLevel.INFO,
  *     'i': LogLevel.INFO,             # <<<<<<<<<<<<<<
  *     'debug1': LogLevel.DEBUG1,
  *     'd': LogLevel.DEBUG1,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INFO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INFO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_i, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_i, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":499
+  /* "pyjoulescope_driver/binding.pyx":501
  *     'info': LogLevel.INFO,
  *     'i': LogLevel.INFO,
  *     'debug1': LogLevel.DEBUG1,             # <<<<<<<<<<<<<<
  *     'd': LogLevel.DEBUG1,
  *     'debug': LogLevel.DEBUG1,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 499, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 499, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_debug1, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_debug1, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":500
+  /* "pyjoulescope_driver/binding.pyx":502
  *     'i': LogLevel.INFO,
  *     'debug1': LogLevel.DEBUG1,
  *     'd': LogLevel.DEBUG1,             # <<<<<<<<<<<<<<
  *     'debug': LogLevel.DEBUG1,
  *     'debug2': LogLevel.DEBUG2,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 500, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DEBUG1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 500, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DEBUG1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_d, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_d, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":501
+  /* "pyjoulescope_driver/binding.pyx":503
  *     'debug1': LogLevel.DEBUG1,
  *     'd': LogLevel.DEBUG1,
  *     'debug': LogLevel.DEBUG1,             # <<<<<<<<<<<<<<
  *     'debug2': LogLevel.DEBUG2,
  *     'debug3': LogLevel.DEBUG3,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_debug, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_debug, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":502
+  /* "pyjoulescope_driver/binding.pyx":504
  *     'd': LogLevel.DEBUG1,
  *     'debug': LogLevel.DEBUG1,
  *     'debug2': LogLevel.DEBUG2,             # <<<<<<<<<<<<<<
  *     'debug3': LogLevel.DEBUG3,
  *     'all': LogLevel.ALL,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DEBUG2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DEBUG2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_debug2, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_debug2, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":503
+  /* "pyjoulescope_driver/binding.pyx":505
  *     'debug': LogLevel.DEBUG1,
  *     'debug2': LogLevel.DEBUG2,
  *     'debug3': LogLevel.DEBUG3,             # <<<<<<<<<<<<<<
  *     'all': LogLevel.ALL,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DEBUG3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_debug3, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_debug3, __pyx_t_2) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":504
+  /* "pyjoulescope_driver/binding.pyx":506
  *     'debug2': LogLevel.DEBUG2,
  *     'debug3': LogLevel.DEBUG3,
  *     'all': LogLevel.ALL,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 504, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ALL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 504, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ALL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_all_2, __pyx_t_3) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_all_2, __pyx_t_3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_level_str_to_int, __pyx_t_1) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_level_str_to_int, __pyx_t_1) < 0) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":509
+  /* "pyjoulescope_driver/binding.pyx":511
  * 
  * _log_level_c_to_py = {
  *     LogLevel.OFF: None,             # <<<<<<<<<<<<<<
  *     LogLevel.EMERGENCY: logging.CRITICAL,
  *     LogLevel.ALERT: logging.CRITICAL,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OFF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OFF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_2, Py_None) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_2, Py_None) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":510
+  /* "pyjoulescope_driver/binding.pyx":512
  * _log_level_c_to_py = {
  *     LogLevel.OFF: None,
  *     LogLevel.EMERGENCY: logging.CRITICAL,             # <<<<<<<<<<<<<<
  *     LogLevel.ALERT: logging.CRITICAL,
  *     LogLevel.CRITICAL: logging.CRITICAL,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_EMERGENCY); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_EMERGENCY); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":511
+  /* "pyjoulescope_driver/binding.pyx":513
  *     LogLevel.OFF: None,
  *     LogLevel.EMERGENCY: logging.CRITICAL,
  *     LogLevel.ALERT: logging.CRITICAL,             # <<<<<<<<<<<<<<
  *     LogLevel.CRITICAL: logging.CRITICAL,
  *     LogLevel.ERROR: logging.ERROR,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ALERT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ALERT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":512
+  /* "pyjoulescope_driver/binding.pyx":514
  *     LogLevel.EMERGENCY: logging.CRITICAL,
  *     LogLevel.ALERT: logging.CRITICAL,
  *     LogLevel.CRITICAL: logging.CRITICAL,             # <<<<<<<<<<<<<<
  *     LogLevel.ERROR: logging.ERROR,
  *     LogLevel.WARNING: logging.WARNING,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":513
+  /* "pyjoulescope_driver/binding.pyx":515
  *     LogLevel.ALERT: logging.CRITICAL,
  *     LogLevel.CRITICAL: logging.CRITICAL,
  *     LogLevel.ERROR: logging.ERROR,             # <<<<<<<<<<<<<<
  *     LogLevel.WARNING: logging.WARNING,
  *     LogLevel.NOTICE: logging.INFO,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":514
+  /* "pyjoulescope_driver/binding.pyx":516
  *     LogLevel.CRITICAL: logging.CRITICAL,
  *     LogLevel.ERROR: logging.ERROR,
  *     LogLevel.WARNING: logging.WARNING,             # <<<<<<<<<<<<<<
  *     LogLevel.NOTICE: logging.INFO,
  *     LogLevel.INFO: logging.INFO,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_WARNING); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":515
+  /* "pyjoulescope_driver/binding.pyx":517
  *     LogLevel.ERROR: logging.ERROR,
  *     LogLevel.WARNING: logging.WARNING,
  *     LogLevel.NOTICE: logging.INFO,             # <<<<<<<<<<<<<<
  *     LogLevel.INFO: logging.INFO,
  *     LogLevel.DEBUG1: logging.DEBUG,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 517, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_NOTICE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_NOTICE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 517, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 517, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_INFO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_INFO); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 517, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":516
+  /* "pyjoulescope_driver/binding.pyx":518
  *     LogLevel.WARNING: logging.WARNING,
  *     LogLevel.NOTICE: logging.INFO,
  *     LogLevel.INFO: logging.INFO,             # <<<<<<<<<<<<<<
  *     LogLevel.DEBUG1: logging.DEBUG,
  *     LogLevel.DEBUG2: logging.DEBUG,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INFO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INFO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INFO); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INFO); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":517
+  /* "pyjoulescope_driver/binding.pyx":519
  *     LogLevel.NOTICE: logging.INFO,
  *     LogLevel.INFO: logging.INFO,
  *     LogLevel.DEBUG1: logging.DEBUG,             # <<<<<<<<<<<<<<
  *     LogLevel.DEBUG2: logging.DEBUG,
  *     LogLevel.DEBUG3: logging.DEBUG,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 517, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 519, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DEBUG1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 517, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DEBUG1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 519, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 517, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 519, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 517, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":518
+  /* "pyjoulescope_driver/binding.pyx":520
  *     LogLevel.INFO: logging.INFO,
  *     LogLevel.DEBUG1: logging.DEBUG,
  *     LogLevel.DEBUG2: logging.DEBUG,             # <<<<<<<<<<<<<<
  *     LogLevel.DEBUG3: logging.DEBUG,
  *     LogLevel.ALL: logging.NOTSET,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DEBUG2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DEBUG2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 520, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":519
+  /* "pyjoulescope_driver/binding.pyx":521
  *     LogLevel.DEBUG1: logging.DEBUG,
  *     LogLevel.DEBUG2: logging.DEBUG,
  *     LogLevel.DEBUG3: logging.DEBUG,             # <<<<<<<<<<<<<<
  *     LogLevel.ALL: logging.NOTSET,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DEBUG3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DEBUG3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DEBUG); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_2) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":520
+  /* "pyjoulescope_driver/binding.pyx":522
  *     LogLevel.DEBUG2: logging.DEBUG,
  *     LogLevel.DEBUG3: logging.DEBUG,
  *     LogLevel.ALL: logging.NOTSET,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogLevel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ALL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ALL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NOTSET); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_NOTSET); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 509, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_t_3, __pyx_t_5) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_level_c_to_py, __pyx_t_1) < 0) __PYX_ERR(0, 508, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_level_c_to_py, __pyx_t_1) < 0) __PYX_ERR(0, 510, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":524
+  /* "pyjoulescope_driver/binding.pyx":526
  * 
  * 
  * def log_level_c_to_py(lvl):             # <<<<<<<<<<<<<<
  *     return _log_level_c_to_py.get(int(lvl))
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_19pyjoulescope_driver_7binding_3log_level_c_to_py, NULL, __pyx_n_s_pyjoulescope_driver_binding); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 524, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_19pyjoulescope_driver_7binding_3log_level_c_to_py, NULL, __pyx_n_s_pyjoulescope_driver_binding); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_level_c_to_py_2, __pyx_t_1) < 0) __PYX_ERR(0, 524, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_level_c_to_py_2, __pyx_t_1) < 0) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":528
+  /* "pyjoulescope_driver/binding.pyx":530
  * 
  * 
  * class SubscribeFlags:             # <<<<<<<<<<<<<<
  *     NONE = 0                ## No flags (always 0).
  *     RETAIN = (1 << 0)       ## Immediately forward retained PUB and/or METADATA, depending upon JSDRV_PUBSUB_SFLAG_PUB and JSDRV_PUBSUB_SFLAG_METADATA_RSP.
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SubscribeFlags, __pyx_n_s_SubscribeFlags, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SubscribeFlags, __pyx_n_s_SubscribeFlags, (PyObject *) NULL, __pyx_n_s_pyjoulescope_driver_binding, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 530, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pyjoulescope_driver/binding.pyx":529
+  /* "pyjoulescope_driver/binding.pyx":531
  * 
  * class SubscribeFlags:
  *     NONE = 0                ## No flags (always 0).             # <<<<<<<<<<<<<<
  *     RETAIN = (1 << 0)       ## Immediately forward retained PUB and/or METADATA, depending upon JSDRV_PUBSUB_SFLAG_PUB and JSDRV_PUBSUB_SFLAG_METADATA_RSP.
  *     PUB = (1 << 1)          ## Do not receive normal topic publish.
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NONE, __pyx_int_0) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_NONE, __pyx_int_0) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":530
+  /* "pyjoulescope_driver/binding.pyx":532
  * class SubscribeFlags:
  *     NONE = 0                ## No flags (always 0).
  *     RETAIN = (1 << 0)       ## Immediately forward retained PUB and/or METADATA, depending upon JSDRV_PUBSUB_SFLAG_PUB and JSDRV_PUBSUB_SFLAG_METADATA_RSP.             # <<<<<<<<<<<<<<
  *     PUB = (1 << 1)          ## Do not receive normal topic publish.
  *     METADATA_REQ = (1 << 2) ## Subscribe to receive metadata requests like "%", "a/b/%", and "a/b/c%".
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_RETAIN, __pyx_int_1) < 0) __PYX_ERR(0, 530, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_RETAIN, __pyx_int_1) < 0) __PYX_ERR(0, 532, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":531
+  /* "pyjoulescope_driver/binding.pyx":533
  *     NONE = 0                ## No flags (always 0).
  *     RETAIN = (1 << 0)       ## Immediately forward retained PUB and/or METADATA, depending upon JSDRV_PUBSUB_SFLAG_PUB and JSDRV_PUBSUB_SFLAG_METADATA_RSP.
  *     PUB = (1 << 1)          ## Do not receive normal topic publish.             # <<<<<<<<<<<<<<
  *     METADATA_REQ = (1 << 2) ## Subscribe to receive metadata requests like "%", "a/b/%", and "a/b/c%".
  *     METADATA_RSP = (1 << 3) ## Subscribe to receive metadata responses like "a/b/c$.
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_PUB, __pyx_int_2) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_PUB, __pyx_int_2) < 0) __PYX_ERR(0, 533, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":532
+  /* "pyjoulescope_driver/binding.pyx":534
  *     RETAIN = (1 << 0)       ## Immediately forward retained PUB and/or METADATA, depending upon JSDRV_PUBSUB_SFLAG_PUB and JSDRV_PUBSUB_SFLAG_METADATA_RSP.
  *     PUB = (1 << 1)          ## Do not receive normal topic publish.
  *     METADATA_REQ = (1 << 2) ## Subscribe to receive metadata requests like "%", "a/b/%", and "a/b/c%".             # <<<<<<<<<<<<<<
  *     METADATA_RSP = (1 << 3) ## Subscribe to receive metadata responses like "a/b/c$.
  *     QUERY_REQ = (1 << 4)    ## Subscribe to receive query requests like "&", "a/b/&", and "a/b/c&".
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_METADATA_REQ, __pyx_int_4) < 0) __PYX_ERR(0, 532, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_METADATA_REQ, __pyx_int_4) < 0) __PYX_ERR(0, 534, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":533
+  /* "pyjoulescope_driver/binding.pyx":535
  *     PUB = (1 << 1)          ## Do not receive normal topic publish.
  *     METADATA_REQ = (1 << 2) ## Subscribe to receive metadata requests like "%", "a/b/%", and "a/b/c%".
  *     METADATA_RSP = (1 << 3) ## Subscribe to receive metadata responses like "a/b/c$.             # <<<<<<<<<<<<<<
  *     QUERY_REQ = (1 << 4)    ## Subscribe to receive query requests like "&", "a/b/&", and "a/b/c&".
  *     QUERY_RSP = (1 << 5)    ## Subscribe to receive query responses like "a/b/c?".
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_METADATA_RSP, __pyx_int_8) < 0) __PYX_ERR(0, 533, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_METADATA_RSP, __pyx_int_8) < 0) __PYX_ERR(0, 535, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":534
+  /* "pyjoulescope_driver/binding.pyx":536
  *     METADATA_REQ = (1 << 2) ## Subscribe to receive metadata requests like "%", "a/b/%", and "a/b/c%".
  *     METADATA_RSP = (1 << 3) ## Subscribe to receive metadata responses like "a/b/c$.
  *     QUERY_REQ = (1 << 4)    ## Subscribe to receive query requests like "&", "a/b/&", and "a/b/c&".             # <<<<<<<<<<<<<<
  *     QUERY_RSP = (1 << 5)    ## Subscribe to receive query responses like "a/b/c?".
  *     RETURN_CODE = (1 << 6)  ## Subscribe to receive return code messages like "a/b/c#".
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_QUERY_REQ, __pyx_int_16) < 0) __PYX_ERR(0, 534, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_QUERY_REQ, __pyx_int_16) < 0) __PYX_ERR(0, 536, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":535
+  /* "pyjoulescope_driver/binding.pyx":537
  *     METADATA_RSP = (1 << 3) ## Subscribe to receive metadata responses like "a/b/c$.
  *     QUERY_REQ = (1 << 4)    ## Subscribe to receive query requests like "&", "a/b/&", and "a/b/c&".
  *     QUERY_RSP = (1 << 5)    ## Subscribe to receive query responses like "a/b/c?".             # <<<<<<<<<<<<<<
  *     RETURN_CODE = (1 << 6)  ## Subscribe to receive return code messages like "a/b/c#".
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_QUERY_RSP, __pyx_int_32) < 0) __PYX_ERR(0, 535, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_QUERY_RSP, __pyx_int_32) < 0) __PYX_ERR(0, 537, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":536
+  /* "pyjoulescope_driver/binding.pyx":538
  *     QUERY_REQ = (1 << 4)    ## Subscribe to receive query requests like "&", "a/b/&", and "a/b/c&".
  *     QUERY_RSP = (1 << 5)    ## Subscribe to receive query responses like "a/b/c?".
  *     RETURN_CODE = (1 << 6)  ## Subscribe to receive return code messages like "a/b/c#".             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_RETURN_CODE, __pyx_int_64) < 0) __PYX_ERR(0, 536, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_RETURN_CODE, __pyx_int_64) < 0) __PYX_ERR(0, 538, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":528
+  /* "pyjoulescope_driver/binding.pyx":530
  * 
  * 
  * class SubscribeFlags:             # <<<<<<<<<<<<<<
  *     NONE = 0                ## No flags (always 0).
  *     RETAIN = (1 << 0)       ## Immediately forward retained PUB and/or METADATA, depending upon JSDRV_PUBSUB_SFLAG_PUB and JSDRV_PUBSUB_SFLAG_METADATA_RSP.
  */
-  __pyx_t_5 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_SubscribeFlags, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_SubscribeFlags, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 530, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SubscribeFlags, __pyx_t_5) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SubscribeFlags, __pyx_t_5) < 0) __PYX_ERR(0, 530, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":540
+  /* "pyjoulescope_driver/binding.pyx":542
  * 
  * _SUBSCRIBE_FLAG_LOOKUP = {
  *     None: SubscribeFlags.PUB | SubscribeFlags.RETAIN,             # <<<<<<<<<<<<<<
  *     'pub': SubscribeFlags.PUB,
  *     'pub_retain': SubscribeFlags.PUB | SubscribeFlags.RETAIN,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_PUB); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_PUB); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_RETAIN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_RETAIN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyNumber_Or(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Or(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, Py_None, __pyx_t_5) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, Py_None, __pyx_t_5) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":541
+  /* "pyjoulescope_driver/binding.pyx":543
  * _SUBSCRIBE_FLAG_LOOKUP = {
  *     None: SubscribeFlags.PUB | SubscribeFlags.RETAIN,
  *     'pub': SubscribeFlags.PUB,             # <<<<<<<<<<<<<<
  *     'pub_retain': SubscribeFlags.PUB | SubscribeFlags.RETAIN,
  *     'metadata_req': SubscribeFlags.METADATA_REQ,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_PUB); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_PUB); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_pub, __pyx_t_2) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_pub, __pyx_t_2) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":542
+  /* "pyjoulescope_driver/binding.pyx":544
  *     None: SubscribeFlags.PUB | SubscribeFlags.RETAIN,
  *     'pub': SubscribeFlags.PUB,
  *     'pub_retain': SubscribeFlags.PUB | SubscribeFlags.RETAIN,             # <<<<<<<<<<<<<<
  *     'metadata_req': SubscribeFlags.METADATA_REQ,
  *     'metadata_rsp': SubscribeFlags.METADATA_RSP,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_PUB); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_PUB); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RETAIN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RETAIN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Or(__pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Or(__pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_pub_retain, __pyx_t_2) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_pub_retain, __pyx_t_2) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":543
+  /* "pyjoulescope_driver/binding.pyx":545
  *     'pub': SubscribeFlags.PUB,
  *     'pub_retain': SubscribeFlags.PUB | SubscribeFlags.RETAIN,
  *     'metadata_req': SubscribeFlags.METADATA_REQ,             # <<<<<<<<<<<<<<
  *     'metadata_rsp': SubscribeFlags.METADATA_RSP,
  *     'metadata_rsp_retain': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_METADATA_REQ); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_METADATA_REQ); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata_req, __pyx_t_3) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata_req, __pyx_t_3) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":544
+  /* "pyjoulescope_driver/binding.pyx":546
  *     'pub_retain': SubscribeFlags.PUB | SubscribeFlags.RETAIN,
  *     'metadata_req': SubscribeFlags.METADATA_REQ,
  *     'metadata_rsp': SubscribeFlags.METADATA_RSP,             # <<<<<<<<<<<<<<
  *     'metadata_rsp_retain': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,
  *     'metadata': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 544, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_METADATA_RSP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_METADATA_RSP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata_rsp, __pyx_t_2) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata_rsp, __pyx_t_2) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":545
+  /* "pyjoulescope_driver/binding.pyx":547
  *     'metadata_req': SubscribeFlags.METADATA_REQ,
  *     'metadata_rsp': SubscribeFlags.METADATA_RSP,
  *     'metadata_rsp_retain': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,             # <<<<<<<<<<<<<<
  *     'metadata': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,
  *     'query_req': SubscribeFlags.QUERY_REQ,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_METADATA_RSP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_METADATA_RSP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RETAIN); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RETAIN); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Or(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Or(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata_rsp_retain, __pyx_t_2) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata_rsp_retain, __pyx_t_2) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":546
+  /* "pyjoulescope_driver/binding.pyx":548
  *     'metadata_rsp': SubscribeFlags.METADATA_RSP,
  *     'metadata_rsp_retain': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,
  *     'metadata': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,             # <<<<<<<<<<<<<<
  *     'query_req': SubscribeFlags.QUERY_REQ,
  *     'query_rsp': SubscribeFlags.QUERY_RSP,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_METADATA_RSP); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_METADATA_RSP); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RETAIN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RETAIN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Or(__pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Or(__pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata, __pyx_t_2) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata, __pyx_t_2) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":547
+  /* "pyjoulescope_driver/binding.pyx":549
  *     'metadata_rsp_retain': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,
  *     'metadata': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,
  *     'query_req': SubscribeFlags.QUERY_REQ,             # <<<<<<<<<<<<<<
  *     'query_rsp': SubscribeFlags.QUERY_RSP,
  *     'return_code': SubscribeFlags.RETURN_CODE,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 549, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_QUERY_REQ); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 547, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_QUERY_REQ); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 549, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_query_req, __pyx_t_3) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_query_req, __pyx_t_3) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":548
+  /* "pyjoulescope_driver/binding.pyx":550
  *     'metadata': SubscribeFlags.METADATA_RSP | SubscribeFlags.RETAIN,
  *     'query_req': SubscribeFlags.QUERY_REQ,
  *     'query_rsp': SubscribeFlags.QUERY_RSP,             # <<<<<<<<<<<<<<
  *     'return_code': SubscribeFlags.RETURN_CODE,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_QUERY_RSP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_QUERY_RSP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_query_rsp, __pyx_t_2) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_query_rsp, __pyx_t_2) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":549
+  /* "pyjoulescope_driver/binding.pyx":551
  *     'query_req': SubscribeFlags.QUERY_REQ,
  *     'query_rsp': SubscribeFlags.QUERY_RSP,
  *     'return_code': SubscribeFlags.RETURN_CODE,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 549, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SubscribeFlags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 551, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RETURN_CODE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 549, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RETURN_CODE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 551, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_return_code, __pyx_t_3) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_return_code, __pyx_t_3) < 0) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SUBSCRIBE_FLAG_LOOKUP, __pyx_t_1) < 0) __PYX_ERR(0, 539, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SUBSCRIBE_FLAG_LOOKUP, __pyx_t_1) < 0) __PYX_ERR(0, 541, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":554
+  /* "pyjoulescope_driver/binding.pyx":556
  * 
  * _DEVICE_OPEN_MODES = {
  *     0: 0,             # <<<<<<<<<<<<<<
  *     'defaults': 0,
  *     None: 0,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 554, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_0, __pyx_int_0) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_defaults, __pyx_int_0) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_0, __pyx_int_0) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_defaults, __pyx_int_0) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":556
+  /* "pyjoulescope_driver/binding.pyx":558
  *     0: 0,
  *     'defaults': 0,
  *     None: 0,             # <<<<<<<<<<<<<<
  *     1: 1,
  *     'restore': 1,
  */
-  if (PyDict_SetItem(__pyx_t_1, Py_None, __pyx_int_0) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_1, __pyx_int_1) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_restore, __pyx_int_1) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_int_255, __pyx_int_255) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_raw, __pyx_int_255) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DEVICE_OPEN_MODES, __pyx_t_1) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, Py_None, __pyx_int_0) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_1, __pyx_int_1) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_restore, __pyx_int_1) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_int_255, __pyx_int_255) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_raw, __pyx_int_255) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DEVICE_OPEN_MODES, __pyx_t_1) < 0) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":564
+  /* "pyjoulescope_driver/binding.pyx":566
  * 
  * 
  * cdef int32_t _driver_count = 0             # <<<<<<<<<<<<<<
  * _TIMEOUT_MS_DEFAULT = 1000
  * _TIMEOUT_MS_INIT = 5000
  */
   __pyx_v_19pyjoulescope_driver_7binding__driver_count = 0;
 
-  /* "pyjoulescope_driver/binding.pyx":565
+  /* "pyjoulescope_driver/binding.pyx":567
  * 
  * cdef int32_t _driver_count = 0
  * _TIMEOUT_MS_DEFAULT = 1000             # <<<<<<<<<<<<<<
  * _TIMEOUT_MS_INIT = 5000
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TIMEOUT_MS_DEFAULT, __pyx_int_1000) < 0) __PYX_ERR(0, 565, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TIMEOUT_MS_DEFAULT, __pyx_int_1000) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":566
+  /* "pyjoulescope_driver/binding.pyx":568
  * cdef int32_t _driver_count = 0
  * _TIMEOUT_MS_DEFAULT = 1000
  * _TIMEOUT_MS_INIT = 5000             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TIMEOUT_MS_INIT, __pyx_int_5000) < 0) __PYX_ERR(0, 566, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TIMEOUT_MS_INIT, __pyx_int_5000) < 0) __PYX_ERR(0, 568, __pyx_L1_error)
 
-  /* "pyjoulescope_driver/binding.pyx":577
+  /* "pyjoulescope_driver/binding.pyx":579
  * 
  * 
  * def _handle_rc(rc, src, cause=None):             # <<<<<<<<<<<<<<
  *     if rc:
  *         if cause:
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_19pyjoulescope_driver_7binding_5_handle_rc, NULL, __pyx_n_s_pyjoulescope_driver_binding); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_19pyjoulescope_driver_7binding_5_handle_rc, NULL, __pyx_n_s_pyjoulescope_driver_binding); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_handle_rc, __pyx_t_1) < 0) __PYX_ERR(0, 577, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_handle_rc, __pyx_t_1) < 0) __PYX_ERR(0, 579, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyjoulescope_driver/binding.pyx":1
  * # Copyright 2022-2023 Jetperch LLC             # <<<<<<<<<<<<<<
  * #
  * # Licensed under the Apache License, Version 2.0 (the "License");
  */
```

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/__init__.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import gpi, info, program, record, scan, set_parameter, statistics, threads
+from . import api_timeout, gpi, info, program, record, scan, set_parameter, statistics, threads
 
-__all__ = [gpi, info, program, record, scan, set_parameter, statistics, threads]
+__all__ = [api_timeout, gpi, info, program, record, scan, set_parameter, statistics, threads]
 """This list of available command modules.  Each module must contain a 
 parser_config(subparser) function.  The function must return the callable(args)
 that will be executed for the command."""
```

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/gpi.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/gpi.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/info.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/program.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/program.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/record.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/record.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/scan.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/scan.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/set_parameter.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/set_parameter.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/entry_points/statistics.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/entry_points/statistics.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/img_alpha.img` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_alpha.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/img_beta.img` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_beta.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/img_stable.img` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/img_stable.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/program.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/program.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/record.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/record.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 
 import copy
 import numpy as np
 from pyjoulescope_driver import time64
 import logging
 
 
+_PYJLS_VERSION_MIN = (0, 5, 0)  # inclusive
+_PYJLS_VERSION_MAX = (1, 0, 0)  # exclusive
+
+
 try:
-    from pyjls import Writer, SignalType, DataType
+    from pyjls import Writer, SignalType, DataType, __version__
     _DTYPE_MAP = {
         'f32': DataType.F32,
         'u8': DataType.U8,
         'u4': DataType.U4,
         'u1': DataType.U1,
     }
 except ImportError:
@@ -127,14 +131,19 @@
     Call :meth:`open` to start recording and :meth:`close` to stop.
     """
 
     def __init__(self, driver, device_path, signals=None):
         if Writer is None:
             raise RuntimeError('pyjls package not found.  Install using:\n' +
                                '  pip3 install -U pyjls')
+        pyjls_version = [int(x) for x in __version__.split('.')]
+        if pyjls_version < _PYJLS_VERSION_MIN or pyjls_version >= _PYJLS_VERSION_MAX:
+            raise ImportError(f'Unsupported pyjls version {__version__}\n' +
+                              f'  Require {_PYJLS_VERSION_MIN} <= pyjls version < {_PYJLS_VERSION_MAX}\n' +
+                              '  pip3 install -U pyjls')
         self._utc_interval = time64.MINUTE
         self._log = logging.getLogger(__name__)
         self._wr = None
         self._data_map = {}
         self._driver = driver
         self._device_path = device_path
         self._on_data_fn = self._on_data  # bind and save for unsubscribe
```

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/release.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/release.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/test/test_release.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/test_release.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/test/test_time64.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/test/test_time64.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/time64.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/time64.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver/version.py` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 __title__ = "pyjoulescope_driver"
 __description__ = 'Joulescope™ driver'
 __url__ = 'https://joulescope.readthedocs.io'
 __author__ = 'Jetperch LLC'
 __author_email__ = 'joulescope-dev@jetperch.com'
 __license__ = 'Apache 2.0'
```

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver.egg-info/PKG-INFO` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoulescope-driver
-Version: 1.3.2
+Version: 1.3.3
 Summary: Joulescope™ driver
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjoulescope_driver-1.3.2/pyjoulescope_driver.egg-info/SOURCES.txt` & `pyjoulescope_driver-1.3.3/pyjoulescope_driver.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 pyjoulescope_driver.egg-info/PKG-INFO
 pyjoulescope_driver.egg-info/SOURCES.txt
 pyjoulescope_driver.egg-info/dependency_links.txt
 pyjoulescope_driver.egg-info/entry_points.txt
 pyjoulescope_driver.egg-info/requires.txt
 pyjoulescope_driver.egg-info/top_level.txt
 pyjoulescope_driver/entry_points/__init__.py
+pyjoulescope_driver/entry_points/api_timeout.py
 pyjoulescope_driver/entry_points/gpi.py
 pyjoulescope_driver/entry_points/info.py
 pyjoulescope_driver/entry_points/program.py
 pyjoulescope_driver/entry_points/record.py
 pyjoulescope_driver/entry_points/scan.py
 pyjoulescope_driver/entry_points/set_parameter.py
 pyjoulescope_driver/entry_points/statistics.py
```

### Comparing `pyjoulescope_driver-1.3.2/pyproject.toml` & `pyjoulescope_driver-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/setup.py` & `pyjoulescope_driver-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/backend/libusb/backend.c` & `pyjoulescope_driver-1.3.3/src/backend/libusb/backend.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/backend/libusb/msg_queue.c` & `pyjoulescope_driver-1.3.3/src/backend/libusb/msg_queue.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/backend/posix.c` & `pyjoulescope_driver-1.3.3/src/backend/posix.c`

 * *Files 5% similar despite different names*

```diff
@@ -56,33 +56,39 @@
         return NULL;
     }
     jsdrv_cstr_copy(mutex->name, name, sizeof(mutex->name));
     return mutex;
 }
 
 void jsdrv_os_mutex_free(jsdrv_os_mutex_t mutex) {
-    pthread_mutex_destroy(&mutex->mutex);
-    jsdrv_free(mutex);
+    if (NULL != mutex) {
+        pthread_mutex_destroy(&mutex->mutex);
+        jsdrv_free(mutex);
+    }
 }
 
 void jsdrv_os_mutex_lock(jsdrv_os_mutex_t mutex) {
     char msg[128];
-    int rc = pthread_mutex_lock(&mutex->mutex);
-    if (rc) {
-        snprintf(msg, sizeof(msg), "mutex lock '%s' failed %d", mutex->name, rc);
-        JSDRV_FATAL(msg);
+    if (NULL != mutex) {
+        int rc = pthread_mutex_lock(&mutex->mutex);
+        if (rc) {
+            snprintf(msg, sizeof(msg), "mutex lock '%s' failed %d", mutex->name, rc);
+            JSDRV_FATAL(msg);
+        }
     }
 }
 
 void jsdrv_os_mutex_unlock(jsdrv_os_mutex_t mutex) {
     char msg[128];
-    int rc = pthread_mutex_unlock(&mutex->mutex);
-    if (rc) {
-        snprintf(msg, sizeof(msg), "mutex unlock '%s' failed %d", mutex->name, rc);
-        JSDRV_FATAL(msg);
+    if (NULL != mutex) {
+        int rc = pthread_mutex_unlock(&mutex->mutex);
+        if (rc) {
+            snprintf(msg, sizeof(msg), "mutex unlock '%s' failed %d", mutex->name, rc);
+            JSDRV_FATAL(msg);
+        }
     }
 }
 
 void jsdrv_fatal(const char * file, uint32_t line, const char * msg) {
     printf("FATAL: %s:%u %s\n", file, line, msg);
     fflush(stdout);
     exit(1);
@@ -152,15 +158,34 @@
 void jsdrv_thread_sleep_ms(uint32_t duration_ms) {
     struct timespec ts;
     ts.tv_sec = duration_ms / 1000;
     ts.tv_nsec = (duration_ms - (ts.tv_sec * 1000)) * 1000000;
     nanosleep(&ts, NULL);
 }
 
+static jsdrv_os_mutex_t heap_mutex = NULL;
+
+void jsdrv_free(void * ptr) {
+    jsdrv_os_mutex_lock(heap_mutex);
+    free(ptr);
+    jsdrv_os_mutex_unlock(heap_mutex);
+}
+
+void * jsdrv_alloc(size_t size_bytes) {
+    jsdrv_os_mutex_lock(heap_mutex);
+    void * ptr = malloc(size_bytes);
+    if (!ptr) {
+        JSDRV_FATAL("out of memory");
+    }
+    jsdrv_os_mutex_unlock(heap_mutex);
+    return ptr;
+}
+
 int32_t jsdrv_platform_initialize(void) {
+    heap_mutex = jsdrv_os_mutex_alloc("heap");
     struct rlimit limit = {
         .rlim_cur = 0,
         .rlim_max = 0,
     };
     getrlimit(RLIMIT_NOFILE, &limit);
     if (limit.rlim_max < 4096) {
         JSDRV_LOGE("file descriptor limit too small: %llu", limit.rlim_max);
```

### Comparing `pyjoulescope_driver-1.3.2/src/backend/windows.c` & `pyjoulescope_driver-1.3.3/src/backend/windows.c`

 * *Files 7% similar despite different names*

```diff
@@ -86,36 +86,36 @@
             NULL);                  // unnamed mutex
     JSDRV_ASSERT_ALLOC(mutex->mutex);
     jsdrv_cstr_copy(mutex->name, name, sizeof(mutex->name));
     return mutex;
 }
 
 void jsdrv_os_mutex_free(jsdrv_os_mutex_t mutex) {
-    if (mutex) {
+    if (NULL != mutex) {
         CloseHandle(mutex->mutex);
         jsdrv_free(mutex);
     }
 }
 
 void jsdrv_os_mutex_lock(jsdrv_os_mutex_t mutex) {
     char msg[128];
-    if (mutex && mutex->mutex) {
+    if ((NULL != mutex) && mutex->mutex) {
         DWORD rc = WaitForSingleObject(mutex->mutex, JSDRV_CONFIG_OS_MUTEX_LOCK_TIMEOUT_MS);
         if (WAIT_OBJECT_0 != rc) {
             _snprintf_s(msg, sizeof(msg), sizeof(msg), "mutex lock '%s' failed", mutex->name);
             JSDRV_FATAL(msg);
         }
     } else {
         JSDRV_LOGD1("lock, but mutex is null");
     }
 }
 
 void jsdrv_os_mutex_unlock(jsdrv_os_mutex_t mutex) {
     char msg[128];
-    if (mutex && mutex->mutex) {
+    if ((NULL != mutex) && mutex->mutex) {
         if (!ReleaseMutex(mutex->mutex)) {
             _snprintf_s(msg, sizeof(msg), sizeof(msg), "mutex unlock '%s' failed", mutex->name);
             JSDRV_FATAL(msg);
         }
     } else {
         JSDRV_LOGD1("unlock, but mutex is null");
     }
@@ -179,10 +179,29 @@
     return (thread->thread_id == GetCurrentThreadId());
 }
 
 void jsdrv_thread_sleep_ms(uint32_t duration_ms) {
     Sleep(duration_ms);
 }
 
+static jsdrv_os_mutex_t heap_mutex = NULL;
+
+void jsdrv_free(void * ptr) {
+    jsdrv_os_mutex_lock(heap_mutex);
+    free(ptr);
+    jsdrv_os_mutex_unlock(heap_mutex);
+}
+
+void * jsdrv_alloc(size_t size_bytes) {
+    jsdrv_os_mutex_lock(heap_mutex);
+    void * ptr = malloc(size_bytes);
+    if (!ptr) {
+        JSDRV_FATAL("out of memory");
+    }
+    jsdrv_os_mutex_unlock(heap_mutex);
+    return ptr;
+}
+
 int32_t jsdrv_platform_initialize(void) {
+    heap_mutex = jsdrv_os_mutex_alloc("heap");
     return 0;
 }
```

### Comparing `pyjoulescope_driver-1.3.2/src/backend/winusb/backend.c` & `pyjoulescope_driver-1.3.3/src/backend/winusb/backend.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/backend/winusb/device_change_notifier.c` & `pyjoulescope_driver-1.3.3/src/backend/winusb/device_change_notifier.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/backend/winusb/device_change_notifier.h` & `pyjoulescope_driver-1.3.3/src/backend/winusb/device_change_notifier.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/backend/winusb/msg_queue.c` & `pyjoulescope_driver-1.3.3/src/backend/winusb/msg_queue.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/buffer.c` & `pyjoulescope_driver-1.3.3/src/buffer.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/buffer_signal.c` & `pyjoulescope_driver-1.3.3/src/buffer_signal.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/cstr.c` & `pyjoulescope_driver-1.3.3/src/cstr.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/devices.c` & `pyjoulescope_driver-1.3.3/src/devices.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/downsample.c` & `pyjoulescope_driver-1.3.3/src/downsample.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/emu.c` & `pyjoulescope_driver-1.3.3/src/emu.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/emulated.c` & `pyjoulescope_driver-1.3.3/src/emulated.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/error_code.c` & `pyjoulescope_driver-1.3.3/src/error_code.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/js110_api.h` & `pyjoulescope_driver-1.3.3/src/js110_api.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/js110_cal.c` & `pyjoulescope_driver-1.3.3/src/js110_cal.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/js110_sample_processor.c` & `pyjoulescope_driver-1.3.3/src/js110_sample_processor.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/js110_stats.c` & `pyjoulescope_driver-1.3.3/src/js110_stats.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/js110_usb.c` & `pyjoulescope_driver-1.3.3/src/js110_usb.c`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 static const struct param_s PARAMS[] = {
     {
         "s/i/range/select",
         "{"
             "\"dtype\": \"u8\","
             "\"brief\": \"The current range selection.\","
-            "\"default\": 0,"
+            "\"default\": 128,"
             "\"options\": ["
                 "[128, \"auto\"],"
                 "[1, \"10 A\"],"
                 "[2, \"2 A\"],"
                 "[4, \"180 mA\"],"
                 "[8, \"18 mA\"],"
                 "[16, \"1.8 mA\"],"
@@ -703,14 +703,44 @@
     if (wait_for_sensor_command(d)) {
         JSDRV_LOGW("stream_settings_send did not work");
         return JSDRV_ERROR_IO;
     }
     return 0;
 }
 
+static int32_t stream_settings_sync(struct js110_dev_s * d) {
+    struct js110_host_packet_s pkt;
+    memset(&pkt, 0, sizeof(pkt));
+
+    usb_setup_t setup = { .s = {
+            .bmRequestType = USB_REQUEST_TYPE(IN, VENDOR, DEVICE),
+            .bRequest = JS110_HOST_USB_REQUEST_SETTINGS,
+            .wValue = 0,
+            .wIndex = 0,
+            .wLength = 16,
+    }};
+    uint32_t size = 0;
+    if (jsdrvb_ctrl_in(d, setup, &pkt, &size)) {
+        JSDRV_LOGW("stream_settings_sync failed");
+        return JSDRV_ERROR_IO;
+    } else if ((size != 16)
+                || (pkt.header.version != JS110_HOST_API_VERSION)
+                || (pkt.header.type != JS110_HOST_PACKET_TYPE_SETTINGS)) {
+        JSDRV_LOGW("stream_settings_sync unexpected response: size=%d, ver=%d, type=%d",
+                   (int) size, (int) pkt.header.version, (int) pkt.header.type);
+        return JSDRV_ERROR_IO;
+    } else {
+        d->param_values[PARAM_I_RANGE_SELECT].value.u8 = pkt.payload.settings.select;
+        d->param_values[PARAM_V_RANGE_SELECT].value.u8 = (pkt.payload.settings.options >> 1) & 1;
+        send_to_frontend(d, "s/i/range/select", &d->param_values[PARAM_I_RANGE_SELECT]);
+        send_to_frontend(d, "s/v/range/select", &d->param_values[PARAM_V_RANGE_SELECT]);
+    }
+    return 0;
+}
+
 static int32_t extio_settings_send(struct js110_dev_s * d) {
     struct js110_host_packet_s pkt;
     memset(&pkt, 0, sizeof(pkt));
     pkt.header.version = JS110_HOST_API_VERSION;
     pkt.header.length = 24;
     pkt.header.type = JS110_HOST_PACKET_TYPE_EXTIO;
     pkt.payload.extio.flags = 0;
@@ -735,14 +765,51 @@
     if (wait_for_sensor_command(d)) {
         JSDRV_LOGW("extio_settings_send did not work");
         return JSDRV_ERROR_IO;
     }
     return 0;
 }
 
+static int32_t extio_settings_sync(struct js110_dev_s * d) {
+    struct js110_host_packet_s pkt;
+    memset(&pkt, 0, sizeof(pkt));
+
+    usb_setup_t setup = { .s = {
+            .bmRequestType = USB_REQUEST_TYPE(IN, VENDOR, DEVICE),
+            .bRequest = JS110_HOST_USB_REQUEST_EXTIO,
+            .wValue = 0,
+            .wIndex = 0,
+            .wLength = 24,
+    }};
+    uint32_t size = 0;
+    if (jsdrvb_ctrl_in(d, setup, &pkt, &size)) {
+        JSDRV_LOGW("extio_settings_sync failed");
+        return JSDRV_ERROR_IO;
+    } else if ((size != 24)
+               || (pkt.header.version != JS110_HOST_API_VERSION)
+               || (pkt.header.type != JS110_HOST_PACKET_TYPE_EXTIO)) {
+        JSDRV_LOGW("extio_settings_sync unexpected response: size=%d, ver=%d, type=%d",
+                   (int) size, (int) pkt.header.version, (int) pkt.header.type);
+        return JSDRV_ERROR_IO;
+    } else {
+        d->param_values[PARAM_I_LSB_SOURCE].value.u8 = pkt.payload.extio.current_gpi;
+        d->param_values[PARAM_V_LSB_SOURCE].value.u8 = pkt.payload.extio.voltage_gpi;
+        d->param_values[PARAM_GPO0_VALUE].value.u8 = pkt.payload.extio.gpo0;
+        d->param_values[PARAM_GPO1_VALUE].value.u8 = pkt.payload.extio.gpo1;
+        d->param_values[PARAM_EXTIO_VOLTAGE].value.u32 = pkt.payload.extio.io_voltage_mv;
+
+        send_to_frontend(d, "s/i/lsb_src", &d->param_values[PARAM_I_LSB_SOURCE]);
+        send_to_frontend(d, "s/v/lsb_src", &d->param_values[PARAM_V_LSB_SOURCE]);
+        send_to_frontend(d, "s/gpo/0/value", &d->param_values[PARAM_GPO0_VALUE]);
+        send_to_frontend(d, "s/gpo/1/value", &d->param_values[PARAM_GPO1_VALUE]);
+        send_to_frontend(d, "s/extio/voltage", &d->param_values[PARAM_EXTIO_VOLTAGE]);
+    }
+    return 0;
+}
+
 static int32_t extio_gpi_recv(struct js110_dev_s * d, uint8_t * gpi) {
     struct js110_host_packet_s pkt;
     memset(&pkt, 0, sizeof(pkt));
     uint32_t sz = 0;
     usb_setup_t setup = { .s = {
             .bmRequestType = USB_REQUEST_TYPE(IN, VENDOR, DEVICE),
             .bRequest = JS110_HOST_USB_REQUEST_EXTIO,
@@ -904,17 +971,17 @@
     js110_stats_sample_count_set(&d->stats, v.value.u32);
 }
 
 static void on_stats_ctrl(struct js110_dev_s * d, const struct jsdrv_union_s * value) {
     on_update_ctrl(d, value, PARAM_STATS_CTRL);
 }
 
-static int32_t d_open_ll(struct js110_dev_s * d) {
+static int32_t d_open_ll(struct js110_dev_s * d, int32_t opt) {
     JSDRV_LOGI("open_ll");
-    struct jsdrvp_msg_s * m = jsdrvp_msg_alloc_value(d->context, JSDRV_MSG_OPEN, &jsdrv_union_i32(0));
+    struct jsdrvp_msg_s * m = jsdrvp_msg_alloc_value(d->context, JSDRV_MSG_OPEN, &jsdrv_union_i32(opt & 1));
     msg_queue_push(d->ll.cmd_q, m);
     m = ll_await_topic(d, JSDRV_MSG_OPEN, TIMEOUT_MS);
     if (!m) {
         JSDRV_LOGW("ll_driver open timed out");
         return JSDRV_ERROR_TIMED_OUT;
     }
     int32_t rc = m->value.value.i32;
@@ -923,15 +990,15 @@
         JSDRV_LOGE("open_ll failed");
         return rc;
     }
     d->state = ST_OPENING;
     return 0;
 }
 
-static int32_t d_open(struct js110_dev_s * d) {
+static int32_t d_open(struct js110_dev_s * d, int32_t opt) {
     JSDRV_LOGI("open");
     usb_setup_t setup = { .s = {
             .bmRequestType = USB_REQUEST_TYPE(OUT, VENDOR, DEVICE),
             .bRequest = JS110_HOST_USB_REQUEST_LOOPBACK_BUFFER,
             .wValue = 0,
             .wIndex = 0,
             .wLength = 16,
@@ -949,26 +1016,30 @@
         return JSDRV_ERROR_IO;
     }
 
     if (0 != memcmp(buf_out, buf_in, sizeof(buf_in))) {
         JSDRV_LOGE("loopback failed");
     }
 
-    ROE(stream_settings_send(d));
-    ROE(calibration_get(d));
-
     // Publish topic metadata
     for (int i = 0; NULL != PARAMS[i].topic; ++i) {
         const struct param_s * p = &PARAMS[i];
         struct jsdrv_topic_s topic;
         jsdrv_topic_set(&topic, p->topic);
         jsdrv_topic_suffix_add(&topic, JSDRV_TOPIC_SUFFIX_METADATA_RSP);
         send_to_frontend(d, topic.topic, &jsdrv_union_cjson_r(p->meta));
     }
 
+    ROE(calibration_get(d));
+    if (opt != JSDRV_DEVICE_OPEN_MODE_DEFAULTS) {
+        ROE(stream_settings_sync(d));
+        ROE(extio_settings_sync(d));
+    }
+    ROE(stream_settings_send(d));
+
     // todo info_get(d) -> version, jsdrvb_ctrl_in JS110_HOST_USB_REQUEST_INFO
 
     // Publish topic values
     for (int i = 0; NULL != PARAMS[i].topic; ++i) {
         send_to_frontend(d, PARAMS[i].topic, &d->param_values[i]);
     }
 
@@ -1050,17 +1121,21 @@
         } else {
             JSDRV_LOGE("handle_cmd unsupported %s", msg->topic);
         }
     } else if (!topic) {
         JSDRV_LOGE("handle_cmd mismatch %s, %s", msg->topic, d->ll.prefix);
     } else if (topic[0] == JSDRV_MSG_COMMAND_PREFIX_CHAR) {
         if (0 == strcmp(JSDRV_MSG_OPEN, topic)) {
-            status = d_open_ll(d);
+            int32_t opt = 0;
+            if ((msg->value.type == JSDRV_UNION_U32) || (msg->value.type == JSDRV_UNION_I32)) {
+                opt = msg->value.value.i32;
+            }
+            status = d_open_ll(d, opt);
             if (0 == status) {
-                status = d_open(d);
+                status = d_open(d, opt);
                 if (status) {
                     d_close(d);
                 }
             }
             send_to_frontend(d, JSDRV_MSG_OPEN "#", &jsdrv_union_i32(status));
         } else if (0 == strcmp(JSDRV_MSG_CLOSE, topic)) {
             status = d_close(d);
```

### Comparing `pyjoulescope_driver-1.3.2/src/js220_i128.c` & `pyjoulescope_driver-1.3.3/src/js220_i128.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/js220_params.c` & `pyjoulescope_driver-1.3.3/src/js220_params.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/js220_stats.c` & `pyjoulescope_driver-1.3.3/src/js220_stats.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/js220_usb.c` & `pyjoulescope_driver-1.3.3/src/js220_usb.c`

 * *Files 0% similar despite different names*

```diff
@@ -926,14 +926,15 @@
         if (jsdrv_cstr_starts_with(topic, "h/mem/")) {
             handle_cmd_mem(d, msg);
         } else if (0 == strcmp("h/!reset", topic)) {   // value=target
             rc = handle_reset(d, msg->value.value.i32);
             send_return_code_to_frontend(d, topic, rc);
         } else if (0 == strcmp("h/timeout", topic)) {
             jsdrv_thread_sleep_ms(msg->value.value.u32);
+            JSDRV_LOGI("JS220 timeout done: %" PRIu32, msg->value.value.u32);
             send_return_code_to_frontend(d, topic, 0);
         } else if (0 == strcmp("h/fs", topic)) {
             rc = on_sampling_frequency(d, &msg->value);
             send_return_code_to_frontend(d, topic, rc);
         } else {
             JSDRV_LOGE("topic invalid: %s", msg->topic);
             send_return_code_to_frontend(d, topic, JSDRV_ERROR_PARAMETER_INVALID);
```

### Comparing `pyjoulescope_driver-1.3.2/src/jsdrv.c` & `pyjoulescope_driver-1.3.3/src/jsdrv.c`

 * *Files 1% similar despite different names*

```diff
@@ -92,36 +92,40 @@
     struct jsdrvp_msg_s * m = msg_queue_pop_immediate(context->msg_free);
     if (!m) {
         m = jsdrv_alloc_clr(sizeof(struct jsdrvp_msg_s));
         JSDRV_LOGD3("jsdrvp_msg_alloc %p", m);
         jsdrv_list_initialize(&m->item);
     }
     m->inner_msg_type = JSDRV_MSG_TYPE_NORMAL;
-    m->topic[0] = 0;
     m->source = 0;
     m->u32_a = 0;
     m->u32_b = 0;
+    m->topic[0] = 0;
     memset(&m->value, 0, sizeof(m->value));
     m->payload.str[0] = 0;
     memset(&m->extra, 0, sizeof(m->extra));
+    m->timeout = NULL;
     return m;
 }
 
 struct jsdrvp_msg_s * jsdrvp_msg_alloc_data(struct jsdrv_context_s * context, const char * topic) {
     struct jsdrvp_msg_s * m = msg_queue_pop_immediate(context->msg_free_data);
     if (!m) {
         m = jsdrv_alloc_clr(STREAM_MSG_SZ);
         JSDRV_LOGD3("jsdrvp_msg_alloc_data %p sz=%zu", m, STREAM_MSG_SZ);
         jsdrv_list_initialize(&m->item);
     }
     m->inner_msg_type = JSDRV_MSG_TYPE_DATA;
+    m->source = 0;
+    m->u32_a = 0;
+    m->u32_b = 0;
     jsdrv_cstr_copy(m->topic, topic, sizeof(m->topic));
     m->value = jsdrv_union_bin(&m->payload.bin[0], 0);
-    m->u32_a = 0;
     memset(&m->extra, 0, sizeof(m->extra));
+    m->timeout = NULL;
     return m;
 }
 
 struct jsdrvp_msg_s * jsdrvp_msg_clone(struct jsdrv_context_s * context, const struct jsdrvp_msg_s * msg_src) {
     struct jsdrvp_msg_s * m;
     if (msg_src->inner_msg_type == JSDRV_MSG_TYPE_DATA) {
         m = jsdrvp_msg_alloc_data(context, msg_src->topic);
@@ -340,14 +344,19 @@
             return true;
         } else if (0 == strcmp(JSDRV_MSG_FINALIZE, msg->topic)) {
             // all timeouts, including this one, expire on finalize
             jsdrvp_msg_free(c, msg);
             JSDRV_LOGI("USB backend finalize");
             c->do_exit = true;
             return false;
+        } else if (0 == strcmp(JSDRV_MSG_TIMEOUT, msg->topic)) {
+            // ignore the message so it times out.
+            jsdrvp_msg_free(c, msg);
+            JSDRV_LOGI("%s request", JSDRV_MSG_TIMEOUT);
+            return true;
         }
     }
     jsdrv_pubsub_publish(c->pubsub, msg);  // msg ownership relinquished
     return true;
 }
 
 static struct frontend_dev_s * device_lookup(struct jsdrv_context_s * c, const char * topic) {
```

### Comparing `pyjoulescope_driver-1.3.2/src/json.c` & `pyjoulescope_driver-1.3.3/src/json.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/meta.c` & `pyjoulescope_driver-1.3.3/src/meta.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/pubsub.c` & `pyjoulescope_driver-1.3.3/src/pubsub.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/sample_buffer_f32.c` & `pyjoulescope_driver-1.3.3/src/sample_buffer_f32.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/statistics.c` & `pyjoulescope_driver-1.3.3/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/time.c` & `pyjoulescope_driver-1.3.3/src/time.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/topic.c` & `pyjoulescope_driver-1.3.3/src/topic.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/union.c` & `pyjoulescope_driver-1.3.3/src/union.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/src/version.c` & `pyjoulescope_driver-1.3.3/src/version.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/third-party/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/.gitlab-ci.yml` & `pyjoulescope_driver-1.3.3/third-party/cmocka/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/.ycm_extra_conf.py` & `pyjoulescope_driver-1.3.3/third-party/cmocka/.ycm_extra_conf.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/5.patch` & `pyjoulescope_driver-1.3.3/third-party/cmocka/5.patch`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/third-party/cmocka/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/CPackConfig.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/CPackConfig.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/CompilerChecks.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/CompilerChecks.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/ConfigureChecks.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/ConfigureChecks.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/INSTALL.md` & `pyjoulescope_driver-1.3.3/third-party/cmocka/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/README.md` & `pyjoulescope_driver-1.3.3/third-party/cmocka/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/FindNSIS.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/FindNSIS.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/cmake/Toolchain-cross-m32.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/cmake/Toolchain-cross-m32.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/config.h.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/coverity/coverity_assert_model.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/coverity/coverity_assert_model.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/index.html` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/index.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/mainpage.dox` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/mainpage.dox`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/README.md` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/header.html` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/header.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/doc.svg` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/doc.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/folderclosed.svg` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/folderclosed.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/folderopen.svg` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/folderopen.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/mag_glass.svg` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/mag_glass.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/nav_edge_left.svg` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_left.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/nav_edge_right.svg` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/nav_edge_right.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/img/splitbar_handle.svg` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/img/splitbar_handle.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/js/striped_bg.js` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/js/striped_bg.js`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/doc/that_style/that_style.css` & `pyjoulescope_driver-1.3.3/third-party/cmocka/doc/that_style/that_style.css`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/allocate_module.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/allocate_module.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/allocate_module_test.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/allocate_module_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_macro.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_macro_test.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_macro_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_module.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_module.h` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/assert_module_test.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/assert_module_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/calculator.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/calculator.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/calculator_test.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/calculator_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/database.h` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/database.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/chef.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/chef.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/chef.h` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/chef.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/README.md` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/proc_uptime.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/proc_uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/proc_uptime.h` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/proc_uptime.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/test_uptime.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/test_uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/example/mock/uptime/uptime.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/example/mock/uptime/uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/include/cmocka.h` & `pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/include/cmocka_pbc.h` & `pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka_pbc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/include/cmocka_private.h` & `pyjoulescope_driver-1.3.3/third-party/cmocka/include/cmocka_private.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/src/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/third-party/cmocka/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/src/cmocka.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/src/cmocka.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/src/cmocka.def` & `pyjoulescope_driver-1.3.3/third-party/cmocka/src/cmocka.def`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/cmocka_test.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/cmocka_test.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/ctest-default.cmake` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/ctest-default.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_alloc.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_alloc.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_assert_macros.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_assert_macros.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_assert_macros_fail.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_assert_macros_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_basics.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_basics.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_cmockery.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_cmockery.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_exception_handler.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_exception_handler.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_fixtures.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_fixtures.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_float_macros.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_float_macros.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_group_fixtures.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_fixtures.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_group_setup_assert.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_setup_assert.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_group_setup_fail.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_group_setup_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_groups.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_groups.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_ordering.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_ordering.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_ordering_fail.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_ordering_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_returns.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_returns.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_returns_fail.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_returns_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_setup_fail.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_setup_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_skip.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_skip.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_skip_filter.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_skip_filter.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_strmatch.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_strmatch.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/cmocka/tests/test_wildcard.c` & `pyjoulescope_driver-1.3.3/third-party/cmocka/tests/test_wildcard.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.github/cifuzz.yml` & `pyjoulescope_driver-1.3.3/third-party/libusb/.github/cifuzz.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.github/workflows/linux.yml` & `pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.github/workflows/macos.yml` & `pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.github/workflows/msys2.yml` & `pyjoulescope_driver-1.3.3/third-party/libusb/.github/workflows/msys2.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.gitignore` & `pyjoulescope_driver-1.3.3/third-party/libusb/.gitignore`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.private/appveyor_build.sh` & `pyjoulescope_driver-1.3.3/third-party/libusb/.private/appveyor_build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.private/bm.sh` & `pyjoulescope_driver-1.3.3/third-party/libusb/.private/bm.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.private/ci-build.sh` & `pyjoulescope_driver-1.3.3/third-party/libusb/.private/ci-build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.private/ci-container-build.sh` & `pyjoulescope_driver-1.3.3/third-party/libusb/.private/ci-container-build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.private/post-rewrite.sh` & `pyjoulescope_driver-1.3.3/third-party/libusb/.private/post-rewrite.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.private/pre-commit.sh` & `pyjoulescope_driver-1.3.3/third-party/libusb/.private/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.private/wbs.txt` & `pyjoulescope_driver-1.3.3/third-party/libusb/.private/wbs.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/.travis.yml` & `pyjoulescope_driver-1.3.3/third-party/libusb/.travis.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/CMakeLists.txt` & `pyjoulescope_driver-1.3.3/third-party/libusb/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/INSTALL_WIN.txt` & `pyjoulescope_driver-1.3.3/third-party/libusb/INSTALL_WIN.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/Makefile.am` & `pyjoulescope_driver-1.3.3/third-party/libusb/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/README-FORK.md` & `pyjoulescope_driver-1.3.3/third-party/libusb/README-FORK.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/README.git` & `pyjoulescope_driver-1.3.3/third-party/libusb/README.git`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/common.xcconfig` & `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/common.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/config.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/debug.xcconfig` & `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/debug.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/libusb.xcconfig` & `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/libusb_debug.xcconfig` & `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb_debug.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/libusb_release.xcconfig` & `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/libusb_release.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/Xcode/release.xcconfig` & `pyjoulescope_driver-1.3.3/third-party/libusb/Xcode/release.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/android/config.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/android/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/android/examples/unrooted_android.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/unrooted_android.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/android/examples/unrooted_android.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/android/examples/unrooted_android.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/Android.mk` & `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/Android.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/Application.mk` & `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/Application.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/examples.mk` & `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/examples.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/libusb.mk` & `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/libusb.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/android/jni/tests.mk` & `pyjoulescope_driver-1.3.3/third-party/libusb/android/jni/tests.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/appveyor.yml` & `pyjoulescope_driver-1.3.3/third-party/libusb/appveyor.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/configure.ac` & `pyjoulescope_driver-1.3.3/third-party/libusb/configure.ac`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/doc/Makefile.in` & `pyjoulescope_driver-1.3.3/third-party/libusb/doc/Makefile.in`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/doc/doxygen.cfg.in` & `pyjoulescope_driver-1.3.3/third-party/libusb/doc/doxygen.cfg.in`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/doc/libusb.png` & `pyjoulescope_driver-1.3.3/third-party/libusb/doc/libusb.png`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/examples/dpfp.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/examples/dpfp.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/examples/ezusb.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/examples/ezusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/examples/ezusb.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/examples/ezusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/examples/fxload.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/examples/fxload.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/examples/hotplugtest.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/examples/hotplugtest.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/examples/listdevs.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/examples/listdevs.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/examples/sam3u_benchmark.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/examples/sam3u_benchmark.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/examples/testlibusb.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/examples/testlibusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/examples/xusb.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/examples/xusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/include/linux/config.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/include/linux/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/include/macos/config.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/include/macos/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/Makefile.am` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/Makefile.am.extra` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/Makefile.am.extra`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/core.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/core.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/descriptor.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/descriptor.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/hotplug.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/hotplug.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/io.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/io.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/libusb-1.0.def` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb-1.0.def`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/libusb-1.0.rc` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb-1.0.rc`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/libusb.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/libusbi.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/libusbi.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/darwin_usb.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/darwin_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/darwin_usb.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/darwin_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/emscripten_webusb.cpp` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/emscripten_webusb.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/events_posix.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/events_posix.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_posix.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/events_windows.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/events_windows.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/events_windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_pollfs.cpp` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_pollfs.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_usb.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_usb_backend.cpp` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_backend.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_usb_raw.cpp` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_raw.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/haiku_usb_raw.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/haiku_usb_raw.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/linux_netlink.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_netlink.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/linux_udev.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_udev.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/linux_usbfs.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_usbfs.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/linux_usbfs.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/linux_usbfs.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/netbsd_usb.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/netbsd_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/null_usb.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/null_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/openbsd_usb.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/openbsd_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/sunos_usb.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/sunos_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/sunos_usb.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/sunos_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/threads_posix.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/threads_posix.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_posix.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/threads_windows.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/threads_windows.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/threads_windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_common.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_common.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_common.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_common.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_usbdk.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_usbdk.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_usbdk.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_usbdk.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_winusb.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_winusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/os/windows_winusb.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/os/windows_winusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/strerror.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/strerror.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/libusb/sync.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/libusb/sync.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/Base.props` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/Configuration.Base.props` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/Configuration.DynamicLibrary.props` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/Configuration.DynamicLibrary.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/ProjectConfigurations.Base.props` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/ProjectConfigurations.Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/build_all.ps1` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/build_all.ps1`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/config.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/dpfp.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/dpfp.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/dpfp_threaded.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/dpfp_threaded.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/fxload.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/fxload.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/getopt/getopt.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/getopt/getopt.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/getopt/getopt1.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt/getopt1.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/getopt.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/getopt.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/hotplugtest.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/hotplugtest.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/libusb.sln` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb.sln`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/libusb_dll.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb_dll.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/libusb_static.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/libusb_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/listdevs.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/listdevs.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/sam3u_benchmark.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/sam3u_benchmark.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/stress.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/stress.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/testlibusb.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/testlibusb.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/msvc/xusb.vcxproj` & `pyjoulescope_driver-1.3.3/third-party/libusb/msvc/xusb.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/tests/Makefile.am` & `pyjoulescope_driver-1.3.3/third-party/libusb/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/tests/libusb_testlib.h` & `pyjoulescope_driver-1.3.3/third-party/libusb/tests/libusb_testlib.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/tests/stress.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/tests/stress.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/tests/testlib.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/tests/testlib.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/libusb/tests/umockdev.c` & `pyjoulescope_driver-1.3.3/third-party/libusb/tests/umockdev.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/tinyprintf/tinyprintf.c` & `pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/tinyprintf/tinyprintf.h` & `pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.3.2/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new` & `pyjoulescope_driver-1.3.3/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new`

 * *Files identical despite different names*

