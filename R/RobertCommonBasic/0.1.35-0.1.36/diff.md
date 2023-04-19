# Comparing `tmp/RobertCommonBasic-0.1.35.tar.gz` & `tmp/RobertCommonBasic-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonBasic-0.1.35.tar", last modified: Mon Apr 17 08:26:15 2023, max compression
+gzip compressed data, was "RobertCommonBasic-0.1.36.tar", last modified: Wed Apr 19 11:44:17 2023, max compression
```

## Comparing `RobertCommonBasic-0.1.35.tar` & `RobertCommonBasic-0.1.36.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.033093 RobertCommonBasic-0.1.35/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.35/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.35/MANIFEST.in
--rw-rw-rw-   0        0        0     1739 2023-04-17 08:26:15.033093 RobertCommonBasic-0.1.35/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2022-01-13 05:29:18.000000 RobertCommonBasic-0.1.35/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.901099 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/
--rw-rw-rw-   0        0        0     1739 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4427 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-17 08:26:14.000000 RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      194 2023-03-29 09:51:16.000000 RobertCommonBasic-0.1.35/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.903098 RobertCommonBasic-0.1.35/robertcommonbasic/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.35/robertcommonbasic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.904098 RobertCommonBasic-0.1.35/robertcommonbasic/basic/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.905101 RobertCommonBasic-0.1.35/robertcommonbasic/basic/base/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/base/__init__.py
--rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/base/constant.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.909098 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cache/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cache/__init__.py
--rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cache/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.911102 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cls/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cls/__init__.py
--rw-rw-rw-   0        0        0    12322 2023-04-03 03:01:59.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/cls/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.924625 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/__init__.py
--rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/conversion.py
--rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/crc16.py
--rw-rw-rw-   0        0        0     2229 2022-11-14 03:21:43.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/csv.py
--rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/datatuple.py
--rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/frame.py
--rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/nametuple.py
--rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/type.py
--rw-rw-rw-   0        0        0     5064 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.926624 RobertCommonBasic-0.1.35/robertcommonbasic/basic/decorator/
--rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/decorator/__init__.py
--rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/decorator/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.931661 RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/__init__.py
--rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/schedule.py
--rw-rw-rw-   0        0        0    10445 2023-04-10 06:28:17.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.938849 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/__init__.py
--rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/aes.py
--rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/dsa.py
--rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/hash.py
--rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/md5.py
--rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/rsa.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.941815 RobertCommonBasic-0.1.35/robertcommonbasic/basic/error/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/error/__init__.py
--rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/error/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.943816 RobertCommonBasic-0.1.35/robertcommonbasic/basic/exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/exector/__init__.py
--rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/exector/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.952815 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/
--rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/__init__.py
--rw-rw-rw-   0        0        0     3113 2023-02-21 06:19:45.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/csv.py
--rw-rw-rw-   0        0        0     1328 2022-11-18 03:22:13.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/ini.py
--rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/log.py
--rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/xml.py
--rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/yaml.py
--rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/zip.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.958676 RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/__init__.py
--rw-rw-rw-   0        0        0     6070 2023-04-10 02:23:47.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/utils.py
--rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/watch.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.960677 RobertCommonBasic-0.1.35/robertcommonbasic/basic/net/
--rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/net/__init__.py
--rw-rw-rw-   0        0        0     5874 2023-04-11 03:18:26.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/net/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.970684 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/__init__.py
--rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/cmd.py
--rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/env.py
--rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/file.py
--rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/path.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.974027 RobertCommonBasic-0.1.35/robertcommonbasic/basic/process/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/process/__init__.py
--rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/process/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.979023 RobertCommonBasic-0.1.35/robertcommonbasic/basic/profile/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/profile/__init__.py
--rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/profile/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.983538 RobertCommonBasic-0.1.35/robertcommonbasic/basic/re/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/re/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-02-09 02:47:33.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/re/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.986573 RobertCommonBasic-0.1.35/robertcommonbasic/basic/safetext/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/safetext/__init__.py
--rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/safetext/converter.py
--rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/safetext/funcs.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.989573 RobertCommonBasic-0.1.35/robertcommonbasic/basic/sugar/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/sugar/__init__.py
--rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/sugar/funcs.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.991573 RobertCommonBasic-0.1.35/robertcommonbasic/basic/validation/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/validation/__init__.py
--rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.35/robertcommonbasic/basic/validation/input.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.992572 RobertCommonBasic-0.1.35/robertcommonbasic/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.994858 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:14.997335 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_cls/
--rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_cls/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.006595 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/
--rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/__init__.py
--rw-rw-rw-   0        0        0      729 2022-06-23 09:21:24.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
--rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
--rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_frame.py
--rw-rw-rw-   0        0        0     3568 2023-04-11 13:11:50.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.008595 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_dt/
--rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_dt/__init__.py
--rw-rw-rw-   0        0        0     2169 2023-02-20 02:34:17.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.013873 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/
--rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
--rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
--rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
--rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.016095 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_exector/__init__.py
--rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.023096 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_csv.py
--rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_xml.py
--rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_zip.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.025100 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_net/
--rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_net/__init__.py
--rw-rw-rw-   0        0        0      558 2023-04-11 03:14:26.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_net/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.027094 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_os/
--rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_os/__init__.py
--rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_os/test_env.py
--rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_os/test_file.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.030093 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_re/
--rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_re/__init__.py
--rw-rw-rw-   0        0        0      605 2023-04-11 09:07:57.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_re/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:26:15.032094 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_validation/
--rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_validation/__init__.py
--rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_validation/test_input.py
--rw-rw-rw-   0        0        0       42 2023-04-17 08:26:15.033093 RobertCommonBasic-0.1.35/setup.cfg
--rw-rw-rw-   0        0        0     3876 2023-04-17 08:23:01.000000 RobertCommonBasic-0.1.35/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.571110 RobertCommonBasic-0.1.36/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.36/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.36/MANIFEST.in
+-rw-rw-rw-   0        0        0     1739 2023-04-19 11:44:17.571110 RobertCommonBasic-0.1.36/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2022-01-13 05:29:18.000000 RobertCommonBasic-0.1.36/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.378931 RobertCommonBasic-0.1.36/RobertCommonBasic.egg-info/
+-rw-rw-rw-   0        0        0     1739 2023-04-19 11:44:17.000000 RobertCommonBasic-0.1.36/RobertCommonBasic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4427 2023-04-19 11:44:17.000000 RobertCommonBasic-0.1.36/RobertCommonBasic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:44:17.000000 RobertCommonBasic-0.1.36/RobertCommonBasic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-04-19 11:44:17.000000 RobertCommonBasic-0.1.36/RobertCommonBasic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-19 11:44:17.000000 RobertCommonBasic-0.1.36/RobertCommonBasic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      187 2023-04-19 11:40:39.000000 RobertCommonBasic-0.1.36/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.393510 RobertCommonBasic-0.1.36/robertcommonbasic/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.36/robertcommonbasic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.394940 RobertCommonBasic-0.1.36/robertcommonbasic/basic/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.397252 RobertCommonBasic-0.1.36/robertcommonbasic/basic/base/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/base/__init__.py
+-rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/base/constant.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.399783 RobertCommonBasic-0.1.36/robertcommonbasic/basic/cache/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/cache/__init__.py
+-rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/cache/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.402113 RobertCommonBasic-0.1.36/robertcommonbasic/basic/cls/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/cls/__init__.py
+-rw-rw-rw-   0        0        0    12322 2023-04-03 03:01:59.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/cls/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.418723 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/__init__.py
+-rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/conversion.py
+-rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/crc16.py
+-rw-rw-rw-   0        0        0     2229 2022-11-14 03:21:43.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/csv.py
+-rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/datatuple.py
+-rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/frame.py
+-rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/nametuple.py
+-rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/type.py
+-rw-rw-rw-   0        0        0     5064 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.423926 RobertCommonBasic-0.1.36/robertcommonbasic/basic/decorator/
+-rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/decorator/__init__.py
+-rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/decorator/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.428442 RobertCommonBasic-0.1.36/robertcommonbasic/basic/dt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/dt/__init__.py
+-rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/dt/schedule.py
+-rw-rw-rw-   0        0        0    10445 2023-04-10 06:28:17.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/dt/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.447651 RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/__init__.py
+-rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/aes.py
+-rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/dsa.py
+-rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/hash.py
+-rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/md5.py
+-rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/rsa.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.456365 RobertCommonBasic-0.1.36/robertcommonbasic/basic/error/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/error/__init__.py
+-rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/error/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.466933 RobertCommonBasic-0.1.36/robertcommonbasic/basic/exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/exector/__init__.py
+-rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/exector/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.478882 RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/__init__.py
+-rw-rw-rw-   0        0        0     3113 2023-02-21 06:19:45.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/csv.py
+-rw-rw-rw-   0        0        0     1328 2022-11-18 03:22:13.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/ini.py
+-rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/log.py
+-rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/xml.py
+-rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/yaml.py
+-rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/zip.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.483359 RobertCommonBasic-0.1.36/robertcommonbasic/basic/log/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/log/__init__.py
+-rw-rw-rw-   0        0        0     6070 2023-04-10 02:23:47.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/log/utils.py
+-rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/log/watch.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.485608 RobertCommonBasic-0.1.36/robertcommonbasic/basic/net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/net/__init__.py
+-rw-rw-rw-   0        0        0     5874 2023-04-11 03:18:26.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/net/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.492452 RobertCommonBasic-0.1.36/robertcommonbasic/basic/os/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/os/__init__.py
+-rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/os/cmd.py
+-rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/os/env.py
+-rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/os/file.py
+-rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/os/path.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.494553 RobertCommonBasic-0.1.36/robertcommonbasic/basic/process/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/process/__init__.py
+-rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/process/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.498849 RobertCommonBasic-0.1.36/robertcommonbasic/basic/profile/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/profile/__init__.py
+-rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/profile/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.503506 RobertCommonBasic-0.1.36/robertcommonbasic/basic/re/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/re/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-02-09 02:47:33.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/re/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.507670 RobertCommonBasic-0.1.36/robertcommonbasic/basic/safetext/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/safetext/__init__.py
+-rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/safetext/converter.py
+-rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/safetext/funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.510679 RobertCommonBasic-0.1.36/robertcommonbasic/basic/sugar/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/sugar/__init__.py
+-rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/sugar/funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.514488 RobertCommonBasic-0.1.36/robertcommonbasic/basic/validation/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/validation/__init__.py
+-rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.36/robertcommonbasic/basic/validation/input.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.515498 RobertCommonBasic-0.1.36/robertcommonbasic/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.516494 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.518494 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_cls/
+-rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_cls/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.525679 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/
+-rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/__init__.py
+-rw-rw-rw-   0        0        0      729 2022-06-23 09:21:24.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
+-rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
+-rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/test_frame.py
+-rw-rw-rw-   0        0        0     3568 2023-04-11 13:11:50.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.527686 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_dt/
+-rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_dt/__init__.py
+-rw-rw-rw-   0        0        0     2169 2023-02-20 02:34:17.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.538188 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_encrypt/
+-rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
+-rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
+-rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
+-rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.541195 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_exector/__init__.py
+-rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.554551 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_file/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_file/test_csv.py
+-rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_file/test_xml.py
+-rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_file/test_zip.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.557133 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_net/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-04-11 03:14:26.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_net/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.563464 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_os/
+-rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_os/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_os/test_env.py
+-rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_os/test_file.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.567042 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_re/
+-rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_re/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-04-11 09:07:57.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_re/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:44:17.570105 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_validation/
+-rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_validation/__init__.py
+-rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_validation/test_input.py
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:44:17.572203 RobertCommonBasic-0.1.36/setup.cfg
+-rw-rw-rw-   0        0        0     3876 2023-04-19 11:43:47.000000 RobertCommonBasic-0.1.36/setup.py
```

### Comparing `RobertCommonBasic-0.1.35/LICENSE` & `RobertCommonBasic-0.1.36/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/PKG-INFO` & `RobertCommonBasic-0.1.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.35
+Version: 0.1.36
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.35/README.md` & `RobertCommonBasic-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/PKG-INFO` & `RobertCommonBasic-0.1.36/RobertCommonBasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.35
+Version: 0.1.36
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.35/RobertCommonBasic.egg-info/SOURCES.txt` & `RobertCommonBasic-0.1.36/RobertCommonBasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/cache/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/cache/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/cls/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/cls/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/conversion.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/crc16.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/crc16.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/csv.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/datatuple.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/datatuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/frame.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/nametuple.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/nametuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/data/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/data/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/decorator/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/schedule.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/dt/schedule.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/dt/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/dt/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/aes.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/dsa.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/hash.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/hash.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/encrypt/rsa.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/error/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/error/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/exector/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/exector/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/csv.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/ini.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/log.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/log.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/xml.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/file/zip.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/file/zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/log/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/log/watch.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/log/watch.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/net/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/net/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/file.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/os/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/os/path.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/os/path.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/process/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/process/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/profile/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/profile/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/re/utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/re/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/basic/validation/input.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/basic/validation/input.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_cls/test_utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_cls/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_conversion.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/test_conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_frame.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/test_frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_data/test_utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_data/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_dt/test_utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_dt/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_exector/test_utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_exector/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_csv.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_file/test_csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_xml.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_file/test_xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_file/test_zip.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_file/test_zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_net/test_utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_net/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/robertcommonbasic/tests/test_basic/test_re/test_utils.py` & `RobertCommonBasic-0.1.36/robertcommonbasic/tests/test_basic/test_re/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.35/setup.py` & `RobertCommonBasic-0.1.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonBasic'
 DESCRIPTION = 'Robert Common Basic Library'
 URL = 'https://github.com/hun0423/RobertCommonBasic'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.35'
-DATE = '2023-04-17'
+VERSION = '0.1.36'
+DATE = '2023-04-19'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

