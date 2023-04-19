# Comparing `tmp/gyp-next-0.15.0.tar.gz` & `tmp/gyp-next-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyp-next-0.15.0.tar", last modified: Wed Apr 19 10:19:26 2023, max compression
+gzip compressed data, was "dist/gyp-next-0.4.0.tar", last modified: Tue Jul 14 07:18:34 2020, max compression
```

## Comparing `gyp-next-0.15.0.tar` & `gyp-next-0.4.0.tar`

### file list

```diff
@@ -1,58 +1,55 @@
-drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2023-04-19 10:19:26.031267 gyp-next-0.15.0/
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)      514 2020-04-14 06:16:26.000000 gyp-next-0.15.0/AUTHORS
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1537 2020-05-17 18:15:26.000000 gyp-next-0.15.0/LICENSE
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     3836 2023-04-19 10:19:26.031267 gyp-next-0.15.0/PKG-INFO
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1136 2023-04-19 10:05:15.000000 gyp-next-0.15.0/README.md
-drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2023-04-19 10:19:26.000267 gyp-next-0.15.0/pylib/
-drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2023-04-19 10:19:26.024267 gyp-next-0.15.0/pylib/gyp/
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    13031 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/MSVSNew.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     6739 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/MSVSProject.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    45350 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/MSVSSettings.py
--rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)    74297 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/MSVSSettings_test.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1789 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/MSVSToolFile.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     5333 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/MSVSUserFile.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    10231 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/MSVSUtil.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    19742 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/MSVSVersion.py
--rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)    24134 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/__init__.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    22667 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/common.py
--rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     2162 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/common_test.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     5287 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/easy_xml.py
--rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     3835 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/easy_xml_test.py
--rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     1886 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/flock_tool.py
-drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2023-04-19 10:19:26.030267 gyp-next-0.15.0/pylib/gyp/generator/
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)        0 2020-03-09 11:55:08.000000 gyp-next-0.15.0/pylib/gyp/generator/__init__.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    31576 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/analyzer.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    49966 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/android.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    49200 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/cmake.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     4596 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/compile_commands_json.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     3101 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/dump_dependency_json.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    17501 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/eclipse.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     3505 2020-04-07 01:30:05.000000 gyp-next-0.15.0/pylib/gyp/generator/gypd.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1713 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/gypsh.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   110357 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/make.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   150599 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/msvs.py
--rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     1266 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/msvs_test.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   118347 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/ninja.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1910 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/ninja_test.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    66020 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/xcode.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)      672 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/generator/xcode_test.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   126426 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/input.py
--rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     3425 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/input_test.py
--rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)    30260 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/mac_tool.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    54137 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/msvs_emulation.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     5640 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/ninja_syntax.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1293 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/simple_copy.py
--rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)    15131 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/win_tool.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    81728 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/xcode_emulation.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    12124 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/xcode_ninja.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   135649 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/xcodeproj_file.py
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     2245 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pylib/gyp/xml_fix.py
-drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2023-04-19 10:19:26.031267 gyp-next-0.15.0/pylib/gyp_next.egg-info/
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     3836 2023-04-19 10:19:25.000000 gyp-next-0.15.0/pylib/gyp_next.egg-info/PKG-INFO
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1397 2023-04-19 10:19:25.000000 gyp-next-0.15.0/pylib/gyp_next.egg-info/SOURCES.txt
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)        1 2023-04-19 10:19:25.000000 gyp-next-0.15.0/pylib/gyp_next.egg-info/dependency_links.txt
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)       40 2023-04-19 10:19:25.000000 gyp-next-0.15.0/pylib/gyp_next.egg-info/entry_points.txt
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)       26 2023-04-19 10:19:25.000000 gyp-next-0.15.0/pylib/gyp_next.egg-info/requires.txt
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)        4 2023-04-19 10:19:25.000000 gyp-next-0.15.0/pylib/gyp_next.egg-info/top_level.txt
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     2822 2023-04-19 10:05:15.000000 gyp-next-0.15.0/pyproject.toml
--rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)       38 2023-04-19 10:19:26.031267 gyp-next-0.15.0/setup.cfg
+drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2020-07-14 07:18:34.643391 gyp-next-0.4.0/
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1484 2020-07-14 07:18:34.643391 gyp-next-0.4.0/PKG-INFO
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)      433 2020-07-14 07:10:43.000000 gyp-next-0.4.0/README.md
+drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2020-07-14 07:18:34.636724 gyp-next-0.4.0/pylib/
+drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2020-07-14 07:18:34.640058 gyp-next-0.4.0/pylib/gyp/
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    13174 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/MSVSNew.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     6767 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/MSVSProject.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    45532 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/MSVSSettings.py
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)    74324 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/MSVSSettings_test.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1797 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/MSVSToolFile.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     5347 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/MSVSUserFile.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    10233 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/MSVSUtil.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    19521 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/MSVSVersion.py
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)    24242 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/__init__.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    22691 2020-05-17 18:15:26.000000 gyp-next-0.4.0/pylib/gyp/common.py
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     2161 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/common_test.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     5251 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/easy_xml.py
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     3795 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/easy_xml_test.py
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     1866 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/flock_tool.py
+drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2020-07-14 07:18:34.640058 gyp-next-0.4.0/pylib/gyp/generator/
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)        0 2020-03-09 11:55:08.000000 gyp-next-0.4.0/pylib/gyp/generator/__init__.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    31751 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/generator/analyzer.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    49701 2020-06-15 06:46:46.000000 gyp-next-0.4.0/pylib/gyp/generator/android.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    49454 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/generator/cmake.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     4581 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/generator/compile_commands_json.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     3139 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/generator/dump_dependency_json.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    17670 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/generator/eclipse.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     3505 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/generator/gypd.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1709 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/generator/gypsh.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   103184 2020-07-14 07:10:43.000000 gyp-next-0.4.0/pylib/gyp/generator/make.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   151165 2020-06-15 06:46:46.000000 gyp-next-0.4.0/pylib/gyp/generator/msvs.py
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     1352 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/generator/msvs_test.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   118221 2020-06-29 07:07:40.000000 gyp-next-0.4.0/pylib/gyp/generator/ninja.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1909 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/generator/ninja_test.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    66163 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/generator/xcode.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)      671 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/generator/xcode_test.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   128939 2020-06-15 06:46:47.000000 gyp-next-0.4.0/pylib/gyp/input.py
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     3424 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/input_test.py
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)    30380 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/mac_tool.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    53276 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/msvs_emulation.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     5650 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/ninja_syntax.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1399 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/simple_copy.py
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)    15388 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/win_tool.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    81503 2020-06-15 06:46:47.000000 gyp-next-0.4.0/pylib/gyp/xcode_emulation.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)    12141 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/xcode_ninja.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)   135751 2020-04-07 01:30:05.000000 gyp-next-0.4.0/pylib/gyp/xcodeproj_file.py
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     2261 2020-03-15 17:46:13.000000 gyp-next-0.4.0/pylib/gyp/xml_fix.py
+drwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)        0 2020-07-14 07:18:34.643391 gyp-next-0.4.0/pylib/gyp_next.egg-info/
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1484 2020-07-14 07:18:34.000000 gyp-next-0.4.0/pylib/gyp_next.egg-info/PKG-INFO
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)     1338 2020-07-14 07:18:34.000000 gyp-next-0.4.0/pylib/gyp_next.egg-info/SOURCES.txt
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)        1 2020-07-14 07:18:34.000000 gyp-next-0.4.0/pylib/gyp_next.egg-info/dependency_links.txt
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)       41 2020-07-14 07:18:34.000000 gyp-next-0.4.0/pylib/gyp_next.egg-info/entry_points.txt
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)        4 2020-07-14 07:18:34.000000 gyp-next-0.4.0/pylib/gyp_next.egg-info/top_level.txt
+-rw-r--r--   0 ryzokuken  (1000) ryzokuken  (1000)       38 2020-07-14 07:18:34.643391 gyp-next-0.4.0/setup.cfg
+-rwxr-xr-x   0 ryzokuken  (1000) ryzokuken  (1000)     1582 2020-07-14 07:10:43.000000 gyp-next-0.4.0/setup.py
```

### Comparing `gyp-next-0.15.0/pylib/gyp/MSVSNew.py` & `gyp-next-0.4.0/pylib/gyp/MSVSNew.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 import hashlib
 import os
 import random
 from operator import attrgetter
 
 import gyp.common
 
+try:
+    cmp
+except NameError:
 
-def cmp(x, y):
-    return (x > y) - (x < y)
+    def cmp(x, y):
+        return (x > y) - (x < y)
 
 
 # Initialize random number generator
 random.seed()
 
 # GUIDs for project types
 ENTRY_TYPE_GUIDS = {
@@ -62,15 +65,15 @@
     )
     return guid
 
 
 # ------------------------------------------------------------------------------
 
 
-class MSVSSolutionEntry:
+class MSVSSolutionEntry(object):
     def __cmp__(self, other):
         # Sort by name then guid (so things are in order on vs2008).
         return cmp((self.name, self.get_guid()), (other.name, other.get_guid()))
 
 
 class MSVSFolder(MSVSSolutionEntry):
     """Folder in a Visual Studio project or solution."""
@@ -183,15 +186,15 @@
     def set_msbuild_toolset(self, msbuild_toolset):
         self.msbuild_toolset = msbuild_toolset
 
 
 # ------------------------------------------------------------------------------
 
 
-class MSVSSolution:
+class MSVSSolution(object):
     """Visual Studio solution."""
 
     def __init__(
         self, path, version, entries=None, variants=None, websiteProperties=True
     ):
         """Initializes the solution.
 
@@ -281,35 +284,37 @@
                 f.write(
                     "\tProjectSection(WebsiteProperties) = preProject\r\n"
                     '\t\tDebug.AspNetCompiler.Debug = "True"\r\n'
                     '\t\tRelease.AspNetCompiler.Debug = "False"\r\n'
                     "\tEndProjectSection\r\n"
                 )
 
-            if isinstance(e, MSVSFolder) and e.items:
-                f.write("\tProjectSection(SolutionItems) = preProject\r\n")
-                for i in e.items:
-                    f.write(f"\t\t{i} = {i}\r\n")
-                f.write("\tEndProjectSection\r\n")
-
-            if isinstance(e, MSVSProject) and e.dependencies:
-                f.write("\tProjectSection(ProjectDependencies) = postProject\r\n")
-                for d in e.dependencies:
-                    f.write(f"\t\t{d.get_guid()} = {d.get_guid()}\r\n")
-                f.write("\tEndProjectSection\r\n")
+            if isinstance(e, MSVSFolder):
+                if e.items:
+                    f.write("\tProjectSection(SolutionItems) = preProject\r\n")
+                    for i in e.items:
+                        f.write("\t\t%s = %s\r\n" % (i, i))
+                    f.write("\tEndProjectSection\r\n")
+
+            if isinstance(e, MSVSProject):
+                if e.dependencies:
+                    f.write("\tProjectSection(ProjectDependencies) = postProject\r\n")
+                    for d in e.dependencies:
+                        f.write("\t\t%s = %s\r\n" % (d.get_guid(), d.get_guid()))
+                    f.write("\tEndProjectSection\r\n")
 
             f.write("EndProject\r\n")
 
         # Global section
         f.write("Global\r\n")
 
         # Configurations (variants)
         f.write("\tGlobalSection(SolutionConfigurationPlatforms) = preSolution\r\n")
         for v in self.variants:
-            f.write(f"\t\t{v} = {v}\r\n")
+            f.write("\t\t%s = %s\r\n" % (v, v))
         f.write("\tEndGlobalSection\r\n")
 
         # Sort config guids for easier diffing of solution changes.
         config_guids = []
         config_guids_overrides = {}
         for e in all_entries:
             if isinstance(e, MSVSProject):
@@ -353,13 +358,13 @@
         # Omit this section if there are no folders
         if any([e.entries for e in all_entries if isinstance(e, MSVSFolder)]):
             f.write("\tGlobalSection(NestedProjects) = preSolution\r\n")
             for e in all_entries:
                 if not isinstance(e, MSVSFolder):
                     continue  # Does not apply to projects, only folders
                 for subentry in e.entries:
-                    f.write(f"\t\t{subentry.get_guid()} = {e.get_guid()}\r\n")
+                    f.write("\t\t%s = %s\r\n" % (subentry.get_guid(), e.get_guid()))
             f.write("\tEndGlobalSection\r\n")
 
         f.write("EndGlobal\r\n")
 
         f.close()
```

### Comparing `gyp-next-0.15.0/pylib/gyp/MSVSProject.py` & `gyp-next-0.4.0/pylib/gyp/MSVSProject.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """Visual Studio project reader/writer."""
 
 import gyp.easy_xml as easy_xml
 
 # ------------------------------------------------------------------------------
 
 
-class Tool:
+class Tool(object):
     """Visual Studio tool."""
 
     def __init__(self, name, attrs=None):
         """Initializes the tool.
 
     Args:
       name: Tool name.
@@ -27,15 +27,15 @@
 
     Returns:
       A new xml.dom.Element for the tool.
     """
         return ["Tool", self._attrs]
 
 
-class Filter:
+class Filter(object):
     """Visual Studio filter - that is, a virtual folder."""
 
     def __init__(self, name, contents=None):
         """Initializes the folder.
 
     Args:
       name: Filter (folder) name.
@@ -44,15 +44,15 @@
         self.name = name
         self.contents = list(contents or [])
 
 
 # ------------------------------------------------------------------------------
 
 
-class Writer:
+class Writer(object):
     """Visual Studio XML project writer."""
 
     def __init__(self, project_path, version, name, guid=None, platforms=None):
         """Initializes the project.
 
     Args:
       project_path: Path to the project file.
@@ -75,15 +75,15 @@
         for platform in platforms:
             self.platform_section.append(["Platform", {"Name": platform}])
         self.tool_files_section = ["ToolFiles"]
         self.configurations_section = ["Configurations"]
         self.files_section = ["Files"]
 
         # Keep a dict keyed on filename to speed up access.
-        self.files_dict = {}
+        self.files_dict = dict()
 
     def AddToolFile(self, path):
         """Adds a tool file to the project.
 
     Args:
       path: Relative path from project to tool file.
     """
```

### Comparing `gyp-next-0.15.0/pylib/gyp/MSVSSettings.py` & `gyp-next-0.4.0/pylib/gyp/MSVSSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 
 This file was created by comparing the projects created by Visual Studio 2008
 and Visual Studio 2010 for all available settings through the user interface.
 The MSBuild schemas were also considered.  They are typically found in the
 MSBuild install directory, e.g. c:\Program Files (x86)\MSBuild
 """
 
-import re
+from __future__ import print_function
+
+from gyp import string_types
+
 import sys
+import re
 
 # Dictionaries of settings validators. The key is the tool name, the value is
 # a dictionary mapping setting names to validation functions.
 _msvs_validators = {}
 _msbuild_validators = {}
 
 
@@ -28,15 +32,15 @@
 _msvs_to_msbuild_converters = {}
 
 
 # Tool name mapping from MSVS to MSBuild.
 _msbuild_name_of_tool = {}
 
 
-class _Tool:
+class _Tool(object):
     """Represents a tool used by MSVS or MSBuild.
 
   Attributes:
       msvs_name: The name of the tool in MSVS.
       msbuild_name: The name of the tool in MSBuild.
   """
 
@@ -60,15 +64,15 @@
 
 
 def _GetMSBuildToolSettings(msbuild_settings, tool):
     """Returns an MSBuild tool dictionary.  Creates it if needed."""
     return msbuild_settings.setdefault(tool.msbuild_name, {})
 
 
-class _Type:
+class _Type(object):
     """Type of settings (Base class)."""
 
     def ValidateMSVS(self, value):
         """Verifies that the value is legal for MSVS.
 
     Args:
       value: the value to check for this type.
@@ -102,35 +106,35 @@
         return value
 
 
 class _String(_Type):
     """A setting that's just a string."""
 
     def ValidateMSVS(self, value):
-        if not isinstance(value, str):
+        if not isinstance(value, string_types):
             raise ValueError("expected string; got %r" % value)
 
     def ValidateMSBuild(self, value):
-        if not isinstance(value, str):
+        if not isinstance(value, string_types):
             raise ValueError("expected string; got %r" % value)
 
     def ConvertToMSBuild(self, value):
         # Convert the macros
         return ConvertVCMacrosToMSBuild(value)
 
 
 class _StringList(_Type):
     """A settings that's a list of strings."""
 
     def ValidateMSVS(self, value):
-        if not isinstance(value, (list, str)):
+        if not isinstance(value, string_types) and not isinstance(value, list):
             raise ValueError("expected string list; got %r" % value)
 
     def ValidateMSBuild(self, value):
-        if not isinstance(value, (list, str)):
+        if not isinstance(value, string_types) and not isinstance(value, list):
             raise ValueError("expected string list; got %r" % value)
 
     def ConvertToMSBuild(self, value):
         # Convert the macros
         if isinstance(value, list):
             return [ConvertVCMacrosToMSBuild(i) for i in value]
         else:
@@ -187,15 +191,15 @@
         used in the array to indicate the unused spot.
     new: an array of labels that are new to MSBuild.
   """
 
     def __init__(self, label_list, new=None):
         _Type.__init__(self)
         self._label_list = label_list
-        self._msbuild_values = {value for value in label_list if value is not None}
+        self._msbuild_values = set(value for value in label_list if value is not None)
         if new is not None:
             self._msbuild_values.update(new)
 
     def ValidateMSVS(self, value):
         # Try to convert.  It will raise an exception if not valid.
         self.ConvertToMSBuild(value)
 
@@ -334,15 +338,15 @@
     flag: the flag to insert at the end of the AdditionalOptions
   """
 
     def _Translate(value, msbuild_settings):
         if value == "true":
             tool_settings = _GetMSBuildToolSettings(msbuild_settings, tool)
             if "AdditionalOptions" in tool_settings:
-                new_flags = "{} {}".format(tool_settings["AdditionalOptions"], flag)
+                new_flags = "%s %s" % (tool_settings["AdditionalOptions"], flag)
             else:
                 new_flags = flag
             tool_settings["AdditionalOptions"] = new_flags
 
     _msvs_validators[tool.msvs_name][msvs_name] = _boolean.ValidateMSVS
     _msvs_to_msbuild_converters[tool.msvs_name][msvs_name] = _Translate
 
@@ -528,22 +532,22 @@
             tool_validators = validators[tool_name]
             for setting, value in settings[tool_name].items():
                 if setting in tool_validators:
                     try:
                         tool_validators[setting](value)
                     except ValueError as e:
                         print(
-                            f"Warning: for {tool_name}/{setting}, {e}",
+                            "Warning: for %s/%s, %s" % (tool_name, setting, e),
                             file=stderr,
                         )
                 else:
                     _ValidateExclusionSetting(
                         setting,
                         tool_validators,
-                        (f"Warning: unrecognized setting {tool_name}/{setting}"),
+                        ("Warning: unrecognized setting %s/%s" % (tool_name, setting)),
                         stderr,
                     )
 
         else:
             print("Warning: unrecognized tool %s" % (tool_name), file=stderr)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/MSVSSettings_test.py` & `gyp-next-0.4.0/pylib/gyp/MSVSSettings_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """Unit tests for the MSVSSettings.py file."""
 
 import unittest
 import gyp.MSVSSettings as MSVSSettings
 
-from io import StringIO
+try:
+    from StringIO import StringIO  # Python 2
+except ImportError:
+    from io import StringIO  # Python 3
 
 
 class TestSequenceFunctions(unittest.TestCase):
     def setUp(self):
         self.stderr = StringIO()
 
     def _ExpectedWarnings(self, expected):
@@ -671,16 +674,15 @@
             [
                 "Warning: while converting VCCLCompilerTool/BasicRuntimeChecks to "
                 "MSBuild, index value (12) not in expected range [0, 4)",
                 "Warning: while converting VCCLCompilerTool/BrowseInformation to "
                 "MSBuild, index value (21) not in expected range [0, 3)",
                 "Warning: while converting VCCLCompilerTool/UsePrecompiledHeader to "
                 "MSBuild, index value (13) not in expected range [0, 3)",
-                "Warning: while converting "
-                "VCCLCompilerTool/GeneratePreprocessedFile to "
+                "Warning: while converting VCCLCompilerTool/GeneratePreprocessedFile to "
                 "MSBuild, value must be one of [0, 1, 2]; got 14",
                 "Warning: while converting VCLinkerTool/Driver to "
                 "MSBuild, index value (10) not in expected range [0, 4)",
                 "Warning: while converting VCLinkerTool/LinkTimeCodeGeneration to "
                 "MSBuild, index value (31) not in expected range [0, 5)",
                 "Warning: while converting VCLinkerTool/ErrorReporting to "
                 "MSBuild, index value (21) not in expected range [0, 3)",
@@ -1342,16 +1344,15 @@
                 "AdditionalOptions": "afdsdafsd",
                 "AssemblyIdentity": "sddfdsadfsa",
                 "ComponentFileName": "fsdfds",
                 "DependencyInformationFile": "$(IntDir)\\mt.depdfd",
                 "EmbedManifest": "false",
                 "GenerateCatalogFiles": "true",
                 "InputResourceManifests": "asfsfdafs",
-                "ManifestResourceFile":
-                    "$(IntDir)\\$(TargetFileName).embed.manifest.resfdsf",
+                "ManifestResourceFile": "$(IntDir)\\$(TargetFileName).embed.manifest.resfdsf",
                 "OutputManifestFile": "$(TargetPath).manifestdfs",
                 "RegistrarScriptFile": "sdfsfd",
                 "ReplacementsFile": "sdffsd",
                 "SuppressStartupBanner": "false",
                 "TypeLibraryFile": "sfsd",
                 "UpdateFileHashes": "true",
                 "UpdateFileHashesSearchPath": "sfsd",
@@ -1527,16 +1528,15 @@
             "": {
                 "EmbedManifest": "false",
                 "GenerateManifest": "false",
                 "IgnoreImportLibrary": "true",
                 "LinkIncremental": "",
             },
             "ManifestResourceCompile": {
-                "ResourceOutputFileName":
-                    "$(IntDir)$(TargetFileName).embed.manifest.resfdsf"
+                "ResourceOutputFileName": "$(IntDir)$(TargetFileName).embed.manifest.resfdsf"
             },
         }
         self.maxDiff = 9999  # on failure display a long diff
         actual_msbuild_settings = MSVSSettings.ConvertToMSBuildSettings(
             msvs_settings, self.stderr
         )
         self.assertEqual(expected_msbuild_settings, actual_msbuild_settings)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/MSVSToolFile.py` & `gyp-next-0.4.0/pylib/gyp/MSVSToolFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # found in the LICENSE file.
 
 """Visual Studio project reader/writer."""
 
 import gyp.easy_xml as easy_xml
 
 
-class Writer:
+class Writer(object):
     """Visual Studio XML tool file writer."""
 
     def __init__(self, tool_file_path, name):
         """Initializes the tool file.
 
     Args:
       tool_file_path: Path to the tool file.
```

### Comparing `gyp-next-0.15.0/pylib/gyp/MSVSUserFile.py` & `gyp-next-0.4.0/pylib/gyp/MSVSUserFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         # Otherwise, if there are any spaces, quote the whole arg.
         elif re.search(r"[ \t\n]", arg):
             arg = '"%s"' % arg
         new_args.append(arg)
     return new_args
 
 
-class Writer:
+class Writer(object):
     """Visual Studio XML user user file writer."""
 
     def __init__(self, user_file_path, version, name):
         """Initializes the user file.
 
     Args:
       user_file_path: Path to the user file.
@@ -89,15 +89,15 @@
       working_directory: other files which may trigger the rule. (optional)
     """
         command = _QuoteWin32CommandLineArgs(command)
 
         abs_command = _FindCommandInPath(command[0])
 
         if environment and isinstance(environment, dict):
-            env_list = [f'{key}="{val}"' for (key, val) in environment.items()]
+            env_list = ['%s="%s"' % (key, val) for (key, val) in environment.items()]
             environment = " ".join(env_list)
         else:
             environment = ""
 
         n_cmd = [
             "DebugSettings",
             {
```

### Comparing `gyp-next-0.15.0/pylib/gyp/MSVSUtil.py` & `gyp-next-0.4.0/pylib/gyp/MSVSUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   Arguments:
     name: name of the target (foo#target)
     suffix: the suffix to be added
   Returns:
     Target name with suffix added (foo_suffix#target)
   """
     parts = name.rsplit("#", 1)
-    parts[0] = f"{parts[0]}_{suffix}"
+    parts[0] = "%s_%s" % (parts[0], suffix)
     return "#".join(parts)
 
 
 def _ShardName(name, number):
     """Add a shard number to the end of a target.
 
   Arguments:
@@ -156,15 +156,15 @@
 
     variables = target_dict.get("variables", {})
     pdb_path = variables.get("msvs_large_pdb_path", None)
     if pdb_path:
         return pdb_path
 
     pdb_base = target_dict.get("product_name", target_dict["target_name"])
-    pdb_base = "{}.{}.pdb".format(pdb_base, TARGET_TYPE_EXT[target_dict["type"]])
+    pdb_base = "%s.%s.pdb" % (pdb_base, TARGET_TYPE_EXT[target_dict["type"]])
     pdb_path = vars["PRODUCT_DIR"] + "/" + pdb_base
 
     return pdb_path
 
 
 def InsertLargePdbShims(target_list, target_dicts, vars):
     """Insert a shim target that forces the linker to use 4KB pagesize PDBs.
```

### Comparing `gyp-next-0.15.0/pylib/gyp/MSVSVersion.py` & `gyp-next-0.4.0/pylib/gyp/MSVSVersion.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 import errno
 import os
 import re
 import subprocess
 import sys
 import glob
 
+PY3 = bytes != str
+
 
 def JoinPath(*args):
     return os.path.normpath(os.path.join(*args))
 
 
-class VisualStudioVersion:
+class VisualStudioVersion(object):
     """Information regarding a version of Visual Studio."""
 
     def __init__(
         self,
         short_name,
         description,
         solution_version,
@@ -170,15 +172,17 @@
     # Setup params to pass to and attempt to launch reg.exe
     cmd = [os.path.join(os.environ.get("WINDIR", ""), sysdir, "reg.exe"), "query", key]
     if value:
         cmd.extend(["/v", value])
     p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     # Obtain the stdout from reg.exe, reading to the end so p.returncode is valid
     # Note that the error text may be in [1] in some cases
-    text = p.communicate()[0].decode("utf-8")
+    text = p.communicate()[0]
+    if PY3:
+        text = text.decode("utf-8")
     # Check return code from reg.exe; officially 0==success and 1==error
     if p.returncode:
         return None
     return text
 
 
 def _RegistryQuery(key, value=None):
@@ -213,23 +217,29 @@
     """Use the _winreg module to obtain the value of a registry key.
 
   Args:
     key: The registry key.
     value: The particular registry value to read.
   Return:
     contents of the registry key's value, or None on failure.  Throws
-    ImportError if winreg is unavailable.
+    ImportError if _winreg is unavailable.
   """
-    from winreg import HKEY_LOCAL_MACHINE, OpenKey, QueryValueEx
+    try:
+        # Python 2
+        from _winreg import HKEY_LOCAL_MACHINE, OpenKey, QueryValueEx
+    except ImportError:
+        # Python 3
+        from winreg import HKEY_LOCAL_MACHINE, OpenKey, QueryValueEx
+
     try:
         root, subkey = key.split("\\", 1)
         assert root == "HKLM"  # Only need HKLM for now.
         with OpenKey(HKEY_LOCAL_MACHINE, subkey) as hkey:
             return QueryValueEx(hkey, value)[0]
-    except OSError:
+    except WindowsError:
         return None
 
 
 def _RegistryGetValue(key, value):
     """Use _winreg or reg.exe to obtain the value of a registry key.
 
   Using _winreg is preferable because it solves an issue on some corporate
@@ -265,26 +275,14 @@
   Setup is based off the GYP_MSVS_VERSION environment variable or whatever is
   autodetected if GYP_MSVS_VERSION is not explicitly specified. If a version is
   passed in that doesn't match a value in versions python will throw a error.
   """
     if path:
         path = os.path.normpath(path)
     versions = {
-        "2022": VisualStudioVersion(
-            "2022",
-            "Visual Studio 2022",
-            solution_version="12.00",
-            project_version="17.0",
-            flat_sln=False,
-            uses_vcxproj=True,
-            path=path,
-            sdk_based=sdk_based,
-            default_toolset="v143",
-            compatible_sdks=["v8.1", "v10.0"],
-        ),
         "2019": VisualStudioVersion(
             "2019",
             "Visual Studio 2019",
             solution_version="12.00",
             project_version="16.0",
             flat_sln=False,
             uses_vcxproj=True,
@@ -424,15 +422,17 @@
     return versions[str(name)]
 
 
 def _ConvertToCygpath(path):
     """Convert to cygwin path if we are using cygwin."""
     if sys.platform == "cygwin":
         p = subprocess.Popen(["cygpath", path], stdout=subprocess.PIPE)
-        path = p.communicate()[0].decode("utf-8").strip()
+        path = p.communicate()[0].strip()
+        if PY3:
+            path = path.decode("utf-8")
     return path
 
 
 def _DetectVisualStudioVersions(versions_to_check, force_express):
     """Collect the list of installed visual studio versions.
 
   Returns:
@@ -444,27 +444,25 @@
       2008(e) - Visual Studio 2008 (9)
       2010(e) - Visual Studio 2010 (10)
       2012(e) - Visual Studio 2012 (11)
       2013(e) - Visual Studio 2013 (12)
       2015    - Visual Studio 2015 (14)
       2017    - Visual Studio 2017 (15)
       2019    - Visual Studio 2019 (16)
-      2022    - Visual Studio 2022 (17)
     Where (e) is e for express editions of MSVS and blank otherwise.
   """
     version_to_year = {
         "8.0": "2005",
         "9.0": "2008",
         "10.0": "2010",
         "11.0": "2012",
         "12.0": "2013",
         "14.0": "2015",
         "15.0": "2017",
         "16.0": "2019",
-        "17.0": "2022",
     }
     versions = []
     for version in versions_to_check:
         # Old method of searching for which VS version is installed
         # We don't use the 2010-encouraged-way because we also want to get the
         # path to the binaries, which it doesn't offer.
         keys = [
@@ -532,29 +530,28 @@
   Returns:
     An object representing a visual studio project format version.
   """
     # In auto mode, check environment variable for override.
     if version == "auto":
         version = os.environ.get("GYP_MSVS_VERSION", "auto")
     version_map = {
-        "auto": ("17.0", "16.0", "15.0", "14.0", "12.0", "10.0", "9.0", "8.0", "11.0"),
+        "auto": ("16.0", "15.0", "14.0", "12.0", "10.0", "9.0", "8.0", "11.0"),
         "2005": ("8.0",),
         "2005e": ("8.0",),
         "2008": ("9.0",),
         "2008e": ("9.0",),
         "2010": ("10.0",),
         "2010e": ("10.0",),
         "2012": ("11.0",),
         "2012e": ("11.0",),
         "2013": ("12.0",),
         "2013e": ("12.0",),
         "2015": ("14.0",),
         "2017": ("15.0",),
         "2019": ("16.0",),
-        "2022": ("17.0",),
     }
     override_path = os.environ.get("GYP_MSVS_OVERRIDE_PATH")
     if override_path:
         msvs_version = os.environ.get("GYP_MSVS_VERSION")
         if not msvs_version:
             raise ValueError(
                 "GYP_MSVS_OVERRIDE_PATH requires GYP_MSVS_VERSION to be "
```

### Comparing `gyp-next-0.15.0/pylib/gyp/__init__.py` & `gyp-next-0.4.0/pylib/gyp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
+from __future__ import print_function
 
 import copy
 import gyp.input
 import argparse
 import os.path
 import re
 import shlex
 import sys
 import traceback
 from gyp.common import GypError
 
+try:
+    # Python 2
+    string_types = basestring
+except NameError:
+    # Python 3
+    string_types = str
 
 # Default debug modes for GYP
 debug = {}
 
 # List of "official" debug modes, but you can use anything you like.
 DEBUG_GENERAL = "general"
 DEBUG_VARIABLES = "variables"
@@ -57,14 +64,15 @@
     format,
     default_variables={},
     includes=[],
     depth=".",
     params=None,
     check=False,
     circular_check=True,
+    duplicate_basename_check=True,
 ):
     """
   Loads one or more specified build files.
   default_variables and includes will be copied before use.
   Returns the generator for the specified format and the
   data returned by loading the specified build files.
   """
@@ -100,28 +108,14 @@
 
     # These parameters are passed in order (as opposed to by key)
     # because ActivePython cannot handle key parameters to __import__.
     generator = __import__(generator_name, globals(), locals(), generator_name)
     for (key, val) in generator.generator_default_variables.items():
         default_variables.setdefault(key, val)
 
-    output_dir = params["options"].generator_output or params["options"].toplevel_dir
-    if default_variables["GENERATOR"] == "ninja":
-        default_variables.setdefault(
-            "PRODUCT_DIR_ABS",
-            os.path.join(
-                output_dir, "out", default_variables.get("build_type", "default")
-            ),
-        )
-    else:
-        default_variables.setdefault(
-            "PRODUCT_DIR_ABS",
-            os.path.join(output_dir, default_variables["CONFIGURATION_NAME"]),
-        )
-
     # Give the generator the opportunity to set additional variables based on
     # the params it will receive in the output phase.
     if getattr(generator, "CalculateVariables", None):
         generator.CalculateVariables(default_variables, params)
 
     # Give the generator the opportunity to set generator_input_info based on
     # the params it will receive in the output phase.
@@ -158,14 +152,15 @@
         build_files,
         default_variables,
         includes[:],
         depth,
         generator_input_info,
         check,
         circular_check,
+        duplicate_basename_check,
         params["parallel"],
         params["root_targets"],
     )
     return [generator] + result
 
 
 def NameValueListToDict(name_value_list):
@@ -196,15 +191,15 @@
     if flags:
         flags = shlex.split(flags)
     return flags
 
 
 def FormatOpt(opt, value):
     if opt.startswith("--"):
-        return f"{opt}={value}"
+        return "%s=%s" % (opt, value)
     return opt + value
 
 
 def RegenerateAppendFlag(flag, values, predicate, env_name, options):
     """Regenerate a list of command line flags, for an option of action='append'.
 
   The |env_name|, if given, is checked in the environment and used to generate
@@ -432,14 +427,28 @@
         "--no-circular-check",
         dest="circular_check",
         action="store_false",
         default=True,
         regenerate=False,
         help="don't check for circular relationships between files",
     )
+    # --no-duplicate-basename-check disables the check for duplicate basenames
+    # in a static_library/shared_library project. Visual C++ 2008 generator
+    # doesn't support this configuration. Libtool on Mac also generates warnings
+    # when duplicate basenames are passed into Make generator on Mac.
+    # TODO(yukawa): Remove this option when these legacy generators are
+    # deprecated.
+    parser.add_argument(
+        "--no-duplicate-basename-check",
+        dest="duplicate_basename_check",
+        action="store_false",
+        default=True,
+        regenerate=False,
+        help="don't check for duplicate basenames",
+    )
     parser.add_argument(
         "--no-parallel",
         action="store_true",
         default=False,
         help="Disable multiprocessing",
     )
     parser.add_argument(
@@ -462,27 +471,16 @@
         "-R",
         "--root-target",
         dest="root_targets",
         action="append",
         metavar="TARGET",
         help="include only TARGET and its deep dependencies",
     )
-    parser.add_argument(
-        "-V",
-        "--version",
-        dest="version",
-        action="store_true",
-        help="Show the version and exit.",
-    )
 
     options, build_files_arg = parser.parse_args(args)
-    if options.version:
-        import pkg_resources
-        print(f"v{pkg_resources.get_distribution('gyp-next').version}")
-        return 0
     build_files = build_files_arg
 
     # Set up the configuration directory (defaults to ~/.gyp)
     if not options.config_dir:
         home = None
         home_dot_gyp = None
         if options.use_environment:
@@ -538,15 +536,15 @@
 
     # Do an extra check to avoid work when we're not debugging.
     if DEBUG_GENERAL in gyp.debug:
         DebugOutput(DEBUG_GENERAL, "running with these options:")
         for option, value in sorted(options.__dict__.items()):
             if option[0] == "_":
                 continue
-            if isinstance(value, str):
+            if isinstance(value, string_types):
                 DebugOutput(DEBUG_GENERAL, "  %s: '%s'", option, value)
             else:
                 DebugOutput(DEBUG_GENERAL, "  %s: %s", option, value)
 
     if not build_files:
         build_files = FindBuildFiles()
     if not build_files:
@@ -620,15 +618,15 @@
     # are global across all generator runs.
     gen_flags = []
     if options.use_environment:
         gen_flags += ShlexEnv("GYP_GENERATOR_FLAGS")
     if options.generator_flags:
         gen_flags += options.generator_flags
     generator_flags = NameValueListToDict(gen_flags)
-    if DEBUG_GENERAL in gyp.debug:
+    if DEBUG_GENERAL in gyp.debug.keys():
         DebugOutput(DEBUG_GENERAL, "generator_flags: %s", generator_flags)
 
     # Generate all requested formats (use a set in case we got one format request
     # twice)
     for format in set(options.formats):
         params = {
             "options": options,
@@ -649,14 +647,15 @@
             format,
             cmdline_default_variables,
             includes,
             options.depth,
             params,
             options.check,
             options.circular_check,
+            options.duplicate_basename_check,
         )
 
         # TODO(mark): Pass |data| for now because the generator needs a list of
         # build files that came in.  In the future, maybe it should just accept
         # a list, and not the whole data dict.
         # NOTE: flat_list is the flattened dependency graph specifying the order
         # that targets may be built.  Build systems that operate serially or that
```

### Comparing `gyp-next-0.15.0/pylib/gyp/common.py` & `gyp-next-0.4.0/pylib/gyp/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,25 @@
 import filecmp
 import os.path
 import re
 import tempfile
 import sys
 import subprocess
 
-from collections.abc import MutableSet
+try:
+    from collections.abc import MutableSet
+except ImportError:
+    from collections import MutableSet
+
+PY3 = bytes != str
 
 
 # A minimal memoizing decorator. It'll blow up if the args aren't immutable,
 # among other "problems".
-class memoize:
+class memoize(object):
     def __init__(self, func):
         self.func = func
         self.cache = {}
 
     def __call__(self, *args):
         try:
             return self.cache[args]
@@ -140,24 +145,28 @@
     # relative_to.
     # If |follow_symlink_path| is true (default) and |path| is a symlink, then
     # this method returns a path to the real file represented by |path|. If it is
     # false, this method returns a path to the symlink. If |path| is not a
     # symlink, this option has no effect.
 
     # Convert to normalized (and therefore absolute paths).
-    path = os.path.realpath(path) if follow_path_symlink else os.path.abspath(path)
+    if follow_path_symlink:
+        path = os.path.realpath(path)
+    else:
+        path = os.path.abspath(path)
     relative_to = os.path.realpath(relative_to)
 
     # On Windows, we can't create a relative path to a different drive, so just
     # use the absolute path.
-    if sys.platform == "win32" and (
-        os.path.splitdrive(path)[0].lower()
-        != os.path.splitdrive(relative_to)[0].lower()
-    ):
-        return path
+    if sys.platform == "win32":
+        if (
+            os.path.splitdrive(path)[0].lower()
+            != os.path.splitdrive(relative_to)[0].lower()
+        ):
+            return path
 
     # Split the paths into components.
     path_split = path.split(os.path.sep)
     relative_to_split = relative_to.split(os.path.sep)
 
     # Determine how much of the prefix the two paths share.
     prefix_len = len(os.path.commonprefix([path_split, relative_to_split]))
@@ -269,15 +278,18 @@
   to remain intact without escaping the $, to allow the argument to contain
   references to variables to be expanded by the shell.
   """
 
     if not isinstance(argument, str):
         argument = str(argument)
 
-    quote = '"' if _quote.search(argument) else ""
+    if _quote.search(argument):
+        quote = '"'
+    else:
+        quote = ""
 
     encoded = quote + re.sub(_escape, r"\\\1", argument) + quote
 
     return encoded
 
 
 def EncodePOSIXShellList(list):
@@ -332,26 +344,22 @@
   Arguments:
     filename: name of the file to potentially write to.
   Returns:
     A file like object which will write to temporary file and only overwrite
     the target if it differs (on close).
   """
 
-    class Writer:
+    class Writer(object):
         """Wrapper around file which only covers the target if it differs."""
 
         def __init__(self):
-            # On Cygwin remove the "dir" argument
-            # `C:` prefixed paths are treated as relative,
-            # consequently ending up with current dir "/cygdrive/c/..."
-            # being prefixed to those, which was
-            # obviously a non-existent path,
-            # for example: "/cygdrive/c/<some folder>/C:\<my win style abs path>".
-            # For more details see:
-            # https://docs.python.org/2/library/tempfile.html#tempfile.mkstemp
+            # On Cygwin remove the "dir" argument because `C:` prefixed paths are treated as relative,
+            # consequently ending up with current dir "/cygdrive/c/..." being prefixed to those, which was
+            # obviously a non-existent path, for example: "/cygdrive/c/<some folder>/C:\<my win style abs path>".
+            # See https://docs.python.org/2/library/tempfile.html#tempfile.mkstemp for more details
             base_temp_dir = "" if IsCygwin() else os.path.dirname(filename)
             # Pick temporary file.
             tmp_fd, self.tmp_path = tempfile.mkstemp(
                 suffix=".tmp",
                 prefix=os.path.split(filename)[1] + ".gyp.",
                 dir=base_temp_dir,
             )
@@ -379,33 +387,31 @@
                         raise
 
                 if same:
                     # The new file is identical to the old one, just get rid of the new
                     # one.
                     os.unlink(self.tmp_path)
                 else:
-                    # The new file is different from the old one,
-                    # or there is no old one.
+                    # The new file is different from the old one, or there is no old one.
                     # Rename the new file to the permanent name.
                     #
                     # tempfile.mkstemp uses an overly restrictive mode, resulting in a
                     # file that can only be read by the owner, regardless of the umask.
-                    # There's no reason to not respect the umask here,
-                    # which means that an extra hoop is required
-                    # to fetch it and reset the new file's mode.
+                    # There's no reason to not respect the umask here, which means that
+                    # an extra hoop is required to fetch it and reset the new file's mode.
                     #
                     # No way to get the umask without setting a new one?  Set a safe one
                     # and then set it back to the old value.
                     umask = os.umask(0o77)
                     os.umask(umask)
                     os.chmod(self.tmp_path, 0o666 & ~umask)
                     if sys.platform == "win32" and os.path.exists(filename):
                         # NOTE: on windows (but not cygwin) rename will not replace an
-                        # existing file, so it must be preceded with a remove.
-                        # Sadly there is no way to make the switch atomic.
+                        # existing file, so it must be preceded with a remove. Sadly there
+                        # is no way to make the switch atomic.
                         os.remove(filename)
                     os.rename(self.tmp_path, filename)
             except Exception:
                 # Don't leave turds behind.
                 os.unlink(self.tmp_path)
                 raise
 
@@ -443,33 +449,26 @@
         return "openbsd"
     if sys.platform.startswith("netbsd"):
         return "netbsd"
     if sys.platform.startswith("aix"):
         return "aix"
     if sys.platform.startswith(("os390", "zos")):
         return "zos"
-    if sys.platform == "os400":
-        return "os400"
 
     return "linux"
 
 
 def CopyTool(flavor, out_path, generator_flags={}):
     """Finds (flock|mac|win)_tool.gyp in the gyp directory and copies it
   to |out_path|."""
     # aix and solaris just need flock emulation. mac and win use more complicated
     # support scripts.
-    prefix = {
-        "aix": "flock",
-        "os400": "flock",
-        "solaris": "flock",
-        "mac": "mac",
-        "ios": "mac",
-        "win": "win",
-    }.get(flavor, None)
+    prefix = {"aix": "flock", "solaris": "flock", "mac": "mac", "win": "win"}.get(
+        flavor, None
+    )
     if not prefix:
         return
 
     # Slurp input file.
     source_path = os.path.join(
         os.path.dirname(os.path.abspath(__file__)), "%s_tool.py" % prefix
     )
@@ -557,16 +556,16 @@
             raise KeyError("set is empty")
         key = self.end[1][0] if last else self.end[2][0]
         self.discard(key)
         return key
 
     def __repr__(self):
         if not self:
-            return f"{self.__class__.__name__}()"
-        return f"{self.__class__.__name__}({list(self)!r})"
+            return "%s()" % (self.__class__.__name__,)
+        return "%s(%r)" % (self.__class__.__name__, list(self))
 
     def __eq__(self, other):
         if isinstance(other, OrderedSet):
             return len(self) == len(other) and list(self) == list(other)
         return set(self) == set(other)
 
     # Extensions to the recipe.
@@ -644,11 +643,13 @@
 
 
 def IsCygwin():
     try:
         out = subprocess.Popen(
             "uname", stdout=subprocess.PIPE, stderr=subprocess.STDOUT
         )
-        stdout = out.communicate()[0].decode("utf-8")
+        stdout, stderr = out.communicate()
+        if PY3:
+            stdout = stdout.decode("utf-8")
         return "CYGWIN" in str(stdout)
     except Exception:
         return False
```

### Comparing `gyp-next-0.15.0/pylib/gyp/common_test.py` & `gyp-next-0.4.0/pylib/gyp/common_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """Unit tests for the common.py file."""
```

### Comparing `gyp-next-0.15.0/pylib/gyp/easy_xml.py` & `gyp-next-0.4.0/pylib/gyp/easy_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) 2011 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
-import sys
 import re
 import os
 import locale
 from functools import reduce
 
 
 def XmlToString(content, encoding="utf-8", pretty=False):
@@ -81,15 +80,15 @@
         )
     xml_parts.append(indentation + "<" + name)
 
     # Optionally in second position is a dictionary of the attributes.
     rest = specification[1:]
     if rest and isinstance(rest[0], dict):
         for at, val in sorted(rest[0].items()):
-            xml_parts.append(f' {at}="{_XmlEscape(val, attr=True)}"')
+            xml_parts.append(' %s="%s"' % (at, _XmlEscape(val, attr=True)))
         rest = rest[1:]
     if rest:
         xml_parts.append(">")
         all_strings = reduce(lambda x, y: x and isinstance(y, str), rest, True)
         multi_line = not all_strings
         if multi_line and new_line:
             xml_parts.append(new_line)
@@ -98,21 +97,20 @@
             # Otherwise recurse over that child definition
             if isinstance(child_spec, str):
                 xml_parts.append(_XmlEscape(child_spec))
             else:
                 _ConstructContentList(xml_parts, child_spec, pretty, level + 1)
         if multi_line and indentation:
             xml_parts.append(indentation)
-        xml_parts.append(f"</{name}>{new_line}")
+        xml_parts.append("</%s>%s" % (name, new_line))
     else:
         xml_parts.append("/>%s" % new_line)
 
 
-def WriteXmlIfChanged(content, path, encoding="utf-8", pretty=False,
-                      win32=(sys.platform == "win32")):
+def WriteXmlIfChanged(content, path, encoding="utf-8", pretty=False, win32=False):
     """ Writes the XML content to disk, touching the file only if it has changed.
 
   Args:
     content:  The structured content to be written.
     path: Location of the file.
     encoding: The encoding to report on the first line of the XML file.
     pretty: True if we want pretty printing with indents and new lines.
@@ -123,17 +121,17 @@
 
     default_encoding = locale.getdefaultlocale()[1]
     if default_encoding and default_encoding.upper() != encoding.upper():
         xml_string = xml_string.encode(encoding)
 
     # Get the old content
     try:
-        with open(path) as file:
+        with open(path, "r") as file:
             existing = file.read()
-    except OSError:
+    except IOError:
         existing = None
 
     # It has changed, write it
     if existing != xml_string:
         with open(path, "wb") as file:
             file.write(xml_string)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/easy_xml_test.py` & `gyp-next-0.4.0/pylib/gyp/easy_xml_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # Copyright (c) 2011 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """ Unit tests for the easy_xml.py file. """
 
 import gyp.easy_xml as easy_xml
 import unittest
 
-from io import StringIO
+try:
+    from StringIO import StringIO  # Python 2
+except ImportError:
+    from io import StringIO  # Python 3
 
 
 class TestSequenceFunctions(unittest.TestCase):
     def setUp(self):
         self.stderr = StringIO()
 
     def test_EasyXml_simple(self):
@@ -72,15 +75,14 @@
             "</PropertyGroup>"
             '<Import Project="$(VCTargetsPath)\\Microsoft.Cpp.props"/>'
             "<PropertyGroup "
             "Condition=\"'$(Configuration)|$(Platform)'=="
             '\'Debug|Win32\'" Label="Configuration">'
             "<ConfigurationType>Application</ConfigurationType>"
             "<CharacterSet>Unicode</CharacterSet>"
-            "<SpectreMitigation>SpectreLoadCF</SpectreMitigation>"
             "</PropertyGroup>"
             "</Project>"
         )
 
         xml = easy_xml.XmlToString(
             [
                 "Project",
@@ -96,15 +98,14 @@
                     "PropertyGroup",
                     {
                         "Condition": "'$(Configuration)|$(Platform)'=='Debug|Win32'",
                         "Label": "Configuration",
                     },
                     ["ConfigurationType", "Application"],
                     ["CharacterSet", "Unicode"],
-                    ["SpectreMitigation", "SpectreLoadCF"]
                 ],
             ]
         )
         self.assertEqual(xml, target)
 
 
 if __name__ == "__main__":
```

### Comparing `gyp-next-0.15.0/pylib/gyp/flock_tool.py` & `gyp-next-0.4.0/pylib/gyp/flock_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # Copyright (c) 2011 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """These functions are executed via gyp-flock-tool when using the Makefile
 generator.  Used on systems that don't have a built-in flock."""
 
@@ -14,15 +14,15 @@
 
 
 def main(args):
     executor = FlockTool()
     executor.Dispatch(args)
 
 
-class FlockTool:
+class FlockTool(object):
     """This class emulates the 'flock' command."""
 
     def Dispatch(self, args):
         """Dispatches a string command to a method."""
         if len(args) < 1:
             raise Exception("Not enough arguments")
 
@@ -37,15 +37,15 @@
         """Emulates the most basic behavior of Linux's flock(1)."""
         # Rely on exception handling to report errors.
         # Note that the stock python on SunOS has a bug
         # where fcntl.flock(fd, LOCK_EX) always fails
         # with EBADF, that's why we use this F_SETLK
         # hack instead.
         fd = os.open(lockfile, os.O_WRONLY | os.O_NOCTTY | os.O_CREAT, 0o666)
-        if sys.platform.startswith("aix") or sys.platform == "os400":
+        if sys.platform.startswith("aix"):
             # Python on AIX is compiled with LARGEFILE support, which changes the
             # struct size.
             op = struct.pack("hhIllqq", fcntl.F_WRLCK, 0, 0, 0, 0, 0, 0)
         else:
             op = struct.pack("hhllhhl", fcntl.F_WRLCK, 0, 0, 0, 0, 0, 0)
         fcntl.fcntl(fd, fcntl.F_SETLK, op)
         return subprocess.call(cmd_list)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/analyzer.py` & `gyp-next-0.4.0/pylib/gyp/generator/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 "a2", and file "b.gyp" contains targets "b1" and "b2" and "a2" has a dependency
 on "b2" and gyp is supplied "a.gyp" then "all" consists of "a1" and "a2".
 Notice that "b1" and "b2" are not in the "all" target as "b.gyp" was not
 directly supplied to gyp. OTOH if both "a.gyp" and "b.gyp" are supplied to gyp
 then the "all" target includes "b1" and "b2".
 """
 
+from __future__ import print_function
 
 import gyp.common
 import json
 import os
 import posixpath
 
 debug = False
@@ -211,15 +212,15 @@
     if "rules" in target_dict:
         for rule in target_dict["rules"]:
             _ExtractSourcesFromAction(rule, base_path, base_path_components, results)
 
     return results
 
 
-class Target:
+class Target(object):
     """Holds information about a particular target:
   deps: set of Targets this Target depends upon. This is not recursive, only the
     direct dependent Targets.
   match_status: one of the MatchStatus values.
   back_deps: set of Targets that have a dependency on this Target.
   visited: used during iteration to indicate whether we've visited this target.
     This is used for two iterations, once in building the set of Targets and
@@ -247,15 +248,15 @@
         self.added_to_compile_targets = False
         self.in_roots = False
         self.is_executable = False
         self.is_static_library = False
         self.is_or_has_linked_ancestor = False
 
 
-class Config:
+class Config(object):
     """Details what we're looking for
   files: set of files to search for
   targets: see file description for details."""
 
     def __init__(self):
         self.files = []
         self.targets = set()
@@ -266,18 +267,18 @@
         """Initializes Config. This is a separate method as it raises an exception
     if there is a parse error."""
         generator_flags = params.get("generator_flags", {})
         config_path = generator_flags.get("config_path", None)
         if not config_path:
             return
         try:
-            f = open(config_path)
+            f = open(config_path, "r")
             config = json.load(f)
             f.close()
-        except OSError:
+        except IOError:
             raise Exception("Unable to open file " + config_path)
         except ValueError as e:
             raise Exception("Unable to parse config file " + config_path + str(e))
         if not isinstance(config, dict):
             raise Exception("config_path must be a JSON file containing a dictionary")
         self.files = config.get("files", [])
         self.additional_compile_target_names = set(
@@ -429,22 +430,22 @@
   . mapping (dictionary) from unqualified name to Target for all the
     Targets in |to_find|.
   . any target names not found. If this is empty all targets were found."""
     result = {}
     if not to_find:
         return {}, []
     to_find = set(to_find)
-    for target_name in all_targets:
+    for target_name in all_targets.keys():
         extracted = gyp.common.ParseQualifiedTarget(target_name)
         if len(extracted) > 1 and extracted[1] in to_find:
             to_find.remove(extracted[1])
             result[extracted[1]] = all_targets[target_name]
             if not to_find:
                 return result, []
-    return result, list(to_find)
+    return result, [x for x in to_find]
 
 
 def _DoesTargetDependOnMatchingTargets(target):
     """Returns true if |target| or any of its dependencies is one of the
   targets containing the files supplied as input to analyzer. This updates
   |matches| of the Targets as it recurses.
   target: the Target to look for."""
@@ -581,15 +582,15 @@
     if not output_path:
         print(json.dumps(values))
         return
     try:
         f = open(output_path, "w")
         f.write(json.dumps(values) + "\n")
         f.close()
-    except OSError as e:
+    except IOError as e:
         print("Error writing to output file", output_path, str(e))
 
 
 def _WasGypIncludeFileModified(params, files):
     """Returns true if one of the files in |files| is in the set of included
   files."""
     if params["options"].includes:
@@ -622,15 +623,15 @@
     else:
         operating_system = flavor
         if flavor == "android":
             operating_system = "linux"  # Keep this legacy behavior for now.
         default_variables.setdefault("OS", operating_system)
 
 
-class TargetCalculator:
+class TargetCalculator(object):
     """Calculates the matching test_targets and matching compile_targets."""
 
     def __init__(
         self,
         files,
         additional_compile_target_names,
         test_target_names,
@@ -679,34 +680,36 @@
         test_target_names_no_all = set(self._test_target_names)
         test_target_names_no_all.discard("all")
         test_targets_no_all = _LookupTargets(
             test_target_names_no_all, self._unqualified_mapping
         )
         test_target_names_contains_all = "all" in self._test_target_names
         if test_target_names_contains_all:
-            test_targets = list(set(test_targets_no_all) | set(self._root_targets))
+            test_targets = [
+                x for x in (set(test_targets_no_all) | set(self._root_targets))
+            ]
         else:
-            test_targets = list(test_targets_no_all)
+            test_targets = [x for x in test_targets_no_all]
         print("supplied test_targets")
         for target_name in self._test_target_names:
             print("\t", target_name)
         print("found test_targets")
         for target in test_targets:
             print("\t", target.name)
         print("searching for matching test targets")
         matching_test_targets = _GetTargetsDependingOnMatchingTargets(test_targets)
         matching_test_targets_contains_all = test_target_names_contains_all and set(
             matching_test_targets
         ) & set(self._root_targets)
         if matching_test_targets_contains_all:
             # Remove any of the targets for all that were not explicitly supplied,
             # 'all' is subsequentely added to the matching names below.
-            matching_test_targets = list(
-                set(matching_test_targets) & set(test_targets_no_all)
-            )
+            matching_test_targets = [
+                x for x in (set(matching_test_targets) & set(test_targets_no_all))
+            ]
         print("matched test_targets")
         for target in matching_test_targets:
             print("\t", target.name)
         matching_target_names = [
             gyp.common.ParseQualifiedTarget(target.name)[1]
             for target in matching_test_targets
         ]
@@ -723,15 +726,17 @@
         for target in self._name_to_target.values():
             target.visited = False
 
         supplied_targets = _LookupTargets(
             self._supplied_target_names_no_all(), self._unqualified_mapping
         )
         if "all" in self._supplied_target_names():
-            supplied_targets = list(set(supplied_targets) | set(self._root_targets))
+            supplied_targets = [
+                x for x in (set(supplied_targets) | set(self._root_targets))
+            ]
         print("Supplied test_targets & compile_targets")
         for target in supplied_targets:
             print("\t", target.name)
         print("Finding compile targets")
         compile_targets = _GetCompileTargets(self._changed_targets, supplied_targets)
         return [
             gyp.common.ParseQualifiedTarget(target.name)[1]
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/android.py` & `gyp-next-0.4.0/pylib/gyp/generator/android.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #
 # The code below generates a separate .mk file for each target, but
 # all are sourced by the top-level GypAndroid.mk.  This means that all
 # variables in .mk-files clobber one another, and furthermore that any
 # variables set potentially clash with other Android build system variables.
 # Try to avoid setting global variables where possible.
 
+from __future__ import print_function
 
 import gyp
 import gyp.common
 import gyp.generator.make as make  # Reuse global functions from make backend.
 import os
 import re
 import subprocess
@@ -79,15 +80,15 @@
 
 def IsCPPExtension(ext):
     return make.COMPILABLE_EXTENSIONS.get(ext) == "cxx"
 
 
 def Sourceify(path):
     """Convert a path to its source directory form. The Android backend does not
-    support options.generator_output, so this function is a noop."""
+     support options.generator_output, so this function is a noop."""
     return path
 
 
 # Map from qualified target to path to output.
 # For Android, the target of these maps is a tuple ('static', 'modulename'),
 # ('dynamic', 'modulename'), or ('path', 'some/path') instead of a string,
 # since we link by module.
@@ -95,19 +96,19 @@
 # Map from qualified target to any linkable output.  A subset
 # of target_outputs.  E.g. when mybinary depends on liba, we want to
 # include liba in the linker line; when otherbinary depends on
 # mybinary, we just want to build mybinary first.
 target_link_deps = {}
 
 
-class AndroidMkWriter:
+class AndroidMkWriter(object):
     """AndroidMkWriter packages up the writing of one target-specific Android.mk.
 
-    Its only real entry point is Write(), and is mostly used for namespacing.
-    """
+  Its only real entry point is Write(), and is mostly used for namespacing.
+  """
 
     def __init__(self, android_top_dir):
         self.android_top_dir = android_top_dir
 
     def Write(
         self,
         qualified_target,
@@ -118,26 +119,26 @@
         configs,
         part_of_all,
         write_alias_target,
         sdk_version,
     ):
         """The main entry point: writes a .mk file for a single target.
 
-        Arguments:
-          qualified_target: target we're generating
-          relative_target: qualified target name relative to the root
-          base_path: path relative to source root we're building in, used to resolve
-                     target-relative paths
-          output_filename: output .mk file name to write
-          spec, configs: gyp info
-          part_of_all: flag indicating this target is part of 'all'
-          write_alias_target: flag indicating whether to create short aliases for
-                              this target
-          sdk_version: what to emit for LOCAL_SDK_VERSION in output
-        """
+    Arguments:
+      qualified_target: target we're generating
+      relative_target: qualified target name relative to the root
+      base_path: path relative to source root we're building in, used to resolve
+                 target-relative paths
+      output_filename: output .mk file name to write
+      spec, configs: gyp info
+      part_of_all: flag indicating this target is part of 'all'
+      write_alias_target: flag indicating whether to create short aliases for
+                          this target
+      sdk_version: what to emit for LOCAL_SDK_VERSION in output
+    """
         gyp.common.EnsureDirExists(output_filename)
 
         self.fp = open(output_filename, "w")
 
         self.fp.write(header)
 
         self.qualified_target = qualified_target
@@ -249,23 +250,23 @@
 
         self.fp.close()
         return self.android_module
 
     def WriteActions(self, actions, extra_sources, extra_outputs):
         """Write Makefile code for any 'actions' from the gyp input.
 
-        extra_sources: a list that will be filled in with newly generated source
-                       files, if any
-        extra_outputs: a list that will be filled in with any outputs of these
-                       actions (used to make other pieces dependent on these
-                       actions)
-        """
+    extra_sources: a list that will be filled in with newly generated source
+                   files, if any
+    extra_outputs: a list that will be filled in with any outputs of these
+                   actions (used to make other pieces dependent on these
+                   actions)
+    """
         for action in actions:
             name = make.StringToMakefileVariable(
-                "{}_{}".format(self.relative_target, action["action_name"])
+                "%s_%s" % (self.relative_target, action["action_name"])
             )
             self.WriteLn('### Rules for action "%s":' % action["action_name"])
             inputs = action["inputs"]
             outputs = action["outputs"]
 
             # Build up a list of outputs.
             # Collect the output dirs we'll need.
@@ -345,37 +346,37 @@
                 % (main_output, " ".join(map(self.LocalPathify, inputs)))
             )
             self.WriteLn('\t@echo "%s"' % quiet_cmd)
             self.WriteLn("\t$(hide)%s\n" % command)
             for output in outputs[1:]:
                 # Make each output depend on the main output, with an empty command
                 # to force make to notice that the mtime has changed.
-                self.WriteLn(f"{self.LocalPathify(output)}: {main_output} ;")
+                self.WriteLn("%s: %s ;" % (self.LocalPathify(output), main_output))
 
             extra_outputs += outputs
             self.WriteLn()
 
         self.WriteLn()
 
     def WriteRules(self, rules, extra_sources, extra_outputs):
         """Write Makefile code for any 'rules' from the gyp input.
 
-        extra_sources: a list that will be filled in with newly generated source
-                       files, if any
-        extra_outputs: a list that will be filled in with any outputs of these
-                       rules (used to make other pieces dependent on these rules)
-        """
+    extra_sources: a list that will be filled in with newly generated source
+                   files, if any
+    extra_outputs: a list that will be filled in with any outputs of these
+                   rules (used to make other pieces dependent on these rules)
+    """
         if len(rules) == 0:
             return
 
         for rule in rules:
             if len(rule.get("rule_sources", [])) == 0:
                 continue
             name = make.StringToMakefileVariable(
-                "{}_{}".format(self.relative_target, rule["rule_name"])
+                "%s_%s" % (self.relative_target, rule["rule_name"])
             )
             self.WriteLn('\n### Generated for rule "%s":' % name)
             self.WriteLn('# "%s":' % rule)
 
             inputs = rule.get("inputs")
             for rule_source in rule.get("rule_sources", []):
                 (rule_source_dirname, rule_source_basename) = os.path.split(rule_source)
@@ -447,25 +448,25 @@
                     "%s: %s $(GYP_TARGET_DEPENDENCIES)"
                     % (main_output, main_output_deps)
                 )
                 self.WriteLn("\t%s\n" % command)
                 for output in outputs[1:]:
                     # Make each output depend on the main output, with an empty command
                     # to force make to notice that the mtime has changed.
-                    self.WriteLn(f"{output}: {main_output} ;")
+                    self.WriteLn("%s: %s ;" % (output, main_output))
                 self.WriteLn()
 
         self.WriteLn()
 
     def WriteCopies(self, copies, extra_outputs):
         """Write Makefile code for any 'copies' from the gyp input.
 
-        extra_outputs: a list that will be filled in with any outputs of this action
-                       (used to make other pieces dependent on this action)
-        """
+    extra_outputs: a list that will be filled in with any outputs of this action
+                   (used to make other pieces dependent on this action)
+    """
         self.WriteLn("### Generated for copy rule.")
 
         variable = make.StringToMakefileVariable(self.relative_target + "_copies")
         outputs = []
         for copy in copies:
             for path in copy["files"]:
                 # The Android build system does not allow generation of files into the
@@ -482,33 +483,33 @@
                 # LocalPathify() calls normpath, stripping trailing slashes.
                 path = Sourceify(self.LocalPathify(path))
                 filename = os.path.split(path)[1]
                 output = Sourceify(
                     self.LocalPathify(os.path.join(copy["destination"], filename))
                 )
 
-                self.WriteLn(f"{output}: {path} $(GYP_TARGET_DEPENDENCIES) | $(ACP)")
+                self.WriteLn(
+                    "%s: %s $(GYP_TARGET_DEPENDENCIES) | $(ACP)" % (output, path)
+                )
                 self.WriteLn("\t@echo Copying: $@")
                 self.WriteLn("\t$(hide) mkdir -p $(dir $@)")
                 self.WriteLn("\t$(hide) $(ACP) -rpf $< $@")
                 self.WriteLn()
                 outputs.append(output)
-        self.WriteLn(
-            "{} = {}".format(variable, " ".join(map(make.QuoteSpaces, outputs)))
-        )
+        self.WriteLn("%s = %s" % (variable, " ".join(map(make.QuoteSpaces, outputs))))
         extra_outputs.append("$(%s)" % variable)
         self.WriteLn()
 
     def WriteSourceFlags(self, spec, configs):
         """Write out the flags and include paths used to compile source files for
-        the current target.
+    the current target.
 
-        Args:
-          spec, configs: input from gyp.
-        """
+    Args:
+      spec, configs: input from gyp.
+    """
         for configname, config in sorted(configs.items()):
             extracted_includes = []
 
             self.WriteLn("\n# Flags passed to both C and C++ files.")
             cflags, includes_from_cflags = self.ExtractIncludesFromCFlags(
                 config.get("cflags", []) + config.get("cflags_c", [])
             )
@@ -549,24 +550,24 @@
         self.WriteLn("LOCAL_CPPFLAGS := $(LOCAL_CPPFLAGS_$(GYP_CONFIGURATION))")
         # Android uses separate flags for assembly file invocations, but gyp expects
         # the same CFLAGS to be applied:
         self.WriteLn("LOCAL_ASFLAGS := $(LOCAL_CFLAGS)")
 
     def WriteSources(self, spec, configs, extra_sources):
         """Write Makefile code for any 'sources' from the gyp input.
-        These are source files necessary to build the current target.
-        We need to handle shared_intermediate directory source files as
-        a special case by copying them to the intermediate directory and
-        treating them as a generated sources. Otherwise the Android build
-        rules won't pick them up.
-
-        Args:
-          spec, configs: input from gyp.
-          extra_sources: Sources generated from Actions or Rules.
-        """
+    These are source files necessary to build the current target.
+    We need to handle shared_intermediate directory source files as
+    a special case by copying them to the intermediate directory and
+    treating them as a genereated sources. Otherwise the Android build
+    rules won't pick them up.
+
+    Args:
+      spec, configs: input from gyp.
+      extra_sources: Sources generated from Actions or Rules.
+    """
         sources = filter(make.Compilable, spec.get("sources", []))
         generated_not_sources = [x for x in extra_sources if not make.Compilable(x)]
         extra_sources = filter(make.Compilable, extra_sources)
 
         # Determine and output the C++ extension used by these sources.
         # We simply find the first C++ file and use that extension.
         all_sources = sources + extra_sources
@@ -612,15 +613,15 @@
             if "$(gyp_intermediate_dir)/" not in local_file:
                 basename = os.path.basename(local_file)
                 local_file = "$(gyp_intermediate_dir)/" + basename
             (root, ext) = os.path.splitext(local_file)
             if IsCPPExtension(ext) and ext != local_cpp_extension:
                 local_file = root + local_cpp_extension
             if local_file != source:
-                self.WriteLn(f"{local_file}: {self.LocalPathify(source)}")
+                self.WriteLn("%s: %s" % (local_file, self.LocalPathify(source)))
                 self.WriteLn("\tmkdir -p $(@D); cp $< $@")
                 origin_src_dirs.append(os.path.dirname(source))
             final_generated_sources.append(local_file)
 
         # We add back in all of the non-compilable stuff to make sure that the
         # make rules have dependencies on them.
         final_generated_sources.extend(generated_not_sources)
@@ -635,18 +636,18 @@
         # Write out the flags used to compile the source; this must be done last
         # so that GYP_COPIED_SOURCE_ORIGIN_DIRS can be used as an include path.
         self.WriteSourceFlags(spec, configs)
 
     def ComputeAndroidModule(self, spec):
         """Return the Android module name used for a gyp spec.
 
-        We use the complete qualified target name to avoid collisions between
-        duplicate targets in different directories. We also add a suffix to
-        distinguish gyp-generated module names.
-        """
+    We use the complete qualified target name to avoid collisions between
+    duplicate targets in different directories. We also add a suffix to
+    distinguish gyp-generated module names.
+    """
 
         if int(spec.get("android_unmangled_name", 0)):
             assert self.type != "shared_library" or self.target.startswith("lib")
             return self.target
 
         if self.type == "shared_library":
             # For reasons of convention, the Android build system requires that all
@@ -657,28 +658,28 @@
 
         if spec["toolset"] == "host":
             suffix = "_$(TARGET_$(GYP_VAR_PREFIX)ARCH)_host_gyp"
         else:
             suffix = "_gyp"
 
         if self.path:
-            middle = make.StringToMakefileVariable(f"{self.path}_{self.target}")
+            middle = make.StringToMakefileVariable("%s_%s" % (self.path, self.target))
         else:
             middle = make.StringToMakefileVariable(self.target)
 
         return "".join([prefix, middle, suffix])
 
     def ComputeOutputParts(self, spec):
         """Return the 'output basename' of a gyp spec, split into filename + ext.
 
-        Android libraries must be named the same thing as their module name,
-        otherwise the linker can't find them, so product_name and so on must be
-        ignored if we are building a library, and the "lib" prepending is
-        not done for Android.
-        """
+    Android libraries must be named the same thing as their module name,
+    otherwise the linker can't find them, so product_name and so on must be
+    ignored if we are building a library, and the "lib" prepending is
+    not done for Android.
+    """
         assert self.type != "loadable_module"  # TODO: not supported?
 
         target = spec["target_name"]
         target_prefix = ""
         target_ext = ""
         if self.type == "static_library":
             target = self.ComputeAndroidModule(spec)
@@ -706,25 +707,25 @@
 
         target_stem = target_prefix + target
         return (target_stem, target_ext)
 
     def ComputeOutputBasename(self, spec):
         """Return the 'output basename' of a gyp spec.
 
-        E.g., the loadable module 'foobar' in directory 'baz' will produce
-          'libfoobar.so'
-        """
+    E.g., the loadable module 'foobar' in directory 'baz' will produce
+      'libfoobar.so'
+    """
         return "".join(self.ComputeOutputParts(spec))
 
     def ComputeOutput(self, spec):
         """Return the 'output' (full output path) of a gyp spec.
 
-        E.g., the loadable module 'foobar' in directory 'baz' will produce
-          '$(obj)/baz/libfoobar.so'
-        """
+    E.g., the loadable module 'foobar' in directory 'baz' will produce
+      '$(obj)/baz/libfoobar.so'
+    """
         if self.type == "executable":
             # We install host executables into shared_intermediate_dir so they can be
             # run by gyp rules that refer to PRODUCT_DIR.
             path = "$(gyp_shared_intermediate_dir)"
         elif self.type == "shared_library":
             if self.toolset == "host":
                 path = "$($(GYP_HOST_VAR_PREFIX)HOST_OUT_INTERMEDIATE_LIBRARIES)"
@@ -735,67 +736,67 @@
             if self.toolset == "host":
                 path = (
                     "$(call intermediates-dir-for,%s,%s,true,,"
                     "$(GYP_HOST_VAR_PREFIX))"
                     % (self.android_class, self.android_module)
                 )
             else:
-                path = "$(call intermediates-dir-for,{},{},,,$(GYP_VAR_PREFIX))".format(
+                path = "$(call intermediates-dir-for,%s,%s,,,$(GYP_VAR_PREFIX))" % (
                     self.android_class,
                     self.android_module,
                 )
 
         assert spec.get("product_dir") is None  # TODO: not supported?
         return os.path.join(path, self.ComputeOutputBasename(spec))
 
     def NormalizeIncludePaths(self, include_paths):
-        """Normalize include_paths.
-        Convert absolute paths to relative to the Android top directory.
+        """ Normalize include_paths.
+    Convert absolute paths to relative to the Android top directory.
 
-        Args:
-          include_paths: A list of unprocessed include paths.
-        Returns:
-          A list of normalized include paths.
-        """
+    Args:
+      include_paths: A list of unprocessed include paths.
+    Returns:
+      A list of normalized include paths.
+    """
         normalized = []
         for path in include_paths:
             if path[0] == "/":
                 path = gyp.common.RelativePath(path, self.android_top_dir)
             normalized.append(path)
         return normalized
 
     def ExtractIncludesFromCFlags(self, cflags):
         """Extract includes "-I..." out from cflags
 
-        Args:
-          cflags: A list of compiler flags, which may be mixed with "-I.."
-        Returns:
-          A tuple of lists: (clean_clfags, include_paths). "-I.." is trimmed.
-        """
+    Args:
+      cflags: A list of compiler flags, which may be mixed with "-I.."
+    Returns:
+      A tuple of lists: (clean_clfags, include_paths). "-I.." is trimmed.
+    """
         clean_cflags = []
         include_paths = []
         for flag in cflags:
             if flag.startswith("-I"):
                 include_paths.append(flag[2:])
             else:
                 clean_cflags.append(flag)
 
         return (clean_cflags, include_paths)
 
     def FilterLibraries(self, libraries):
         """Filter the 'libraries' key to separate things that shouldn't be ldflags.
 
-        Library entries that look like filenames should be converted to android
-        module names instead of being passed to the linker as flags.
+    Library entries that look like filenames should be converted to android
+    module names instead of being passed to the linker as flags.
 
-        Args:
-          libraries: the value of spec.get('libraries')
-        Returns:
-          A tuple (static_lib_modules, dynamic_lib_modules, ldflags)
-        """
+    Args:
+      libraries: the value of spec.get('libraries')
+    Returns:
+      A tuple (static_lib_modules, dynamic_lib_modules, ldflags)
+    """
         static_lib_modules = []
         dynamic_lib_modules = []
         ldflags = []
         for libs in libraries:
             # Libs can have multiple words.
             for lib in libs.split():
                 # Filter the system libraries, which are added by default by the Android
@@ -818,18 +819,18 @@
                 if lib.startswith("-l"):
                     ldflags.append(lib)
         return (static_lib_modules, dynamic_lib_modules, ldflags)
 
     def ComputeDeps(self, spec):
         """Compute the dependencies of a gyp spec.
 
-        Returns a tuple (deps, link_deps), where each is a list of
-        filenames that will need to be put in front of make for either
-        building (deps) or linking (link_deps).
-        """
+    Returns a tuple (deps, link_deps), where each is a list of
+    filenames that will need to be put in front of make for either
+    building (deps) or linking (link_deps).
+    """
         deps = []
         link_deps = []
         if "dependencies" in spec:
             deps.extend(
                 [
                     target_outputs[dep]
                     for dep in spec["dependencies"]
@@ -841,17 +842,17 @@
                     link_deps.append(target_link_deps[dep])
             deps.extend(link_deps)
         return (gyp.common.uniquer(deps), gyp.common.uniquer(link_deps))
 
     def WriteTargetFlags(self, spec, configs, link_deps):
         """Write Makefile code to specify the link flags and library dependencies.
 
-        spec, configs: input from gyp.
-        link_deps: link dependency list; see ComputeDeps()
-        """
+    spec, configs: input from gyp.
+    link_deps: link dependency list; see ComputeDeps()
+    """
         # Libraries (i.e. -lfoo)
         # These must be included even for static libraries as some of them provide
         # implicit include paths through the build system.
         libraries = gyp.common.uniquer(spec.get("libraries", []))
         static_libs, dynamic_libs, ldflags_libs = self.FilterLibraries(libraries)
 
         if self.type != "static_library":
@@ -886,33 +887,33 @@
             self.WriteList(dynamic_libs + shared_link_deps, "LOCAL_SHARED_LIBRARIES")
 
     def WriteTarget(
         self, spec, configs, deps, link_deps, part_of_all, write_alias_target
     ):
         """Write Makefile code to produce the final target of the gyp spec.
 
-        spec, configs: input from gyp.
-        deps, link_deps: dependency lists; see ComputeDeps()
-        part_of_all: flag indicating this target is part of 'all'
-        write_alias_target: flag indicating whether to create short aliases for this
-                            target
-        """
+    spec, configs: input from gyp.
+    deps, link_deps: dependency lists; see ComputeDeps()
+    part_of_all: flag indicating this target is part of 'all'
+    write_alias_target: flag indicating whether to create short aliases for this
+                        target
+    """
         self.WriteLn("### Rules for final target.")
 
         if self.type != "none":
             self.WriteTargetFlags(spec, configs, link_deps)
 
         settings = spec.get("aosp_build_settings", {})
         if settings:
             self.WriteLn("### Set directly by aosp_build_settings.")
             for k, v in settings.items():
                 if isinstance(v, list):
                     self.WriteList(v, k)
                 else:
-                    self.WriteLn(f"{k} := {make.QuoteIfNecessary(v)}")
+                    self.WriteLn("%s := %s" % (k, make.QuoteIfNecessary(v)))
             self.WriteLn("")
 
         # Add to the set of targets which represent the gyp 'all' target. We use the
         # name 'gyp_all_modules' as the Android build system doesn't allow the use
         # of the Make target 'all' and because 'all_modules' is the equivalent of
         # the Make target 'all' on Android.
         if part_of_all and write_alias_target:
@@ -923,15 +924,15 @@
 
         # Add an alias from the gyp target name to the Android module name. This
         # simplifies manual builds of the target, and is required by the test
         # framework.
         if self.target != self.android_module and write_alias_target:
             self.WriteLn("# Alias gyp target name.")
             self.WriteLn(".PHONY: %s" % self.target)
-            self.WriteLn(f"{self.target}: {self.android_module}")
+            self.WriteLn("%s: %s" % (self.target, self.android_module))
             self.WriteLn("")
 
         # Add the command to trigger build of the target type depending
         # on the toolset. Ex: BUILD_STATIC_LIBRARY vs. BUILD_HOST_STATIC_LIBRARY
         # NOTE: This has to come last!
         modifier = ""
         if self.toolset == "host":
@@ -970,46 +971,46 @@
         variable=None,
         prefix="",
         quoter=make.QuoteIfNecessary,
         local_pathify=False,
     ):
         """Write a variable definition that is a list of values.
 
-        E.g. WriteList(['a','b'], 'foo', prefix='blah') writes out
-             foo = blaha blahb
-        but in a pretty-printed style.
-        """
+    E.g. WriteList(['a','b'], 'foo', prefix='blah') writes out
+         foo = blaha blahb
+    but in a pretty-printed style.
+    """
         values = ""
         if value_list:
             value_list = [quoter(prefix + value) for value in value_list]
             if local_pathify:
                 value_list = [self.LocalPathify(value) for value in value_list]
             values = " \\\n\t" + " \\\n\t".join(value_list)
-        self.fp.write(f"{variable} :={values}\n\n")
+        self.fp.write("%s :=%s\n\n" % (variable, values))
 
     def WriteLn(self, text=""):
         self.fp.write(text + "\n")
 
     def LocalPathify(self, path):
         """Convert a subdirectory-relative path into a normalized path which starts
-        with the make variable $(LOCAL_PATH) (i.e. the top of the project tree).
-        Absolute paths, or paths that contain variables, are just normalized."""
+    with the make variable $(LOCAL_PATH) (i.e. the top of the project tree).
+    Absolute paths, or paths that contain variables, are just normalized."""
         if "$(" in path or os.path.isabs(path):
             # path is not a file in the project tree in this case, but calling
             # normpath is still important for trimming trailing slashes.
             return os.path.normpath(path)
         local_path = os.path.join("$(LOCAL_PATH)", self.path, path)
         local_path = os.path.normpath(local_path)
         # Check that normalizing the path didn't ../ itself out of $(LOCAL_PATH)
         # - i.e. that the resulting path is still inside the project tree. The
         # path may legitimately have ended up containing just $(LOCAL_PATH), though,
         # so we don't look for a slash.
         assert local_path.startswith(
             "$(LOCAL_PATH)"
-        ), f"Path {path} attempts to escape from gyp path {self.path} !)"
+        ), "Path %s attempts to escape from gyp path %s !)" % (path, self.path)
         return local_path
 
     def ExpandInputRoot(self, template, expansion, dirname):
         if "%(INPUT_ROOT)s" not in template and "%(INPUT_DIRNAME)s" not in template:
             return template
         path = template % {
             "INPUT_ROOT": expansion,
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/cmake.py` & `gyp-next-0.4.0/pylib/gyp/generator/cmake.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,29 @@
 should not be relied on for building.
 
 When using with kdevelop, use version 4.4+. Previous versions of kdevelop will
 not be able to find the header file directories described in the generated
 CMakeLists.txt file.
 """
 
+from __future__ import print_function
 
 import multiprocessing
 import os
 import signal
+import string
 import subprocess
 import gyp.common
 import gyp.xcode_emulation
 
-_maketrans = str.maketrans
+try:
+    # maketrans moved to str in python3.
+    _maketrans = string.maketrans
+except NameError:
+    _maketrans = str.maketrans
 
 generator_default_variables = {
     "EXECUTABLE_PREFIX": "",
     "EXECUTABLE_SUFFIX": "",
     "STATIC_LIB_PREFIX": "lib",
     "STATIC_LIB_SUFFIX": ".a",
     "SHARED_LIB_PREFIX": "lib",
@@ -213,15 +219,15 @@
     if prepend:
         output.write(prepend)
     output.write("${")
     output.write(variable_name)
     output.write("}")
 
 
-class CMakeTargetType:
+class CMakeTargetType(object):
     def __init__(self, command, modifier, property_modifier):
         self.command = command
         self.modifier = modifier
         self.property_modifier = property_modifier
 
 
 cmake_target_type_from_gyp_target_type = {
@@ -253,15 +259,15 @@
     extra_sources: [(<cmake_src>, <src>)] to append with generated source files.
     extra_deps: [<cmake_taget>] to append with generated targets.
     path_to_gyp: relative path from CMakeLists.txt being generated to
         the Gyp file in which the target being generated is defined.
   """
     for action in actions:
         action_name = StringToCMakeTargetName(action["action_name"])
-        action_target_name = f"{target_name}__{action_name}"
+        action_target_name = "%s__%s" % (target_name, action_name)
 
         inputs = action["inputs"]
         inputs_name = action_target_name + "__input"
         SetVariableList(
             output,
             inputs_name,
             [NormjoinPathForceCMakeSource(path_to_gyp, dep) for dep in inputs],
@@ -272,15 +278,15 @@
             NormjoinPathForceCMakeSource(path_to_gyp, out) for out in outputs
         ]
         outputs_name = action_target_name + "__output"
         SetVariableList(output, outputs_name, cmake_outputs)
 
         # Build up a list of outputs.
         # Collect the output dirs we'll need.
-        dirs = {dir for dir in (os.path.dirname(o) for o in outputs) if dir}
+        dirs = set(dir for dir in (os.path.dirname(o) for o in outputs) if dir)
 
         if int(action.get("process_outputs_as_sources", False)):
             extra_sources.extend(zip(cmake_outputs, outputs))
 
         # add_custom_command
         output.write("add_custom_command(OUTPUT ")
         WriteVariable(output, outputs_name)
@@ -367,15 +373,15 @@
             SetVariable(output, "RULE_INPUT_DIRNAME", rule_source_dirname)
             SetVariable(output, "RULE_INPUT_NAME", rule_source_basename)
             SetVariable(output, "RULE_INPUT_ROOT", rule_source_root)
             SetVariable(output, "RULE_INPUT_EXT", rule_source_ext)
 
             # Build up a list of outputs.
             # Collect the output dirs we'll need.
-            dirs = {dir for dir in (os.path.dirname(o) for o in outputs) if dir}
+            dirs = set(dir for dir in (os.path.dirname(o) for o in outputs) if dir)
 
             # Create variables for the output, as 'local' variable will be unset.
             these_outputs = []
             for output_index, out in enumerate(outputs):
                 output_name = action_name + "_" + str(output_index)
                 SetVariable(
                     output,
@@ -468,15 +474,15 @@
     if not have_copies:
         output.write("add_custom_target(")
         output.write(copy_name)
         output.write(")\n")
         extra_deps.append(copy_name)
         return
 
-    class Copy:
+    class Copy(object):
         def __init__(self, ext, command):
             self.cmake_inputs = []
             self.cmake_outputs = []
             self.gyp_inputs = []
             self.gyp_outputs = []
             self.ext = ext
             self.inputs_name = None
@@ -577,15 +583,15 @@
     )
     cmake_target_full_name = gyp_file + ":" + gyp_target_name
     if gyp_target_toolset and gyp_target_toolset != "target":
         cmake_target_full_name += "_" + gyp_target_toolset
     return StringToCMakeTargetName(cmake_target_full_name)
 
 
-class CMakeNamer:
+class CMakeNamer(object):
     """Converts Gyp target names into CMake target names.
 
   CMake requires that target names be globally unique. One way to ensure
   this is to fully qualify the names of the targets. Unfortunately, this
   ends up with all targets looking like "chrome_chrome_gyp_chrome" instead
   of just "chrome". If this generator were only interested in building, it
   would be possible to fully qualify all target names, then create
@@ -925,15 +931,18 @@
                 "target",
                 target_name,
             )
 
         product_prefix = spec.get("product_prefix", default_product_prefix)
         product_name = spec.get("product_name", default_product_name)
         product_ext = spec.get("product_extension")
-        product_ext = "." + product_ext if product_ext else default_product_ext
+        if product_ext:
+            product_ext = "." + product_ext
+        else:
+            product_ext = default_product_ext
 
         SetTargetProperty(output, cmake_target_name, "PREFIX", product_prefix)
         SetTargetProperty(
             output,
             cmake_target_name,
             cmake_target_type.property_modifier + "_OUTPUT_NAME",
             product_name,
@@ -1034,15 +1043,15 @@
         # Linker flags
         ldflags = config.get("ldflags")
         if ldflags is not None:
             SetTargetProperty(output, cmake_target_name, "LINK_FLAGS", ldflags, " ")
 
         # XCode settings
         xcode_settings = config.get("xcode_settings", {})
-        for xcode_setting, xcode_value in xcode_settings.items():
+        for xcode_setting, xcode_value in xcode_settings.viewitems():
             SetTargetProperty(
                 output,
                 cmake_target_name,
                 "XCODE_ATTRIBUTE_%s" % xcode_setting,
                 xcode_value,
                 "" if isinstance(xcode_value, str) else " ",
             )
@@ -1272,19 +1281,19 @@
     for config_name in configurations:
         # build_dir: relative path from source root to our output files.
         # e.g. "out/Debug"
         build_dir = os.path.normpath(
             os.path.join(generator_dir, output_dir, config_name)
         )
         arguments = ["cmake", "-G", "Ninja"]
-        print(f"Generating [{config_name}]: {arguments}")
+        print("Generating [%s]: %s" % (config_name, arguments))
         subprocess.check_call(arguments, cwd=build_dir)
 
         arguments = ["ninja", "-C", build_dir]
-        print(f"Building [{config_name}]: {arguments}")
+        print("Building [%s]: %s" % (config_name, arguments))
         subprocess.check_call(arguments)
 
 
 def CallGenerateOutputForConfig(arglist):
     # Ignore the interrupt signal so that the parent process catches it and
     # kills all multiprocessing children.
     signal.signal(signal.SIGINT, signal.SIG_IGN)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/compile_commands_json.py` & `gyp-next-0.4.0/pylib/gyp/generator/compile_commands_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "SHARED_LIB_PREFIX": "lib",
     "STATIC_LIB_PREFIX": "lib",
     "STATIC_LIB_SUFFIX": ".a",
 }
 
 
 def IsMac(params):
-    return gyp.common.GetFlavor(params) == "mac"
+    return "mac" == gyp.common.GetFlavor(params)
 
 
 def CalculateVariables(default_variables, params):
     default_variables.setdefault("OS", gyp.common.GetFlavor(params))
 
 
 def AddCommandsForTarget(cwd, target, params, per_config_commands):
@@ -57,16 +57,16 @@
         cflags_c = cflags + cflags_c
         cflags_cc = cflags + cflags_cc
 
         defines = configuration.get("defines", [])
         defines = ["-D" + s for s in defines]
 
         # TODO(bnoordhuis) Handle generated source files.
-        extensions = (".c", ".cc", ".cpp", ".cxx")
-        sources = [s for s in target.get("sources", []) if s.endswith(extensions)]
+        sources = target.get("sources", [])
+        sources = [s for s in sources if s.endswith(".c") or s.endswith(".cc")]
 
         def resolve(filename):
             return os.path.abspath(os.path.join(cwd, filename))
 
         # TODO(bnoordhuis) Handle generated header files.
         include_dirs = configuration.get("include_dirs", [])
         include_dirs = [s for s in include_dirs if not s.startswith("$(obj)")]
@@ -89,15 +89,15 @@
                     defines,
                     includes,
                     cflags,
                     "-c",
                     gyp.common.EncodePOSIXShellArgument(file),
                 )
             )
-            commands.append({"command": command, "directory": output_dir, "file": file})
+            commands.append(dict(command=command, directory=output_dir, file=file))
 
 
 def GenerateOutput(target_list, target_dicts, data, params):
     per_config_commands = {}
     for qualified_target, target in target_dicts.items():
         build_file, target_name, toolset = gyp.common.ParseQualifiedTarget(
             qualified_target
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/dump_dependency_json.py` & `gyp-next-0.4.0/pylib/gyp/generator/dump_dependency_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
+from __future__ import print_function
 
 import os
 import gyp
 import gyp.common
 import gyp.msvs_emulation
 import json
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/eclipse.py` & `gyp-next-0.4.0/pylib/gyp/generator/eclipse.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 from xml.sax.saxutils import escape
 import os.path
 import subprocess
 import gyp
 import gyp.common
 import gyp.msvs_emulation
 import shlex
-import xml.etree.ElementTree as ET
+import xml.etree.cElementTree as ET
+
+PY3 = bytes != str
 
 generator_wants_static_library_dependencies_adjusted = False
 
 generator_default_variables = {}
 
 for dirname in ["INTERMEDIATE_DIR", "PRODUCT_DIR", "LIB_DIR", "SHARED_LIB_DIR"]:
     # Some gyp steps fail if these are empty(!), so we convert them to variables
@@ -99,15 +101,17 @@
         command.extend(["-E", "-xc++", "-v", "-"])
         proc = subprocess.Popen(
             args=command,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
-        output = proc.communicate()[1].decode("utf-8")
+        output = proc.communicate()[1]
+        if PY3:
+            output = output.decode("utf-8")
         # Extract the list of include dirs from the output, which has this format:
         #   ...
         #   #include "..." search starts here:
         #   #include <...> search starts here:
         #    /usr/include/c++/4.6
         #    /usr/local/include
         #   End of search list.
@@ -237,22 +241,27 @@
         return all_defines  # Default defines already processed in the loop above.
     if compiler_path:
         command = shlex.split(compiler_path)
         command.extend(["-E", "-dM", "-"])
         cpp_proc = subprocess.Popen(
             args=command, cwd=".", stdin=subprocess.PIPE, stdout=subprocess.PIPE
         )
-        cpp_output = cpp_proc.communicate()[0].decode("utf-8")
+        cpp_output = cpp_proc.communicate()[0]
+        if PY3:
+            cpp_output = cpp_output.decode("utf-8")
         cpp_lines = cpp_output.split("\n")
         for cpp_line in cpp_lines:
             if not cpp_line.strip():
                 continue
             cpp_line_parts = cpp_line.split(" ", 2)
             key = cpp_line_parts[1]
-            val = cpp_line_parts[2] if len(cpp_line_parts) >= 3 else "1"
+            if len(cpp_line_parts) >= 3:
+                val = cpp_line_parts[2]
+            else:
+                val = "1"
             all_defines[key] = val
 
     return all_defines
 
 
 def WriteIncludePaths(out, eclipse_langs, include_dirs):
     """Write the includes section of a CDT settings export file."""
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/gypd.py` & `gyp-next-0.4.0/pylib/gyp/generator/gypd.py`

 * *Files identical despite different names*

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/gypsh.py` & `gyp-next-0.4.0/pylib/gyp/generator/gypsh.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,14 @@
         "target_dicts": target_dicts,
         "data": data,
     }
 
     # Use a banner that looks like the stock Python one and like what
     # code.interact uses by default, but tack on something to indicate what
     # locals are available, and identify gypsh.
-    banner = "Python {} on {}\nlocals.keys() = {}\ngypsh".format(
+    banner = "Python %s on %s\nlocals.keys() = %s\ngypsh" % (
         sys.version,
         sys.platform,
         repr(sorted(locals.keys())),
     )
 
     code.interact(banner, local=locals)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/make.py` & `gyp-next-0.4.0/pylib/gyp/generator/make.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 #
 # TODOs:
 #
 # Global settings and utility functions are currently stuffed in the
 # toplevel Makefile.  It may make sense to generate some .mk files on
 # the side to keep the files readable.
 
+from __future__ import print_function
 
 import os
 import re
 import subprocess
 import gyp
 import gyp.common
 import gyp.xcode_emulation
 from gyp.common import GetEnvironFallback
+from gyp.common import GypError
 
 import hashlib
 
 generator_default_variables = {
     "EXECUTABLE_PREFIX": "",
     "EXECUTABLE_SUFFIX": "",
     "STATIC_LIB_PREFIX": "lib",
@@ -46,15 +48,15 @@
     "RULE_INPUT_PATH": "$(abspath $<)",
     "RULE_INPUT_EXT": "$(suffix $<)",
     "RULE_INPUT_NAME": "$(notdir $<)",
     "CONFIGURATION_NAME": "$(BUILDTYPE)",
 }
 
 # Make supports multiple toolsets
-generator_supports_multiple_toolsets = gyp.common.CrossCompileRequested()
+generator_supports_multiple_toolsets = True
 
 # Request sorted dependencies in the order from dependents to dependencies.
 generator_wants_sorted_dependencies = False
 
 # Placates pylint.
 generator_additional_non_configuration_keys = []
 generator_additional_path_sections = []
@@ -95,26 +97,23 @@
     else:
         operating_system = flavor
         if flavor == "android":
             operating_system = "linux"  # Keep this legacy behavior for now.
         default_variables.setdefault("OS", operating_system)
         if flavor == "aix":
             default_variables.setdefault("SHARED_LIB_SUFFIX", ".a")
-        elif flavor == "zos":
-            default_variables.setdefault("SHARED_LIB_SUFFIX", ".x")
-            COMPILABLE_EXTENSIONS.update({".pli": "pli"})
         else:
             default_variables.setdefault("SHARED_LIB_SUFFIX", ".so")
         default_variables.setdefault("SHARED_LIB_DIR", "$(builddir)/lib.$(TOOLSET)")
         default_variables.setdefault("LIB_DIR", "$(obj).$(TOOLSET)")
 
 
 def CalculateGeneratorInputInfo(params):
     """Calculate the generator specific info that gets fed to input (called by
-    gyp)."""
+  gyp)."""
     generator_flags = params.get("generator_flags", {})
     android_ndk_version = generator_flags.get("android_ndk_version", None)
     # Android NDK requires a strict link order.
     if android_ndk_version:
         global generator_wants_sorted_dependencies
         generator_wants_sorted_dependencies = True
 
@@ -153,39 +152,14 @@
 
 # Due to circular dependencies between libraries :(, we wrap the
 # special "figure out circular dependencies" flags around the entire
 # input list during linking.
 quiet_cmd_link = LINK($(TOOLSET)) $@
 cmd_link = $(LINK.$(TOOLSET)) -o $@ $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -Wl,--start-group $(LD_INPUTS) $(LIBS) -Wl,--end-group
 
-# Note: this does not handle spaces in paths
-define xargs
-  $(1) $(word 1,$(2))
-$(if $(word 2,$(2)),$(call xargs,$(1),$(wordlist 2,$(words $(2)),$(2))))
-endef
-
-define write-to-file
-  @: >$(1)
-$(call xargs,@printf "%s\\n" >>$(1),$(2))
-endef
-
-OBJ_FILE_LIST := ar-file-list
-
-define create_archive
-        rm -f $(1) $(1).$(OBJ_FILE_LIST); mkdir -p `dirname $(1)`
-        $(call write-to-file,$(1).$(OBJ_FILE_LIST),$(filter %.o,$(2)))
-        $(AR.$(TOOLSET)) crs $(1) @$(1).$(OBJ_FILE_LIST)
-endef
-
-define create_thin_archive
-        rm -f $(1) $(OBJ_FILE_LIST); mkdir -p `dirname $(1)`
-        $(call write-to-file,$(1).$(OBJ_FILE_LIST),$(filter %.o,$(2)))
-        $(AR.$(TOOLSET)) crsT $(1) @$(1).$(OBJ_FILE_LIST)
-endef
-
 # We support two kinds of shared objects (.so):
 # 1) shared_library, which is just bundling together many dependent libraries
 # into a link line.
 # 2) loadable_module, which is generating a module intended for dlopen().
 #
 # They differ only slightly:
 # In the former case, we want to package all dependent code into the .so.
@@ -199,62 +173,37 @@
 # - Set SONAME to the library filename so our binaries don't reference
 # the local, absolute paths used on the link command-line.
 quiet_cmd_solink = SOLINK($(TOOLSET)) $@
 cmd_solink = $(LINK.$(TOOLSET)) -o $@ -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -Wl,-soname=$(@F) -Wl,--whole-archive $(LD_INPUTS) -Wl,--no-whole-archive $(LIBS)
 
 quiet_cmd_solink_module = SOLINK_MODULE($(TOOLSET)) $@
 cmd_solink_module = $(LINK.$(TOOLSET)) -o $@ -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -Wl,-soname=$(@F) -Wl,--start-group $(filter-out FORCE_DO_CMD, $^) -Wl,--end-group $(LIBS)
-"""  # noqa: E501
+"""
 
 LINK_COMMANDS_MAC = """\
 quiet_cmd_alink = LIBTOOL-STATIC $@
 cmd_alink = rm -f $@ && ./gyp-mac-tool filter-libtool libtool $(GYP_LIBTOOLFLAGS) -static -o $@ $(filter %.o,$^)
 
 quiet_cmd_link = LINK($(TOOLSET)) $@
 cmd_link = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o "$@" $(LD_INPUTS) $(LIBS)
 
 quiet_cmd_solink = SOLINK($(TOOLSET)) $@
 cmd_solink = $(LINK.$(TOOLSET)) -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o "$@" $(LD_INPUTS) $(LIBS)
 
 quiet_cmd_solink_module = SOLINK_MODULE($(TOOLSET)) $@
 cmd_solink_module = $(LINK.$(TOOLSET)) -bundle $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(filter-out FORCE_DO_CMD, $^) $(LIBS)
-"""  # noqa: E501
+"""
 
 LINK_COMMANDS_ANDROID = """\
 quiet_cmd_alink = AR($(TOOLSET)) $@
 cmd_alink = rm -f $@ && $(AR.$(TOOLSET)) crs $@ $(filter %.o,$^)
 
 quiet_cmd_alink_thin = AR($(TOOLSET)) $@
 cmd_alink_thin = rm -f $@ && $(AR.$(TOOLSET)) crsT $@ $(filter %.o,$^)
 
-# Note: this does not handle spaces in paths
-define xargs
-  $(1) $(word 1,$(2))
-$(if $(word 2,$(2)),$(call xargs,$(1),$(wordlist 2,$(words $(2)),$(2))))
-endef
-
-define write-to-file
-  @: >$(1)
-$(call xargs,@printf "%s\\n" >>$(1),$(2))
-endef
-
-OBJ_FILE_LIST := ar-file-list
-
-define create_archive
-        rm -f $(1) $(1).$(OBJ_FILE_LIST); mkdir -p `dirname $(1)`
-        $(call write-to-file,$(1).$(OBJ_FILE_LIST),$(filter %.o,$(2)))
-        $(AR.$(TOOLSET)) crs $(1) @$(1).$(OBJ_FILE_LIST)
-endef
-
-define create_thin_archive
-        rm -f $(1) $(OBJ_FILE_LIST); mkdir -p `dirname $(1)`
-        $(call write-to-file,$(1).$(OBJ_FILE_LIST),$(filter %.o,$(2)))
-        $(AR.$(TOOLSET)) crsT $(1) @$(1).$(OBJ_FILE_LIST)
-endef
-
 # Due to circular dependencies between libraries :(, we wrap the
 # special "figure out circular dependencies" flags around the entire
 # input list during linking.
 quiet_cmd_link = LINK($(TOOLSET)) $@
 quiet_cmd_link_host = LINK($(TOOLSET)) $@
 cmd_link = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ -Wl,--start-group $(LD_INPUTS) -Wl,--end-group $(LIBS)
 cmd_link_host = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ -Wl,--start-group $(LD_INPUTS) -Wl,--end-group $(LIBS)
@@ -265,15 +214,15 @@
 quiet_cmd_solink = SOLINK($(TOOLSET)) $@
 cmd_solink = $(LINK.$(TOOLSET)) -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -Wl,-soname=$(@F) -o $@ -Wl,--whole-archive $(LD_INPUTS) -Wl,--no-whole-archive $(LIBS)
 
 quiet_cmd_solink_module = SOLINK_MODULE($(TOOLSET)) $@
 cmd_solink_module = $(LINK.$(TOOLSET)) -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -Wl,-soname=$(@F) -o $@ -Wl,--start-group $(filter-out FORCE_DO_CMD, $^) -Wl,--end-group $(LIBS)
 quiet_cmd_solink_module_host = SOLINK_MODULE($(TOOLSET)) $@
 cmd_solink_module_host = $(LINK.$(TOOLSET)) -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -Wl,-soname=$(@F) -o $@ $(filter-out FORCE_DO_CMD, $^) $(LIBS)
-"""  # noqa: E501
+"""
 
 
 LINK_COMMANDS_AIX = """\
 quiet_cmd_alink = AR($(TOOLSET)) $@
 cmd_alink = rm -f $@ && $(AR.$(TOOLSET)) -X32_64 crs $@ $(filter %.o,$^)
 
 quiet_cmd_alink_thin = AR($(TOOLSET)) $@
@@ -283,51 +232,34 @@
 cmd_link = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(LD_INPUTS) $(LIBS)
 
 quiet_cmd_solink = SOLINK($(TOOLSET)) $@
 cmd_solink = $(LINK.$(TOOLSET)) -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(LD_INPUTS) $(LIBS)
 
 quiet_cmd_solink_module = SOLINK_MODULE($(TOOLSET)) $@
 cmd_solink_module = $(LINK.$(TOOLSET)) -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(filter-out FORCE_DO_CMD, $^) $(LIBS)
-"""  # noqa: E501
-
-
-LINK_COMMANDS_OS400 = """\
-quiet_cmd_alink = AR($(TOOLSET)) $@
-cmd_alink = rm -f $@ && $(AR.$(TOOLSET)) -X64 crs $@ $(filter %.o,$^)
-
-quiet_cmd_alink_thin = AR($(TOOLSET)) $@
-cmd_alink_thin = rm -f $@ && $(AR.$(TOOLSET)) -X64 crs $@ $(filter %.o,$^)
-
-quiet_cmd_link = LINK($(TOOLSET)) $@
-cmd_link = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(LD_INPUTS) $(LIBS)
-
-quiet_cmd_solink = SOLINK($(TOOLSET)) $@
-cmd_solink = $(LINK.$(TOOLSET)) -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(LD_INPUTS) $(LIBS)
-
-quiet_cmd_solink_module = SOLINK_MODULE($(TOOLSET)) $@
-cmd_solink_module = $(LINK.$(TOOLSET)) -shared $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(filter-out FORCE_DO_CMD, $^) $(LIBS)
-"""  # noqa: E501
+"""
 
 
 LINK_COMMANDS_OS390 = """\
 quiet_cmd_alink = AR($(TOOLSET)) $@
 cmd_alink = rm -f $@ && $(AR.$(TOOLSET)) crs $@ $(filter %.o,$^)
 
 quiet_cmd_alink_thin = AR($(TOOLSET)) $@
 cmd_alink_thin = rm -f $@ && $(AR.$(TOOLSET)) crsT $@ $(filter %.o,$^)
 
 quiet_cmd_link = LINK($(TOOLSET)) $@
 cmd_link = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(LD_INPUTS) $(LIBS)
 
 quiet_cmd_solink = SOLINK($(TOOLSET)) $@
-cmd_solink = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(LD_INPUTS) $(LIBS)
+cmd_solink = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(LD_INPUTS) $(LIBS) -Wl,DLL
 
 quiet_cmd_solink_module = SOLINK_MODULE($(TOOLSET)) $@
-cmd_solink_module = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(filter-out FORCE_DO_CMD, $^) $(LIBS)
-"""  # noqa: E501
+cmd_solink_module = $(LINK.$(TOOLSET)) $(GYP_LDFLAGS) $(LDFLAGS.$(TOOLSET)) -o $@ $(filter-out FORCE_DO_CMD, $^) $(LIBS) -Wl,DLL
+
+"""
 
 
 # Header of toplevel Makefile.
 # This should go into the build tree, but it's easier to keep it here for now.
 SHARED_HEADER = (
     """\
 # We borrow heavily from the kernel build setup, though we are simpler since
@@ -375,29 +307,27 @@
 CC.target ?= %(CC.target)s
 CFLAGS.target ?= $(CPPFLAGS) $(CFLAGS)
 CXX.target ?= %(CXX.target)s
 CXXFLAGS.target ?= $(CPPFLAGS) $(CXXFLAGS)
 LINK.target ?= %(LINK.target)s
 LDFLAGS.target ?= $(LDFLAGS)
 AR.target ?= $(AR)
-PLI.target ?= %(PLI.target)s
 
 # C++ apps need to be linked with g++.
 LINK ?= $(CXX.target)
 
 # TODO(evan): move all cross-compilation logic to gyp-time so we don't need
 # to replicate this environment fallback in make as well.
 CC.host ?= %(CC.host)s
 CFLAGS.host ?= $(CPPFLAGS_host) $(CFLAGS_host)
 CXX.host ?= %(CXX.host)s
 CXXFLAGS.host ?= $(CPPFLAGS_host) $(CXXFLAGS_host)
 LINK.host ?= %(LINK.host)s
-LDFLAGS.host ?= $(LDFLAGS_host)
+LDFLAGS.host ?=
 AR.host ?= %(AR.host)s
-PLI.host ?= %(PLI.host)s
 
 # Define a dir function that can handle spaces.
 # http://www.gnu.org/software/make/manual/make.html#Syntax-of-Functions
 # "leading spaces cannot appear in the text of the first argument as written.
 # These characters can be put into the argument value by variable substitution."
 empty :=
 space := $(empty) $(empty)
@@ -469,19 +399,16 @@
 quiet_cmd_touch = TOUCH $@
 cmd_touch = touch $@
 
 quiet_cmd_copy = COPY $@
 # send stderr to /dev/null to ignore messages when linking directories.
 cmd_copy = ln -f "$<" "$@" 2>/dev/null || (rm -rf "$@" && cp %(copy_archive_args)s "$<" "$@")
 
-quiet_cmd_symlink = SYMLINK $@
-cmd_symlink = ln -sf "$<" "$@"
-
 %(link_commands)s
-"""  # noqa: E501
+"""
     r"""
 # Define an escape_quotes function to escape single quotes.
 # This allows us to handle quotes properly as long as we always use
 # use single quotes and escape_quotes.
 escape_quotes = $(subst ','\'',$(1))
 # This comment is here just to include a ' to unconfuse syntax highlighting.
 # Define an escape_vars function to escape '$' variable syntax.
@@ -572,15 +499,15 @@
 %%.d: ;
 
 # Use FORCE_DO_CMD to force a target to run.  Should be coupled with
 # do_cmd.
 .PHONY: FORCE_DO_CMD
 FORCE_DO_CMD:
 
-"""  # noqa: E501
+"""
 )
 
 SHARED_HEADER_MAC_COMMANDS = """
 quiet_cmd_objc = CXX($(TOOLSET)) $@
 cmd_objc = $(CC.$(TOOLSET)) $(GYP_OBJCFLAGS) $(DEPFLAGS) -c -o $@ $<
 
 quiet_cmd_objcxx = CXX($(TOOLSET)) $@
@@ -603,15 +530,15 @@
 cmd_mac_tool = ./gyp-mac-tool $(4) $< "$@"
 
 quiet_cmd_mac_package_framework = PACKAGE FRAMEWORK $@
 cmd_mac_package_framework = ./gyp-mac-tool package-framework "$@" $(4)
 
 quiet_cmd_infoplist = INFOPLIST $@
 cmd_infoplist = $(CC.$(TOOLSET)) -E -P -Wno-trigraphs -x c $(INFOPLIST_DEFINES) "$<" -o "$@"
-"""  # noqa: E501
+"""
 
 
 def WriteRootHeaderSuffixRules(writer):
     extensions = sorted(COMPILABLE_EXTENSIONS.keys(), key=str.lower)
 
     writer.write("# Suffix rules, putting all outputs into $(obj).\n")
     for ext in extensions:
@@ -627,23 +554,14 @@
     writer.write("\n")
     for ext in extensions:
         writer.write("$(obj).$(TOOLSET)/%%.o: $(obj)/%%%s FORCE_DO_CMD\n" % ext)
         writer.write("\t@$(call do_cmd,%s,1)\n" % COMPILABLE_EXTENSIONS[ext])
     writer.write("\n")
 
 
-SHARED_HEADER_OS390_COMMANDS = """
-PLIFLAGS.target ?= -qlp=64 -qlimits=extname=31  $(PLIFLAGS)
-PLIFLAGS.host ?= -qlp=64 -qlimits=extname=31 $(PLIFLAGS)
-
-quiet_cmd_pli = PLI($(TOOLSET)) $@
-cmd_pli = $(PLI.$(TOOLSET)) $(GYP_PLIFLAGS) $(PLIFLAGS.$(TOOLSET)) -c $< && \
-          if [ -f $(notdir $@) ]; then /bin/cp $(notdir $@) $@; else true; fi
-"""
-
 SHARED_HEADER_SUFFIX_RULES_COMMENT1 = """\
 # Suffix rules, putting all outputs into $(obj).
 """
 
 
 SHARED_HEADER_SUFFIX_RULES_COMMENT2 = """\
 # Try building from generated source, too.
@@ -677,53 +595,56 @@
     ".s": "cc",
     ".S": "cc",
 }
 
 
 def Compilable(filename):
     """Return true if the file is compilable (should be in OBJS)."""
-    return any(res for res in (filename.endswith(e) for e in COMPILABLE_EXTENSIONS))
+    for res in (filename.endswith(e) for e in COMPILABLE_EXTENSIONS):
+        if res:
+            return True
+    return False
 
 
 def Linkable(filename):
     """Return true if the file is linkable (should be on the link line)."""
     return filename.endswith(".o")
 
 
 def Target(filename):
     """Translate a compilable filename to its .o target."""
     return os.path.splitext(filename)[0] + ".o"
 
 
 def EscapeShellArgument(s):
     """Quotes an argument so that it will be interpreted literally by a POSIX
-    shell. Taken from
-    http://stackoverflow.com/questions/35817/whats-the-best-way-to-escape-ossystem-calls-in-python
-    """
+     shell. Taken from
+     http://stackoverflow.com/questions/35817/whats-the-best-way-to-escape-ossystem-calls-in-python
+     """
     return "'" + s.replace("'", "'\\''") + "'"
 
 
 def EscapeMakeVariableExpansion(s):
     """Make has its own variable expansion syntax using $. We must escape it for
-    string to be interpreted literally."""
+     string to be interpreted literally."""
     return s.replace("$", "$$")
 
 
 def EscapeCppDefine(s):
     """Escapes a CPP define so that it will reach the compiler unaltered."""
     s = EscapeShellArgument(s)
     s = EscapeMakeVariableExpansion(s)
     # '#' characters must be escaped even embedded in a string, else Make will
     # treat it as the start of a comment.
     return s.replace("#", r"\#")
 
 
 def QuoteIfNecessary(string):
     """TODO: Should this ideally be replaced with one or more of the above
-    functions?"""
+     functions?"""
     if '"' in string:
         string = '"' + string.replace('"', '\\"') + '"'
     return string
 
 
 def StringToMakefileVariable(string):
     """Convert a string to a value that is acceptable as a make variable name."""
@@ -747,39 +668,76 @@
 
 
 def SourceifyAndQuoteSpaces(path):
     """Convert a path to its source directory form and quote spaces."""
     return QuoteSpaces(Sourceify(path))
 
 
+# TODO: Avoid code duplication with _ValidateSourcesForMSVSProject in msvs.py.
+def _ValidateSourcesForOSX(spec, all_sources):
+    """Makes sure if duplicate basenames are not specified in the source list.
+
+  Arguments:
+    spec: The target dictionary containing the properties of the target.
+  """
+    if spec.get("type", None) != "static_library":
+        return
+
+    basenames = {}
+    for source in all_sources:
+        name, ext = os.path.splitext(source)
+        is_compiled_file = ext in [".c", ".cc", ".cpp", ".cxx", ".m", ".mm", ".s", ".S"]
+        if not is_compiled_file:
+            continue
+        basename = os.path.basename(name)  # Don't include extension.
+        basenames.setdefault(basename, []).append(source)
+
+    error = ""
+    for basename, files in basenames.items():
+        if len(files) > 1:
+            error += "  %s: %s\n" % (basename, " ".join(files))
+
+    if error:
+        print(
+            (
+                "static library %s has several files with the same basename:\n"
+                % spec["target_name"]
+            )
+            + error
+            + "libtool on OS X will generate"
+            + " warnings for them."
+        )
+        raise GypError("Duplicate basenames in sources section, see list above")
+
+
 # Map from qualified target to path to output.
 target_outputs = {}
 # Map from qualified target to any linkable output.  A subset
 # of target_outputs.  E.g. when mybinary depends on liba, we want to
 # include liba in the linker line; when otherbinary depends on
 # mybinary, we just want to build mybinary first.
 target_link_deps = {}
 
 
-class MakefileWriter:
+class MakefileWriter(object):
     """MakefileWriter packages up the writing of one target-specific foobar.mk.
 
-    Its only real entry point is Write(), and is mostly used for namespacing.
-    """
+  Its only real entry point is Write(), and is mostly used for namespacing.
+  """
 
     def __init__(self, generator_flags, flavor):
         self.generator_flags = generator_flags
         self.flavor = flavor
 
         self.suffix_rules_srcdir = {}
         self.suffix_rules_objdir1 = {}
         self.suffix_rules_objdir2 = {}
 
         # Generate suffix rules for all compilable extensions.
-        for ext in COMPILABLE_EXTENSIONS:
+        for ext in COMPILABLE_EXTENSIONS.keys():
             # Suffix rules for source folder.
             self.suffix_rules_srcdir.update(
                 {
                     ext: (
                         """\
 $(obj).$(TOOLSET)/$(TARGET)/%%.o: $(srcdir)/%%%s FORCE_DO_CMD
 \t@$(call do_cmd,%s,1)
@@ -814,22 +772,22 @@
             )
 
     def Write(
         self, qualified_target, base_path, output_filename, spec, configs, part_of_all
     ):
         """The main entry point: writes a .mk file for a single target.
 
-        Arguments:
-          qualified_target: target we're generating
-          base_path: path relative to source root we're building in, used to resolve
-                     target-relative paths
-          output_filename: output .mk file name to write
-          spec, configs: gyp info
-          part_of_all: flag indicating this target is part of 'all'
-        """
+    Arguments:
+      qualified_target: target we're generating
+      base_path: path relative to source root we're building in, used to resolve
+                 target-relative paths
+      output_filename: output .mk file name to write
+      spec, configs: gyp info
+      part_of_all: flag indicating this target is part of 'all'
+    """
         gyp.common.EnsureDirExists(output_filename)
 
         self.fp = open(output_filename, "w")
 
         self.fp.write(header)
 
         self.qualified_target = qualified_target
@@ -905,14 +863,18 @@
             )
             self.WriteMacBundleResources(all_mac_bundle_resources, mac_bundle_deps)
             self.WriteMacInfoPlist(mac_bundle_deps)
 
         # Sources.
         all_sources = spec.get("sources", []) + extra_sources
         if all_sources:
+            if self.flavor == "mac":
+                # libtool on OS X generates warnings for duplicate basenames in the same
+                # target.
+                _ValidateSourcesForOSX(spec, all_sources)
             self.WriteSources(
                 configs,
                 deps,
                 all_sources,
                 extra_outputs,
                 extra_link_deps,
                 part_of_all,
@@ -921,15 +883,15 @@
                     lambda p: Sourceify(self.Absolutify(p)),
                     self.Pchify,
                 ),
             )
             sources = [x for x in all_sources if Compilable(x)]
             if sources:
                 self.WriteLn(SHARED_HEADER_SUFFIX_RULES_COMMENT1)
-                extensions = {os.path.splitext(s)[1] for s in sources}
+                extensions = set([os.path.splitext(s)[1] for s in sources])
                 for ext in extensions:
                     if ext in self.suffix_rules_srcdir:
                         self.WriteLn(self.suffix_rules_srcdir[ext])
                 self.WriteLn(SHARED_HEADER_SUFFIX_RULES_COMMENT2)
                 for ext in extensions:
                     if ext in self.suffix_rules_objdir1:
                         self.WriteLn(self.suffix_rules_objdir1[ext])
@@ -965,60 +927,60 @@
             self.WriteAndroidNdkModuleRule(self.target, all_sources, link_deps)
 
         self.fp.close()
 
     def WriteSubMake(self, output_filename, makefile_path, targets, build_dir):
         """Write a "sub-project" Makefile.
 
-        This is a small, wrapper Makefile that calls the top-level Makefile to build
-        the targets from a single gyp file (i.e. a sub-project).
+    This is a small, wrapper Makefile that calls the top-level Makefile to build
+    the targets from a single gyp file (i.e. a sub-project).
 
-        Arguments:
-          output_filename: sub-project Makefile name to write
-          makefile_path: path to the top-level Makefile
-          targets: list of "all" targets for this sub-project
-          build_dir: build output directory, relative to the sub-project
-        """
+    Arguments:
+      output_filename: sub-project Makefile name to write
+      makefile_path: path to the top-level Makefile
+      targets: list of "all" targets for this sub-project
+      build_dir: build output directory, relative to the sub-project
+    """
         gyp.common.EnsureDirExists(output_filename)
         self.fp = open(output_filename, "w")
         self.fp.write(header)
         # For consistency with other builders, put sub-project build output in the
         # sub-project dir (see test/subdirectory/gyptest-subdir-all.py).
         self.WriteLn(
             "export builddir_name ?= %s"
             % os.path.join(os.path.dirname(output_filename), build_dir)
         )
         self.WriteLn(".PHONY: all")
         self.WriteLn("all:")
         if makefile_path:
             makefile_path = " -C " + makefile_path
-        self.WriteLn("\t$(MAKE){} {}".format(makefile_path, " ".join(targets)))
+        self.WriteLn("\t$(MAKE)%s %s" % (makefile_path, " ".join(targets)))
         self.fp.close()
 
     def WriteActions(
         self,
         actions,
         extra_sources,
         extra_outputs,
         extra_mac_bundle_resources,
         part_of_all,
     ):
         """Write Makefile code for any 'actions' from the gyp input.
 
-        extra_sources: a list that will be filled in with newly generated source
-                       files, if any
-        extra_outputs: a list that will be filled in with any outputs of these
-                       actions (used to make other pieces dependent on these
-                       actions)
-        part_of_all: flag indicating this target is part of 'all'
-        """
+    extra_sources: a list that will be filled in with newly generated source
+                   files, if any
+    extra_outputs: a list that will be filled in with any outputs of these
+                   actions (used to make other pieces dependent on these
+                   actions)
+    part_of_all: flag indicating this target is part of 'all'
+    """
         env = self.GetSortedXcodeEnv()
         for action in actions:
             name = StringToMakefileVariable(
-                "{}_{}".format(self.qualified_target, action["action_name"])
+                "%s_%s" % (self.qualified_target, action["action_name"])
             )
             self.WriteLn('### Rules for action "%s":' % action["action_name"])
             inputs = action["inputs"]
             outputs = action["outputs"]
 
             # Build up a list of outputs.
             # Collect the output dirs we'll need.
@@ -1037,19 +999,17 @@
             if self.flavor == "mac":
                 action_commands = [
                     gyp.xcode_emulation.ExpandEnvVars(command, env)
                     for command in action_commands
                 ]
             command = gyp.common.EncodePOSIXShellList(action_commands)
             if "message" in action:
-                self.WriteLn(
-                    "quiet_cmd_{} = ACTION {} $@".format(name, action["message"])
-                )
+                self.WriteLn("quiet_cmd_%s = ACTION %s $@" % (name, action["message"]))
             else:
-                self.WriteLn(f"quiet_cmd_{name} = ACTION {name} $@")
+                self.WriteLn("quiet_cmd_%s = ACTION %s $@" % (name, name))
             if len(dirs) > 0:
                 command = "mkdir -p %s" % " ".join(dirs) + "; " + command
 
             cd_action = "cd %s; " % Sourceify(self.path or ".")
 
             # command and cd_action get written to a toplevel variable called
             # cmd_foo. Toplevel variables can't handle things that change per
@@ -1059,28 +1019,20 @@
 
             # Set LD_LIBRARY_PATH in case the action runs an executable from this
             # build which links to shared libs from this build.
             # actions run on the host, so they should in theory only use host
             # libraries, but until everything is made cross-compile safe, also use
             # target libraries.
             # TODO(piman): when everything is cross-compile safe, remove lib.target
-            if self.flavor == "zos" or self.flavor == "aix":
-                self.WriteLn(
-                    "cmd_%s = LIBPATH=$(builddir)/lib.host:"
-                    "$(builddir)/lib.target:$$LIBPATH; "
-                    "export LIBPATH; "
-                    "%s%s" % (name, cd_action, command)
-                )
-            else:
-                self.WriteLn(
-                    "cmd_%s = LD_LIBRARY_PATH=$(builddir)/lib.host:"
-                    "$(builddir)/lib.target:$$LD_LIBRARY_PATH; "
-                    "export LD_LIBRARY_PATH; "
-                    "%s%s" % (name, cd_action, command)
-                )
+            self.WriteLn(
+                "cmd_%s = LD_LIBRARY_PATH=$(builddir)/lib.host:"
+                "$(builddir)/lib.target:$$LD_LIBRARY_PATH; "
+                "export LD_LIBRARY_PATH; "
+                "%s%s" % (name, cd_action, command)
+            )
             self.WriteLn()
             outputs = [self.Absolutify(o) for o in outputs]
             # The makefile rules are all relative to the top dir, but the gyp actions
             # are defined relative to their containing dir.  This replaces the obj
             # variable for the action rule with an absolute version so that the output
             # goes in the right place.
             # Only write the 'obj' and 'builddir' rules for the "primary" output (:1);
@@ -1109,15 +1061,15 @@
                 [Sourceify(self.Absolutify(i)) for i in inputs],
                 part_of_all=part_of_all,
                 command=name,
             )
 
             # Stuff the outputs in a variable so we can refer to them later.
             outputs_variable = "action_%s_outputs" % name
-            self.WriteLn("{} := {}".format(outputs_variable, " ".join(outputs)))
+            self.WriteLn("%s := %s" % (outputs_variable, " ".join(outputs)))
             extra_outputs.append("$(%s)" % outputs_variable)
             self.WriteLn()
 
         self.WriteLn()
 
     def WriteRules(
         self,
@@ -1125,24 +1077,24 @@
         extra_sources,
         extra_outputs,
         extra_mac_bundle_resources,
         part_of_all,
     ):
         """Write Makefile code for any 'rules' from the gyp input.
 
-        extra_sources: a list that will be filled in with newly generated source
-                       files, if any
-        extra_outputs: a list that will be filled in with any outputs of these
-                       rules (used to make other pieces dependent on these rules)
-        part_of_all: flag indicating this target is part of 'all'
-        """
+    extra_sources: a list that will be filled in with newly generated source
+                   files, if any
+    extra_outputs: a list that will be filled in with any outputs of these
+                   rules (used to make other pieces dependent on these rules)
+    part_of_all: flag indicating this target is part of 'all'
+    """
         env = self.GetSortedXcodeEnv()
         for rule in rules:
             name = StringToMakefileVariable(
-                "{}_{}".format(self.qualified_target, rule["rule_name"])
+                "%s_%s" % (self.qualified_target, rule["rule_name"])
             )
             count = 0
             self.WriteLn("### Generated for rule %s:" % name)
 
             all_outputs = []
 
             for rule_source in rule.get("rule_sources", []):
@@ -1262,18 +1214,18 @@
             self.WriteLn()
         self.WriteLn("### Finished generating for all rules")
         self.WriteLn("")
 
     def WriteCopies(self, copies, extra_outputs, part_of_all):
         """Write Makefile code for any 'copies' from the gyp input.
 
-        extra_outputs: a list that will be filled in with any outputs of this action
-                       (used to make other pieces dependent on this action)
-        part_of_all: flag indicating this target is part of 'all'
-        """
+    extra_outputs: a list that will be filled in with any outputs of this action
+                   (used to make other pieces dependent on this action)
+    part_of_all: flag indicating this target is part of 'all'
+    """
         self.WriteLn("### Generated for copy rule.")
 
         variable = StringToMakefileVariable(self.qualified_target + "_copies")
         outputs = []
         for copy in copies:
             for path in copy["files"]:
                 # Absolutify() may call normpath, and will strip trailing slashes.
@@ -1293,17 +1245,15 @@
                 # can't run scripts, there's no need to write the env then.
                 # WriteDoCmd() will escape spaces for .d files.
                 env = self.GetSortedXcodeEnv()
                 output = gyp.xcode_emulation.ExpandEnvVars(output, env)
                 path = gyp.xcode_emulation.ExpandEnvVars(path, env)
                 self.WriteDoCmd([output], [path], "copy", part_of_all)
                 outputs.append(output)
-        self.WriteLn(
-            "{} = {}".format(variable, " ".join(QuoteSpaces(o) for o in outputs))
-        )
+        self.WriteLn("%s = %s" % (variable, " ".join(QuoteSpaces(o) for o in outputs)))
         extra_outputs.append("$(%s)" % variable)
         self.WriteLn()
 
     def WriteMacBundleResources(self, resources, bundle_deps):
         """Writes Makefile code for 'mac_bundle_resources'."""
         self.WriteLn("### Generated for mac_bundle_resources")
 
@@ -1367,38 +1317,36 @@
         sources,
         extra_outputs,
         extra_link_deps,
         part_of_all,
         precompiled_header,
     ):
         """Write Makefile code for any 'sources' from the gyp input.
-        These are source files necessary to build the current target.
+    These are source files necessary to build the current target.
 
-        configs, deps, sources: input from gyp.
-        extra_outputs: a list of extra outputs this action should be dependent on;
-                       used to serialize action/rules before compilation
-        extra_link_deps: a list that will be filled in with any outputs of
-                         compilation (to be used in link lines)
-        part_of_all: flag indicating this target is part of 'all'
-        """
+    configs, deps, sources: input from gyp.
+    extra_outputs: a list of extra outputs this action should be dependent on;
+                   used to serialize action/rules before compilation
+    extra_link_deps: a list that will be filled in with any outputs of
+                     compilation (to be used in link lines)
+    part_of_all: flag indicating this target is part of 'all'
+    """
 
         # Write configuration-specific variables for CFLAGS, etc.
         for configname in sorted(configs.keys()):
             config = configs[configname]
             self.WriteList(
                 config.get("defines"),
                 "DEFS_%s" % configname,
                 prefix="-D",
                 quoter=EscapeCppDefine,
             )
 
             if self.flavor == "mac":
-                cflags = self.xcode_settings.GetCflags(
-                    configname, arch=config.get("xcode_configuration_platform")
-                )
+                cflags = self.xcode_settings.GetCflags(configname, arch=config.get('xcode_configuration_platform'))
                 cflags_c = self.xcode_settings.GetCflagsC(configname)
                 cflags_cc = self.xcode_settings.GetCflagsCC(configname)
                 cflags_objc = self.xcode_settings.GetCflagsObjC(configname)
                 cflags_objcc = self.xcode_settings.GetCflagsObjCC(configname)
             else:
                 cflags = config.get("cflags")
                 cflags_c = config.get("cflags_c")
@@ -1452,15 +1400,15 @@
                 order_only=True,
             )
 
         pchdeps = precompiled_header.GetObjDependencies(compilable, objs)
         if pchdeps:
             self.WriteLn("# Dependencies from obj files to their precompiled headers")
             for source, obj, gch in pchdeps:
-                self.WriteLn(f"{obj}: {gch}")
+                self.WriteLn("%s: %s" % (obj, gch))
             self.WriteLn("# End precompiled header dependencies")
 
         if objs:
             extra_link_deps.append("$(OBJS)")
             self.WriteLn(
                 """\
 # CFLAGS et al overrides must be target-local.
@@ -1524,32 +1472,32 @@
             var_name = {
                 "c": "GYP_PCH_CFLAGS",
                 "cc": "GYP_PCH_CXXFLAGS",
                 "m": "GYP_PCH_OBJCFLAGS",
                 "mm": "GYP_PCH_OBJCXXFLAGS",
             }[lang]
             self.WriteLn(
-                f"{gch}: {var_name} := {lang_flag} " + "$(DEFS_$(BUILDTYPE)) "
+                "%s: %s := %s " % (gch, var_name, lang_flag) + "$(DEFS_$(BUILDTYPE)) "
                 "$(INCS_$(BUILDTYPE)) "
                 "$(CFLAGS_$(BUILDTYPE)) " + extra_flags
             )
 
-            self.WriteLn(f"{gch}: {input} FORCE_DO_CMD")
+            self.WriteLn("%s: %s FORCE_DO_CMD" % (gch, input))
             self.WriteLn("\t@$(call do_cmd,pch_%s,1)" % lang)
             self.WriteLn("")
             assert " " not in gch, "Spaces in gch filenames not supported (%s)" % gch
             self.WriteLn("all_deps += %s" % gch)
             self.WriteLn("")
 
     def ComputeOutputBasename(self, spec):
         """Return the 'output basename' of a gyp spec.
 
-        E.g., the loadable module 'foobar' in directory 'baz' will produce
-          'libfoobar.so'
-        """
+    E.g., the loadable module 'foobar' in directory 'baz' will produce
+      'libfoobar.so'
+    """
         assert not self.is_mac_bundle
 
         if self.flavor == "mac" and self.type in (
             "static_library",
             "executable",
             "shared_library",
             "loadable_module",
@@ -1566,16 +1514,14 @@
             target_ext = ".a"
         elif self.type in ("loadable_module", "shared_library"):
             if target[:3] == "lib":
                 target = target[3:]
             target_prefix = "lib"
             if self.flavor == "aix":
                 target_ext = ".a"
-            elif self.flavor == "zos":
-                target_ext = ".x"
             else:
                 target_ext = ".so"
         elif self.type == "none":
             target = "%s.stamp" % target
         elif self.type != "executable":
             print(
                 "ERROR: What output file should be generated?",
@@ -1600,17 +1546,17 @@
             and self.type
             in ("static_library", "executable", "shared_library", "loadable_module")
         )
 
     def ComputeOutput(self, spec):
         """Return the 'output' (full output path) of a gyp spec.
 
-        E.g., the loadable module 'foobar' in directory 'baz' will produce
-          '$(obj)/baz/libfoobar.so'
-        """
+    E.g., the loadable module 'foobar' in directory 'baz' will produce
+      '$(obj)/baz/libfoobar.so'
+    """
         assert not self.is_mac_bundle
 
         path = os.path.join("$(obj)." + self.toolset, self.path)
         if self.type == "executable" or self._InstallImmediately():
             path = "$(builddir)"
         path = spec.get("product_dir", path)
         return os.path.join(path, self.ComputeOutputBasename(spec))
@@ -1625,18 +1571,18 @@
         """Return the 'output' (full output path) to the binary in a bundle."""
         path = generator_default_variables["PRODUCT_DIR"]
         return os.path.join(path, self.xcode_settings.GetExecutablePath())
 
     def ComputeDeps(self, spec):
         """Compute the dependencies of a gyp spec.
 
-        Returns a tuple (deps, link_deps), where each is a list of
-        filenames that will need to be put in front of make for either
-        building (deps) or linking (link_deps).
-        """
+    Returns a tuple (deps, link_deps), where each is a list of
+    filenames that will need to be put in front of make for either
+    building (deps) or linking (link_deps).
+    """
         deps = []
         link_deps = []
         if "dependencies" in spec:
             deps.extend(
                 [
                     target_outputs[dep]
                     for dep in spec["dependencies"]
@@ -1648,40 +1594,32 @@
                     link_deps.append(target_link_deps[dep])
             deps.extend(link_deps)
             # TODO: It seems we need to transitively link in libraries (e.g. -lfoo)?
             # This hack makes it work:
             # link_deps.extend(spec.get('libraries', []))
         return (gyp.common.uniquer(deps), gyp.common.uniquer(link_deps))
 
-    def GetSharedObjectFromSidedeck(self, sidedeck):
-        """Return the shared object files based on sidedeck"""
-        return re.sub(r"\.x$", ".so", sidedeck)
-
-    def GetUnversionedSidedeckFromSidedeck(self, sidedeck):
-        """Return the shared object files based on sidedeck"""
-        return re.sub(r"\.\d+\.x$", ".x", sidedeck)
-
     def WriteDependencyOnExtraOutputs(self, target, extra_outputs):
         self.WriteMakeRule(
             [self.output_binary],
             extra_outputs,
             comment="Build our special outputs first.",
             order_only=True,
         )
 
     def WriteTarget(
         self, spec, configs, deps, link_deps, bundle_deps, extra_outputs, part_of_all
     ):
         """Write Makefile code to produce the final target of the gyp spec.
 
-        spec, configs: input from gyp.
-        deps, link_deps: dependency lists; see ComputeDeps()
-        extra_outputs: any extra outputs that our target should depend on
-        part_of_all: flag indicating this target is part of 'all'
-        """
+    spec, configs: input from gyp.
+    deps, link_deps: dependency lists; see ComputeDeps()
+    extra_outputs: any extra outputs that our target should depend on
+    part_of_all: flag indicating this target is part of 'all'
+    """
 
         self.WriteLn("### Rules for final target.")
 
         if extra_outputs:
             self.WriteDependencyOnExtraOutputs(self.output_binary, extra_outputs)
             self.WriteMakeRule(
                 extra_outputs,
@@ -1695,15 +1633,15 @@
             for configname in sorted(configs.keys()):
                 config = configs[configname]
                 if self.flavor == "mac":
                     ldflags = self.xcode_settings.GetLdflags(
                         configname,
                         generator_default_variables["PRODUCT_DIR"],
                         lambda p: Sourceify(self.Absolutify(p)),
-                        arch=config.get("xcode_configuration_platform"),
+                        arch=config.get('xcode_configuration_platform')
                     )
 
                     # TARGET_POSTBUILDS_$(BUILDTYPE) is added to postbuilds later on.
                     gyp_to_build = gyp.common.InvertRelativePath(self.path)
                     target_postbuild = self.xcode_settings.AddImplicitPostbuilds(
                         configname,
                         QuoteSpaces(
@@ -1717,18 +1655,20 @@
                     )
                     if target_postbuild:
                         target_postbuilds[configname] = target_postbuild
                 else:
                     ldflags = config.get("ldflags", [])
                     # Compute an rpath for this output if needed.
                     if any(dep.endswith(".so") or ".so." in dep for dep in deps):
-                        # We want to get the literal string "$ORIGIN"
-                        # into the link command, so we need lots of escaping.
-                        ldflags.append(r"-Wl,-rpath=\$$ORIGIN/")
-                        ldflags.append(r"-Wl,-rpath-link=\$(builddir)/")
+                        # We want to get the literal string "$ORIGIN" into the link command,
+                        # so we need lots of escaping.
+                        ldflags.append(r"-Wl,-rpath=\$$ORIGIN/lib.%s/" % self.toolset)
+                        ldflags.append(
+                            r"-Wl,-rpath-link=\$(builddir)/lib.%s/" % self.toolset
+                        )
                 library_dirs = config.get("library_dirs", [])
                 ldflags += [("-L%s" % library_dir) for library_dir in library_dirs]
                 self.WriteList(ldflags, "LDFLAGS_%s" % configname)
                 if self.flavor == "mac":
                     self.WriteList(
                         self.xcode_settings.GetLibtoolflags(configname),
                         "LIBTOOLFLAGS_%s" % configname,
@@ -1864,43 +1804,29 @@
                 assert " " not in link_dep, (
                     "Spaces in alink input filenames not supported (%s)" % link_dep
                 )
             if (
                 self.flavor not in ("mac", "openbsd", "netbsd", "win")
                 and not self.is_standalone_static_library
             ):
-                if self.flavor in ("linux", "android"):
-                    self.WriteMakeRule(
-                        [self.output_binary],
-                        link_deps,
-                        actions=["$(call create_thin_archive,$@,$^)"],
-                    )
-                else:
-                    self.WriteDoCmd(
-                        [self.output_binary],
-                        link_deps,
-                        "alink_thin",
-                        part_of_all,
-                        postbuilds=postbuilds,
-                    )
+                self.WriteDoCmd(
+                    [self.output_binary],
+                    link_deps,
+                    "alink_thin",
+                    part_of_all,
+                    postbuilds=postbuilds,
+                )
             else:
-                if self.flavor in ("linux", "android"):
-                    self.WriteMakeRule(
-                        [self.output_binary],
-                        link_deps,
-                        actions=["$(call create_archive,$@,$^)"],
-                    )
-                else:
-                    self.WriteDoCmd(
-                        [self.output_binary],
-                        link_deps,
-                        "alink",
-                        part_of_all,
-                        postbuilds=postbuilds,
-                    )
+                self.WriteDoCmd(
+                    [self.output_binary],
+                    link_deps,
+                    "alink",
+                    part_of_all,
+                    postbuilds=postbuilds,
+                )
         elif self.type == "shared_library":
             self.WriteLn(
                 "%s: LD_INPUTS := %s"
                 % (
                     QuoteSpaces(self.output_binary),
                     " ".join(QuoteSpaces(dep) for dep in link_deps),
                 )
@@ -1908,25 +1834,14 @@
             self.WriteDoCmd(
                 [self.output_binary],
                 link_deps,
                 "solink",
                 part_of_all,
                 postbuilds=postbuilds,
             )
-            # z/OS has a .so target as well as a sidedeck .x target
-            if self.flavor == "zos":
-                self.WriteLn(
-                    "%s: %s"
-                    % (
-                        QuoteSpaces(
-                            self.GetSharedObjectFromSidedeck(self.output_binary)
-                        ),
-                        QuoteSpaces(self.output_binary),
-                    )
-                )
         elif self.type == "loadable_module":
             for link_dep in link_deps:
                 assert " " not in link_dep, (
                     "Spaces in module input filenames not supported (%s)" % link_dep
                 )
             if self.toolset == "host" and self.flavor == "android":
                 self.WriteDoCmd(
@@ -1976,24 +1891,22 @@
             if self.type == "shared_library":
                 file_desc = "shared library"
             elif self.type == "static_library":
                 file_desc = "static library"
             else:
                 file_desc = "executable"
             install_path = self._InstallableTargetInstallPath()
-            installable_deps = []
-            if self.flavor != "zos":
-                installable_deps.append(self.output)
+            installable_deps = [self.output]
             if (
                 self.flavor == "mac"
                 and "product_dir" not in spec
                 and self.toolset == "target"
             ):
                 # On mac, products are created in install_path immediately.
-                assert install_path == self.output, "{} != {}".format(
+                assert install_path == self.output, "%s != %s" % (
                     install_path,
                     self.output,
                 )
 
             # Point the target alias to the final binary output.
             self.WriteMakeRule(
                 [self.target], [install_path], comment="Add target alias", phony=True
@@ -2003,93 +1916,59 @@
                 self.WriteDoCmd(
                     [install_path],
                     [self.output],
                     "copy",
                     comment="Copy this to the %s output path." % file_desc,
                     part_of_all=part_of_all,
                 )
-                if self.flavor != "zos":
-                    installable_deps.append(install_path)
-            if self.flavor == "zos" and self.type == "shared_library":
-                # lib.target/libnode.so has a dependency on $(obj).target/libnode.so
-                self.WriteDoCmd(
-                    [self.GetSharedObjectFromSidedeck(install_path)],
-                    [self.GetSharedObjectFromSidedeck(self.output)],
-                    "copy",
-                    comment="Copy this to the %s output path." % file_desc,
-                    part_of_all=part_of_all,
-                )
-                # Create a symlink of libnode.x to libnode.version.x
-                self.WriteDoCmd(
-                    [self.GetUnversionedSidedeckFromSidedeck(install_path)],
-                    [install_path],
-                    "symlink",
-                    comment="Symlnk this to the %s output path." % file_desc,
-                    part_of_all=part_of_all,
-                )
-                # Place libnode.version.so and libnode.x symlink in lib.target dir
-                installable_deps.append(self.GetSharedObjectFromSidedeck(install_path))
-                installable_deps.append(
-                    self.GetUnversionedSidedeckFromSidedeck(install_path)
-                )
+                installable_deps.append(install_path)
             if self.output != self.alias and self.alias != self.target:
                 self.WriteMakeRule(
                     [self.alias],
                     installable_deps,
                     comment="Short alias for building this %s." % file_desc,
                     phony=True,
                 )
-            if self.flavor == "zos" and self.type == "shared_library":
-                # Make sure that .x symlink target is run
-                self.WriteMakeRule(
-                    ["all"],
-                    [
-                        self.GetUnversionedSidedeckFromSidedeck(install_path),
-                        self.GetSharedObjectFromSidedeck(install_path),
-                    ],
-                    comment='Add %s to "all" target.' % file_desc,
-                    phony=True,
-                )
-            elif part_of_all:
+            if part_of_all:
                 self.WriteMakeRule(
                     ["all"],
                     [install_path],
                     comment='Add %s to "all" target.' % file_desc,
                     phony=True,
                 )
 
     def WriteList(self, value_list, variable=None, prefix="", quoter=QuoteIfNecessary):
         """Write a variable definition that is a list of values.
 
-        E.g. WriteList(['a','b'], 'foo', prefix='blah') writes out
-             foo = blaha blahb
-        but in a pretty-printed style.
-        """
+    E.g. WriteList(['a','b'], 'foo', prefix='blah') writes out
+         foo = blaha blahb
+    but in a pretty-printed style.
+    """
         values = ""
         if value_list:
             value_list = [quoter(prefix + value) for value in value_list]
             values = " \\\n\t" + " \\\n\t".join(value_list)
-        self.fp.write(f"{variable} :={values}\n\n")
+        self.fp.write("%s :=%s\n\n" % (variable, values))
 
     def WriteDoCmd(
         self, outputs, inputs, command, part_of_all, comment=None, postbuilds=False
     ):
         """Write a Makefile rule that uses do_cmd.
 
-        This makes the outputs dependent on the command line that was run,
-        as well as support the V= make command line flag.
-        """
+    This makes the outputs dependent on the command line that was run,
+    as well as support the V= make command line flag.
+    """
         suffix = ""
         if postbuilds:
             assert "," not in command
             suffix = ",,1"  # Tell do_cmd to honor $POSTBUILDS
         self.WriteMakeRule(
             outputs,
             inputs,
-            actions=[f"$(call do_cmd,{command}{suffix})"],
+            actions=["$(call do_cmd,%s%s)" % (command, suffix)],
             comment=comment,
             command=command,
             force=True,
         )
         # Add our outputs to the list of targets we read depfiles from.
         # all_deps is only used for deps file reading, and for deps files we replace
         # spaces with ? because escaping doesn't work with make's $(sort) and
@@ -2106,26 +1985,26 @@
         order_only=False,
         force=False,
         phony=False,
         command=None,
     ):
         """Write a Makefile rule, with some extra tricks.
 
-        outputs: a list of outputs for the rule (note: this is not directly
-                 supported by make; see comments below)
-        inputs: a list of inputs for the rule
-        actions: a list of shell commands to run for the rule
-        comment: a comment to put in the Makefile above the rule (also useful
-                 for making this Python script's code self-documenting)
-        order_only: if true, makes the dependency order-only
-        force: if true, include FORCE_DO_CMD as an order-only dep
-        phony: if true, the rule does not actually generate the named output, the
-               output is just a name to run the rule
-        command: (optional) command name to generate unambiguous labels
-        """
+    outputs: a list of outputs for the rule (note: this is not directly
+             supported by make; see comments below)
+    inputs: a list of inputs for the rule
+    actions: a list of shell commands to run for the rule
+    comment: a comment to put in the Makefile above the rule (also useful
+             for making this Python script's code self-documenting)
+    order_only: if true, makes the dependency order-only
+    force: if true, include FORCE_DO_CMD as an order-only dep
+    phony: if true, the rule does not actually generate the named output, the
+           output is just a name to run the rule
+    command: (optional) command name to generate unambiguous labels
+    """
         outputs = [QuoteSpaces(o) for o in outputs]
         inputs = [QuoteSpaces(i) for i in inputs]
 
         if comment:
             self.WriteLn("# " + comment)
         if phony:
             self.WriteLn(".PHONY: " + " ".join(outputs))
@@ -2133,19 +2012,19 @@
             self.WriteLn("%s: TOOLSET := $(TOOLSET)" % outputs[0])
         force_append = " FORCE_DO_CMD" if force else ""
 
         if order_only:
             # Order only rule: Just write a simple rule.
             # TODO(evanm): just make order_only a list of deps instead of this hack.
             self.WriteLn(
-                "{}: | {}{}".format(" ".join(outputs), " ".join(inputs), force_append)
+                "%s: | %s%s" % (" ".join(outputs), " ".join(inputs), force_append)
             )
         elif len(outputs) == 1:
             # Regular rule, one output: Just write a simple rule.
-            self.WriteLn("{}: {}{}".format(outputs[0], " ".join(inputs), force_append))
+            self.WriteLn("%s: %s%s" % (outputs[0], " ".join(inputs), force_append))
         else:
             # Regular rule, more than one output: Multiple outputs are tricky in
             # make. We will write three rules:
             # - All outputs depend on an intermediate file.
             # - Make .INTERMEDIATE depend on the intermediate.
             # - The intermediate file depends on the inputs and executes the
             #   actual command.
@@ -2153,40 +2032,38 @@
             # - The multi-output rule will have an do-nothing recipe.
 
             # Hash the target name to avoid generating overlong filenames.
             cmddigest = hashlib.sha1(
                 (command or self.target).encode("utf-8")
             ).hexdigest()
             intermediate = "%s.intermediate" % cmddigest
-            self.WriteLn("{}: {}".format(" ".join(outputs), intermediate))
+            self.WriteLn("%s: %s" % (" ".join(outputs), intermediate))
             self.WriteLn("\t%s" % "@:")
-            self.WriteLn("{}: {}".format(".INTERMEDIATE", intermediate))
-            self.WriteLn(
-                "{}: {}{}".format(intermediate, " ".join(inputs), force_append)
-            )
+            self.WriteLn("%s: %s" % (".INTERMEDIATE", intermediate))
+            self.WriteLn("%s: %s%s" % (intermediate, " ".join(inputs), force_append))
             actions.insert(0, "$(call do_cmd,touch)")
 
         if actions:
             for action in actions:
                 self.WriteLn("\t%s" % action)
         self.WriteLn()
 
     def WriteAndroidNdkModuleRule(self, module_name, all_sources, link_deps):
         """Write a set of LOCAL_XXX definitions for Android NDK.
 
-        These variable definitions will be used by Android NDK but do nothing for
-        non-Android applications.
+    These variable definitions will be used by Android NDK but do nothing for
+    non-Android applications.
 
-        Arguments:
-          module_name: Android NDK module name, which must be unique among all
-              module names.
-          all_sources: A list of source files (will be filtered by Compilable).
-          link_deps: A list of link dependencies, which must be sorted in
-              the order from dependencies to dependents.
-        """
+    Arguments:
+      module_name: Android NDK module name, which must be unique among all
+          module names.
+      all_sources: A list of source files (will be filtered by Compilable).
+      link_deps: A list of link dependencies, which must be sorted in
+          the order from dependencies to dependents.
+    """
         if self.type not in ("executable", "shared_library", "static_library"):
             return
 
         self.WriteLn("# Variable definitions for Android applications")
         self.WriteLn("include $(CLEAR_VARS)")
         self.WriteLn("LOCAL_MODULE := " + module_name)
         self.WriteLn(
@@ -2290,37 +2167,37 @@
         for k, v in env:
             # For
             #  foo := a\ b
             # the escaped space does the right thing. For
             #  export foo := a\ b
             # it does not -- the backslash is written to the env as literal character.
             # So don't escape spaces in |env[k]|.
-            self.WriteLn(f"{QuoteSpaces(target)}: export {k} := {v}")
+            self.WriteLn("%s: export %s := %s" % (QuoteSpaces(target), k, v))
 
     def Objectify(self, path):
         """Convert a path to its output directory form."""
         if "$(" in path:
             path = path.replace("$(obj)/", "$(obj).%s/$(TARGET)/" % self.toolset)
         if "$(obj)" not in path:
-            path = f"$(obj).{self.toolset}/$(TARGET)/{path}"
+            path = "$(obj).%s/$(TARGET)/%s" % (self.toolset, path)
         return path
 
     def Pchify(self, path, lang):
         """Convert a prefix header path to its output directory form."""
         path = self.Absolutify(path)
         if "$(" in path:
             path = path.replace(
-                "$(obj)/", f"$(obj).{self.toolset}/$(TARGET)/pch-{lang}"
+                "$(obj)/", "$(obj).%s/$(TARGET)/pch-%s" % (self.toolset, lang)
             )
             return path
-        return f"$(obj).{self.toolset}/$(TARGET)/pch-{lang}/{path}"
+        return "$(obj).%s/$(TARGET)/pch-%s/%s" % (self.toolset, lang, path)
 
     def Absolutify(self, path):
         """Convert a subdirectory-relative path into a base-relative path.
-        Skips over paths that contain variables."""
+    Skips over paths that contain variables."""
         if "$(" in path:
             # Don't call normpath in this case, as it might collapse the
             # path too aggressively if it features '..'. However it's still
             # important to strip trailing slashes.
             return path.rstrip("/")
         return os.path.normpath(os.path.join(self.path, path))
 
@@ -2331,27 +2208,22 @@
             "INPUT_ROOT": expansion,
             "INPUT_DIRNAME": dirname,
         }
         return path
 
     def _InstallableTargetInstallPath(self):
         """Returns the location of the final output for an installable target."""
-        # Functionality removed for all platforms to match Xcode and hoist
-        # shared libraries into PRODUCT_DIR for users:
         # Xcode puts shared_library results into PRODUCT_DIR, and some gyp files
         # rely on this. Emulate this behavior for mac.
-        # if self.type == "shared_library" and (
-        #     self.flavor != "mac" or self.toolset != "target"
-        # ):
-        #    # Install all shared libs into a common directory (per toolset) for
-        #    # convenient access with LD_LIBRARY_PATH.
-        #    return "$(builddir)/lib.%s/%s" % (self.toolset, self.alias)
-        if self.flavor == "zos" and self.type == "shared_library":
+        if self.type == "shared_library" and (
+            self.flavor != "mac" or self.toolset != "target"
+        ):
+            # Install all shared libs into a common directory (per toolset) for
+            # convenient access with LD_LIBRARY_PATH.
             return "$(builddir)/lib.%s/%s" % (self.toolset, self.alias)
-
         return "$(builddir)/" + self.alias
 
 
 def WriteAutoRegenerationRule(params, root_makefile, makefile_name, build_files):
     """Write the target to regenerate the Makefile."""
     options = params["options"]
     build_files_args = [
@@ -2383,15 +2255,15 @@
 def PerformBuild(data, configurations, params):
     options = params["options"]
     for config in configurations:
         arguments = ["make"]
         if options.toplevel_dir and options.toplevel_dir != ".":
             arguments += "-C", options.toplevel_dir
         arguments.append("BUILDTYPE=" + config)
-        print(f"Building [{config}]: {arguments}")
+        print("Building [%s]: %s" % (config, arguments))
         subprocess.check_call(arguments)
 
 
 def GenerateOutput(target_list, target_dicts, data, params):
     options = params["options"]
     flavor = gyp.common.GetFlavor(params)
     generator_flags = params.get("generator_flags", {})
@@ -2417,15 +2289,15 @@
         )
         return base_path, output_file
 
     # TODO:  search for the first non-'Default' target.  This can go
     # away when we add verification that all targets have the
     # necessary configurations.
     default_configuration = None
-    toolsets = {target_dicts[target]["toolset"] for target in target_list}
+    toolsets = set([target_dicts[target]["toolset"] for target in target_list])
     for target in target_list:
         spec = target_dicts[target]
         if spec["default_configuration"] != "Default":
             default_configuration = spec["default_configuration"]
             break
     if not default_configuration:
         default_configuration = "Default"
@@ -2455,20 +2327,18 @@
         "srcdir": srcdir,
         "copy_archive_args": copy_archive_arguments,
         "makedep_args": makedep_arguments,
         "CC.target": GetEnvironFallback(("CC_target", "CC"), "$(CC)"),
         "AR.target": GetEnvironFallback(("AR_target", "AR"), "$(AR)"),
         "CXX.target": GetEnvironFallback(("CXX_target", "CXX"), "$(CXX)"),
         "LINK.target": GetEnvironFallback(("LINK_target", "LINK"), "$(LINK)"),
-        "PLI.target": GetEnvironFallback(("PLI_target", "PLI"), "pli"),
         "CC.host": GetEnvironFallback(("CC_host", "CC"), "gcc"),
         "AR.host": GetEnvironFallback(("AR_host", "AR"), "ar"),
         "CXX.host": GetEnvironFallback(("CXX_host", "CXX"), "g++"),
         "LINK.host": GetEnvironFallback(("LINK_host", "LINK"), "$(CXX.host)"),
-        "PLI.host": GetEnvironFallback(("PLI_host", "PLI"), "pli"),
     }
     if flavor == "mac":
         flock_command = "./gyp-mac-tool flock"
         header_params.update(
             {
                 "flock": flock_command,
                 "flock_index": 2,
@@ -2476,53 +2346,33 @@
                 "extra_commands": SHARED_HEADER_MAC_COMMANDS,
             }
         )
     elif flavor == "android":
         header_params.update({"link_commands": LINK_COMMANDS_ANDROID})
     elif flavor == "zos":
         copy_archive_arguments = "-fPR"
-        CC_target = GetEnvironFallback(("CC_target", "CC"), "njsc")
-        makedep_arguments = "-MMD"
-        if CC_target == "clang":
-            CC_host = GetEnvironFallback(("CC_host", "CC"), "clang")
-            CXX_target = GetEnvironFallback(("CXX_target", "CXX"), "clang++")
-            CXX_host = GetEnvironFallback(("CXX_host", "CXX"), "clang++")
-        elif CC_target == "ibm-clang64":
-            CC_host = GetEnvironFallback(("CC_host", "CC"), "ibm-clang64")
-            CXX_target = GetEnvironFallback(("CXX_target", "CXX"), "ibm-clang++64")
-            CXX_host = GetEnvironFallback(("CXX_host", "CXX"), "ibm-clang++64")
-        elif CC_target == "ibm-clang":
-            CC_host = GetEnvironFallback(("CC_host", "CC"), "ibm-clang")
-            CXX_target = GetEnvironFallback(("CXX_target", "CXX"), "ibm-clang++")
-            CXX_host = GetEnvironFallback(("CXX_host", "CXX"), "ibm-clang++")
-        else:
-            # Node.js versions prior to v18:
-            makedep_arguments = "-qmakedep=gcc"
-            CC_host = GetEnvironFallback(("CC_host", "CC"), "njsc")
-            CXX_target = GetEnvironFallback(("CXX_target", "CXX"), "njsc++")
-            CXX_host = GetEnvironFallback(("CXX_host", "CXX"), "njsc++")
+        makedep_arguments = "-qmakedep=gcc"
         header_params.update(
             {
                 "copy_archive_args": copy_archive_arguments,
                 "makedep_args": makedep_arguments,
                 "link_commands": LINK_COMMANDS_OS390,
-                "extra_commands": SHARED_HEADER_OS390_COMMANDS,
-                "CC.target": CC_target,
-                "CXX.target": CXX_target,
-                "CC.host": CC_host,
-                "CXX.host": CXX_host,
+                "CC.target": GetEnvironFallback(("CC_target", "CC"), "njsc"),
+                "CXX.target": GetEnvironFallback(("CXX_target", "CXX"), "njsc++"),
+                "CC.host": GetEnvironFallback(("CC_host", "CC"), "njsc"),
+                "CXX.host": GetEnvironFallback(("CXX_host", "CXX"), "njsc++"),
             }
         )
     elif flavor == "solaris":
         copy_archive_arguments = "-pPRf@"
         header_params.update(
             {
                 "copy_archive_args": copy_archive_arguments,
                 "flock": "./gyp-flock-tool flock",
-                "flock_index": 2,
+                "flock_index": 2
             }
         )
     elif flavor == "freebsd":
         # Note: OpenBSD has sysutils/flock. lockf seems to be FreeBSD specific.
         header_params.update({"flock": "lockf"})
     elif flavor == "openbsd":
         copy_archive_arguments = "-pPRf"
@@ -2533,24 +2383,14 @@
             {
                 "copy_archive_args": copy_archive_arguments,
                 "link_commands": LINK_COMMANDS_AIX,
                 "flock": "./gyp-flock-tool flock",
                 "flock_index": 2,
             }
         )
-    elif flavor == "os400":
-        copy_archive_arguments = "-pPRf"
-        header_params.update(
-            {
-                "copy_archive_args": copy_archive_arguments,
-                "link_commands": LINK_COMMANDS_OS400,
-                "flock": "./gyp-flock-tool flock",
-                "flock_index": 2,
-            }
-        )
 
     build_file, _, _ = gyp.common.ParseQualifiedTarget(target_list[0])
     make_global_settings_array = data[build_file].get("make_global_settings", [])
     wrappers = {}
     for key, value in make_global_settings_array:
         if key.endswith("_wrapper"):
             wrappers[key[: -len("_wrapper")]] = "$(abspath %s)" % value
@@ -2558,28 +2398,28 @@
     for key, value in make_global_settings_array:
         if re.match(".*_wrapper", key):
             continue
         if value[0] != "$":
             value = "$(abspath %s)" % value
         wrapper = wrappers.get(key)
         if wrapper:
-            value = f"{wrapper} {value}"
+            value = "%s %s" % (wrapper, value)
             del wrappers[key]
         if key in ("CC", "CC.host", "CXX", "CXX.host"):
             make_global_settings += (
                 "ifneq (,$(filter $(origin %s), undefined default))\n" % key
             )
             # Let gyp-time envvars win over global settings.
             env_key = key.replace(".", "_")  # CC.host -> CC_host
             if env_key in os.environ:
                 value = os.environ[env_key]
-            make_global_settings += f"  {key} = {value}\n"
+            make_global_settings += "  %s = %s\n" % (key, value)
             make_global_settings += "endif\n"
         else:
-            make_global_settings += f"{key} ?= {value}\n"
+            make_global_settings += "%s ?= %s\n" % (key, value)
     # TODO(ukai): define cmd when only wrapper is specified in
     # make_global_settings.
 
     header_params["make_global_settings"] = make_global_settings
 
     gyp.common.EnsureDirExists(makefile_path)
     root_makefile = open(makefile_path, "w")
@@ -2609,16 +2449,16 @@
     build_files = set()
     include_list = set()
     for qualified_target in target_list:
         build_file, target, toolset = gyp.common.ParseQualifiedTarget(qualified_target)
 
         this_make_global_settings = data[build_file].get("make_global_settings", [])
         assert make_global_settings_array == this_make_global_settings, (
-            "make_global_settings needs to be the same for all targets "
-            f"{this_make_global_settings} vs. {make_global_settings}"
+            "make_global_settings needs to be the same for all targets. %s vs. %s"
+            % (this_make_global_settings, make_global_settings)
         )
 
         build_files.add(gyp.common.RelativePath(build_file, options.toplevel_dir))
         included_files = data[build_file]["included_files"]
         for included_file in included_files:
             # The included_files entries are relative to the dir of the build file
             # that included them, so we have to undo that and then make them relative
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/msvs.py` & `gyp-next-0.4.0/pylib/gyp/generator/msvs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
+from __future__ import print_function
 
 import ntpath
 import os
 import posixpath
 import re
 import subprocess
 import sys
@@ -21,14 +22,16 @@
 import gyp.MSVSToolFile as MSVSToolFile
 import gyp.MSVSUserFile as MSVSUserFile
 import gyp.MSVSUtil as MSVSUtil
 import gyp.MSVSVersion as MSVSVersion
 from gyp.common import GypError
 from gyp.common import OrderedSet
 
+PY3 = bytes != str
+
 
 # Regular expression for validating Visual Studio GUIDs.  If the GUID
 # contains lowercase hex letters, MSVS will be fine. However,
 # IncrediBuild BuildConsole will parse the solution file, but then
 # silently skip building the target causing hard to track down errors.
 # Note that this only happens with the BuildConsole, and does not occur
 # if IncrediBuild is executed from inside Visual Studio.  This regex
@@ -77,14 +80,15 @@
     "msvs_external_builder_out_dir",
     "msvs_external_builder_build_cmd",
     "msvs_external_builder_clean_cmd",
     "msvs_external_builder_clcompile_cmd",
     "msvs_enable_winrt",
     "msvs_requires_importlibrary",
     "msvs_enable_winphone",
+    "msvs_enable_marmasm",
     "msvs_application_type_revision",
     "msvs_target_platform_version",
     "msvs_target_platform_minversion",
 ]
 
 generator_filelist_paths = None
 
@@ -113,15 +117,17 @@
     if not cached_domain or not cached_username:
         domain = os.environ.get("USERDOMAIN")
         username = os.environ.get("USERNAME")
         if not domain or not username:
             call = subprocess.Popen(
                 ["net", "config", "Workstation"], stdout=subprocess.PIPE
             )
-            config = call.communicate()[0].decode("utf-8")
+            config = call.communicate()[0]
+            if PY3:
+                config = config.decode("utf-8")
             username_re = re.compile(r"^User name\s+(\S+)", re.MULTILINE)
             username_match = username_re.search(config)
             if username_match:
                 username = username_match.group(1)
             domain_re = re.compile(r"^Logon domain\s+(\S+)", re.MULTILINE)
             domain_match = domain_re.search(config)
             if domain_match:
@@ -148,53 +154,49 @@
   """
     normalized = os.path.normpath(source)
     if source.count("$") == normalized.count("$"):
         source = normalized
     return source
 
 
-def _FixPath(path, separator="\\"):
+def _FixPath(path):
     """Convert paths to a form that will make sense in a vcproj file.
 
   Arguments:
     path: The path to convert, may contain / etc.
   Returns:
     The path with all slashes made into backslashes.
   """
     if (
         fixpath_prefix
         and path
         and not os.path.isabs(path)
-        and path[0] != "$"
+        and not path[0] == "$"
         and not _IsWindowsAbsPath(path)
     ):
         path = os.path.join(fixpath_prefix, path)
-    if separator == "\\":
-        path = path.replace("/", "\\")
+    path = path.replace("/", "\\")
     path = _NormalizedSource(path)
-    if separator == "/":
-        path = path.replace("\\", "/")
-    if path and path[-1] == separator:
+    if path and path[-1] == "\\":
         path = path[:-1]
     return path
 
 
 def _IsWindowsAbsPath(path):
     """
-  On Cygwin systems Python needs a little help determining if a path
-  is an absolute Windows path or not, so that
+  On Cygwin systems Python needs a little help determining if a path is an absolute Windows path or not, so that
   it does not treat those as relative, which results in bad paths like:
   '..\\C:\\<some path>\\some_source_code_file.cc'
   """
     return path.startswith("c:") or path.startswith("C:")
 
 
-def _FixPaths(paths, separator="\\"):
+def _FixPaths(paths):
     """Fix each of the paths of the list."""
-    return [_FixPath(i, separator) for i in paths]
+    return [_FixPath(i) for i in paths]
 
 
 def _ConvertSourcesToFilterHierarchy(
     sources, prefix=None, excluded=None, list_excluded=True, msvs_version=None
 ):
     """Converts a list split source file paths into a vcproj folder hierarchy.
 
@@ -277,17 +279,17 @@
     # TODO(bradnelson): ugly hack, fix this more generally!!!
     if "Directories" in setting or "Dependencies" in setting:
         if type(value) == str:
             value = value.replace("/", "\\")
         else:
             value = [i.replace("/", "\\") for i in value]
     if not tools.get(tool_name):
-        tools[tool_name] = {}
+        tools[tool_name] = dict()
     tool = tools[tool_name]
-    if setting == "CompileAsWinRT":
+    if "CompileAsWinRT" == setting:
         return
     if tool.get(setting):
         if only_if_unset:
             return
         if type(tool[setting]) == list and type(value) == list:
             tool[setting] += value
         else:
@@ -313,15 +315,15 @@
         return config_name[0 : -len(platform_name) - 1]
     else:
         return config_name
 
 
 def _ConfigFullName(config_name, config_data):
     platform_name = _ConfigPlatform(config_data)
-    return f"{_ConfigBaseName(config_name, platform_name)}|{platform_name}"
+    return "%s|%s" % (_ConfigBaseName(config_name, platform_name), platform_name)
 
 
 def _ConfigWindowsTargetPlatformVersion(config_data, version):
     target_ver = config_data.get("msvs_windows_target_platform_version")
     if target_ver and re.match(r"^\d+", target_ver):
         return target_ver
     config_ver = config_data.get("msvs_windows_sdk_version")
@@ -334,23 +336,23 @@
             sdk_dir = MSVSVersion._RegistryGetValue(key % ver, "InstallationFolder")
             if not sdk_dir:
                 continue
             version = MSVSVersion._RegistryGetValue(key % ver, "ProductVersion") or ""
             # Find a matching entry in sdk_dir\include.
             expected_sdk_dir = r"%s\include" % sdk_dir
             names = sorted(
-                (
+                [
                     x
                     for x in (
                         os.listdir(expected_sdk_dir)
                         if os.path.isdir(expected_sdk_dir)
                         else []
                     )
                     if x.startswith(version)
-                ),
+                ],
                 reverse=True,
             )
             if names:
                 return names[0]
             else:
                 print(
                     "Warning: No include files found for detected "
@@ -408,31 +410,29 @@
         if has_input_path and direct_cmd.find("INPUTPATH") >= 0:
             cmd += "set INPUTPATH=$(InputPath) && "
         cmd += 'bash -c "%(cmd)s"'
         cmd = cmd % {"cygwin_dir": cygwin_dir, "cmd": direct_cmd}
         return input_dir_preamble + cmd
     else:
         # Convert cat --> type to mimic unix.
-        command = ["type"] if cmd[0] == "cat" else [cmd[0].replace("/", "\\")]
+        if cmd[0] == "cat":
+            command = ["type"]
+        else:
+            command = [cmd[0].replace("/", "\\")]
         # Add call before command to ensure that commands can be tied together one
         # after the other without aborting in Incredibuild, since IB makes a bat
         # file out of the raw command string, and some commands (like python) are
         # actually batch files themselves.
         command.insert(0, "call")
         # Fix the paths
         # TODO(quote): This is a really ugly heuristic, and will miss path fixing
-        #              for arguments like "--arg=path", arg=path, or "/opt:path".
-        # If the argument starts with a slash or dash, or contains an equal sign,
-        # it's probably a command line switch.
-        # Return the path with forward slashes because the command using it might
-        # not support backslashes.
-        arguments = [
-            i if (i[:1] in "/-" or "=" in i) else _FixPath(i, "/")
-            for i in cmd[1:]
-        ]
+        #              for arguments like "--arg=path" or "/opt:path".
+        # If the argument starts with a slash or dash, it's probably a command line
+        # switch
+        arguments = [i if (i[:1] in "/-") else _FixPath(i) for i in cmd[1:]]
         arguments = [i.replace("$(InputDir)", "%INPUTDIR%") for i in arguments]
         arguments = [MSVSSettings.FixVCMacroSlashes(i) for i in arguments]
         if quote_cmd:
             # Support a mode for using cmd directly.
             # Convert any paths to native form (first element is used directly).
             # TODO(quote):  regularize quoting path names throughout the module
             arguments = ['"%s"' % i for i in arguments]
@@ -616,15 +616,15 @@
   Arguments:
     p: the target project
     rules: the set of rules to include
     output_dir: the directory in which the project/gyp resides
     spec: the project dict
     options: global generator options
   """
-    rules_filename = "{}{}.rules".format(spec["target_name"], options.suffix)
+    rules_filename = "%s%s.rules" % (spec["target_name"], options.suffix)
     rules_file = MSVSToolFile.Writer(
         os.path.join(output_dir, rules_filename), spec["target_name"]
     )
     # Add each rule.
     for r in rules:
         rule_name = r["rule_name"]
         rule_ext = r["extension"]
@@ -662,15 +662,15 @@
     rules: the list of rules to include
     output_dir: path containing project and gyp files
     spec: project specification data
     sources: set of sources known
     options: global generator options
     actions_to_add: The list of actions we will add to.
   """
-    filename = "{}_rules{}.mk".format(spec["target_name"], options.suffix)
+    filename = "%s_rules%s.mk" % (spec["target_name"], options.suffix)
     mk_file = gyp.common.WriteOnDiff(os.path.join(output_dir, filename))
     # Find cygwin style versions of some paths.
     mk_file.write('OutDirCygwin:=$(shell cygpath -u "$(OutDir)")\n')
     mk_file.write('IntDirCygwin:=$(shell cygpath -u "$(IntDir)")\n')
     # Gather stuff needed to emit all: target.
     all_inputs = OrderedSet()
     all_outputs = OrderedSet()
@@ -705,15 +705,15 @@
             inputs = [_Cygwinify(i) for i in inputs]
             outputs = [_Cygwinify(i) for i in outputs]
             # Prepare the command line for this rule.
             cmd = [_RuleExpandPath(c, tf) for c in rule["action"]]
             cmd = ['"%s"' % i for i in cmd]
             cmd = " ".join(cmd)
             # Add it to the makefile.
-            mk_file.write("{}: {}\n".format(" ".join(outputs), " ".join(inputs)))
+            mk_file.write("%s: %s\n" % (" ".join(outputs), " ".join(inputs)))
             mk_file.write("\t%s\n\n" % cmd)
     # Close up the file.
     mk_file.close()
 
     # Add makefile to list of sources.
     sources.add(filename)
     # Add a build action to call makefile.
@@ -842,15 +842,15 @@
 
 
 def _EscapeCppDefineForMSVS(s):
     """Escapes a CPP define so that it will reach the compiler unaltered."""
     s = _EscapeEnvironmentVariableExpansion(s)
     s = _EscapeCommandLineArgumentForMSVS(s)
     s = _EscapeVCProjCommandLineArgListItem(s)
-    # cl.exe replaces literal # characters with = in preprocessor definitions for
+    # cl.exe replaces literal # characters with = in preprocesor definitions for
     # some reason. Octal-encode to work around that.
     s = s.replace("#", "\\%03o" % ord("#"))
     return s
 
 
 quote_replacer_regex2 = re.compile(r'(\\+)"')
 
@@ -881,15 +881,15 @@
 
 
 def _EscapeCppDefineForMSBuild(s):
     """Escapes a CPP define so that it will reach the compiler unaltered."""
     s = _EscapeEnvironmentVariableExpansion(s)
     s = _EscapeCommandLineArgumentForMSBuild(s)
     s = _EscapeMSBuildSpecialCharacters(s)
-    # cl.exe replaces literal # characters with = in preprocessor definitions for
+    # cl.exe replaces literal # characters with = in preprocesor definitions for
     # some reason. Octal-encode to work around that.
     s = s.replace("#", "\\%03o" % ord("#"))
     return s
 
 
 def _GenerateRulesForMSVS(
     p, output_dir, options, spec, sources, excluded_sources, actions_to_add
@@ -1025,14 +1025,53 @@
 
     if version.UsesVcxproj():
         return _GenerateMSBuildProject(project, options, version, generator_flags, spec)
     else:
         return _GenerateMSVSProject(project, options, version, generator_flags)
 
 
+# TODO: Avoid code duplication with _ValidateSourcesForOSX in make.py.
+def _ValidateSourcesForMSVSProject(spec, version):
+    """Makes sure if duplicate basenames are not specified in the source list.
+
+  Arguments:
+    spec: The target dictionary containing the properties of the target.
+    version: The VisualStudioVersion object.
+  """
+    # This validation should not be applied to MSVC2010 and later.
+    assert not version.UsesVcxproj()
+
+    # TODO: Check if MSVC allows this for loadable_module targets.
+    if spec.get("type", None) not in ("static_library", "shared_library"):
+        return
+    sources = spec.get("sources", [])
+    basenames = {}
+    for source in sources:
+        name, ext = os.path.splitext(source)
+        is_compiled_file = ext in [".c", ".cc", ".cpp", ".cxx", ".m", ".mm", ".s", ".S"]
+        if not is_compiled_file:
+            continue
+        basename = os.path.basename(name)  # Don't include extension.
+        basenames.setdefault(basename, []).append(source)
+
+    error = ""
+    for basename, files in basenames.items():
+        if len(files) > 1:
+            error += "  %s: %s\n" % (basename, " ".join(files))
+
+    if error:
+        print(
+            "static library %s has several files with the same basename:\n"
+            % spec["target_name"]
+            + error
+            + "MSVC08 cannot handle that."
+        )
+        raise GypError("Duplicate basenames in sources section, see list above")
+
+
 def _GenerateMSVSProject(project, options, version, generator_flags):
     """Generates a .vcproj file.  It may create .rules and .user files too.
 
   Arguments:
     project: The project object we will generate the file for.
     options: Global options passed to the generator.
     version: The VisualStudioVersion object.
@@ -1051,14 +1090,19 @@
     gyp_path = _NormalizedSource(project.build_file)
     relative_path_of_gyp_file = gyp.common.RelativePath(gyp_path, project_dir)
 
     config_type = _GetMSVSConfigurationType(spec, project.build_file)
     for config_name, config in spec["configurations"].items():
         _AddConfigurationToMSVSProject(p, spec, config_type, config_name, config)
 
+    # MSVC08 and prior version cannot handle duplicate basenames in the same
+    # target.
+    # TODO: Take excluded sources into consideration if possible.
+    _ValidateSourcesForMSVSProject(spec, version)
+
     # Prepare list of sources and excluded sources.
     gyp_file = os.path.split(project.build_file)[1]
     sources, excluded_sources = _PrepareListOfSources(spec, generator_flags, gyp_file)
 
     # Add rules.
     actions_to_add = {}
     _GenerateRulesForMSVS(
@@ -1182,15 +1226,15 @@
     disabled_warnings = _GetDisabledWarnings(config)
     prebuild = config.get("msvs_prebuild")
     postbuild = config.get("msvs_postbuild")
     def_file = _GetModuleDefinition(spec)
     precompiled_header = config.get("msvs_precompiled_header")
 
     # Prepare the list of tools as a dictionary.
-    tools = {}
+    tools = dict()
     # Add in user specified msvs_settings.
     msvs_settings = config.get("msvs_settings", {})
     MSVSSettings.ValidateMSVSSettings(msvs_settings)
 
     # Prevent default library inheritance from the environment.
     _ToolAppend(tools, "VCLinkerTool", "AdditionalDependencies", ["$(NOINHERIT)"])
 
@@ -1367,25 +1411,28 @@
     target_extension = spec.get("product_extension")
     if target_extension:
         return "." + target_extension
     return None
 
 
 def _GetDefines(config):
-    """Returns the list of preprocessor definitions for this configuration.
+    """Returns the list of preprocessor definitions for this configuation.
 
   Arguments:
     config: The dictionary that defines the special processing to be done
             for this configuration.
   Returns:
     The list of preprocessor definitions.
   """
     defines = []
     for d in config.get("defines", []):
-        fd = "=".join([str(dpart) for dpart in d]) if isinstance(d, list) else str(d)
+        if type(d) == list:
+            fd = "=".join([str(dpart) for dpart in d])
+        else:
+            fd = str(d)
         defines.append(fd)
     return defines
 
 
 def _GetDisabledWarnings(config):
     return [str(i) for i in config.get("msvs_disabled_warnings", [])]
 
@@ -1569,15 +1616,15 @@
     )
 
     # Prune filters with a single child to flatten ugly directory structures
     # such as ../../src/modules/module1 etc.
     if version.UsesVcxproj():
         while (
             all([isinstance(s, MSVSProject.Filter) for s in sources])
-            and len({s.name for s in sources}) == 1
+            and len(set([s.name for s in sources])) == 1
         ):
             assert all([len(s.contents) == 1 for s in sources])
             sources = [s.contents[0] for s in sources]
     else:
         while len(sources) == 1 and isinstance(sources[0], MSVSProject.Filter):
             sources = sources[0].contents
 
@@ -1588,15 +1635,18 @@
     # If any non-native rules use 'idl' as an extension exclude idl files.
     # Gather a list here to use later.
     using_idl = False
     for rule in spec.get("rules", []):
         if rule["extension"] == "idl" and int(rule.get("msvs_external_rule", 0)):
             using_idl = True
             break
-    excluded_idl = [i for i in sources if i.endswith(".idl")] if using_idl else []
+    if using_idl:
+        excluded_idl = [i for i in sources if i.endswith(".idl")]
+    else:
+        excluded_idl = []
     return excluded_idl
 
 
 def _GetPrecompileRelatedFiles(spec):
     # Gather a list of precompiled header related sources.
     precompiled_related = []
     for _, config in spec["configurations"].items():
@@ -1772,49 +1822,49 @@
             # _AddCustomBuildToolForMSVS() will call _FixPath() on the inputs and
             # outputs, so do the same for our generated command line.
             if src.endswith("/"):
                 src_bare = src[:-1]
                 base_dir = posixpath.split(src_bare)[0]
                 outer_dir = posixpath.split(src_bare)[1]
                 fixed_dst = _FixPath(dst)
-                full_dst = f'"{fixed_dst}\\{outer_dir}\\"'
-                cmd = 'mkdir {} 2>nul & cd "{}" && xcopy /e /f /y "{}" {}'.format(
+                full_dst = '"%s\\%s\\"' % (fixed_dst, outer_dir)
+                cmd = 'mkdir %s 2>nul & cd "%s" && xcopy /e /f /y "%s" %s' % (
                     full_dst,
                     _FixPath(base_dir),
                     outer_dir,
                     full_dst,
                 )
                 copies.append(
                     (
                         [src],
                         ["dummy_copies", dst],
                         cmd,
-                        f"Copying {src} to {fixed_dst}",
+                        "Copying %s to %s" % (src, fixed_dst),
                     )
                 )
             else:
                 fix_dst = _FixPath(cpy["destination"])
-                cmd = 'mkdir "{}" 2>nul & set ERRORLEVEL=0 & copy /Y "{}" "{}"'.format(
+                cmd = 'mkdir "%s" 2>nul & set ERRORLEVEL=0 & copy /Y "%s" "%s"' % (
                     fix_dst,
                     _FixPath(src),
                     _FixPath(dst),
                 )
-                copies.append(([src], [dst], cmd, f"Copying {src} to {fix_dst}"))
+                copies.append(([src], [dst], cmd, "Copying %s to %s" % (src, fix_dst)))
     return copies
 
 
 def _GetPathDict(root, path):
     # |path| will eventually be empty (in the recursive calls) if it was initially
     # relative; otherwise it will eventually end up as '\', 'D:\', etc.
     if not path or path.endswith(os.sep):
         return root
     parent, folder = os.path.split(path)
     parent_dict = _GetPathDict(root, parent)
     if folder not in parent_dict:
-        parent_dict[folder] = {}
+        parent_dict[folder] = dict()
     return parent_dict[folder]
 
 
 def _DictsToFolders(base_path, bucket, flat):
     # Convert to folders recursively.
     children = []
     for folder, contents in bucket.items():
@@ -1894,20 +1944,20 @@
 def _GetPlatformOverridesOfProject(spec):
     # Prepare a dict indicating which project configurations are used for which
     # solution configurations for this target.
     config_platform_overrides = {}
     for config_name, c in spec["configurations"].items():
         config_fullname = _ConfigFullName(config_name, c)
         platform = c.get("msvs_target_platform", _ConfigPlatform(c))
-        fixed_config_fullname = "{}|{}".format(
+        fixed_config_fullname = "%s|%s" % (
             _ConfigBaseName(config_name, _ConfigPlatform(c)),
             platform,
         )
         if spec["toolset"] == "host" and generator_supports_multiple_toolsets:
-            fixed_config_fullname = f"{config_name}|x64"
+            fixed_config_fullname = "%s|x64" % (config_name,)
         config_platform_overrides[config_fullname] = fixed_config_fullname
     return config_platform_overrides
 
 
 def _CreateProjectObjects(target_list, target_dicts, options, msvs_version):
     """Create a MSVSProject object for the targets found in target list.
 
@@ -2052,15 +2102,15 @@
             continue
         sln_path = build_file_root + options.suffix + ".sln"
         if options.generator_output:
             sln_path = os.path.join(options.generator_output, sln_path)
 
     for config in configurations:
         arguments = [devenv, sln_path, "/Build", config]
-        print(f"Building [{config}]: {arguments}")
+        print("Building [%s]: %s" % (config, arguments))
         subprocess.check_call(arguments)
 
 
 def CalculateGeneratorInputInfo(params):
     if params.get("flavor") == "ninja":
         toplevel = params["options"].toplevel_dir
         qualified_out_dir = os.path.normpath(
@@ -2167,20 +2217,15 @@
         if generator_flags.get("msvs_error_on_missing_sources", False):
             raise GypError(error_message)
         else:
             print("Warning: " + error_message, file=sys.stdout)
 
 
 def _GenerateMSBuildFiltersFile(
-    filters_path,
-    source_files,
-    rule_dependencies,
-    extension_to_rule_name,
-    platforms,
-    toolset,
+    filters_path, source_files, rule_dependencies, extension_to_rule_name, platforms
 ):
     """Generate the filters file.
 
   This file is used by Visual Studio to organize the presentation of source
   files into folders.
 
   Arguments:
@@ -2192,15 +2237,14 @@
     source_group = []
     _AppendFiltersForMSBuild(
         "",
         source_files,
         rule_dependencies,
         extension_to_rule_name,
         platforms,
-        toolset,
         filter_group,
         source_group,
     )
     if filter_group:
         content = [
             "Project",
             {
@@ -2218,35 +2262,34 @@
 
 def _AppendFiltersForMSBuild(
     parent_filter_name,
     sources,
     rule_dependencies,
     extension_to_rule_name,
     platforms,
-    toolset,
     filter_group,
     source_group,
 ):
     """Creates the list of filters and sources to be added in the filter file.
 
   Args:
       parent_filter_name: The name of the filter under which the sources are
           found.
       sources: The hierarchy of filters and sources to process.
       extension_to_rule_name: A dictionary mapping file extensions to rules.
       filter_group: The list to which filter entries will be appended.
-      source_group: The list to which source entries will be appended.
+      source_group: The list to which source entries will be appeneded.
   """
     for source in sources:
         if isinstance(source, MSVSProject.Filter):
             # We have a sub-filter.  Create the name of that sub-filter.
             if not parent_filter_name:
                 filter_name = source.name
             else:
-                filter_name = f"{parent_filter_name}\\{source.name}"
+                filter_name = "%s\\%s" % (parent_filter_name, source.name)
             # Add the filter to the group.
             filter_group.append(
                 [
                     "Filter",
                     {"Include": filter_name},
                     ["UniqueIdentifier", MSVSNew.MakeGuid(source.name)],
                 ]
@@ -2254,32 +2297,31 @@
             # Recurse and add its dependents.
             _AppendFiltersForMSBuild(
                 filter_name,
                 source.contents,
                 rule_dependencies,
                 extension_to_rule_name,
                 platforms,
-                toolset,
                 filter_group,
                 source_group,
             )
         else:
             # It's a source.  Create a source entry.
             _, element = _MapFileToMsBuildSourceType(
-                source, rule_dependencies, extension_to_rule_name, platforms, toolset
+                source, rule_dependencies, extension_to_rule_name, platforms
             )
             source_entry = [element, {"Include": source}]
             # Specify the filter it is part of, if any.
             if parent_filter_name:
                 source_entry.append(["Filter", parent_filter_name])
             source_group.append(source_entry)
 
 
 def _MapFileToMsBuildSourceType(
-    source, rule_dependencies, extension_to_rule_name, platforms, toolset
+    source, rule_dependencies, extension_to_rule_name, platforms
 ):
     """Returns the group and element type of the source file.
 
   Arguments:
       source: The source file name.
       extension_to_rule_name: A dictionary mapping file extensions to rules.
 
@@ -2299,16 +2341,17 @@
         element = "ClInclude"
     elif ext == ".rc":
         group = "resource"
         element = "ResourceCompile"
     elif ext in [".s", ".asm"]:
         group = "masm"
         element = "MASM"
-        if "arm64" in platforms and toolset == "target":
-            element = "MARMASM"
+        for platform in platforms:
+            if platform.lower() in ["arm", "arm64"]:
+                element = "MARMASM"
     elif ext == ".idl":
         group = "midl"
         element = "Midl"
     elif source in rule_dependencies:
         group = "rule_dependency"
         element = "CustomBuild"
     else:
@@ -2327,16 +2370,16 @@
     targets_files_of_rules,
     actions_to_add,
     rule_dependencies,
     extension_to_rule_name,
 ):
     # MSBuild rules are implemented using three files: an XML file, a .targets
     # file and a .props file.
-    # For more details see:
-    # https://devblogs.microsoft.com/cppblog/quick-help-on-vs2010-custom-build-rule/
+    # See http://blogs.msdn.com/b/vcblog/archive/2010/04/21/quick-help-on-vs2010-custom-build-rule.aspx
+    # for more details.
     rules = spec.get("rules", [])
     rules_native = [r for r in rules if not int(r.get("msvs_external_rule", 0))]
     rules_external = [r for r in rules if int(r.get("msvs_external_rule", 0))]
 
     msbuild_rules = []
     for rule in rules_native:
         # Skip a rule with no action and no inputs.
@@ -2366,15 +2409,15 @@
     if rules_external:
         _GenerateExternalRules(
             rules_external, output_dir, spec, sources, options, actions_to_add
         )
     _AdjustSourcesForRules(rules, sources, excluded_sources, True)
 
 
-class MSBuildRule:
+class MSBuildRule(object):
     """Used to store information used to generate an MSBuild rule.
 
   Attributes:
     rule_name: The rule name, sanitized to use in XML.
     target_name: The name of the target.
     after_targets: The name of the AfterTargets element.
     before_targets: The name of the BeforeTargets element.
@@ -2565,15 +2608,15 @@
         ]
         read_tlog_section = [
             "WriteLinesToFile",
             {
                 "Condition": "'@(%s)' != '' and '%%(%s.ExcludedFromBuild)' != "
                 "'true'" % (rule.tlog, rule.tlog),
                 "File": "$(IntDir)$(ProjectName).read.1.tlog",
-                "Lines": f"^%({rule.tlog}.Source);%({rule.tlog}.Inputs)",
+                "Lines": "^%%(%s.Source);%%(%s.Inputs)" % (rule.tlog, rule.tlog),
             },
         ]
         command_and_input_section = [
             rule_name,
             {
                 "Condition": "'@(%s)' != '' and '%%(%s.ExcludedFromBuild)' != "
                 "'true'" % (rule_name, rule_name),
@@ -2911,15 +2954,15 @@
     )
 
 
 def _GetMSBuildProjectConfigurations(configurations, spec):
     group = ["ItemGroup", {"Label": "ProjectConfigurations"}]
     for (name, settings) in sorted(configurations.items()):
         configuration, platform = _GetConfigurationAndPlatform(name, settings, spec)
-        designation = f"{configuration}|{platform}"
+        designation = "%s|%s" % (configuration, platform)
         group.append(
             [
                 "ProjectConfiguration",
                 {"Include": designation},
                 ["Configuration", configuration],
                 ["Platform", platform],
             ]
@@ -3002,27 +3045,24 @@
     properties = {}
     for name, settings in spec["configurations"].items():
         msbuild_attributes = _GetMSBuildAttributes(spec, settings, build_file)
         condition = _GetConfigurationCondition(name, settings, spec)
         character_set = msbuild_attributes.get("CharacterSet")
         config_type = msbuild_attributes.get("ConfigurationType")
         _AddConditionalProperty(properties, condition, "ConfigurationType", config_type)
-        spectre_mitigation = msbuild_attributes.get('SpectreMitigation')
-        if spectre_mitigation:
-            _AddConditionalProperty(properties, condition, "SpectreMitigation",
-                                    spectre_mitigation)
         if config_type == "Driver":
             _AddConditionalProperty(properties, condition, "DriverType", "WDM")
             _AddConditionalProperty(
                 properties, condition, "TargetVersion", _ConfigTargetVersion(settings)
             )
-        if character_set and "msvs_enable_winrt" not in spec:
-            _AddConditionalProperty(
-                properties, condition, "CharacterSet", character_set
-            )
+        if character_set:
+            if "msvs_enable_winrt" not in spec:
+                _AddConditionalProperty(
+                    properties, condition, "CharacterSet", character_set
+                )
     return _GetMSBuildPropertyGroup(spec, "Configuration", properties)
 
 
 def _GetMSBuildLocalProperties(msbuild_toolset):
     # Currently the only local property we support is PlatformToolset
     properties = {}
     if msbuild_toolset:
@@ -3094,16 +3134,14 @@
             if not directory.endswith("\\"):
                 directory += "\\"
             msbuild_attributes[a] = directory
         elif a == "CharacterSet":
             msbuild_attributes[a] = _ConvertMSVSCharacterSet(msvs_attributes[a])
         elif a == "ConfigurationType":
             msbuild_attributes[a] = _ConvertMSVSConfigurationType(msvs_attributes[a])
-        elif a == "SpectreMitigation":
-            msbuild_attributes[a] = msvs_attributes[a]
         else:
             print("Warning: Do not know how to convert MSVS attribute " + a)
     return msbuild_attributes
 
 
 def _ConvertMSVSCharacterSet(char_set):
     if char_set.isdigit():
@@ -3281,19 +3319,21 @@
             # Variable references that refer to names not in properties are excluded
             # These can exist for instance to refer built in definitions like
             # $(SolutionDir).
             #
             # Self references are ignored. Self reference is used in a few places to
             # append to the default value. I.e. PATH=$(PATH);other_path
             edges.update(
-                {
-                    v
-                    for v in MSVS_VARIABLE_REFERENCE.findall(value)
-                    if v in properties and v != node
-                }
+                set(
+                    [
+                        v
+                        for v in MSVS_VARIABLE_REFERENCE.findall(value)
+                        if v in properties and v != node
+                    ]
+                )
             )
         return edges
 
     properties_ordered = gyp.common.TopologicallySorted(properties.keys(), GetEdges)
     # Walk properties in the reverse of a topological sort on
     # user_of_variable -> used_variable as this ensures variables are
     # defined before they are used.
@@ -3318,22 +3358,23 @@
         group = [
             "ItemDefinitionGroup",
             {"Condition": _GetConfigurationCondition(name, configuration, spec)},
         ]
         for tool_name, tool_settings in sorted(msbuild_settings.items()):
             # Skip the tool named '' which is a holder of global settings handled
             # by _GetMSBuildConfigurationGlobalProperties.
-            if tool_name and tool_settings:
-                tool = [tool_name]
-                for name, value in sorted(tool_settings.items()):
-                    formatted_value = _GetValueFormattedForMSBuild(
-                        tool_name, name, value
-                    )
-                    tool.append([name, formatted_value])
-                group.append(tool)
+            if tool_name:
+                if tool_settings:
+                    tool = [tool_name]
+                    for name, value in sorted(tool_settings.items()):
+                        formatted_value = _GetValueFormattedForMSBuild(
+                            tool_name, name, value
+                        )
+                        tool.append([name, formatted_value])
+                    group.append(tool)
         groups.append(group)
     return groups
 
 
 def _FinalizeMSBuildSettings(spec, configuration):
     if "msbuild_settings" in configuration:
         converted = False
@@ -3453,15 +3494,18 @@
         # For most tools, entries in a list should be separated with ';' but some
         # settings use a space.  Check for those first.
         exceptions = {
             "ClCompile": ["AdditionalOptions"],
             "Link": ["AdditionalOptions"],
             "Lib": ["AdditionalOptions"],
         }
-        char = " " if name in exceptions.get(tool_name, []) else ";"
+        if tool_name in exceptions and name in exceptions[tool_name]:
+            char = " "
+        else:
+            char = ";"
         formatted_value = char.join(
             [MSVSSettings.ConvertVCMacrosToMSBuild(i) for i in value]
         )
     else:
         formatted_value = MSVSSettings.ConvertVCMacrosToMSBuild(value)
     return formatted_value
 
@@ -3575,17 +3619,16 @@
                 for config_name, configuration in spec["configurations"].items():
                     precompiled_source = configuration.get(
                         "msvs_precompiled_source", ""
                     )
                     if precompiled_source != "":
                         precompiled_source = _FixPath(precompiled_source)
                         if not extensions_excluded_from_precompile:
-                            # If the precompiled header is generated by a C source,
-                            # we must not try to use it for C++ sources,
-                            # and vice versa.
+                            # If the precompiled header is generated by a C source, we must
+                            # not try to use it for C++ sources, and vice versa.
                             basename, extension = os.path.splitext(precompiled_source)
                             if extension == ".c":
                                 extensions_excluded_from_precompile = [
                                     ".cc",
                                     ".cpp",
                                     ".cxx",
                                 ]
@@ -3609,26 +3652,15 @@
                                 detail.append(["ForcedIncludeFiles", ""])
 
                 group, element = _MapFileToMsBuildSourceType(
                     source,
                     rule_dependencies,
                     extension_to_rule_name,
                     _GetUniquePlatforms(spec),
-                    spec["toolset"],
                 )
-                if group == "compile" and not os.path.isabs(source):
-                    # Add an <ObjectFileName> value to support duplicate source
-                    # file basenames, except for absolute paths to avoid paths
-                    # with more than 260 characters.
-                    file_name = os.path.splitext(source)[0] + ".obj"
-                    if file_name.startswith("..\\"):
-                        file_name = re.sub(r"^(\.\.\\)+", "", file_name)
-                    elif file_name.startswith("$("):
-                        file_name = re.sub(r"^\$\([^)]+\)\\", "", file_name)
-                    detail.append(["ObjectFileName", "$(IntDir)\\" + file_name])
                 grouped_sources[group].append([element, {"Include": source}] + detail)
 
 
 def _GetMSBuildProjectReferences(project):
     references = []
     if project.dependencies:
         group = ["ItemGroup"]
@@ -3668,29 +3700,27 @@
         references.append(group)
     return references
 
 
 def _GenerateMSBuildProject(project, options, version, generator_flags, spec):
     spec = project.spec
     configurations = spec["configurations"]
-    toolset = spec["toolset"]
     project_dir, project_file_name = os.path.split(project.path)
     gyp.common.EnsureDirExists(project.path)
     # Prepare list of sources and excluded sources.
 
     gyp_file = os.path.split(project.build_file)[1]
     sources, excluded_sources = _PrepareListOfSources(spec, generator_flags, gyp_file)
     # Add rules.
     actions_to_add = {}
     props_files_of_rules = set()
     targets_files_of_rules = set()
     rule_dependencies = set()
     extension_to_rule_name = {}
     list_excluded = generator_flags.get("msvs_list_excluded_files", True)
-    platforms = _GetUniquePlatforms(spec)
 
     # Don't generate rules if we are using an external builder like ninja.
     if not spec.get("msvs_external_builder"):
         _GenerateRulesForMSBuild(
             project_dir,
             options,
             spec,
@@ -3725,16 +3755,15 @@
     )
 
     _GenerateMSBuildFiltersFile(
         project.path + ".filters",
         sources,
         rule_dependencies,
         extension_to_rule_name,
-        platforms,
-        toolset,
+        _GetUniquePlatforms(spec),
     )
     missing_sources = _VerifySourcesExist(sources, project_dir)
 
     for configuration in configurations.values():
         _FinalizeMSBuildSettings(spec, configuration)
 
     # Add attributes to root element
@@ -3779,15 +3808,15 @@
     content += _GetMSBuildConfigurationDetails(spec, project.build_file)
     if spec.get("msvs_enable_winphone"):
         content += _GetMSBuildLocalProperties("v120_wp81")
     else:
         content += _GetMSBuildLocalProperties(project.msbuild_toolset)
     content += import_cpp_props_section
     content += import_masm_props_section
-    if "arm64" in platforms and toolset == "target":
+    if spec.get("msvs_enable_marmasm"):
         content += import_marmasm_props_section
     content += _GetMSBuildExtensions(props_files_of_rules)
     content += _GetMSBuildPropertySheets(configurations, spec)
     content += macro_section
     content += _GetMSBuildConfigurationGlobalProperties(
         spec, configurations, project.build_file
     )
@@ -3801,15 +3830,15 @@
         actions_spec,
         sources_handled_by_action,
         list_excluded,
     )
     content += _GetMSBuildProjectReferences(project)
     content += import_cpp_targets_section
     content += import_masm_targets_section
-    if "arm64" in platforms and toolset == "target":
+    if spec.get("msvs_enable_marmasm"):
         content += import_marmasm_targets_section
     content += _GetMSBuildExtensionTargets(targets_files_of_rules)
 
     if spec.get("msvs_external_builder"):
         content += _GetMSBuildExternalBuilderTargets(spec)
 
     # TODO(jeanluc) File a bug to get rid of runas.  We had in MSVS:
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/msvs_test.py` & `gyp-next-0.4.0/pylib/gyp/generator/msvs_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """ Unit tests for the msvs.py file. """
 
 import gyp.generator.msvs as msvs
 import unittest
 
-from io import StringIO
+try:
+    from StringIO import StringIO  # Python 2
+except ImportError:
+    from io import StringIO  # Python 3
 
 
 class TestSequenceFunctions(unittest.TestCase):
     def setUp(self):
         self.stderr = StringIO()
 
     def test_GetLibraries(self):
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/ninja.py` & `gyp-next-0.4.0/pylib/gyp/generator/ninja.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2013 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
+from __future__ import print_function
 
 import collections
 import copy
 import hashlib
 import json
 import multiprocessing
 import os.path
@@ -15,15 +16,18 @@
 import sys
 import gyp
 import gyp.common
 import gyp.msvs_emulation
 import gyp.MSVSUtil as MSVSUtil
 import gyp.xcode_emulation
 
-from io import StringIO
+try:
+    from cStringIO import StringIO
+except ImportError:
+    from io import StringIO
 
 from gyp.common import GetEnvironFallback
 import gyp.ninja_syntax as ninja_syntax
 
 generator_default_variables = {
     "EXECUTABLE_PREFIX": "",
     "EXECUTABLE_SUFFIX": "",
@@ -68,63 +72,63 @@
     if arg.startswith(prefix):
         return arg[len(prefix) :]
     return arg
 
 
 def QuoteShellArgument(arg, flavor):
     """Quote a string such that it will be interpreted as a single argument
-    by the shell."""
+  by the shell."""
     # Rather than attempting to enumerate the bad shell characters, just
     # allow common OK ones and quote anything else.
     if re.match(r"^[a-zA-Z0-9_=.\\/-]+$", arg):
         return arg  # No quoting necessary.
     if flavor == "win":
         return gyp.msvs_emulation.QuoteForRspFile(arg)
     return "'" + arg.replace("'", "'" + '"\'"' + "'") + "'"
 
 
 def Define(d, flavor):
     """Takes a preprocessor define and returns a -D parameter that's ninja- and
-    shell-escaped."""
+  shell-escaped."""
     if flavor == "win":
-        # cl.exe replaces literal # characters with = in preprocessor definitions for
+        # cl.exe replaces literal # characters with = in preprocesor definitions for
         # some reason. Octal-encode to work around that.
         d = d.replace("#", "\\%03o" % ord("#"))
     return QuoteShellArgument(ninja_syntax.escape("-D" + d), flavor)
 
 
 def AddArch(output, arch):
     """Adds an arch string to an output path."""
     output, extension = os.path.splitext(output)
-    return f"{output}.{arch}{extension}"
+    return "%s.%s%s" % (output, arch, extension)
 
 
-class Target:
+class Target(object):
     """Target represents the paths used within a single gyp target.
 
-    Conceptually, building a single target A is a series of steps:
+  Conceptually, building a single target A is a series of steps:
 
-    1) actions/rules/copies  generates source/resources/etc.
-    2) compiles              generates .o files
-    3) link                  generates a binary (library/executable)
-    4) bundle                merges the above in a mac bundle
-
-    (Any of these steps can be optional.)
-
-    From a build ordering perspective, a dependent target B could just
-    depend on the last output of this series of steps.
-
-    But some dependent commands sometimes need to reach inside the box.
-    For example, when linking B it needs to get the path to the static
-    library generated by A.
-
-    This object stores those paths.  To keep things simple, member
-    variables only store concrete paths to single files, while methods
-    compute derived values like "the last output of the target".
-    """
+  1) actions/rules/copies  generates source/resources/etc.
+  2) compiles              generates .o files
+  3) link                  generates a binary (library/executable)
+  4) bundle                merges the above in a mac bundle
+
+  (Any of these steps can be optional.)
+
+  From a build ordering perspective, a dependent target B could just
+  depend on the last output of this series of steps.
+
+  But some dependent commands sometimes need to reach inside the box.
+  For example, when linking B it needs to get the path to the static
+  library generated by A.
+
+  This object stores those paths.  To keep things simple, member
+  variables only store concrete paths to single files, while methods
+  compute derived values like "the last output of the target".
+  """
 
     def __init__(self, type):
         # Gyp type ("static_library", etc.) of this target.
         self.type = type
         # File representing whether any input dependencies necessary for
         # dependent actions have completed.
         self.preaction_stamp = None
@@ -155,37 +159,37 @@
 
     def Linkable(self):
         """Return true if this is a target that can be linked against."""
         return self.type in ("static_library", "shared_library")
 
     def UsesToc(self, flavor):
         """Return true if the target should produce a restat rule based on a TOC
-        file."""
+    file."""
         # For bundles, the .TOC should be produced for the binary, not for
         # FinalOutput(). But the naive approach would put the TOC file into the
         # bundle, so don't do this for bundles for now.
         if flavor == "win" or self.bundle:
             return False
         return self.type in ("shared_library", "loadable_module")
 
     def PreActionInput(self, flavor):
         """Return the path, if any, that should be used as a dependency of
-        any dependent action step."""
+    any dependent action step."""
         if self.UsesToc(flavor):
             return self.FinalOutput() + ".TOC"
         return self.FinalOutput() or self.preaction_stamp
 
     def PreCompileInput(self):
         """Return the path, if any, that should be used as a dependency of
-        any dependent compile step."""
+    any dependent compile step."""
         return self.actions_stamp or self.precompile_stamp
 
     def FinalOutput(self):
         """Return the last output of the target, which depends on all prior
-        steps."""
+    steps."""
         return self.bundle or self.binary or self.actions_stamp
 
 
 # A small discourse on paths as used within the Ninja build:
 # All files we produce (both at gyp and at build time) appear in the
 # build directory (e.g. out/Debug).
 #
@@ -206,33 +210,33 @@
 #   into the equivalent ninja path.
 #
 # - GypPathToUniqueOutput translates a gyp path into a ninja path to write
 #   an output file; the result can be namespaced such that it is unique
 #   to the input file name as well as the output target name.
 
 
-class NinjaWriter:
+class NinjaWriter(object):
     def __init__(
         self,
         hash_for_rules,
         target_outputs,
         base_dir,
         build_dir,
         output_file,
         toplevel_build,
         output_file_name,
         flavor,
         toplevel_dir=None,
     ):
         """
-        base_dir: path from source root to directory containing this gyp file,
-                  by gyp semantics, all input paths are relative to this
-        build_dir: path from source root to build output
-        toplevel_dir: path to the toplevel directory
-        """
+    base_dir: path from source root to directory containing this gyp file,
+              by gyp semantics, all input paths are relative to this
+    build_dir: path from source root to build output
+    toplevel_dir: path to the toplevel directory
+    """
 
         self.hash_for_rules = hash_for_rules
         self.target_outputs = target_outputs
         self.base_dir = base_dir
         self.build_dir = build_dir
         self.ninja = ninja_syntax.Writer(output_file)
         self.toplevel_build = toplevel_build
@@ -255,18 +259,18 @@
         # Relative path from base dir to build dir.
         base_to_top = gyp.common.InvertRelativePath(base_dir, toplevel_dir)
         self.base_to_build = os.path.join(base_to_top, build_dir)
 
     def ExpandSpecial(self, path, product_dir=None):
         """Expand specials like $!PRODUCT_DIR in |path|.
 
-        If |product_dir| is None, assumes the cwd is already the product
-        dir.  Otherwise, |product_dir| is the relative path to the product
-        dir.
-        """
+    If |product_dir| is None, assumes the cwd is already the product
+    dir.  Otherwise, |product_dir| is the relative path to the product
+    dir.
+    """
 
         PRODUCT_DIR = "$!PRODUCT_DIR"
         if PRODUCT_DIR in path:
             if product_dir:
                 path = path.replace(PRODUCT_DIR, product_dir)
             else:
                 path = path.replace(PRODUCT_DIR + "/", "")
@@ -295,17 +299,17 @@
         path = path.replace(generator_default_variables["RULE_INPUT_PATH"], source)
         path = path.replace(generator_default_variables["RULE_INPUT_EXT"], ext)
         path = path.replace(generator_default_variables["RULE_INPUT_NAME"], name)
         return path
 
     def GypPathToNinja(self, path, env=None):
         """Translate a gyp path to a ninja path, optionally expanding environment
-        variable references in |path| with |env|.
+    variable references in |path| with |env|.
 
-        See the above discourse on path conversions."""
+    See the above discourse on path conversions."""
         if env:
             if self.flavor == "mac":
                 path = gyp.xcode_emulation.ExpandEnvVars(path, env)
             elif self.flavor == "win":
                 path = gyp.msvs_emulation.ExpandMacros(path, env)
         if path.startswith("$!"):
             expanded = self.ExpandSpecial(path)
@@ -316,19 +320,19 @@
             path = self.ExpandSpecial(path)
         assert "$" not in path, path
         return os.path.normpath(os.path.join(self.build_to_base, path))
 
     def GypPathToUniqueOutput(self, path, qualified=True):
         """Translate a gyp path to a ninja path for writing output.
 
-        If qualified is True, qualify the resulting filename with the name
-        of the target.  This is necessary when e.g. compiling the same
-        path twice for two separate output targets.
+    If qualified is True, qualify the resulting filename with the name
+    of the target.  This is necessary when e.g. compiling the same
+    path twice for two separate output targets.
 
-        See the above discourse on path conversions."""
+    See the above discourse on path conversions."""
 
         path = self.ExpandSpecial(path)
         assert not path.startswith("$"), path
 
         # Translate the path following this scheme:
         #   Input: foo/bar.gyp, target targ, references baz/out.o
         #   Output: obj/foo/baz/targ.out.o (if qualified)
@@ -353,38 +357,38 @@
             path_basename = self.name + "." + path_basename
         return os.path.normpath(
             os.path.join(obj, self.base_dir, path_dir, path_basename)
         )
 
     def WriteCollapsedDependencies(self, name, targets, order_only=None):
         """Given a list of targets, return a path for a single file
-        representing the result of building all the targets or None.
+    representing the result of building all the targets or None.
 
-        Uses a stamp file if necessary."""
+    Uses a stamp file if necessary."""
 
         assert targets == [item for item in targets if item], targets
         if len(targets) == 0:
             assert not order_only
             return None
         if len(targets) > 1 or order_only:
             stamp = self.GypPathToUniqueOutput(name + ".stamp")
             targets = self.ninja.build(stamp, "stamp", targets, order_only=order_only)
             self.ninja.newline()
         return targets[0]
 
     def _SubninjaNameForArch(self, arch):
         output_file_base = os.path.splitext(self.output_file_name)[0]
-        return f"{output_file_base}.{arch}.ninja"
+        return "%s.%s.ninja" % (output_file_base, arch)
 
     def WriteSpec(self, spec, config_name, generator_flags):
         """The main entry point for NinjaWriter: write the build rules for a spec.
 
-        Returns a Target object, which represents the output paths for this spec.
-        Returns None if there are no outputs (e.g. a settings-only 'none' type
-        target)."""
+    Returns a Target object, which represents the output paths for this spec.
+    Returns None if there are no outputs (e.g. a settings-only 'none' type
+    target)."""
 
         self.config_name = config_name
         self.name = spec["target_name"]
         self.toolset = spec["toolset"]
         config = spec["configurations"][config_name]
         self.target = Target(spec["type"])
         self.is_standalone_static_library = bool(
@@ -410,25 +414,28 @@
             self.ninja.variable("cc_host", "$cl_" + arch)
             self.ninja.variable("cxx_host", "$cl_" + arch)
             self.ninja.variable("asm", "$ml_" + arch)
 
         if self.flavor == "mac":
             self.archs = self.xcode_settings.GetActiveArchs(config_name)
             if len(self.archs) > 1:
-                self.arch_subninjas = {
-                    arch: ninja_syntax.Writer(
-                        OpenOutput(
-                            os.path.join(
-                                self.toplevel_build, self._SubninjaNameForArch(arch)
-                            ),
-                            "w",
-                        )
+                self.arch_subninjas = dict(
+                    (
+                        arch,
+                        ninja_syntax.Writer(
+                            OpenOutput(
+                                os.path.join(
+                                    self.toplevel_build, self._SubninjaNameForArch(arch)
+                                ),
+                                "w",
+                            )
+                        ),
                     )
                     for arch in self.archs
-                }
+                )
 
         # Compute predepends for all rules.
         # actions_depends is the dependencies this target depends on before running
         # any of its action/rule/copy steps.
         # compile_depends is the dependencies this target depends on before running
         # any of its compile steps.
         actions_depends = []
@@ -547,15 +554,15 @@
             return None
 
         assert self.target.FinalOutput(), output
         return self.target
 
     def _WinIdlRule(self, source, prebuild, outputs):
         """Handle the implicit VS .idl rule for one source file. Fills |outputs|
-        with files that are generated."""
+    with files that are generated."""
         outdir, output, vars, flags = self.msvs_settings.GetIdlBuildData(
             source, self.config_name
         )
         outdir = self.GypPathToNinja(outdir)
 
         def fix_path(path, rel=None):
             path = os.path.join(outdir, path)
@@ -584,15 +591,15 @@
             self._WinIdlRule(source, prebuild, outputs)
         return outputs
 
     def WriteActionsRulesCopies(
         self, spec, extra_sources, prebuild, mac_bundle_depends
     ):
         """Write out the Actions, Rules, and Copies steps.  Return a path
-        representing the outputs of these steps."""
+    representing the outputs of these steps."""
         outputs = []
         if self.is_mac_bundle:
             mac_bundle_resources = spec.get("mac_bundle_resources", [])[:]
         else:
             mac_bundle_resources = []
         extra_mac_bundle_resources = []
 
@@ -627,49 +634,49 @@
             self.WriteMacInfoPlist(partial_info_plist, mac_bundle_depends)
 
         return stamp
 
     def GenerateDescription(self, verb, message, fallback):
         """Generate and return a description of a build step.
 
-        |verb| is the short summary, e.g. ACTION or RULE.
-        |message| is a hand-written description, or None if not available.
-        |fallback| is the gyp-level name of the step, usable as a fallback.
-        """
+    |verb| is the short summary, e.g. ACTION or RULE.
+    |message| is a hand-written description, or None if not available.
+    |fallback| is the gyp-level name of the step, usable as a fallback.
+    """
         if self.toolset != "target":
             verb += "(%s)" % self.toolset
         if message:
-            return f"{verb} {self.ExpandSpecial(message)}"
+            return "%s %s" % (verb, self.ExpandSpecial(message))
         else:
-            return f"{verb} {self.name}: {fallback}"
+            return "%s %s: %s" % (verb, self.name, fallback)
 
     def WriteActions(
         self, actions, extra_sources, prebuild, extra_mac_bundle_resources
     ):
         # Actions cd into the base directory.
         env = self.GetToolchainEnv()
         all_outputs = []
         for action in actions:
             # First write out a rule for the action.
-            name = "{}_{}".format(action["action_name"], self.hash_for_rules)
+            name = "%s_%s" % (action["action_name"], self.hash_for_rules)
             description = self.GenerateDescription(
                 "ACTION", action.get("message", None), name
             )
-            win_shell_flags = (
-                self.msvs_settings.GetRuleShellFlags(action)
+            is_cygwin = (
+                self.msvs_settings.IsRuleRunUnderCygwin(action)
                 if self.flavor == "win"
-                else None
+                else False
             )
             args = action["action"]
             depfile = action.get("depfile", None)
             if depfile:
                 depfile = self.ExpandSpecial(depfile, self.base_to_build)
             pool = "console" if int(action.get("ninja_use_console", 0)) else None
             rule_name, _ = self.WriteNewNinjaRule(
-                name, args, description, win_shell_flags, env, pool, depfile=depfile
+                name, args, description, is_cygwin, env, pool, depfile=depfile
             )
 
             inputs = [self.GypPathToNinja(i, env) for i in action["inputs"]]
             if int(action.get("process_outputs_as_sources", False)):
                 extra_sources += action["outputs"]
             if int(action.get("process_outputs_as_mac_bundle_resources", False)):
                 extra_mac_bundle_resources += action["outputs"]
@@ -695,49 +702,49 @@
         all_outputs = []
         for rule in rules:
             # Skip a rule with no action and no inputs.
             if "action" not in rule and not rule.get("rule_sources", []):
                 continue
 
             # First write out a rule for the rule action.
-            name = "{}_{}".format(rule["rule_name"], self.hash_for_rules)
+            name = "%s_%s" % (rule["rule_name"], self.hash_for_rules)
 
             args = rule["action"]
             description = self.GenerateDescription(
                 "RULE",
                 rule.get("message", None),
                 ("%s " + generator_default_variables["RULE_INPUT_PATH"]) % name,
             )
-            win_shell_flags = (
-                self.msvs_settings.GetRuleShellFlags(rule)
+            is_cygwin = (
+                self.msvs_settings.IsRuleRunUnderCygwin(rule)
                 if self.flavor == "win"
-                else None
+                else False
             )
             pool = "console" if int(rule.get("ninja_use_console", 0)) else None
             rule_name, args = self.WriteNewNinjaRule(
-                name, args, description, win_shell_flags, env, pool
+                name, args, description, is_cygwin, env, pool
             )
 
             # TODO: if the command references the outputs directly, we should
             # simplify it to just use $out.
 
             # Rules can potentially make use of some special variables which
             # must vary per source file.
             # Compute the list of variables we'll need to provide.
             special_locals = ("source", "root", "dirname", "ext", "name")
-            needed_variables = {"source"}
+            needed_variables = set(["source"])
             for argument in args:
                 for var in special_locals:
                     if "${%s}" % var in argument:
                         needed_variables.add(var)
             needed_variables = sorted(needed_variables)
 
             def cygwin_munge(path):
                 # pylint: disable=cell-var-from-loop
-                if win_shell_flags and win_shell_flags.cygwin:
+                if is_cygwin:
                     return path.replace("\\", "/")
                 return path
 
             inputs = [self.GypPathToNinja(i, env) for i in rule.get("inputs", [])]
 
             # If there are n source files matching the rule, and m additional rule
             # inputs, then adding 'inputs' to each build edge written below will
@@ -770,18 +777,17 @@
                     extra_sources += outputs
 
                 was_mac_bundle_resource = source in mac_bundle_resources
                 if was_mac_bundle_resource or int(
                     rule.get("process_outputs_as_mac_bundle_resources", False)
                 ):
                     extra_mac_bundle_resources += outputs
-                    # Note: This is n_resources * n_outputs_in_rule.
-                    # Put to-be-removed items in a set and
-                    # remove them all in a single pass
-                    # if this becomes a performance issue.
+                    # Note: This is n_resources * n_outputs_in_rule.  Put to-be-removed
+                    # items in a set and remove them all in a single pass if this becomes
+                    # a performance issue.
                     if was_mac_bundle_resource:
                         mac_bundle_resources.remove(source)
 
                 extra_bindings = []
                 for var in needed_variables:
                     if var == "root":
                         extra_bindings.append(("root", cygwin_munge(root)))
@@ -806,15 +812,15 @@
                     elif var == "name":
                         extra_bindings.append(("name", cygwin_munge(basename)))
                     else:
                         assert var is None, repr(var)
 
                 outputs = [self.GypPathToNinja(o, env) for o in outputs]
                 if self.flavor == "win":
-                    # WriteNewNinjaRule uses unique_name to create a rsp file on win.
+                    # WriteNewNinjaRule uses unique_name for creating an rsp file on win.
                     extra_bindings.append(
                         ("unique_name", hashlib.md5(outputs[0]).hexdigest())
                     )
 
                 self.ninja.build(
                     outputs,
                     rule_name,
@@ -843,20 +849,19 @@
                 src = self.GypPathToNinja(path, env)
                 dst = self.GypPathToNinja(
                     os.path.join(to_copy["destination"], basename), env
                 )
                 outputs += self.ninja.build(dst, "copy", src, order_only=prebuild)
                 if self.is_mac_bundle:
                     # gyp has mac_bundle_resources to copy things into a bundle's
-                    # Resources folder, but there's no built-in way to copy files
-                    # to other places in the bundle.
-                    # Hence, some targets use copies for this.
-                    # Check if this file is copied into the current bundle,
-                    # and if so add it to the bundle depends so
-                    # that dependent targets get rebuilt if the copy input changes.
+                    # Resources folder, but there's no built-in way to copy files to other
+                    # places in the bundle. Hence, some targets use copies for this. Check
+                    # if this file is copied into the current bundle, and if so add it to
+                    # the bundle depends so that dependent targets get rebuilt if the copy
+                    # input changes.
                     if dst.startswith(
                         self.xcode_settings.GetBundleContentsFolderPath()
                     ):
                         mac_bundle_depends.append(dst)
 
         return outputs
 
@@ -864,15 +869,15 @@
         """Prebuild steps to generate hmap files and copy headers to destination."""
         framework = self.ComputeMacBundleOutput()
         all_sources = spec["sources"]
         copy_headers = spec["mac_framework_headers"]
         output = self.GypPathToUniqueOutput("headers.hmap")
         self.xcode_settings.header_map_path = output
         all_headers = map(
-            self.GypPathToNinja, filter(lambda x: x.endswith(".h"), all_sources)
+            self.GypPathToNinja, filter(lambda x: x.endswith((".h")), all_sources)
         )
         variables = [
             ("framework", framework),
             ("copy_headers", map(self.GypPathToNinja, copy_headers)),
         ]
         outputs.extend(
             self.ninja.build(
@@ -914,19 +919,19 @@
             else:
                 xcassets.append(res)
         return xcassets
 
     def WriteMacXCassets(self, xcassets, bundle_depends):
         """Writes ninja edges for 'mac_bundle_resources' .xcassets files.
 
-        This add an invocation of 'actool' via the 'mac_tool.py' helper script.
-        It assumes that the assets catalogs define at least one imageset and
-        thus an Assets.car file will be generated in the application resources
-        directory. If this is not the case, then the build will probably be done
-        at each invocation of ninja."""
+    This add an invocation of 'actool' via the 'mac_tool.py' helper script.
+    It assumes that the assets catalogs define at least one imageset and
+    thus an Assets.car file will be generated in the application resources
+    directory. If this is not the case, then the build will probably be done
+    at each invocation of ninja."""
         if not xcassets:
             return
 
         extra_arguments = {}
         settings_to_arg = {
             "XCASSETS_APP_ICON": "app-icon",
             "XCASSETS_LAUNCH_IMAGE": "launch-image",
@@ -1036,27 +1041,30 @@
                 config,
                 sources,
                 predepends,
                 precompiled_header,
                 spec,
             )
         else:
-            return {
-                arch: self.WriteSourcesForArch(
-                    self.arch_subninjas[arch],
-                    config_name,
-                    config,
-                    sources,
-                    predepends,
-                    precompiled_header,
-                    spec,
-                    arch=arch,
+            return dict(
+                (
+                    arch,
+                    self.WriteSourcesForArch(
+                        self.arch_subninjas[arch],
+                        config_name,
+                        config,
+                        sources,
+                        predepends,
+                        precompiled_header,
+                        spec,
+                        arch=arch,
+                    ),
                 )
                 for arch in self.archs
-            }
+            )
 
     def WriteSourcesForArch(
         self,
         ninja_file,
         config_name,
         config,
         sources,
@@ -1217,15 +1225,15 @@
                 self.target.uses_cpp = True
             elif ext == "c" or (ext == "S" and self.flavor != "win"):
                 command = "cc"
             elif ext == "s" and self.flavor != "win":  # Doesn't generate .o.d files.
                 command = "cc_s"
             elif (
                 self.flavor == "win"
-                and ext in ("asm", "S")
+                and ext == "asm"
                 and not self.msvs_settings.HasExplicitAsmRules(spec)
             ):
                 command = "asm"
                 # Add the _asm suffix as msvs is capable of handling .cc and
                 # .asm files of the same name without collision.
                 obj_ext = "_asm.obj"
             elif self.flavor == "mac" and ext == "m":
@@ -1413,19 +1421,15 @@
         output = self.ComputeOutput(spec, arch)
         if arch is None and not self.is_mac_bundle:
             self.AppendPostbuildVariable(extra_bindings, spec, output, output)
 
         is_executable = spec["type"] == "executable"
         # The ldflags config key is not used on mac or win. On those platforms
         # linker flags are set via xcode_settings and msvs_settings, respectively.
-        if self.toolset == "target":
-            env_ldflags = os.environ.get("LDFLAGS", "").split()
-        elif self.toolset == "host":
-            env_ldflags = os.environ.get("LDFLAGS_host", "").split()
-
+        env_ldflags = os.environ.get("LDFLAGS", "").split()
         if self.flavor == "mac":
             ldflags = self.xcode_settings.GetLdflags(
                 config_name,
                 self.ExpandSpecial(generator_default_variables["PRODUCT_DIR"]),
                 self.GypPathToNinja,
                 arch,
             )
@@ -1505,16 +1509,16 @@
 
         if command in ("solink", "solink_module"):
             extra_bindings.append(("soname", os.path.split(output)[1]))
             extra_bindings.append(("lib", gyp.common.EncodePOSIXShellArgument(output)))
             if self.flavor != "win":
                 link_file_list = output
                 if self.is_mac_bundle:
-                    # 'Dependency Framework.framework/Versions/A/Dependency Framework'
-                    # -> 'Dependency Framework.framework.rsp'
+                    # 'Dependency Framework.framework/Versions/A/Dependency Framework' ->
+                    # 'Dependency Framework.framework.rsp'
                     link_file_list = self.xcode_settings.GetWrapperName()
                 if arch:
                     link_file_list += "." + arch
                 link_file_list += ".rsp"
                 # If an rspfile contains spaces, ninja surrounds the filename with
                 # quotes around it and then passes it to open(), creating a file with
                 # quotes in its name (and when looking for the rsp file, the name
@@ -1579,15 +1583,15 @@
             # TODO(evan): don't call this function for 'none' target types, as
             # it doesn't do anything, and we fake out a 'binary' with a stamp file.
             self.target.binary = compile_deps
             self.target.type = "none"
         elif spec["type"] == "static_library":
             self.target.binary = self.ComputeOutput(spec)
             if (
-                self.flavor not in ("ios", "mac", "netbsd", "openbsd", "win")
+                self.flavor not in ("mac", "openbsd", "netbsd", "win")
                 and not self.is_standalone_static_library
             ):
                 self.ninja.build(
                     self.target.binary, "alink_thin", link_deps, order_only=compile_deps
                 )
             else:
                 variables = []
@@ -1620,16 +1624,15 @@
                             output,
                             "alink",
                             link_deps[arch],
                             order_only=compile_deps,
                             variables=variables,
                         )
                         inputs.append(output)
-                    # TODO: It's not clear if
-                    # libtool_flags should be passed to the alink
+                    # TODO: It's not clear if libtool_flags should be passed to the alink
                     # call that combines single-arch .a files into a fat .a file.
                     self.AppendPostbuildVariable(
                         variables, spec, self.target.binary, self.target.binary
                     )
                     self.ninja.build(
                         self.target.binary,
                         "alink",
@@ -1719,16 +1722,16 @@
         """Adds a 'postbuild' variable if there is a postbuild for |output|."""
         postbuild = self.GetPostbuildCommand(spec, output, binary, is_command_start)
         if postbuild:
             variables.append(("postbuilds", postbuild))
 
     def GetPostbuildCommand(self, spec, output, output_binary, is_command_start):
         """Returns a shell command that runs all the postbuilds, and removes
-        |output| if any of them fails. If |is_command_start| is False, then the
-        returned string will start with ' && '."""
+    |output| if any of them fails. If |is_command_start| is False, then the
+    returned string will start with ' && '."""
         if not self.xcode_settings or spec["type"] == "none" or not output:
             return ""
         output = QuoteShellArgument(output, self.flavor)
         postbuilds = gyp.xcode_emulation.GetSpecPostbuildCommands(spec, quiet=True)
         if output_binary is not None:
             postbuilds = self.xcode_settings.AddImplicitPostbuilds(
                 self.config_name,
@@ -1766,16 +1769,16 @@
         if is_command_start:
             return "(" + command_string + " && "
         else:
             return "$ && (" + command_string
 
     def ComputeExportEnvString(self, env):
         """Given an environment, returns a string looking like
-            'export FOO=foo; export BAR="${FOO} bar;'
-        that exports |env| to the shell."""
+        'export FOO=foo; export BAR="${FOO} bar;'
+    that exports |env| to the shell."""
         export_str = []
         for k, v in env:
             export_str.append(
                 "export %s=%s;"
                 % (k, ninja_syntax.escape(gyp.common.EncodePOSIXShellArgument(v)))
             )
         return " ".join(export_str)
@@ -1811,15 +1814,18 @@
         DEFAULT_EXTENSION = {
             "loadable_module": default_variables["SHARED_LIB_SUFFIX"],
             "shared_library": default_variables["SHARED_LIB_SUFFIX"],
             "static_library": default_variables["STATIC_LIB_SUFFIX"],
             "executable": default_variables["EXECUTABLE_SUFFIX"],
         }
         extension = spec.get("product_extension")
-        extension = "." + extension if extension else DEFAULT_EXTENSION.get(type, "")
+        if extension:
+            extension = "." + extension
+        else:
+            extension = DEFAULT_EXTENSION.get(type, "")
 
         if "product_name" in spec:
             # If we were given an explicit name, use that.
             target = spec["product_name"]
         else:
             # Otherwise, derive a name from the target name.
             target = spec["target_name"]
@@ -1829,15 +1835,15 @@
 
         if type in (
             "static_library",
             "loadable_module",
             "shared_library",
             "executable",
         ):
-            return f"{prefix}{target}{extension}"
+            return "%s%s%s" % (prefix, target, extension)
         elif type == "none":
             return "%s.stamp" % target
         else:
             raise Exception("Unhandled output type %s" % type)
 
     def ComputeOutput(self, spec, arch=None):
         """Compute the path for the final output of the spec."""
@@ -1892,20 +1898,20 @@
     def WriteVariableList(self, ninja_file, var, values):
         assert not isinstance(values, str)
         if values is None:
             values = []
         ninja_file.variable(var, " ".join(values))
 
     def WriteNewNinjaRule(
-        self, name, args, description, win_shell_flags, env, pool, depfile=None
+        self, name, args, description, is_cygwin, env, pool, depfile=None
     ):
         """Write out a new ninja "rule" statement for a given command.
 
-        Returns the name of the new rule, and a copy of |args| with variables
-        expanded."""
+    Returns the name of the new rule, and a copy of |args| with variables
+    expanded."""
 
         if self.flavor == "win":
             args = [
                 self.msvs_settings.ConvertVSMacros(
                     arg, self.base_to_build, config=self.config_name
                 )
                 for arg in args
@@ -1939,22 +1945,21 @@
         # the arguments to point to the proper locations.
         rspfile = None
         rspfile_content = None
         args = [self.ExpandSpecial(arg, self.base_to_build) for arg in args]
         if self.flavor == "win":
             rspfile = rule_name + ".$unique_name.rsp"
             # The cygwin case handles this inside the bash sub-shell.
-            run_in = "" if win_shell_flags.cygwin else " " + self.build_to_base
-            if win_shell_flags.cygwin:
+            run_in = "" if is_cygwin else " " + self.build_to_base
+            if is_cygwin:
                 rspfile_content = self.msvs_settings.BuildCygwinBashCommandLine(
                     args, self.build_to_base
                 )
             else:
-                rspfile_content = gyp.msvs_emulation.EncodeRspFileList(
-                    args, win_shell_flags.quote)
+                rspfile_content = gyp.msvs_emulation.EncodeRspFileList(args)
             command = (
                 "%s gyp-win-tool action-wrapper $arch " % sys.executable
                 + rspfile
                 + run_in
             )
         else:
             env = self.ComputeExportEnvString(env)
@@ -2105,16 +2110,16 @@
             ]
 
         stat = MEMORYSTATUSEX()
         stat.dwLength = ctypes.sizeof(stat)
         ctypes.windll.kernel32.GlobalMemoryStatusEx(ctypes.byref(stat))
 
         # VS 2015 uses 20% more working set than VS 2013 and can consume all RAM
-        # on a 64 GiB machine.
-        mem_limit = max(1, stat.ullTotalPhys // (5 * (2 ** 30)))  # total / 5GiB
+        # on a 64 GB machine.
+        mem_limit = max(1, stat.ullTotalPhys // (5 * (2 ** 30)))  # total / 5GB
         hard_cap = max(1, int(os.environ.get("GYP_LINK_CONCURRENCY_MAX", 2 ** 32)))
         return min(mem_limit, hard_cap)
     elif sys.platform.startswith("linux"):
         if os.path.exists("/proc/meminfo"):
             with open("/proc/meminfo") as meminfo:
                 memtotal_re = re.compile(r"^MemTotal:\s*(\d*)\s*kB")
                 for line in meminfo:
@@ -2135,15 +2140,15 @@
     else:
         # TODO(scottmg): Implement this for other platforms.
         return 1
 
 
 def _GetWinLinkRuleNameSuffix(embed_manifest):
     """Returns the suffix used to select an appropriate linking rule depending on
-    whether the manifest embedding is enabled."""
+  whether the manifest embedding is enabled."""
     return "_embed" if embed_manifest else ""
 
 
 def _AddWinLinkRules(master_ninja, embed_manifest):
     """Adds link rules for Windows platform to |master_ninja|."""
 
     def FullLinkCommand(ldcmd, out, binary_type):
@@ -2383,14 +2388,15 @@
             "cc_host", CommandWithWrapper("CC.host", wrappers, cc_host)
         )
         master_ninja.variable(
             "cxx_host", CommandWithWrapper("CXX.host", wrappers, cxx_host)
         )
         if flavor == "win":
             master_ninja.variable("ld_host", ld_host)
+            master_ninja.variable("ldxx_host", ldxx_host)
         else:
             master_ninja.variable(
                 "ld_host", CommandWithWrapper("LINK", wrappers, ld_host)
             )
             master_ninja.variable(
                 "ldxx_host", CommandWithWrapper("LINK", wrappers, ldxx_host)
             )
@@ -2489,15 +2495,15 @@
             command=(
                 "%s gyp-win-tool asm-wrapper "
                 "$arch $asm $defines $includes $asmflags /c /Fo $out $in"
                 % sys.executable
             ),
         )
 
-    if flavor not in ("ios", "mac", "win"):
+    if flavor != "mac" and flavor != "win":
         master_ninja.rule(
             "alink",
             description="AR $out",
             command="rm -f $out && $ar rcs $arflags $out $in",
         )
         master_ninja.rule(
             "alink_thin",
@@ -2525,20 +2531,17 @@
             }
         )
 
         master_ninja.rule(
             "solink",
             description="SOLINK $lib",
             restat=True,
-            command=mtime_preserving_solink_base
-            % {"suffix": "@$link_file_list"},
+            command=mtime_preserving_solink_base % {"suffix": "@$link_file_list"},
             rspfile="$link_file_list",
-            rspfile_content=(
-                "-Wl,--whole-archive $in $solibs -Wl," "--no-whole-archive $libs"
-            ),
+            rspfile_content="-Wl,--whole-archive $in $solibs -Wl,--no-whole-archive $libs",
             pool="link_pool",
         )
         master_ninja.rule(
             "solink_module",
             description="SOLINK(module) $lib",
             restat=True,
             command=mtime_preserving_solink_base % {"suffix": "@$link_file_list"},
@@ -2787,16 +2790,16 @@
 
     for qualified_target in target_list:
         # qualified_target is like: third_party/icu/icu.gyp:icui18n#target
         build_file, name, toolset = gyp.common.ParseQualifiedTarget(qualified_target)
 
         this_make_global_settings = data[build_file].get("make_global_settings", [])
         assert make_global_settings == this_make_global_settings, (
-            "make_global_settings needs to be the same for all targets. "
-            f"{this_make_global_settings} vs. {make_global_settings}"
+            "make_global_settings needs to be the same for all targets. %s vs. %s"
+            % (this_make_global_settings, make_global_settings)
         )
 
         spec = target_dicts[qualified_target]
         if flavor == "mac":
             gyp.xcode_emulation.MergeGlobalXcodeSettingsToSpec(data[build_file], spec)
 
         # If build_file is a symlink, we must not follow it because there's a chance
@@ -2880,15 +2883,15 @@
 
 
 def PerformBuild(data, configurations, params):
     options = params["options"]
     for config in configurations:
         builddir = os.path.join(options.toplevel_dir, "out", config)
         arguments = ["ninja", "-C", builddir]
-        print(f"Building [{config}]: {arguments}")
+        print("Building [%s]: %s" % (config, arguments))
         subprocess.check_call(arguments)
 
 
 def CallGenerateOutputForConfig(arglist):
     # Ignore the interrupt signal so that the parent process catches it and
     # kills all multiprocessing children.
     signal.signal(signal.SIGINT, signal.SIG_IGN)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/ninja_test.py` & `gyp-next-0.4.0/pylib/gyp/generator/ninja_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """ Unit tests for the ninja.py file. """
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/xcode.py` & `gyp-next-0.4.0/pylib/gyp/generator/xcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
+from __future__ import print_function
 
 import filecmp
 import gyp.common
 import gyp.xcodeproj_file
 import gyp.xcode_ninja
 import errno
 import os
@@ -105,15 +106,15 @@
     for configuration_name in configuration_names:
         xcbc = gyp.xcodeproj_file.XCBuildConfiguration({"name": configuration_name})
         xccl.AppendProperty("buildConfigurations", xcbc)
     xccl.SetProperty("defaultConfigurationName", configuration_names[0])
     return xccl
 
 
-class XcodeProject:
+class XcodeProject(object):
     def __init__(self, gyp_path, path, build_file_dict):
         self.gyp_path = gyp_path
         self.path = path
         self.project = gyp.xcodeproj_file.PBXProject(path=path)
         projectDirPath = gyp.common.RelativePath(
             os.path.dirname(os.path.abspath(self.gyp_path)),
             os.path.dirname(path) or ".",
@@ -435,15 +436,15 @@
                         )
 
         # Update all references to other projects, to make sure that the lists of
         # remote products are complete.  Otherwise, Xcode will fill them in when
         # it opens the project file, which will result in unnecessary diffs.
         # TODO(mark): This is evil because it relies on internal knowledge of
         # PBXProject._other_pbxprojects.
-        for other_pbxproject in self.project._other_pbxprojects:
+        for other_pbxproject in self.project._other_pbxprojects.keys():
             self.project.AddOrGetProjectReference(other_pbxproject)
 
         self.project.SortRemoteProductReferences()
 
         # Give everything an ID.
         self.project_file.ComputeIDs()
 
@@ -589,15 +590,15 @@
 
 _xcode_define_re = re.compile(r"([\\\"\' ])")
 
 
 def EscapeXcodeDefine(s):
     """We must escape the defines that we give to XCode so that it knows not to
      split on spaces and to respect backslash and quote literals. However, we
-     must not quote the define, or Xcode will incorrectly interpret variables
+     must not quote the define, or Xcode will incorrectly intepret variables
      especially $(inherited)."""
     return re.sub(_xcode_define_re, r"\\\1", s)
 
 
 def PerformBuild(data, configurations, params):
     options = params["options"]
 
@@ -608,15 +609,15 @@
         xcodeproj_path = build_file_root + options.suffix + ".xcodeproj"
         if options.generator_output:
             xcodeproj_path = os.path.join(options.generator_output, xcodeproj_path)
 
     for config in configurations:
         arguments = ["xcodebuild", "-project", xcodeproj_path]
         arguments += ["-configuration", config]
-        print(f"Building [{config}]: {arguments}")
+        print("Building [%s]: %s" % (config, arguments))
         subprocess.check_call(arguments)
 
 
 def CalculateGeneratorInputInfo(params):
     toplevel = params["options"].toplevel_dir
     if params.get("flavor") == "ninja":
         generator_dir = os.path.relpath(params["options"].generator_output or ".")
@@ -730,16 +731,15 @@
             "mac_kernel_extension": "com.apple.product-type.kernel-extension",
             "executable+bundle": "com.apple.product-type.application",
             "loadable_module+bundle": "com.apple.product-type.bundle",
             "loadable_module+xctest": "com.apple.product-type.bundle.unit-test",
             "loadable_module+xcuitest": "com.apple.product-type.bundle.ui-testing",
             "shared_library+bundle": "com.apple.product-type.framework",
             "executable+extension+bundle": "com.apple.product-type.app-extension",
-            "executable+watch+extension+bundle":
-                "com.apple.product-type.watchkit-extension",
+            "executable+watch+extension+bundle": "com.apple.product-type.watchkit-extension",
             "executable+watch+bundle": "com.apple.product-type.application.watchapp",
             "mac_kernel_extension+bundle": "com.apple.product-type.kernel-extension",
         }
 
         target_properties = {
             "buildConfigurationList": xccl,
             "name": target_name,
@@ -1022,15 +1022,15 @@
                     "INPUT_FILE_DIRNAME": rule_source_dirname,
                 }
 
                 concrete_outputs_for_this_rule_source = []
                 for output in rule.get("outputs", []):
                     # Fortunately, Xcode and make both use $(VAR) format for their
                     # variables, so the expansion is the only transformation necessary.
-                    # Any remaining $(VAR)-type variables in the string can be given
+                    # Any remaning $(VAR)-type variables in the string can be given
                     # directly to make, which will pick up the correct settings from
                     # what Xcode puts into the environment.
                     concrete_output = ExpandXcodeVariables(output, rule_input_dict)
                     concrete_outputs_for_this_rule_source.append(concrete_output)
 
                     # Add all concrete outputs to the project.
                     pbxp.AddOrGetFileInRootGroup(concrete_output)
@@ -1067,15 +1067,15 @@
                 action = ExpandXcodeVariables(action_string, rule_input_dict)
                 actions.append(action)
 
             if len(concrete_outputs_all) > 0:
                 # TODO(mark): There's a possibility for collision here.  Consider
                 # target "t" rule "A_r" and target "t_A" rule "r".
                 makefile_name = "%s.make" % re.sub(
-                    "[^a-zA-Z0-9_]", "_", "{}_{}".format(target_name, rule["rule_name"])
+                    "[^a-zA-Z0-9_]", "_", "%s_%s" % (target_name, rule["rule_name"])
                 )
                 makefile_path = os.path.join(
                     xcode_projects[build_file].path, makefile_name
                 )
                 # TODO(mark): try/close?  Write to a temporary file and swap it only
                 # if it's got changes?
                 makefile = open(makefile_path, "w")
@@ -1097,15 +1097,15 @@
                     if (
                         concrete_output_index
                         == len(concrete_outputs_by_rule_source) - 1
                     ):
                         eol = ""
                     else:
                         eol = " \\"
-                    makefile.write(f"    {concrete_output}{eol}\n")
+                    makefile.write("    %s%s\n" % (concrete_output, eol))
 
                 for (rule_source, concrete_outputs, message, action) in zip(
                     rule["rule_sources"],
                     concrete_outputs_by_rule_source,
                     messages,
                     actions,
                 ):
@@ -1114,16 +1114,19 @@
                     # Add a rule that declares it can build each concrete output of a
                     # rule source.  Collect the names of the directories that are
                     # required.
                     concrete_output_dirs = []
                     for concrete_output_index, concrete_output in enumerate(
                         concrete_outputs
                     ):
-                        bol = "" if concrete_output_index == 0 else "    "
-                        makefile.write(f"{bol}{concrete_output} \\\n")
+                        if concrete_output_index == 0:
+                            bol = ""
+                        else:
+                            bol = "    "
+                        makefile.write("%s%s \\\n" % (bol, concrete_output))
 
                         concrete_output_dir = posixpath.dirname(concrete_output)
                         if (
                             concrete_output_dir
                             and concrete_output_dir not in concrete_output_dirs
                         ):
                             concrete_output_dirs.append(concrete_output_dir)
@@ -1135,25 +1138,25 @@
                     prerequisites = [rule_source]
                     prerequisites.extend(rule.get("inputs", []))
                     for prerequisite_index, prerequisite in enumerate(prerequisites):
                         if prerequisite_index == len(prerequisites) - 1:
                             eol = ""
                         else:
                             eol = " \\"
-                        makefile.write(f"    {prerequisite}{eol}\n")
+                        makefile.write("    %s%s\n" % (prerequisite, eol))
 
                     # Make sure that output directories exist before executing the rule
                     # action.
                     if len(concrete_output_dirs) > 0:
                         makefile.write(
                             '\t@mkdir -p "%s"\n' % '" "'.join(concrete_output_dirs)
                         )
 
-                    # The rule message and action have already had
-                    # the necessary variable substitutions performed.
+                    # The rule message and action have already had the necessary variable
+                    # substitutions performed.
                     if message:
                         # Mark it with note: so Xcode picks it up in build output.
                         makefile.write("\t@echo note: %s\n" % message)
                     makefile.write("\t%s\n" % action)
 
                 makefile.close()
 
@@ -1197,16 +1200,16 @@
                     }
                 )
 
                 if support_xct:
                     support_xct.AppendProperty("buildPhases", ssbp)
                 else:
                     # TODO(mark): this assumes too much knowledge of the internals of
-                    # xcodeproj_file; some of these smarts should move
-                    # into xcodeproj_file itself.
+                    # xcodeproj_file; some of these smarts should move into xcodeproj_file
+                    # itself.
                     xct._properties["buildPhases"].insert(prebuild_index, ssbp)
                     prebuild_index = prebuild_index + 1
 
             # Extra rule inputs also go into the project file.  Concrete outputs were
             # already added when they were computed.
             groups = ["inputs", "inputs_excluded"]
             if skip_excluded_files:
```

### Comparing `gyp-next-0.15.0/pylib/gyp/generator/xcode_test.py` & `gyp-next-0.4.0/pylib/gyp/generator/xcode_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # Copyright (c) 2013 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """ Unit tests for the xcode.py file. """
```

### Comparing `gyp-next-0.15.0/pylib/gyp/input.py` & `gyp-next-0.4.0/pylib/gyp/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
+from __future__ import print_function
 
 import ast
 
 import gyp.common
 import gyp.simple_copy
 import multiprocessing
 import os.path
@@ -16,14 +17,16 @@
 import sys
 import threading
 import traceback
 from distutils.version import StrictVersion
 from gyp.common import GypError
 from gyp.common import OrderedSet
 
+PY3 = bytes != str
+
 # A list of types that are treated as linkable.
 linkable_types = [
     "executable",
     "shared_library",
     "loadable_module",
     "mac_kernel_extension",
     "windows_driver",
@@ -59,15 +62,15 @@
     # because there's no way for a regular expression to be treated as a path.
     while section and section[-1:] in "=+?!":
         section = section[:-1]
 
     if section in path_sections:
         return True
 
-    # Sections matching the regexp '_(dir|file|path)s?$' are also
+    # Sections mathing the regexp '_(dir|file|path)s?$' are also
     # considered PathSections. Using manual string matching since that
     # is much faster than the regexp and this can be called hundreds of
     # thousands of times so micro performance matters.
     if "_" in section:
         tail = section[-6:]
         if tail[-1] == "s":
             tail = tail[:-1]
@@ -221,17 +224,25 @@
 
 
 def LoadOneBuildFile(build_file_path, data, aux_data, includes, is_target, check):
     if build_file_path in data:
         return data[build_file_path]
 
     if os.path.exists(build_file_path):
-        build_file_contents = open(build_file_path, encoding="utf-8").read()
+        # Open the build file for read ('r') with universal-newlines mode ('U')
+        # to make sure platform specific newlines ('\r\n' or '\r') are converted to '\n'
+        # which otherwise will fail eval()
+        if sys.platform == "zos":
+            # On z/OS, universal-newlines mode treats the file as an ascii file. But since
+            # node-gyp produces ebcdic files, do not use that mode.
+            build_file_contents = open(build_file_path, "r").read()
+        else:
+            build_file_contents = open(build_file_path, "rU").read()
     else:
-        raise GypError(f"{build_file_path} not found (cwd: {os.getcwd()})")
+        raise GypError("%s not found (cwd: %s)" % (build_file_path, os.getcwd()))
 
     build_file_data = None
     try:
         if check:
             build_file_data = CheckedEval(build_file_contents)
         else:
             build_file_data = eval(build_file_contents, {"__builtins__": {}}, None)
@@ -552,15 +563,15 @@
         return None
 
 
 class ParallelProcessingError(Exception):
     pass
 
 
-class ParallelState:
+class ParallelState(object):
     """Class to keep track of state when processing input files in parallel.
 
   If build files are loaded in parallel, use this to keep track of
   state during farming out and processing parallel jobs. It's stored
   in a global so that the callback function can have access to it.
   """
 
@@ -866,15 +877,18 @@
                 build_file_dir = None
 
         # Support <|(listfile.txt ...) which generates a file
         # containing items from a gyp list, generated at gyp time.
         # This works around actions/rules which have more inputs than will
         # fit on the command line.
         if file_list:
-            contents_list = contents if type(contents) is list else contents.split(" ")
+            if type(contents) is list:
+                contents_list = contents
+            else:
+                contents_list = contents.split(" ")
             replacement = contents_list[0]
             if os.path.isabs(replacement):
                 raise GypError('| cannot handle absolute paths, got "%s"' % replacement)
 
             if not generator_filelist_paths:
                 path = os.path.join(build_file_dir, replacement)
             else:
@@ -954,34 +968,42 @@
                         "Unknown command string '%s' in '%s'."
                         % (command_string, contents)
                     )
                 else:
                     # Fix up command with platform specific workarounds.
                     contents = FixupPlatformCommand(contents)
                     try:
-                        # stderr will be printed no matter what
-                        result = subprocess.run(
+                        p = subprocess.Popen(
                             contents,
-                            stdout=subprocess.PIPE,
                             shell=use_shell,
+                            stdout=subprocess.PIPE,
+                            stderr=subprocess.PIPE,
+                            stdin=subprocess.PIPE,
                             cwd=build_file_dir,
-                            check=False
                         )
                     except Exception as e:
                         raise GypError(
                             "%s while executing command '%s' in %s"
                             % (e, contents, build_file)
                         )
 
-                    if result.returncode > 0:
+                    p_stdout, p_stderr = p.communicate("")
+                    if PY3:
+                        p_stdout = p_stdout.decode("utf-8")
+                        p_stderr = p_stderr.decode("utf-8")
+
+                    if p.wait() != 0 or p_stderr:
+                        sys.stderr.write(p_stderr)
+                        # Simulate check_call behavior, since check_call only exists
+                        # in python 2.5 and later.
                         raise GypError(
                             "Call to '%s' returned exit status %d while in %s."
-                            % (contents, result.returncode, build_file)
+                            % (contents, p.returncode, build_file)
                         )
-                    replacement = result.stdout.decode("utf-8").rstrip()
+                    replacement = p_stdout.rstrip()
 
                 cached_command_results[cache_key] = replacement
             else:
                 gyp.DebugOutput(
                     gyp.DEBUG_VARIABLES,
                     "Had cache value for command '%s' in directory '%s'",
                     contents,
@@ -1193,15 +1215,15 @@
             e.offset,
             e.text,
         )
         raise syntax_error
     except NameError as e:
         gyp.common.ExceptionAppend(
             e,
-            f"while evaluating condition '{cond_expr_expanded}' in {build_file}",
+            "while evaluating condition '%s' in %s" % (cond_expr_expanded, build_file),
         )
         raise GypError(e)
 
 
 def ProcessConditionsInDict(the_dict, phase, variables, build_file):
     # Process a 'conditions' or 'target_conditions' section in the_dict,
     # depending on phase.
@@ -1623,22 +1645,23 @@
     """Remove self dependencies from targets that have the prune_self_dependency
   variable set."""
     for target_name, target_dict in targets.items():
         for dependency_key in dependency_sections:
             dependencies = target_dict.get(dependency_key, [])
             if dependencies:
                 for t in dependencies:
-                    if t == target_name and (
-                        targets[t]
-                        .get("variables", {})
-                        .get("prune_self_dependency", 0)
-                    ):
-                        target_dict[dependency_key] = Filter(
-                            dependencies, target_name
-                        )
+                    if t == target_name:
+                        if (
+                            targets[t]
+                            .get("variables", {})
+                            .get("prune_self_dependency", 0)
+                        ):
+                            target_dict[dependency_key] = Filter(
+                                dependencies, target_name
+                            )
 
 
 def RemoveLinkDependenciesFromNoneTargets(targets):
     """Remove dependencies having the 'link_dependency' attribute from the 'none'
   targets."""
     for target_name, target_dict in targets.items():
         for dependency_key in dependency_sections:
@@ -1648,15 +1671,15 @@
                     if target_dict.get("type", None) == "none":
                         if targets[t].get("variables", {}).get("link_dependency", 0):
                             target_dict[dependency_key] = Filter(
                                 target_dict[dependency_key], t
                             )
 
 
-class DependencyGraphNode:
+class DependencyGraphNode(object):
     """
 
   Attributes:
     ref: A reference to an object that this DependencyGraphNode represents.
     dependencies: List of DependencyGraphNodes on which this one depends.
     dependents: List of DependencyGraphNodes that depend on this one.
   """
@@ -1704,18 +1727,18 @@
                 # TODO: We want to check through the
                 # node_dependent.dependencies list but if it's long and we
                 # always start at the beginning, then we get O(n^2) behaviour.
                 for node_dependent_dependency in sorted(
                     node_dependent.dependencies, key=ExtractNodeRef
                 ):
                     if node_dependent_dependency.ref not in flat_list:
-                        # The dependent one or more dependencies not in flat_list.
-                        # There will be more chances to add it to flat_list
-                        # when examining it again as a dependent of those other
-                        # dependencies, provided that there are no cycles.
+                        # The dependent one or more dependencies not in flat_list.  There
+                        # will be more chances to add it to flat_list when examining
+                        # it again as a dependent of those other dependencies, provided
+                        # that there are no cycles.
                         is_in_degree_zero = False
                         break
 
                 if is_in_degree_zero:
                     # All of the dependent's dependencies are already in flat_list.  Add
                     # it to in_degree_zeros where it will be processed in a future
                     # iteration of the outer loop.
@@ -2225,20 +2248,23 @@
             return x in s
         return x in items
 
     prepend_index = 0
 
     # Make membership testing of hashables in |to| (in particular, strings)
     # faster.
-    hashable_to_set = {x for x in to if is_hashable(x)}
+    hashable_to_set = set(x for x in to if is_hashable(x))
     for item in fro:
         singleton = False
         if type(item) in (str, int):
             # The cheap and easy case.
-            to_item = MakePathRelative(to_file, fro_file, item) if is_paths else item
+            if is_paths:
+                to_item = MakePathRelative(to_file, fro_file, item)
+            else:
+                to_item = item
 
             if not (type(item) is str and item.startswith("-")):
                 # Any string that doesn't begin with a "-" is a singleton - it can
                 # only appear once in a list, to be enforced by the list merge append
                 # or prepend.
                 singleton = True
         elif type(item) is dict:
@@ -2397,15 +2423,15 @@
                 + k
             )
 
 
 def MergeConfigWithInheritance(
     new_configuration_dict, build_file, target_dict, configuration, visited
 ):
-    # Skip if previously visited.
+    # Skip if previously visted.
     if configuration in visited:
         return
 
     # Look at this configuration.
     configuration_dict = target_dict["configurations"][configuration]
 
     # Merge in parents.
@@ -2456,27 +2482,30 @@
             continue
         # Configurations inherit (most) settings from the enclosing target scope.
         # Get the inheritance relationship right by making a copy of the target
         # dict.
         new_configuration_dict = {}
         for (key, target_val) in target_dict.items():
             key_ext = key[-1:]
-            key_base = key[:-1] if key_ext in key_suffixes else key
+            if key_ext in key_suffixes:
+                key_base = key[:-1]
+            else:
+                key_base = key
             if key_base not in non_configuration_keys:
                 new_configuration_dict[key] = gyp.simple_copy.deepcopy(target_val)
 
         # Merge in configuration (with all its parents first).
         MergeConfigWithInheritance(
             new_configuration_dict, build_file, target_dict, configuration, []
         )
 
         merged_configurations[configuration] = new_configuration_dict
 
     # Put the new configurations back into the target dict as a configuration.
-    for configuration in merged_configurations:
+    for configuration in merged_configurations.keys():
         target_dict["configurations"][configuration] = merged_configurations[
             configuration
         ]
 
     # Now drop all the abstract ones.
     configs = target_dict["configurations"]
     target_dict["configurations"] = {
@@ -2485,24 +2514,27 @@
 
     # Now that all of the target's configurations have been built, go through
     # the target dict's keys and remove everything that's been moved into a
     # "configurations" section.
     delete_keys = []
     for key in target_dict:
         key_ext = key[-1:]
-        key_base = key[:-1] if key_ext in key_suffixes else key
+        if key_ext in key_suffixes:
+            key_base = key[:-1]
+        else:
+            key_base = key
         if key_base not in non_configuration_keys:
             delete_keys.append(key)
     for key in delete_keys:
         del target_dict[key]
 
     # Check the configurations to see if they contain invalid keys.
-    for configuration in target_dict["configurations"]:
+    for configuration in target_dict["configurations"].keys():
         configuration_dict = target_dict["configurations"][configuration]
-        for key in configuration_dict:
+        for key in configuration_dict.keys():
             if key in invalid_configuration_keys:
                 raise GypError(
                     "%s not allowed in the %s configuration, found in "
                     "target %s" % (key, configuration, target)
                 )
 
 
@@ -2605,34 +2637,34 @@
         regex_key = list_key + "/"
         if regex_key in the_dict:
             for regex_item in the_dict[regex_key]:
                 [action, pattern] = regex_item
                 pattern_re = re.compile(pattern)
 
                 if action == "exclude":
-                    # This item matches an exclude regex, set its value to 0 (exclude).
+                    # This item matches an exclude regex, so set its value to 0 (exclude).
                     action_value = 0
                 elif action == "include":
-                    # This item matches an include regex, set its value to 1 (include).
+                    # This item matches an include regex, so set its value to 1 (include).
                     action_value = 1
                 else:
                     # This is an action that doesn't make any sense.
                     raise ValueError(
                         "Unrecognized action "
                         + action
                         + " in "
                         + name
                         + " key "
                         + regex_key
                     )
 
                 for index, list_item in enumerate(the_list):
                     if list_actions[index] == action_value:
-                        # Even if the regex matches, nothing will change so continue
-                        # (regex searches are expensive).
+                        # Even if the regex matches, nothing will change so continue (regex
+                        # searches are expensive).
                         continue
                     if pattern_re.search(list_item):
                         # Regular expression match.
                         list_actions[index] = action_value
 
             # The "whatever/" list is no longer needed, dump it.
             del the_dict[regex_key]
@@ -2714,14 +2746,44 @@
     ):
         raise GypError(
             "Target %s has type %s but standalone_static_library flag is"
             " only valid for static_library type." % (target, target_type)
         )
 
 
+def ValidateSourcesInTarget(target, target_dict, build_file, duplicate_basename_check):
+    if not duplicate_basename_check:
+        return
+    if target_dict.get("type", None) != "static_library":
+        return
+    sources = target_dict.get("sources", [])
+    basenames = {}
+    for source in sources:
+        name, ext = os.path.splitext(source)
+        is_compiled_file = ext in [".c", ".cc", ".cpp", ".cxx", ".m", ".mm", ".s", ".S"]
+        if not is_compiled_file:
+            continue
+        basename = os.path.basename(name)  # Don't include extension.
+        basenames.setdefault(basename, []).append(source)
+
+    error = ""
+    for basename, files in basenames.items():
+        if len(files) > 1:
+            error += "  %s: %s\n" % (basename, " ".join(files))
+
+    if error:
+        print(
+            "static library %s has several files with the same basename:\n" % target
+            + error
+            + "libtool on Mac cannot handle that. Use "
+            "--no-duplicate-basename-check to disable this validation."
+        )
+        raise GypError("Duplicate basenames in sources section, see list above")
+
+
 def ValidateRulesInTarget(target, target_dict, extra_sources_for_rules):
     """Ensures that the rules sections in target_dict are valid and consistent,
   and determines which sources they apply to.
 
   Arguments:
     target: string, name of target.
     target_dict: dict, target spec containing "rules" and "sources" lists.
@@ -2736,15 +2798,15 @@
 
     rules = target_dict.get("rules", [])
     for rule in rules:
         # Make sure that there's no conflict among rule names and extensions.
         rule_name = rule["rule_name"]
         if rule_name in rule_names:
             raise GypError(
-                f"rule {rule_name} exists in duplicate, target {target}"
+                "rule %s exists in duplicate, target %s" % (rule_name, target)
             )
         rule_names[rule_name] = rule
 
         rule_extension = rule["extension"]
         if rule_extension.startswith("."):
             rule_extension = rule_extension[1:]
         if rule_extension in rule_extensions:
@@ -2955,14 +3017,15 @@
     build_files,
     variables,
     includes,
     depth,
     generator_input_info,
     check,
     circular_check,
+    duplicate_basename_check,
     parallel,
     root_targets,
 ):
     SetGeneratorGlobals(generator_input_info)
     # A generator can have other lists (in addition to sources) be processed
     # for rules.
     extra_sources_for_rules = generator_input_info["extra_sources_for_rules"]
@@ -3100,14 +3163,17 @@
     # needed.  Not all generators will need to use the rule_sources lists, but
     # some may, and it seems best to build the list in a common spot.
     # Also validate actions and run_as elements in targets.
     for target in flat_list:
         target_dict = targets[target]
         build_file = gyp.common.BuildFile(target)
         ValidateTargetType(target, target_dict)
+        ValidateSourcesInTarget(
+            target, target_dict, build_file, duplicate_basename_check
+        )
         ValidateRulesInTarget(target, target_dict, extra_sources_for_rules)
         ValidateRunAsInTarget(target, target_dict, build_file)
         ValidateActionsInTarget(target, target_dict, build_file)
 
     # Generators might not expect ints.  Turn them into strs.
     TurnIntIntoStrInDict(data)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/input_test.py` & `gyp-next-0.4.0/pylib/gyp/input_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # Copyright 2013 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """Unit tests for the input.py file."""
```

### Comparing `gyp-next-0.15.0/pylib/gyp/mac_tool.py` & `gyp-next-0.4.0/pylib/gyp/mac_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """Utility functions to perform Xcode-style build steps.
 
 These functions are executed via gyp-mac-tool when using the Makefile generator.
 """
 
+from __future__ import print_function
 
 import fcntl
 import fnmatch
 import glob
 import json
 import os
 import plistlib
 import re
 import shutil
 import struct
 import subprocess
 import sys
 import tempfile
 
+PY3 = bytes != str
+
 
 def main(args):
     executor = MacTool()
     exit_code = executor.Dispatch(args)
     if exit_code is not None:
         sys.exit(exit_code)
 
 
-class MacTool:
+class MacTool(object):
     """This class performs all the Mac tooling steps. The methods can either be
   executed directly, or dispatched from an argument list."""
 
     def Dispatch(self, args):
         """Dispatches a string command to a method."""
         if len(args) < 1:
             raise Exception("Not enough arguments")
@@ -172,15 +175,15 @@
             return "UTF-8"
         else:
             return None
 
     def ExecCopyInfoPlist(self, source, dest, convert_to_binary, *keys):
         """Copies the |source| Info.plist to the destination directory |dest|."""
         # Read the source Info.plist into memory.
-        with open(source) as fd:
+        with open(source, "r") as fd:
             lines = fd.read()
 
         # Insert synthesized key/value pairs (e.g. BuildMachineOSBuild).
         plist = plistlib.readPlistFromString(lines)
         if keys:
             plist.update(json.loads(keys[0]))
         lines = plistlib.writePlistToString(plist)
@@ -244,15 +247,15 @@
         # '?' characters are used instead.
         signature_code = plist.get("CFBundleSignature", "????")
         if len(signature_code) != 4:  # Wrong length resets everything, too.
             signature_code = "?" * 4
 
         dest = os.path.join(os.path.dirname(info_plist), "PkgInfo")
         with open(dest, "w") as fp:
-            fp.write(f"{package_type}{signature_code}")
+            fp.write("%s%s" % (package_type, signature_code))
 
     def ExecFlock(self, lockfile, *cmd_list):
         """Emulates the most basic behavior of Linux's flock(1)."""
         # Rely on exception handling to report errors.
         fd = os.open(lockfile, os.O_RDONLY | os.O_NOCTTY | os.O_CREAT, 0o666)
         fcntl.flock(fd, fcntl.LOCK_EX)
         return subprocess.call(cmd_list)
@@ -271,15 +274,17 @@
         env = os.environ.copy()
         # Ref:
         # http://www.opensource.apple.com/source/cctools/cctools-809/misc/libtool.c
         # The problem with this flag is that it resets the file mtime on the file to
         # epoch=0, e.g. 1970-1-1 or 1969-12-31 depending on timezone.
         env["ZERO_AR_DATE"] = "1"
         libtoolout = subprocess.Popen(cmd_list, stderr=subprocess.PIPE, env=env)
-        err = libtoolout.communicate()[1].decode("utf-8")
+        _, err = libtoolout.communicate()
+        if PY3:
+            err = err.decode("utf-8")
         for line in err.splitlines():
             if not libtool_re.match(line) and not libtool_re5.match(line):
                 print(line, file=sys.stderr)
         # Unconditionally touch the output .a file on the command line if present
         # and the command succeeded. A bit hacky.
         if not libtoolout.returncode:
             for i in range(len(cmd_list) - 1):
@@ -531,15 +536,15 @@
         valid_provisioning_profiles = {}
         for profile_path in provisioning_profiles:
             profile_data = self._LoadProvisioningProfile(profile_path)
             app_id_pattern = profile_data.get("Entitlements", {}).get(
                 "application-identifier", ""
             )
             for team_identifier in profile_data.get("TeamIdentifier", []):
-                app_id = f"{team_identifier}.{bundle_identifier}"
+                app_id = "%s.%s" % (team_identifier, bundle_identifier)
                 if fnmatch.fnmatch(app_id, app_id_pattern):
                     valid_provisioning_profiles[app_id_pattern] = (
                         profile_path,
                         profile_data,
                         team_identifier,
                     )
         if not valid_provisioning_profiles:
```

### Comparing `gyp-next-0.15.0/pylib/gyp/msvs_emulation.py` & `gyp-next-0.4.0/pylib/gyp/msvs_emulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,158 +3,154 @@
 # found in the LICENSE file.
 
 """
 This module helps emulate Visual Studio 2008 behavior on top of other
 build systems, primarily ninja.
 """
 
-import collections
 import os
 import re
 import subprocess
 import sys
 
 from gyp.common import OrderedSet
 import gyp.MSVSUtil
 import gyp.MSVSVersion
 
+PY3 = bytes != str
+
 windows_quoter_regex = re.compile(r'(\\*)"')
 
 
-def QuoteForRspFile(arg, quote_cmd=True):
+def QuoteForRspFile(arg):
     """Quote a command line argument so that it appears as one argument when
-    processed via cmd.exe and parsed by CommandLineToArgvW (as is typical for
-    Windows programs)."""
+  processed via cmd.exe and parsed by CommandLineToArgvW (as is typical for
+  Windows programs)."""
     # See http://goo.gl/cuFbX and http://goo.gl/dhPnp including the comment
     # threads. This is actually the quoting rules for CommandLineToArgvW, not
     # for the shell, because the shell doesn't do anything in Windows. This
     # works more or less because most programs (including the compiler, etc.)
     # use that function to handle command line arguments.
 
     # Use a heuristic to try to find args that are paths, and normalize them
     if arg.find("/") > 0 or arg.count("/") > 1:
         arg = os.path.normpath(arg)
 
     # For a literal quote, CommandLineToArgvW requires 2n+1 backslashes
     # preceding it, and results in n backslashes + the quote. So we substitute
     # in 2* what we match, +1 more, plus the quote.
-    if quote_cmd:
-        arg = windows_quoter_regex.sub(lambda mo: 2 * mo.group(1) + '\\"', arg)
+    arg = windows_quoter_regex.sub(lambda mo: 2 * mo.group(1) + '\\"', arg)
 
     # %'s also need to be doubled otherwise they're interpreted as batch
     # positional arguments. Also make sure to escape the % so that they're
     # passed literally through escaping so they can be singled to just the
     # original %. Otherwise, trying to pass the literal representation that
     # looks like an environment variable to the shell (e.g. %PATH%) would fail.
     arg = arg.replace("%", "%%")
 
     # These commands are used in rsp files, so no escaping for the shell (via ^)
     # is necessary.
 
-    # As a workaround for programs that don't use CommandLineToArgvW, gyp
-    # supports msvs_quote_cmd=0, which simply disables all quoting.
-    if quote_cmd:
-        # Finally, wrap the whole thing in quotes so that the above quote rule
-        # applies and whitespace isn't a word break.
-        return f'"{arg}"'
-
-    return arg
+    # Finally, wrap the whole thing in quotes so that the above quote rule
+    # applies and whitespace isn't a word break.
+    return '"' + arg + '"'
 
 
-def EncodeRspFileList(args, quote_cmd):
+def EncodeRspFileList(args):
     """Process a list of arguments using QuoteCmdExeArgument."""
     # Note that the first argument is assumed to be the command. Don't add
     # quotes around it because then built-ins like 'echo', etc. won't work.
     # Take care to normpath only the path in the case of 'call ../x.bat' because
     # otherwise the whole thing is incorrectly interpreted as a path and not
     # normalized correctly.
     if not args:
         return ""
     if args[0].startswith("call "):
         call, program = args[0].split(" ", 1)
         program = call + " " + os.path.normpath(program)
     else:
         program = os.path.normpath(args[0])
-    return (program + " "
-            + " ".join(QuoteForRspFile(arg, quote_cmd) for arg in args[1:]))
+    return program + " " + " ".join(QuoteForRspFile(arg) for arg in args[1:])
 
 
 def _GenericRetrieve(root, default, path):
     """Given a list of dictionary keys |path| and a tree of dicts |root|, find
-    value at path, or return |default| if any of the path doesn't exist."""
+  value at path, or return |default| if any of the path doesn't exist."""
     if not root:
         return default
     if not path:
         return root
     return _GenericRetrieve(root.get(path[0]), default, path[1:])
 
 
 def _AddPrefix(element, prefix):
     """Add |prefix| to |element| or each subelement if element is iterable."""
     if element is None:
         return element
     # Note, not Iterable because we don't want to handle strings like that.
-    if isinstance(element, (list, tuple)):
+    if isinstance(element, list) or isinstance(element, tuple):
         return [prefix + e for e in element]
     else:
         return prefix + element
 
 
 def _DoRemapping(element, map):
     """If |element| then remap it through |map|. If |element| is iterable then
-    each item will be remapped. Any elements not found will be removed."""
+  each item will be remapped. Any elements not found will be removed."""
     if map is not None and element is not None:
         if not callable(map):
             map = map.get  # Assume it's a dict, otherwise a callable to do the remap.
-        if isinstance(element, (list, tuple)):
+        if isinstance(element, list) or isinstance(element, tuple):
             element = filter(None, [map(elem) for elem in element])
         else:
             element = map(element)
     return element
 
 
 def _AppendOrReturn(append, element):
     """If |append| is None, simply return |element|. If |append| is not None,
-    then add |element| to it, adding each item in |element| if it's a list or
-    tuple."""
+  then add |element| to it, adding each item in |element| if it's a list or
+  tuple."""
     if append is not None and element is not None:
-        if isinstance(element, (list, tuple)):
+        if isinstance(element, list) or isinstance(element, tuple):
             append.extend(element)
         else:
             append.append(element)
     else:
         return element
 
 
 def _FindDirectXInstallation():
     """Try to find an installation location for the DirectX SDK. Check for the
-    standard environment variable, and if that doesn't exist, try to find
-    via the registry. May return None if not found in either location."""
+  standard environment variable, and if that doesn't exist, try to find
+  via the registry. May return None if not found in either location."""
     # Return previously calculated value, if there is one
     if hasattr(_FindDirectXInstallation, "dxsdk_dir"):
         return _FindDirectXInstallation.dxsdk_dir
 
     dxsdk_dir = os.environ.get("DXSDK_DIR")
     if not dxsdk_dir:
         # Setup params to pass to and attempt to launch reg.exe.
         cmd = ["reg.exe", "query", r"HKLM\Software\Microsoft\DirectX", "/s"]
         p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        stdout = p.communicate()[0].decode("utf-8")
+        stdout = p.communicate()[0]
+        if PY3:
+            stdout = stdout.decode("utf-8")
         for line in stdout.splitlines():
             if "InstallPath" in line:
                 dxsdk_dir = line.split("    ")[3] + "\\"
 
     # Cache return value
     _FindDirectXInstallation.dxsdk_dir = dxsdk_dir
     return dxsdk_dir
 
 
 def GetGlobalVSMacroEnv(vs_version):
     """Get a dict of variables mapping internal VS macro names to their gyp
-    equivalents. Returns all variables that are independent of the target."""
+  equivalents. Returns all variables that are independent of the target."""
     env = {}
     # '$(VSInstallDir)' and '$(VCInstallDir)' are available when and only when
     # Visual Studio is actually installed.
     if vs_version.Path():
         env["$(VSInstallDir)"] = vs_version.Path()
         env["$(VCInstallDir)"] = os.path.join(vs_version.Path(), "VC") + "\\"
     # Chromium uses DXSDK_DIR in include/lib paths, but it may or may not be
@@ -167,15 +163,15 @@
     # the WDK_DIR environment variable, may be None.
     env["$(WDK_DIR)"] = os.environ.get("WDK_DIR", "")
     return env
 
 
 def ExtractSharedMSVSSystemIncludes(configs, generator_flags):
     """Finds msvs_system_include_dirs that are common to all targets, removes
-    them from all targets, and returns an OrderedSet containing them."""
+  them from all targets, and returns an OrderedSet containing them."""
     all_system_includes = OrderedSet(configs[0].get("msvs_system_include_dirs", []))
     for config in configs[1:]:
         system_includes = config.get("msvs_system_include_dirs", [])
         all_system_includes = all_system_includes & OrderedSet(system_includes)
     if not all_system_includes:
         return None
     # Expand macros in all_system_includes.
@@ -193,18 +189,18 @@
         if includes:  # Don't insert a msvs_system_include_dirs key if not needed.
             # This must check the unexpanded includes list:
             new_includes = [i for i in includes if i not in all_system_includes]
             config["msvs_system_include_dirs"] = new_includes
     return expanded_system_includes
 
 
-class MsvsSettings:
+class MsvsSettings(object):
     """A class that understands the gyp 'msvs_...' values (especially the
-    msvs_settings field). They largely correpond to the VS2008 IDE DOM. This
-    class helps map those settings to command line options."""
+  msvs_settings field). They largely correpond to the VS2008 IDE DOM. This
+  class helps map those settings to command line options."""
 
     def __init__(self, spec, generator_flags):
         self.spec = spec
         self.vs_version = GetVSVersion(generator_flags)
 
         supported_fields = [
             ("msvs_configuration_attributes", dict),
@@ -229,37 +225,38 @@
             "msvs_postbuild",
         ]
         unsupported = []
         for field in unsupported_fields:
             for config in configs.values():
                 if field in config:
                     unsupported += [
-                        "{} not supported (target {}).".format(
-                            field, spec["target_name"]
-                        )
+                        "%s not supported (target %s)." % (field, spec["target_name"])
                     ]
         if unsupported:
             raise Exception("\n".join(unsupported))
 
     def GetExtension(self):
         """Returns the extension for the target, with no leading dot.
 
-        Uses 'product_extension' if specified, otherwise uses MSVS defaults based on
-        the target type.
-        """
+    Uses 'product_extension' if specified, otherwise uses MSVS defaults based on
+    the target type.
+    """
         ext = self.spec.get("product_extension", None)
         if ext:
             return ext
         return gyp.MSVSUtil.TARGET_TYPE_EXT.get(self.spec["type"], "")
 
     def GetVSMacroEnv(self, base_to_build=None, config=None):
         """Get a dict of variables mapping internal VS macro names to their gyp
-        equivalents."""
+    equivalents."""
         target_arch = self.GetArch(config)
-        target_platform = "Win32" if target_arch == "x86" else target_arch
+        if target_arch == "x86":
+            target_platform = "Win32"
+        else:
+            target_platform = target_arch
         target_name = self.spec.get("product_prefix", "") + self.spec.get(
             "product_name", self.spec["target_name"]
         )
         target_dir = base_to_build + "\\" if base_to_build else ""
         target_ext = "." + self.GetExtension()
         target_file_name = target_name + target_ext
 
@@ -293,23 +290,23 @@
             if not lib.lower().endswith(".lib") and not lib.lower().endswith(".obj")
             else lib
             for lib in libs
         ]
 
     def _GetAndMunge(self, field, path, default, prefix, append, map):
         """Retrieve a value from |field| at |path| or return |default|. If
-        |append| is specified, and the item is found, it will be appended to that
-        object instead of returned. If |map| is specified, results will be
-        remapped through |map| before being returned or appended."""
+    |append| is specified, and the item is found, it will be appended to that
+    object instead of returned. If |map| is specified, results will be
+    remapped through |map| before being returned or appended."""
         result = _GenericRetrieve(field, default, path)
         result = _DoRemapping(result, map)
         result = _AddPrefix(result, prefix)
         return _AppendOrReturn(append, result)
 
-    class _GetWrapper:
+    class _GetWrapper(object):
         def __init__(self, parent, field, base_path, append=None):
             self.parent = parent
             self.field = field
             self.base_path = [base_path]
             self.append = append
 
         def __call__(self, name, map=None, prefix="", default=None):
@@ -320,29 +317,29 @@
                 prefix=prefix,
                 append=self.append,
                 map=map,
             )
 
     def GetArch(self, config):
         """Get architecture based on msvs_configuration_platform and
-        msvs_target_platform. Returns either 'x86' or 'x64'."""
+    msvs_target_platform. Returns either 'x86' or 'x64'."""
         configuration_platform = self.msvs_configuration_platform.get(config, "")
         platform = self.msvs_target_platform.get(config, "")
         if not platform:  # If no specific override, use the configuration's.
             platform = configuration_platform
         # Map from platform to architecture.
         return {"Win32": "x86", "x64": "x64", "ARM64": "arm64"}.get(platform, "x86")
 
     def _TargetConfig(self, config):
         """Returns the target-specific configuration."""
         # There's two levels of architecture/platform specification in VS. The
         # first level is globally for the configuration (this is what we consider
         # "the" config at the gyp level, which will be something like 'Debug' or
         # 'Release'), VS2015 and later only use this level
-        if int(self.vs_version.short_name) >= 2015:
+        if self.vs_version.short_name >= 2015:
             return config
         # and a second target-specific configuration, which is an
         # override for the global one. |config| is remapped here to take into
         # account the local target-specific overrides to the global configuration.
         arch = self.GetArch(config)
         if arch == "x64" and not config.endswith("_x64"):
             config += "_x64"
@@ -367,39 +364,39 @@
             prefix,
             append,
             map,
         )
 
     def AdjustIncludeDirs(self, include_dirs, config):
         """Updates include_dirs to expand VS specific paths, and adds the system
-        include dirs used for platform SDK and similar."""
+    include dirs used for platform SDK and similar."""
         config = self._TargetConfig(config)
         includes = include_dirs + self.msvs_system_include_dirs[config]
         includes.extend(
             self._Setting(
                 ("VCCLCompilerTool", "AdditionalIncludeDirectories"), config, default=[]
             )
         )
         return [self.ConvertVSMacros(p, config=config) for p in includes]
 
     def AdjustMidlIncludeDirs(self, midl_include_dirs, config):
         """Updates midl_include_dirs to expand VS specific paths, and adds the
-        system include dirs used for platform SDK and similar."""
+    system include dirs used for platform SDK and similar."""
         config = self._TargetConfig(config)
         includes = midl_include_dirs + self.msvs_system_include_dirs[config]
         includes.extend(
             self._Setting(
                 ("VCMIDLTool", "AdditionalIncludeDirectories"), config, default=[]
             )
         )
         return [self.ConvertVSMacros(p, config=config) for p in includes]
 
     def GetComputedDefines(self, config):
         """Returns the set of defines that are injected to the defines list based
-        on other VS settings."""
+    on other VS settings."""
         config = self._TargetConfig(config)
         defines = []
         if self._ConfigAttrib(["CharacterSet"], config) == "1":
             defines.extend(("_UNICODE", "UNICODE"))
         if self._ConfigAttrib(["CharacterSet"], config) == "2":
             defines.append("_MBCS")
         defines.extend(
@@ -407,47 +404,47 @@
                 ("VCCLCompilerTool", "PreprocessorDefinitions"), config, default=[]
             )
         )
         return defines
 
     def GetCompilerPdbName(self, config, expand_special):
         """Get the pdb file name that should be used for compiler invocations, or
-        None if there's no explicit name specified."""
+    None if there's no explicit name specified."""
         config = self._TargetConfig(config)
         pdbname = self._Setting(("VCCLCompilerTool", "ProgramDataBaseFileName"), config)
         if pdbname:
             pdbname = expand_special(self.ConvertVSMacros(pdbname))
         return pdbname
 
     def GetMapFileName(self, config, expand_special):
         """Gets the explicitly overridden map file name for a target or returns None
-        if it's not set."""
+    if it's not set."""
         config = self._TargetConfig(config)
         map_file = self._Setting(("VCLinkerTool", "MapFileName"), config)
         if map_file:
             map_file = expand_special(self.ConvertVSMacros(map_file, config=config))
         return map_file
 
     def GetOutputName(self, config, expand_special):
         """Gets the explicitly overridden output name for a target or returns None
-        if it's not overridden."""
+    if it's not overridden."""
         config = self._TargetConfig(config)
         type = self.spec["type"]
         root = "VCLibrarianTool" if type == "static_library" else "VCLinkerTool"
         # TODO(scottmg): Handle OutputDirectory without OutputFile.
         output_file = self._Setting((root, "OutputFile"), config)
         if output_file:
             output_file = expand_special(
                 self.ConvertVSMacros(output_file, config=config)
             )
         return output_file
 
     def GetPDBName(self, config, expand_special, default):
         """Gets the explicitly overridden pdb name for a target or returns
-        default if it's not overridden, or if no pdb will be generated."""
+    default if it's not overridden, or if no pdb will be generated."""
         config = self._TargetConfig(config)
         output_file = self._Setting(("VCLinkerTool", "ProgramDatabaseFile"), config)
         generate_debug_info = self._Setting(
             ("VCLinkerTool", "GenerateDebugInformation"), config
         )
         if generate_debug_info == "true":
             if output_file:
@@ -455,15 +452,15 @@
             else:
                 return default
         else:
             return None
 
     def GetNoImportLibrary(self, config):
         """If NoImportLibrary: true, ninja will not expect the output to include
-        an import library."""
+    an import library."""
         config = self._TargetConfig(config)
         noimplib = self._Setting(("NoImportLibrary",), config)
         return noimplib == "true"
 
     def GetAsmflags(self, config):
         """Returns the flags that need to be added to ml invocations."""
         config = self._TargetConfig(config)
@@ -538,25 +535,26 @@
             [
                 "/FI" + f
                 for f in self._Setting(
                     ("VCCLCompilerTool", "ForcedIncludeFiles"), config, default=[]
                 )
             ]
         )
-        if float(self.vs_version.project_version) >= 12.0:
+        if self.vs_version.project_version >= 12.0:
             # New flag introduced in VS2013 (project version 12.0) Forces writes to
             # the program database (PDB) to be serialized through MSPDBSRV.EXE.
             # https://msdn.microsoft.com/en-us/library/dn502518.aspx
             cflags.append("/FS")
         # ninja handles parallelism by itself, don't have the compiler do it too.
         cflags = [x for x in cflags if not x.startswith("/MP")]
         return cflags
 
     def _GetPchFlags(self, config, extension):
-        """Get the flags to be added to the cflags for precompiled header support."""
+        """Get the flags to be added to the cflags for precompiled header support.
+    """
         config = self._TargetConfig(config)
         # The PCH is only built once by a particular source file. Usage of PCH must
         # only be for the same language (i.e. C vs. C++), so only include the pch
         # flags when the language matches.
         if self.msvs_precompiled_header[config]:
             source_ext = os.path.splitext(self.msvs_precompiled_source[config])[1]
             if _LanguageMatchesForPch(source_ext, extension):
@@ -573,15 +571,15 @@
     def GetCflagsCC(self, config):
         """Returns the flags that need to be added to .cc compilations."""
         config = self._TargetConfig(config)
         return ["/TP"] + self._GetPchFlags(config, ".cc")
 
     def _GetAdditionalLibraryDirectories(self, root, config, gyp_to_build_path):
         """Get and normalize the list of paths in AdditionalLibraryDirectories
-        setting."""
+    setting."""
         config = self._TargetConfig(config)
         libpaths = self._Setting(
             (root, "AdditionalLibraryDirectories"), config, default=[]
         )
         libpaths = [
             os.path.normpath(gyp_to_build_path(self.ConvertVSMacros(p, config=config)))
             for p in libpaths
@@ -620,22 +618,22 @@
                 return gyp_to_build_path(def_files[0])
             elif len(def_files) > 1:
                 raise Exception("Multiple .def files")
         return None
 
     def _GetDefFileAsLdflags(self, ldflags, gyp_to_build_path):
         """.def files get implicitly converted to a ModuleDefinitionFile for the
-        linker in the VS generator. Emulate that behaviour here."""
+    linker in the VS generator. Emulate that behaviour here."""
         def_file = self.GetDefFile(gyp_to_build_path)
         if def_file:
             ldflags.append('/DEF:"%s"' % def_file)
 
     def GetPGDName(self, config, expand_special):
         """Gets the explicitly overridden pgd name for a target or returns None
-        if it's not overridden."""
+    if it's not overridden."""
         config = self._TargetConfig(config)
         output_file = self._Setting(("VCLinkerTool", "ProfileGuidedDatabase"), config)
         if output_file:
             output_file = expand_special(
                 self.ConvertVSMacros(output_file, config=config)
             )
         return output_file
@@ -647,15 +645,15 @@
         expand_special,
         manifest_base_name,
         output_name,
         is_executable,
         build_dir,
     ):
         """Returns the flags that need to be added to link commands, and the
-        manifest files."""
+    manifest files."""
         config = self._TargetConfig(config)
         ldflags = []
         ld = self._GetWrapper(
             self, self.msvs_settings[config], "VCLinkerTool", append=ldflags
         )
         self._GetDefFileAsLdflags(ldflags, gyp_to_build_path)
         ld("GenerateDebugInformation", map={"true": "/DEBUG"})
@@ -707,15 +705,15 @@
         )
         if stack_reserve_size:
             stack_commit_size = self._Setting(
                 ("VCLinkerTool", "StackCommitSize"), config, default=""
             )
             if stack_commit_size:
                 stack_commit_size = "," + stack_commit_size
-            ldflags.append(f"/STACK:{stack_reserve_size}{stack_commit_size}")
+            ldflags.append("/STACK:%s%s" % (stack_reserve_size, stack_commit_size))
 
         ld("TerminalServerAware", map={"1": ":NO", "2": ""}, prefix="/TSAWARE")
         ld("LinkIncremental", map={"1": ":NO", "2": ""}, prefix="/INCREMENTAL")
         ld("BaseAddress", prefix="/BASE:")
         ld("FixedBaseAddress", map={"1": ":NO", "2": ""}, prefix="/FIXED")
         ld("RandomizedBaseAddress", map={"1": ":NO", "2": ""}, prefix="/DYNAMICBASE")
         ld("DataExecutionPrevention", map={"1": ":NO", "2": ""}, prefix="/NXCOMPAT")
@@ -731,15 +729,18 @@
         ld("ResourceOnlyDLL", map={"true": "/NOENTRY"})
         ld("EntryPointSymbol", prefix="/ENTRY:")
         ld("Profile", map={"true": "/PROFILE"})
         ld("LargeAddressAware", map={"1": ":NO", "2": ""}, prefix="/LARGEADDRESSAWARE")
         # TODO(scottmg): This should sort of be somewhere else (not really a flag).
         ld("AdditionalDependencies", prefix="")
 
-        safeseh_default = "true" if self.GetArch(config) == "x86" else None
+        if self.GetArch(config) == "x86":
+            safeseh_default = "true"
+        else:
+            safeseh_default = None
         ld(
             "ImageHasSafeExceptionHandlers",
             map={"false": ":NO", "true": ""},
             prefix="/SAFESEH",
             default=safeseh_default,
         )
 
@@ -770,20 +771,20 @@
         ldflags.extend(manifest_flags)
         return ldflags, intermediate_manifest, manifest_files
 
     def _GetLdManifestFlags(
         self, config, name, gyp_to_build_path, allow_isolation, build_dir
     ):
         """Returns a 3-tuple:
-        - the set of flags that need to be added to the link to generate
-          a default manifest
-        - the intermediate manifest that the linker will generate that should be
-          used to assert it doesn't add anything to the merged one.
-        - the list of all the manifest files to be merged by the manifest tool and
-          included into the link."""
+    - the set of flags that need to be added to the link to generate
+      a default manifest
+    - the intermediate manifest that the linker will generate that should be
+      used to assert it doesn't add anything to the merged one.
+    - the list of all the manifest files to be merged by the manifest tool and
+      included into the link."""
         generate_manifest = self._Setting(
             ("VCLinkerTool", "GenerateManifest"), config, default="true"
         )
         if generate_manifest != "true":
             # This means not only that the linker should not generate the intermediate
             # manifest but also that the manifest tool should do nothing even when
             # additional manifests are specified.
@@ -809,16 +810,16 @@
         config = self._TargetConfig(config)
         enable_uac = self._Setting(
             ("VCLinkerTool", "EnableUAC"), config, default="true"
         )
         manifest_files = []
         generated_manifest_outer = (
             "<?xml version='1.0' encoding='UTF-8' standalone='yes'?>"
-            "<assembly xmlns='urn:schemas-microsoft-com:asm.v1' manifestVersion='1.0'>"
-            "%s</assembly>"
+            "<assembly xmlns='urn:schemas-microsoft-com:asm.v1' manifestVersion='1.0'>%s"
+            "</assembly>"
         )
         if enable_uac == "true":
             execution_level = self._Setting(
                 ("VCLinkerTool", "UACExecutionLevel"), config, default="0"
             )
             execution_level_map = {
                 "0": "asInvoker",
@@ -830,18 +831,18 @@
                 ("VCLinkerTool", "UACUIAccess"), config, default="false"
             )
 
             inner = """
 <trustInfo xmlns="urn:schemas-microsoft-com:asm.v3">
   <security>
     <requestedPrivileges>
-      <requestedExecutionLevel level='{}' uiAccess='{}' />
+      <requestedExecutionLevel level='%s' uiAccess='%s' />
     </requestedPrivileges>
   </security>
-</trustInfo>""".format(
+</trustInfo>""" % (
                 execution_level_map[execution_level],
                 ui_access,
             )
         else:
             inner = ""
 
         generated_manifest_contents = generated_manifest_outer % inner
@@ -862,28 +863,28 @@
             flags.append("/ALLOWISOLATION")
 
         manifest_files += self._GetAdditionalManifestFiles(config, gyp_to_build_path)
         return flags, output_name, manifest_files
 
     def _GetAdditionalManifestFiles(self, config, gyp_to_build_path):
         """Gets additional manifest files that are added to the default one
-        generated by the linker."""
+    generated by the linker."""
         files = self._Setting(
             ("VCManifestTool", "AdditionalManifestFiles"), config, default=[]
         )
         if isinstance(files, str):
             files = files.split(";")
         return [
             os.path.normpath(gyp_to_build_path(self.ConvertVSMacros(f, config=config)))
             for f in files
         ]
 
     def IsUseLibraryDependencyInputs(self, config):
         """Returns whether the target should be linked via Use Library Dependency
-        Inputs (using component .objs of a given .lib)."""
+    Inputs (using component .objs of a given .lib)."""
         config = self._TargetConfig(config)
         uldi = self._Setting(("VCLinkerTool", "UseLibraryDependencyInputs"), config)
         return uldi == "true"
 
     def IsEmbedManifest(self, config):
         """Returns whether manifest should be linked into binary."""
         config = self._TargetConfig(config)
@@ -896,91 +897,85 @@
         """Returns whether the target should be linked incrementally."""
         config = self._TargetConfig(config)
         link_inc = self._Setting(("VCLinkerTool", "LinkIncremental"), config)
         return link_inc != "1"
 
     def GetRcflags(self, config, gyp_to_ninja_path):
         """Returns the flags that need to be added to invocations of the resource
-        compiler."""
+    compiler."""
         config = self._TargetConfig(config)
         rcflags = []
         rc = self._GetWrapper(
             self, self.msvs_settings[config], "VCResourceCompilerTool", append=rcflags
         )
         rc("AdditionalIncludeDirectories", map=gyp_to_ninja_path, prefix="/I")
         rcflags.append("/I" + gyp_to_ninja_path("."))
         rc("PreprocessorDefinitions", prefix="/d")
         # /l arg must be in hex without leading '0x'
         rc("Culture", prefix="/l", map=lambda x: hex(int(x))[2:])
         return rcflags
 
     def BuildCygwinBashCommandLine(self, args, path_to_base):
         """Build a command line that runs args via cygwin bash. We assume that all
-        incoming paths are in Windows normpath'd form, so they need to be
-        converted to posix style for the part of the command line that's passed to
-        bash. We also have to do some Visual Studio macro emulation here because
-        various rules use magic VS names for things. Also note that rules that
-        contain ninja variables cannot be fixed here (for example ${source}), so
-        the outer generator needs to make sure that the paths that are written out
-        are in posix style, if the command line will be used here."""
+    incoming paths are in Windows normpath'd form, so they need to be
+    converted to posix style for the part of the command line that's passed to
+    bash. We also have to do some Visual Studio macro emulation here because
+    various rules use magic VS names for things. Also note that rules that
+    contain ninja variables cannot be fixed here (for example ${source}), so
+    the outer generator needs to make sure that the paths that are written out
+    are in posix style, if the command line will be used here."""
         cygwin_dir = os.path.normpath(
             os.path.join(path_to_base, self.msvs_cygwin_dirs[0])
         )
         cd = ("cd %s" % path_to_base).replace("\\", "/")
         args = [a.replace("\\", "/").replace('"', '\\"') for a in args]
         args = ["'%s'" % a.replace("'", "'\\''") for a in args]
         bash_cmd = " ".join(args)
         cmd = (
             'call "%s\\setup_env.bat" && set CYGWIN=nontsec && ' % cygwin_dir
-            + f'bash -c "{cd} ; {bash_cmd}"'
+            + 'bash -c "%s ; %s"' % (cd, bash_cmd)
         )
         return cmd
 
-    RuleShellFlags = collections.namedtuple("RuleShellFlags", ["cygwin", "quote"])
-
-    def GetRuleShellFlags(self, rule):
-        """Return RuleShellFlags about how the given rule should be run. This
-        includes whether it should run under cygwin (msvs_cygwin_shell), and
-        whether the commands should be quoted (msvs_quote_cmd)."""
-        # If the variable is unset, or set to 1 we use cygwin
-        cygwin = int(rule.get("msvs_cygwin_shell",
-                              self.spec.get("msvs_cygwin_shell", 1))) != 0
-        # Default to quoting. There's only a few special instances where the
-        # target command uses non-standard command line parsing and handle quotes
-        # and quote escaping differently.
-        quote_cmd = int(rule.get("msvs_quote_cmd", 1))
-        assert quote_cmd != 0 or cygwin != 1, \
-               "msvs_quote_cmd=0 only applicable for msvs_cygwin_shell=0"
-        return MsvsSettings.RuleShellFlags(cygwin, quote_cmd)
+    def IsRuleRunUnderCygwin(self, rule):
+        """Determine if an action should be run under cygwin. If the variable is
+    unset, or set to 1 we use cygwin."""
+        return (
+            int(rule.get("msvs_cygwin_shell", self.spec.get("msvs_cygwin_shell", 1)))
+            != 0
+        )
 
     def _HasExplicitRuleForExtension(self, spec, extension):
         """Determine if there's an explicit rule for a particular extension."""
-        return any(rule["extension"] == extension for rule in spec.get("rules", []))
+        for rule in spec.get("rules", []):
+            if rule["extension"] == extension:
+                return True
+        return False
 
     def _HasExplicitIdlActions(self, spec):
         """Determine if an action should not run midl for .idl files."""
         return any(
             [action.get("explicit_idl_action", 0) for action in spec.get("actions", [])]
         )
 
     def HasExplicitIdlRulesOrActions(self, spec):
         """Determine if there's an explicit rule or action for idl files. When
-        there isn't we need to generate implicit rules to build MIDL .idl files."""
+    there isn't we need to generate implicit rules to build MIDL .idl files."""
         return self._HasExplicitRuleForExtension(
             spec, "idl"
         ) or self._HasExplicitIdlActions(spec)
 
     def HasExplicitAsmRules(self, spec):
         """Determine if there's an explicit rule for asm files. When there isn't we
-        need to generate implicit rules to assemble .asm files."""
+    need to generate implicit rules to assemble .asm files."""
         return self._HasExplicitRuleForExtension(spec, "asm")
 
     def GetIdlBuildData(self, source, config):
         """Determine the implicit outputs for an idl file. Returns output
-        directory, outputs, and variables and flags that are required."""
+    directory, outputs, and variables and flags that are required."""
         config = self._TargetConfig(config)
         midl_get = self._GetWrapper(self, self.msvs_settings[config], "VCMIDLTool")
 
         def midl(name, default=None):
             return self.ConvertVSMacros(midl_get(name, default=default), config=config)
 
         tlb = midl("TypeLibraryName", default="${root}.tlb")
@@ -1011,58 +1006,58 @@
     c_exts = (".c",)
     cc_exts = (".cc", ".cxx", ".cpp")
     return (source_ext in c_exts and pch_source_ext in c_exts) or (
         source_ext in cc_exts and pch_source_ext in cc_exts
     )
 
 
-class PrecompiledHeader:
+class PrecompiledHeader(object):
     """Helper to generate dependencies and build rules to handle generation of
-    precompiled headers. Interface matches the GCH handler in xcode_emulation.py.
-    """
+  precompiled headers. Interface matches the GCH handler in xcode_emulation.py.
+  """
 
     def __init__(
         self, settings, config, gyp_to_build_path, gyp_to_unique_output, obj_ext
     ):
         self.settings = settings
         self.config = config
         pch_source = self.settings.msvs_precompiled_source[self.config]
         self.pch_source = gyp_to_build_path(pch_source)
         filename, _ = os.path.splitext(pch_source)
         self.output_obj = gyp_to_unique_output(filename + obj_ext).lower()
 
     def _PchHeader(self):
         """Get the header that will appear in an #include line for all source
-        files."""
+    files."""
         return self.settings.msvs_precompiled_header[self.config]
 
     def GetObjDependencies(self, sources, objs, arch):
         """Given a list of sources files and the corresponding object files,
-        returns a list of the pch files that should be depended upon. The
-        additional wrapping in the return value is for interface compatibility
-        with make.py on Mac, and xcode_emulation.py."""
+    returns a list of the pch files that should be depended upon. The
+    additional wrapping in the return value is for interface compatibility
+    with make.py on Mac, and xcode_emulation.py."""
         assert arch is None
         if not self._PchHeader():
             return []
         pch_ext = os.path.splitext(self.pch_source)[1]
         for source in sources:
             if _LanguageMatchesForPch(os.path.splitext(source)[1], pch_ext):
                 return [(None, None, self.output_obj)]
         return []
 
     def GetPchBuildCommands(self, arch):
         """Not used on Windows as there are no additional build steps required
-        (instead, existing steps are modified in GetFlagsModifications below)."""
+    (instead, existing steps are modified in GetFlagsModifications below)."""
         return []
 
     def GetFlagsModifications(
         self, input, output, implicit, command, cflags_c, cflags_cc, expand_special
     ):
         """Get the modified cflags and implicit dependencies that should be used
-        for the pch compilation step."""
+    for the pch compilation step."""
         if input == self.pch_source:
             pch_output = ["/Yc" + self._PchHeader()]
             if command == "cxx":
                 return (
                     [("cflags_cc", map(expand_special, cflags_cc + pch_output))],
                     self.output_obj,
                     [],
@@ -1091,25 +1086,25 @@
 def _GetVsvarsSetupArgs(generator_flags, arch):
     vs = GetVSVersion(generator_flags)
     return vs.SetupScript()
 
 
 def ExpandMacros(string, expansions):
     """Expand $(Variable) per expansions dict. See MsvsSettings.GetVSMacroEnv
-    for the canonical way to retrieve a suitable dict."""
+  for the canonical way to retrieve a suitable dict."""
     if "$" in string:
         for old, new in expansions.items():
             assert "$(" not in new, new
             string = string.replace(old, new)
     return string
 
 
 def _ExtractImportantEnvironment(output_of_set):
     """Extracts environment variables required for the toolchain to run from
-    a textual dump output by the cmd.exe 'set' command."""
+  a textual dump output by the cmd.exe 'set' command."""
     envvars_to_save = (
         "goma_.*",  # TODO(scottmg): This is ugly, but needed for goma.
         "include",
         "lib",
         "libpath",
         "path",
         "pathext",
@@ -1141,50 +1136,50 @@
                 "required to be set to valid path" % required
             )
     return env
 
 
 def _FormatAsEnvironmentBlock(envvar_dict):
     """Format as an 'environment block' directly suitable for CreateProcess.
-    Briefly this is a list of key=value\0, terminated by an additional \0. See
-    CreateProcess documentation for more details."""
+  Briefly this is a list of key=value\0, terminated by an additional \0. See
+  CreateProcess documentation for more details."""
     block = ""
     nul = "\0"
     for key, value in envvar_dict.items():
         block += key + "=" + value + nul
     block += nul
     return block
 
 
 def _ExtractCLPath(output_of_where):
     """Gets the path to cl.exe based on the output of calling the environment
-    setup batch file, followed by the equivalent of `where`."""
+  setup batch file, followed by the equivalent of `where`."""
     # Take the first line, as that's the first found in the PATH.
     for line in output_of_where.strip().splitlines():
         if line.startswith("LOC:"):
             return line[len("LOC:") :].strip()
 
 
 def GenerateEnvironmentFiles(
     toplevel_build_dir, generator_flags, system_includes, open_out
 ):
     """It's not sufficient to have the absolute path to the compiler, linker,
-    etc. on Windows, as those tools rely on .dlls being in the PATH. We also
-    need to support both x86 and x64 compilers within the same build (to support
-    msvs_target_platform hackery). Different architectures require a different
-    compiler binary, and different supporting environment variables (INCLUDE,
-    LIB, LIBPATH). So, we extract the environment here, wrap all invocations
-    of compiler tools (cl, link, lib, rc, midl, etc.) via win_tool.py which
-    sets up the environment, and then we do not prefix the compiler with
-    an absolute path, instead preferring something like "cl.exe" in the rule
-    which will then run whichever the environment setup has put in the path.
-    When the following procedure to generate environment files does not
-    meet your requirement (e.g. for custom toolchains), you can pass
-    "-G ninja_use_custom_environment_files" to the gyp to suppress file
-    generation and use custom environment files prepared by yourself."""
+  etc. on Windows, as those tools rely on .dlls being in the PATH. We also
+  need to support both x86 and x64 compilers within the same build (to support
+  msvs_target_platform hackery). Different architectures require a different
+  compiler binary, and different supporting environment variables (INCLUDE,
+  LIB, LIBPATH). So, we extract the environment here, wrap all invocations
+  of compiler tools (cl, link, lib, rc, midl, etc.) via win_tool.py which
+  sets up the environment, and then we do not prefix the compiler with
+  an absolute path, instead preferring something like "cl.exe" in the rule
+  which will then run whichever the environment setup has put in the path.
+  When the following procedure to generate environment files does not
+  meet your requirement (e.g. for custom toolchains), you can pass
+  "-G ninja_use_custom_environment_files" to the gyp to suppress file
+  generation and use custom environment files prepared by yourself."""
     archs = ("x86", "x64")
     if generator_flags.get("ninja_use_custom_environment_files", 0):
         cl_paths = {}
         for arch in archs:
             cl_paths[arch] = "cl.exe"
         return cl_paths
     vs = GetVSVersion(generator_flags)
@@ -1192,15 +1187,17 @@
     for arch in archs:
         # Extract environment variables for subprocesses.
         args = vs.SetupScript(arch)
         args.extend(("&&", "set"))
         popen = subprocess.Popen(
             args, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
         )
-        variables = popen.communicate()[0].decode("utf-8")
+        variables, _ = popen.communicate()
+        if PY3:
+            variables = variables.decode("utf-8")
         if popen.returncode != 0:
             raise Exception('"%s" failed with error %d' % (args, popen.returncode))
         env = _ExtractImportantEnvironment(variables)
 
         # Inject system includes from gyp files into INCLUDE.
         if system_includes:
             system_includes = system_includes | OrderedSet(
@@ -1215,25 +1212,27 @@
 
         # Find cl.exe location for this architecture.
         args = vs.SetupScript(arch)
         args.extend(
             ("&&", "for", "%i", "in", "(cl.exe)", "do", "@echo", "LOC:%~$PATH:i")
         )
         popen = subprocess.Popen(args, shell=True, stdout=subprocess.PIPE)
-        output = popen.communicate()[0].decode("utf-8")
+        output, _ = popen.communicate()
+        if PY3:
+            output = output.decode("utf-8")
         cl_paths[arch] = _ExtractCLPath(output)
     return cl_paths
 
 
 def VerifyMissingSources(sources, build_dir, generator_flags, gyp_to_ninja):
     """Emulate behavior of msvs_error_on_missing_sources present in the msvs
-    generator: Check that all regular source files, i.e. not created at run time,
-    exist on disk. Missing files cause needless recompilation when building via
-    VS, and we want this check to match for people/bots that build using ninja,
-    so they're not surprised when the VS build fails."""
+  generator: Check that all regular source files, i.e. not created at run time,
+  exist on disk. Missing files cause needless recompilation when building via
+  VS, and we want this check to match for people/bots that build using ninja,
+  so they're not surprised when the VS build fails."""
     if int(generator_flags.get("msvs_error_on_missing_sources", 0)):
         no_specials = filter(lambda x: "$" not in x, sources)
         relative = [os.path.join(build_dir, gyp_to_ninja(s)) for s in no_specials]
         missing = [x for x in relative if not os.path.exists(x)]
         if missing:
             # They'll look like out\Release\..\..\stuff\things.cc, so normalize the
             # path for a slightly less crazy looking output.
```

### Comparing `gyp-next-0.15.0/pylib/gyp/ninja_syntax.py` & `gyp-next-0.4.0/pylib/gyp/ninja_syntax.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import textwrap
 
 
 def escape_path(word):
     return word.replace("$ ", "$$ ").replace(" ", "$ ").replace(":", "$:")
 
 
-class Writer:
+class Writer(object):
     def __init__(self, output, width=78):
         self.output = output
         self.width = width
 
     def newline(self):
         self.output.write("\n")
 
@@ -29,15 +29,15 @@
             self.output.write("# " + line + "\n")
 
     def variable(self, key, value, indent=0):
         if value is None:
             return
         if isinstance(value, list):
             value = " ".join(filter(None, value))  # Filter out empty strings.
-        self._line(f"{key} = {value}", indent)
+        self._line("%s = %s" % (key, value), indent)
 
     def pool(self, name, depth):
         self._line("pool %s" % name)
         self.variable("depth", depth, indent=1)
 
     def rule(
         self,
@@ -85,15 +85,15 @@
             all_inputs.extend(implicit)
         if order_only:
             order_only = map(escape_path, self._as_list(order_only))
             all_inputs.append("||")
             all_inputs.extend(order_only)
 
         self._line(
-            "build {}: {}".format(" ".join(out_outputs), " ".join([rule] + all_inputs))
+            "build %s: %s" % (" ".join(out_outputs), " ".join([rule] + all_inputs))
         )
 
         if variables:
             if isinstance(variables, dict):
                 iterator = iter(variables.items())
             else:
                 iterator = iter(variables)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/simple_copy.py` & `gyp-next-0.4.0/pylib/gyp/simple_copy.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,15 +32,18 @@
 _deepcopy_dispatch = d = {}
 
 
 def _deepcopy_atomic(x):
     return x
 
 
-types = bool, float, int, str, type, type(None)
+try:
+    types = bool, float, int, str, type, type(None), long, unicode
+except NameError:  # Python 3
+    types = bool, float, int, str, type, type(None)
 
 for x in types:
     d[x] = _deepcopy_atomic
 
 
 def _deepcopy_list(x):
     return [deepcopy(a) for a in x]
```

### Comparing `gyp-next-0.15.0/pylib/gyp/win_tool.py` & `gyp-next-0.4.0/pylib/gyp/win_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # Copyright (c) 2012 Google Inc. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 """Utility functions for Windows builds.
 
 These functions are executed via gyp-win-tool when using the ninja generator.
 """
 
+from __future__ import print_function
 
 import os
 import re
 import shutil
 import subprocess
 import stat
 import string
 import sys
 
 BASE_DIR = os.path.dirname(os.path.abspath(__file__))
+PY3 = bytes != str
 
 # A regex matching an argument corresponding to the output filename passed to
 # link.exe.
 _LINK_EXE_OUT_ARG = re.compile("/OUT:(?P<out>.+)$", re.IGNORECASE)
 
 
 def main(args):
     executor = WinTool()
     exit_code = executor.Dispatch(args)
     if exit_code is not None:
         sys.exit(exit_code)
 
 
-class WinTool:
+class WinTool(object):
     """This class performs all the Windows tooling steps. The methods can either
   be executed directly, or dispatched from an argument list."""
 
     def _UseSeparateMspdbsrv(self, env, args):
         """Allows to use a unique instance of mspdbsrv.exe per linker instead of a
     shared one."""
         if len(args) < 1:
@@ -135,15 +137,17 @@
         link = subprocess.Popen(
             args,
             shell=sys.platform == "win32",
             env=env,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         )
-        out = link.communicate()[0].decode("utf-8")
+        out, _ = link.communicate()
+        if PY3:
+            out = out.decode("utf-8")
         for line in out.splitlines():
             if (
                 not line.startswith("   Creating library ")
                 and not line.startswith("Generating code")
                 and not line.startswith("Finished generating code")
             ):
                 print(line)
@@ -215,25 +219,25 @@
                 "-manifest %(out)s.manifest %(intermediate_manifest)s "
                 "-out:%(out)s.assert.manifest" % variables
             )
             assert_manifest = "%(out)s.assert.manifest" % variables
             our_manifest = "%(out)s.manifest" % variables
             # Load and normalize the manifests. mt.exe sometimes removes whitespace,
             # and sometimes doesn't unfortunately.
-            with open(our_manifest) as our_f, open(assert_manifest) as assert_f:
-                translator = str.maketrans("", "", string.whitespace)
-                our_data = our_f.read().translate(translator)
-                assert_data = assert_f.read().translate(translator)
+            with open(our_manifest, "r") as our_f:
+                with open(assert_manifest, "r") as assert_f:
+                    our_data = our_f.read().translate(None, string.whitespace)
+                    assert_data = assert_f.read().translate(None, string.whitespace)
             if our_data != assert_data:
                 os.unlink(out)
 
                 def dump(filename):
                     print(filename, file=sys.stderr)
                     print("-----", file=sys.stderr)
-                    with open(filename) as f:
+                    with open(filename, "r") as f:
                         print(f.read(), file=sys.stderr)
                         print("-----", file=sys.stderr)
 
                 dump(intermediate_manifest)
                 dump(our_manifest)
                 dump(assert_manifest)
                 sys.stderr.write(
@@ -248,15 +252,17 @@
         """Run manifest tool with environment set. Strip out undesirable warning
     (some XML blocks are recognized by the OS loader, but not the manifest
     tool)."""
         env = self._GetEnv(arch)
         popen = subprocess.Popen(
             args, shell=True, env=env, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
         )
-        out = popen.communicate()[0].decode("utf-8")
+        out, _ = popen.communicate()
+        if PY3:
+            out = out.decode("utf-8")
         for line in out.splitlines():
             if line and "manifest authoring warning 81010002" not in line:
                 print(line)
         return popen.returncode
 
     def ExecManifestToRc(self, arch, *args):
         """Creates a resource file pointing a SxS assembly manifest.
@@ -292,34 +298,38 @@
                 idl,
             ]
         )
         env = self._GetEnv(arch)
         popen = subprocess.Popen(
             args, shell=True, env=env, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
         )
-        out = popen.communicate()[0].decode("utf-8")
+        out, _ = popen.communicate()
+        if PY3:
+            out = out.decode("utf-8")
         # Filter junk out of stdout, and write filtered versions. Output we want
         # to filter is pairs of lines that look like this:
         # Processing C:\Program Files (x86)\Microsoft SDKs\...\include\objidl.idl
         # objidl.idl
         lines = out.splitlines()
         prefixes = ("Processing ", "64 bit Processing ")
-        processing = {os.path.basename(x) for x in lines if x.startswith(prefixes)}
+        processing = set(os.path.basename(x) for x in lines if x.startswith(prefixes))
         for line in lines:
             if not line.startswith(prefixes) and line not in processing:
                 print(line)
         return popen.returncode
 
     def ExecAsmWrapper(self, arch, *args):
         """Filter logo banner from invocations of asm.exe."""
         env = self._GetEnv(arch)
         popen = subprocess.Popen(
             args, shell=True, env=env, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
         )
-        out = popen.communicate()[0].decode("utf-8")
+        out, _ = popen.communicate()
+        if PY3:
+            out = out.decode("utf-8")
         for line in out.splitlines():
             if (
                 not line.startswith("Copyright (C) Microsoft Corporation")
                 and not line.startswith("Microsoft (R) Macro Assembler")
                 and not line.startswith(" Assembling: ")
                 and line
             ):
@@ -329,15 +339,17 @@
     def ExecRcWrapper(self, arch, *args):
         """Filter logo banner from invocations of rc.exe. Older versions of RC
     don't support the /nologo flag."""
         env = self._GetEnv(arch)
         popen = subprocess.Popen(
             args, shell=True, env=env, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
         )
-        out = popen.communicate()[0].decode("utf-8")
+        out, _ = popen.communicate()
+        if PY3:
+            out = out.decode("utf-8")
         for line in out.splitlines():
             if (
                 not line.startswith("Microsoft (R) Windows (R) Resource Compiler")
                 and not line.startswith("Copyright (C) Microsoft Corporation")
                 and line
             ):
                 print(line)
```

### Comparing `gyp-next-0.15.0/pylib/gyp/xcode_emulation.py` & `gyp-next-0.4.0/pylib/gyp/xcode_emulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 # found in the LICENSE file.
 
 """
 This module contains classes that help to emulate xcodebuild behavior on top of
 other build systems, such as make and ninja.
 """
 
+from __future__ import print_function
 
 import copy
 import gyp.common
 import os
 import os.path
 import re
 import shlex
 import subprocess
 import sys
 from gyp.common import GypError
 
+PY3 = bytes != str
+
 # Populated lazily by XcodeVersion, for efficiency, and to fix an issue when
 # "xcodebuild" is called too quickly (it has been found to return incorrect
 # version number).
 XCODE_VERSION_CACHE = None
 
 # Populated lazily by GetXcodeArchsDefault, to an |XcodeArchsDefault| instance
 # corresponding to the installed version of Xcode.
@@ -33,15 +36,15 @@
   and optionally for $(ARCHS_STANDARD_INCLUDING_64_BIT)."""
     mapping = {"$(ARCHS_STANDARD)": archs}
     if archs_including_64_bit:
         mapping["$(ARCHS_STANDARD_INCLUDING_64_BIT)"] = archs_including_64_bit
     return mapping
 
 
-class XcodeArchsDefault:
+class XcodeArchsDefault(object):
     """A class to resolve ARCHS variable from xcode_settings, resolving Xcode
   macros and implementing filtering by VALID_ARCHS. The expansion of macros
   depends on the SDKROOT used ("macosx", "iphoneos", "iphonesimulator") and
   on the version of Xcode.
   """
 
     # Match variable like $(ARCHS_STANDARD).
@@ -106,15 +109,15 @@
   For "macosx" SDKROOT, all version starting with Xcode 5.0 includes 64-bit
   architecture as part of $(ARCHS_STANDARD) and default to only building it.
 
   For "iphoneos" and "iphonesimulator" SDKROOT, 64-bit architectures are part
   of $(ARCHS_STANDARD_INCLUDING_64_BIT) from Xcode 5.0. From Xcode 5.1, they
   are also part of $(ARCHS_STANDARD).
 
-  All these rules are coded in the construction of the |XcodeArchsDefault|
+  All thoses rules are coded in the construction of the |XcodeArchsDefault|
   object to use depending on the version of Xcode detected. The object is
   for performance reason."""
     global XCODE_ARCHS_DEFAULT_CACHE
     if XCODE_ARCHS_DEFAULT_CACHE:
         return XCODE_ARCHS_DEFAULT_CACHE
     xcode_version, _ = XcodeVersion()
     if xcode_version < "0500":
@@ -141,15 +144,15 @@
             XcodeArchsVariableMapping(
                 ["armv7", "armv7s", "arm64"], ["armv7", "armv7s", "arm64"]
             ),
         )
     return XCODE_ARCHS_DEFAULT_CACHE
 
 
-class XcodeSettings:
+class XcodeSettings(object):
     """A class that understands the gyp 'xcode_settings' object."""
 
     # Populated lazily by _SdkPath(). Shared by all XcodeSettings, so cached
     # at class-level for efficiency.
     _sdk_path_cache = {}
     _platform_path_cache = {}
     _sdk_root_cache = {}
@@ -274,15 +277,15 @@
             return "." + self.spec.get("product_extension", wrapper_extension)
         elif self.spec["type"] == "executable":
             if self._IsIosAppExtension() or self._IsIosWatchKitExtension():
                 return "." + self.spec.get("product_extension", "appex")
             else:
                 return "." + self.spec.get("product_extension", "app")
         else:
-            assert False, "Don't know extension for '{}', target '{}'".format(
+            assert False, "Don't know extension for '%s', target '%s'" % (
                 self.spec["type"],
                 self.spec["target_name"],
             )
 
     def GetProductName(self):
         """Returns PRODUCT_NAME."""
         return self.spec.get("product_name", self.spec["target_name"])
@@ -647,49 +650,48 @@
         self._WarnUnimplemented("GCC_DEBUGGING_SYMBOLS")
         self._WarnUnimplemented("GCC_ENABLE_OBJC_EXCEPTIONS")
 
         # TODO: This is exported correctly, but assigning to it is not supported.
         self._WarnUnimplemented("MACH_O_TYPE")
         self._WarnUnimplemented("PRODUCT_TYPE")
 
-        # If GYP_CROSSCOMPILE (--cross-compiling), disable architecture-specific
-        # additions and assume these will be provided as required via CC_host,
-        # CXX_host, CC_target and CXX_target.
-        if not gyp.common.CrossCompileRequested():
-            if arch is not None:
-                archs = [arch]
-            else:
-                assert self.configname
-                archs = self.GetActiveArchs(self.configname)
-            if len(archs) != 1:
-                # TODO: Supporting fat binaries will be annoying.
-                self._WarnUnimplemented("ARCHS")
-                archs = ["i386"]
-            cflags.append("-arch " + archs[0])
-
-            if archs[0] in ("i386", "x86_64"):
-                if self._Test("GCC_ENABLE_SSE3_EXTENSIONS", "YES", default="NO"):
-                    cflags.append("-msse3")
-                if self._Test(
-                    "GCC_ENABLE_SUPPLEMENTAL_SSE3_INSTRUCTIONS", "YES", default="NO"
-                ):
-                    cflags.append("-mssse3")  # Note 3rd 's'.
-                if self._Test("GCC_ENABLE_SSE41_EXTENSIONS", "YES", default="NO"):
-                    cflags.append("-msse4.1")
-                if self._Test("GCC_ENABLE_SSE42_EXTENSIONS", "YES", default="NO"):
-                    cflags.append("-msse4.2")
+        if arch is not None:
+            archs = [arch]
+        else:
+            assert self.configname
+            archs = self.GetActiveArchs(self.configname)
+        if len(archs) != 1:
+            # TODO: Supporting fat binaries will be annoying.
+            self._WarnUnimplemented("ARCHS")
+            archs = ["i386"]
+        cflags.append("-arch " + archs[0])
+
+        if archs[0] in ("i386", "x86_64"):
+            if self._Test("GCC_ENABLE_SSE3_EXTENSIONS", "YES", default="NO"):
+                cflags.append("-msse3")
+            if self._Test(
+                "GCC_ENABLE_SUPPLEMENTAL_SSE3_INSTRUCTIONS", "YES", default="NO"
+            ):
+                cflags.append("-mssse3")  # Note 3rd 's'.
+            if self._Test("GCC_ENABLE_SSE41_EXTENSIONS", "YES", default="NO"):
+                cflags.append("-msse4.1")
+            if self._Test("GCC_ENABLE_SSE42_EXTENSIONS", "YES", default="NO"):
+                cflags.append("-msse4.2")
 
         cflags += self._Settings().get("WARNING_CFLAGS", [])
 
         if self._IsXCTest():
             platform_root = self._XcodePlatformPath(configname)
             if platform_root:
                 cflags.append("-F" + platform_root + "/Developer/Library/Frameworks/")
 
-        framework_root = sdk_root if sdk_root else ""
+        if sdk_root:
+            framework_root = sdk_root
+        else:
+            framework_root = ""
         config = self.spec["configurations"][self.configname]
         framework_dirs = config.get("mac_framework_dirs", [])
         for directory in framework_dirs:
             cflags.append("-F" + directory.replace("$(SDKROOT)", framework_root))
 
         self.configname = None
         return cflags
@@ -932,25 +934,24 @@
         if "ORDER_FILE" in self._Settings():
             ldflags.append(
                 "-Wl,-order_file "
                 + "-Wl,"
                 + gyp_to_build_path(self._Settings()["ORDER_FILE"])
             )
 
-        if not gyp.common.CrossCompileRequested():
-            if arch is not None:
-                archs = [arch]
-            else:
-                assert self.configname
-                archs = self.GetActiveArchs(self.configname)
-            if len(archs) != 1:
-                # TODO: Supporting fat binaries will be annoying.
-                self._WarnUnimplemented("ARCHS")
-                archs = ["i386"]
-            ldflags.append("-arch " + archs[0])
+        if arch is not None:
+            archs = [arch]
+        else:
+            assert self.configname
+            archs = self.GetActiveArchs(self.configname)
+        if len(archs) != 1:
+            # TODO: Supporting fat binaries will be annoying.
+            self._WarnUnimplemented("ARCHS")
+            archs = ["i386"]
+        ldflags.append("-arch " + archs[0])
 
         # Xcode adds the product directory by default.
         # Rewrite -L. to -L./ to work around http://www.openradar.me/25313838
         ldflags.append("-L" + (product_dir if product_dir != "." else "./"))
 
         install_name = self.GetInstallName()
         if install_name and self.spec["type"] != "loadable_module":
@@ -1078,15 +1079,15 @@
 
             explicit_strip_flags = self._Settings().get("STRIPFLAGS", "")
             if explicit_strip_flags:
                 strip_flags += " " + _NormalizeEnvVarReferences(explicit_strip_flags)
 
             if not quiet:
                 result.append("echo STRIP\\(%s\\)" % self.spec["target_name"])
-            result.append(f"strip {strip_flags} {output_binary}")
+            result.append("strip %s %s" % (strip_flags, output_binary))
 
         self.configname = None
         return result
 
     def _GetDebugInfoPostbuilds(self, configname, output, output_binary, quiet):
         """Returns a list of shell commands that contain the shell commands
     necessary to massage this target's debug information. These should be run
@@ -1100,15 +1101,15 @@
             and self._Test(
                 "DEBUG_INFORMATION_FORMAT", "dwarf-with-dsym", default="dwarf"
             )
             and self.spec["type"] != "static_library"
         ):
             if not quiet:
                 result.append("echo DSYMUTIL\\(%s\\)" % self.spec["target_name"])
-            result.append("dsymutil {} -o {}".format(output_binary, output + ".dSYM"))
+            result.append("dsymutil %s -o %s" % (output_binary, output + ".dSYM"))
 
         self.configname = None
         return result
 
     def _GetTargetPostbuilds(self, configname, output, output_binary, quiet=False):
         """Returns a list of shell commands that contain the shell commands
     to run as postbuilds for this target, before the actual postbuilds."""
@@ -1133,15 +1134,15 @@
         settings = self.xcode_settings[configname]
 
         # Xcode expects XCTests to be copied into the TEST_HOST dir.
         if self._IsXCTest():
             source = os.path.join("${BUILT_PRODUCTS_DIR}", product_name)
             test_host = os.path.dirname(settings.get("TEST_HOST"))
             xctest_destination = os.path.join(test_host, "PlugIns", product_name)
-            postbuilds.extend([f"ditto {source} {xctest_destination}"])
+            postbuilds.extend(["ditto %s %s" % (source, xctest_destination)])
 
         key = self._GetIOSCodeSignIdentityKey(settings)
         if not key:
             return postbuilds
 
         # Warn for any unimplemented signing xcode keys.
         unimpl = ["OTHER_CODE_SIGN_FLAGS"]
@@ -1160,15 +1161,15 @@
             frameworks = [
                 "Developer/Library/PrivateFrameworks/IDEBundleInjection.framework",
                 "Developer/Library/Frameworks/XCTest.framework",
             ]
             for framework in frameworks:
                 source = os.path.join(platform_root, framework)
                 destination = os.path.join(frameworks_dir, os.path.basename(framework))
-                postbuilds.extend([f"ditto {source} {destination}"])
+                postbuilds.extend(["ditto %s %s" % (source, destination)])
 
                 # Then re-sign everything with 'preserve=True'
                 postbuilds.extend(
                     [
                         '%s code-sign-bundle "%s" "%s" "%s" "%s" %s'
                         % (
                             os.path.join("${TARGET_BUILD_DIR}", "gyp-mac-tool"),
@@ -1241,15 +1242,18 @@
         return pre + postbuilds + post
 
     def _AdjustLibrary(self, library, config_name=None):
         if library.endswith(".framework"):
             l_flag = "-framework " + os.path.splitext(os.path.basename(library))[0]
         else:
             m = self.library_re.match(library)
-            l_flag = "-l" + m.group(1) if m else library
+            if m:
+                l_flag = "-l" + m.group(1)
+            else:
+                l_flag = library
 
         sdk_root = self._SdkPath(config_name)
         if not sdk_root:
             sdk_root = ""
         # Xcode 7 started shipping with ".tbd" (text based stubs) files instead of
         # ".dylib" without providing a real support for them. What it does, for
         # "/usr/lib" libraries, is do "-L/usr/lib -lname" which is dependent on the
@@ -1358,15 +1362,15 @@
                 sdk_root = items[-1]
                 sdk_path = self._XcodeSdkPath(sdk_root)
                 if sdk_path == default_sdk_path:
                     return sdk_root
         return ""
 
 
-class MacPrefixHeader:
+class MacPrefixHeader(object):
     """A class that helps with emulating Xcode's GCC_PREFIX_HEADER feature.
 
   This feature consists of several pieces:
   * If GCC_PREFIX_HEADER is present, all compilations in that project get an
     additional |-include path_to_prefix_header| cflag.
   * If GCC_PRECOMPILE_PREFIX_HEADER is present too, then the prefix header is
     instead compiled, and all other compilations in the project get an
@@ -1520,53 +1524,55 @@
     """Returns the version of command-line tools from pkgutil."""
     # pkgutil output looks like
     #   package-id: com.apple.pkg.CLTools_Executables
     #   version: 5.0.1.0.1.1382131676
     #   volume: /
     #   location: /
     #   install-time: 1382544035
-    #   groups: com.apple.FindSystemFiles.pkg-group
-    #           com.apple.DevToolsBoth.pkg-group
-    #           com.apple.DevToolsNonRelocatableShared.pkg-group
+    #   groups: com.apple.FindSystemFiles.pkg-group com.apple.DevToolsBoth.pkg-group com.apple.DevToolsNonRelocatableShared.pkg-group
     STANDALONE_PKG_ID = "com.apple.pkg.DeveloperToolsCLILeo"
     FROM_XCODE_PKG_ID = "com.apple.pkg.DeveloperToolsCLI"
     MAVERICKS_PKG_ID = "com.apple.pkg.CLTools_Executables"
 
     regex = re.compile("version: (?P<version>.+)")
     for key in [MAVERICKS_PKG_ID, STANDALONE_PKG_ID, FROM_XCODE_PKG_ID]:
         try:
             output = GetStdout(["/usr/sbin/pkgutil", "--pkg-info", key])
             return re.search(regex, output).groupdict()["version"]
         except GypError:
             continue
 
-    regex = re.compile(r"Command Line Tools for Xcode\s+(?P<version>\S+)")
+    regex = re.compile(r'Command Line Tools for Xcode\s+(?P<version>\S+)')
     try:
         output = GetStdout(["/usr/sbin/softwareupdate", "--history"])
         return re.search(regex, output).groupdict()["version"]
     except GypError:
         return None
 
 
 def GetStdoutQuiet(cmdlist):
     """Returns the content of standard output returned by invoking |cmdlist|.
   Ignores the stderr.
   Raises |GypError| if the command return with a non-zero return code."""
     job = subprocess.Popen(cmdlist, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    out = job.communicate()[0].decode("utf-8")
+    out = job.communicate()[0]
+    if PY3:
+        out = out.decode("utf-8")
     if job.returncode != 0:
         raise GypError("Error %d running %s" % (job.returncode, cmdlist[0]))
     return out.rstrip("\n")
 
 
 def GetStdout(cmdlist):
     """Returns the content of standard output returned by invoking |cmdlist|.
   Raises |GypError| if the command return with a non-zero return code."""
     job = subprocess.Popen(cmdlist, stdout=subprocess.PIPE)
-    out = job.communicate()[0].decode("utf-8")
+    out = job.communicate()[0]
+    if PY3:
+        out = out.decode("utf-8")
     if job.returncode != 0:
         sys.stderr.write(out + "\n")
         raise GypError("Error %d running %s" % (job.returncode, cmdlist[0]))
     return out.rstrip("\n")
 
 
 def MergeGlobalXcodeSettingsToSpec(global_dict, spec):
@@ -1722,16 +1728,15 @@
 
     # These are filled in on an as-needed basis.
     env = {
         "BUILT_FRAMEWORKS_DIR": built_products_dir,
         "BUILT_PRODUCTS_DIR": built_products_dir,
         "CONFIGURATION": configuration,
         "PRODUCT_NAME": xcode_settings.GetProductName(),
-        # For FULL_PRODUCT_NAME see:
-        # /Developer/Platforms/MacOSX.platform/Developer/Library/Xcode/Specifications/MacOSX\ Product\ Types.xcspec  # noqa: E501
+        # See /Developer/Platforms/MacOSX.platform/Developer/Library/Xcode/Specifications/MacOSX\ Product\ Types.xcspec for FULL_PRODUCT_NAME
         "SRCROOT": srcroot,
         "SOURCE_ROOT": "${SRCROOT}",
         # This is not true for static libraries, but currently the env is only
         # written for bundles:
         "TARGET_BUILD_DIR": built_products_dir,
         "TEMP_DIR": "${TMPDIR}",
         "XCODE_VERSION_ACTUAL": XcodeVersion()[0],
@@ -1854,15 +1859,15 @@
 
     def GetEdges(node):
         # Use a definition of edges such that user_of_variable -> used_varible.
         # This happens to be easier in this case, since a variable's
         # definition contains all variables it references in a single string.
         # We can then reverse the result of the topological sort at the end.
         # Since: reverse(topsort(DAG)) = topsort(reverse_edges(DAG))
-        matches = {v for v in regex.findall(env[node]) if v in env}
+        matches = set([v for v in regex.findall(env[node]) if v in env])
         for dependee in matches:
             assert "${" not in dependee, "Nested variables not supported: " + dependee
         return matches
 
     try:
         # Topologically sort, and then reverse, because we used an edge definition
         # that's inverted from the expected result of this function (see comment
```

### Comparing `gyp-next-0.15.0/pylib/gyp/xcode_ninja.py` & `gyp-next-0.4.0/pylib/gyp/xcode_ninja.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
         name = xml.sax.saxutils.quoteattr("group:" + name)
         output_string += "  <FileRef location = %s></FileRef>\n" % name
     output_string += "</Workspace>\n"
 
     workspace_file = os.path.join(workspace_path, "contents.xcworkspacedata")
 
     try:
-        with open(workspace_file) as input_file:
+        with open(workspace_file, "r") as input_file:
             input_string = input_file.read()
             if input_string == output_string:
                 return
-    except OSError:
+    except IOError:
         # Ignore errors if the file doesn't exist.
         pass
 
     with open(workspace_file, "w") as output_file:
         output_file.write(output_string)
 
 
@@ -210,15 +210,15 @@
     target_extras = generator_flags.get("xcode_ninja_target_pattern", None)
 
     for old_qualified_target in target_list:
         spec = target_dicts[old_qualified_target]
         if IsValidTargetForWrapper(target_extras, executable_target_pattern, spec):
             # Add to new_target_list.
             target_name = spec.get("target_name")
-            new_target_name = f"{main_gyp}:{target_name}#target"
+            new_target_name = "%s:%s#target" % (main_gyp, target_name)
             new_target_list.append(new_target_name)
 
             # Add to new_target_dicts.
             new_target_dicts[new_target_name] = _TargetFromSpec(spec, params)
 
             # Add to new_data.
             for old_target in data[old_qualified_target.split(":")[0]]["targets"]:
@@ -278,15 +278,15 @@
             os.path.relpath(os.path.join(base, file), relative_path) for file in files
         ]
 
     sources_target["sources"] = sorted(set(sources))
 
     # Put sources_to_index in it's own gyp.
     sources_gyp = os.path.join(os.path.dirname(main_gyp), sources_target_name + ".gyp")
-    fully_qualified_target_name = f"{sources_gyp}:{sources_target_name}#target"
+    fully_qualified_target_name = "%s:%s#target" % (sources_gyp, sources_target_name)
 
     # Add to new_target_list, new_target_dicts and new_data.
     new_target_list.append(fully_qualified_target_name)
     new_target_dicts[fully_qualified_target_name] = sources_target
     new_data_target = {}
     new_data_target["target_name"] = sources_target["target_name"]
     new_data_target["_DEPTH"] = depth
```

### Comparing `gyp-next-0.15.0/pylib/gyp/xcodeproj_file.py` & `gyp-next-0.4.0/pylib/gyp/xcodeproj_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,25 +134,27 @@
 are assumed to already be encoded in UTF-8.  Obviously, if you're just using
 ASCII, you won't encounter difficulties because ASCII is a UTF-8 subset.
 Strings of class unicode are handled properly and encoded in UTF-8 when
 a project file is output.
 """
 
 import gyp.common
-from functools import cmp_to_key
 import hashlib
-from operator import attrgetter
 import posixpath
 import re
 import struct
 import sys
 
+try:
+    basestring, cmp, unicode
+except NameError:  # Python 3
+    basestring = unicode = str
 
-def cmp(x, y):
-    return (x > y) - (x < y)
+    def cmp(x, y):
+        return (x > y) - (x < y)
 
 
 # See XCObject._EncodeString.  This pattern is used to determine when a string
 # can be printed unquoted.  Strings that match this pattern may be printed
 # unquoted.  Strings that do not match must be quoted and may be further
 # transformed to be properly encoded.  Note that this expression matches the
 # characters listed with "+", for 1 or more occurrences: if a string is empty,
@@ -193,15 +195,15 @@
     return (source_tree, output_path)
 
 
 def ConvertVariablesToShellSyntax(input_string):
     return re.sub(r"\$\((.*?)\)", "${\\1}", input_string)
 
 
-class XCObject:
+class XCObject(object):
     """The abstract base of all class types used in Xcode project files.
 
   Class variables:
     _schema: A dictionary defining the properties of this class.  The keys to
              _schema are string property keys as used in project files.  Values
              are a list of four or five elements:
              [ is_list, property_type, is_strong, is_required, default ]
@@ -295,16 +297,16 @@
         self._SetDefaultsFromSchema()
         self.UpdateProperties(properties)
 
     def __repr__(self):
         try:
             name = self.Name()
         except NotImplementedError:
-            return f"<{self.__class__.__name__} at 0x{id(self):x}>"
-        return f"<{self.__class__.__name__} {name!r} at 0x{id(self):x}>"
+            return "<%s at 0x%x>" % (self.__class__.__name__, id(self))
+        return "<%s %r at 0x%x>" % (self.__class__.__name__, name, id(self))
 
     def Copy(self):
         """Make a copy of this object.
 
     The new object will have its own copy of lists and dicts.  Any XCObject
     objects owned by this object (marked "strong") will be copied in the
     new object, even those found in lists.  If this object has any weak
@@ -319,15 +321,15 @@
             if isinstance(value, XCObject):
                 if is_strong:
                     new_value = value.Copy()
                     new_value.parent = that
                     that._properties[key] = new_value
                 else:
                     that._properties[key] = value
-            elif isinstance(value, (str, int)):
+            elif isinstance(value, (basestring, int)):
                 that._properties[key] = value
             elif isinstance(value, list):
                 if is_strong:
                     # If is_strong is True, each element is an XCObject, so it's safe to
                     # call Copy.
                     that._properties[key] = []
                     for item in value:
@@ -421,16 +423,14 @@
       If the hash were updated only with the value of data, it would be
       possible for clowns to induce collisions by manipulating the names of
       their objects.  By adding the length, it's exceedingly less likely that
       ID collisions will be encountered, intentionally or not.
       """
 
             hash.update(struct.pack(">i", len(data)))
-            if isinstance(data, str):
-                data = data.encode("utf-8")
             hash.update(data)
 
         if seed_hash is None:
             seed_hash = hashlib.sha1()
 
         hash = seed_hash.copy()
 
@@ -511,15 +511,15 @@
     def PBXProjectAncestor(self):
         # The base case for recursion is defined at PBXProject.PBXProjectAncestor.
         if self.parent:
             return self.parent.PBXProjectAncestor()
         return None
 
     def _EncodeComment(self, comment):
-        """Encodes a comment to be placed in the project file output, mimicking
+        """Encodes a comment to be placed in the project file output, mimicing
     Xcode behavior.
     """
 
         # This mimics Xcode behavior by wrapping the comment in "/*" and "*/".  If
         # the string already contains a "*/", it is turned into "(*)/".  This keeps
         # the file writer from outputting something that would be treated as the
         # end of a comment in the middle of something intended to be entirely a
@@ -539,15 +539,15 @@
         if char == "\\":
             return "\\\\"
         if char == '"':
             return '\\"'
         return self._encode_transforms[ord(char)]
 
     def _EncodeString(self, value):
-        """Encodes a string to be placed in the project file output, mimicking
+        """Encodes a string to be placed in the project file output, mimicing
     Xcode behavior.
     """
 
         # Use quotation marks when any character outside of the range A-Z, a-z, 0-9,
         # $ (dollar sign), . (period), and _ (underscore) is present.  Also use
         # quotation marks to represent empty strings.
         #
@@ -582,15 +582,15 @@
         return '"' + _escaped.sub(self._EncodeTransform, value) + '"'
 
     def _XCPrint(self, file, tabs, line):
         file.write("\t" * tabs + line)
 
     def _XCPrintableValue(self, tabs, value, flatten_list=False):
         """Returns a representation of value that may be printed in a project file,
-    mimicking Xcode's behavior.
+    mimicing Xcode's behavior.
 
     _XCPrintableValue can handle str and int values, XCObjects (which are
     made printable by returning their id property), and list and dict objects
     composed of any of the above types.  When printing a list or dict, and
     _should_print_single_line is False, the tabs parameter is used to determine
     how much to indent the lines corresponding to the items in the list or
     dict.
@@ -612,15 +612,15 @@
             end_tabs = "\t" * tabs
 
         if isinstance(value, XCObject):
             printable += value.id
             comment = value.Comment()
         elif isinstance(value, str):
             printable += self._EncodeString(value)
-        elif isinstance(value, str):
+        elif isinstance(value, basestring):
             printable += self._EncodeString(value.encode("utf-8"))
         elif isinstance(value, int):
             printable += str(value)
         elif isinstance(value, list):
             if flatten_list and len(value) <= 1:
                 if len(value) == 0:
                     printable += self._EncodeString("")
@@ -787,30 +787,30 @@
                         + " of "
                         + self.__class__.__name__
                         + " must be list, not "
                         + value.__class__.__name__
                     )
                 for item in value:
                     if not isinstance(item, property_type) and not (
-                        isinstance(item, str) and property_type == str
+                        isinstance(item, basestring) and property_type == str
                     ):
                         # Accept unicode where str is specified.  str is treated as
                         # UTF-8-encoded.
                         raise TypeError(
                             "item of "
                             + property
                             + " of "
                             + self.__class__.__name__
                             + " must be "
                             + property_type.__name__
                             + ", not "
                             + item.__class__.__name__
                         )
             elif not isinstance(value, property_type) and not (
-                isinstance(value, str) and property_type == str
+                isinstance(value, basestring) and property_type == str
             ):
                 # Accept unicode where str is specified.  str is treated as
                 # UTF-8-encoded.
                 raise TypeError(
                     property
                     + " of "
                     + self.__class__.__name__
@@ -823,20 +823,20 @@
             # Checks passed, perform the assignment.
             if do_copy:
                 if isinstance(value, XCObject):
                     if is_strong:
                         self._properties[property] = value.Copy()
                     else:
                         self._properties[property] = value
-                elif isinstance(value, (str, int)):
+                elif isinstance(value, (basestring, int)):
                     self._properties[property] = value
                 elif isinstance(value, list):
                     if is_strong:
-                        # If is_strong is True, each element is an XCObject,
-                        # so it's safe to call Copy.
+                        # If is_strong is True, each element is an XCObject, so it's safe
+                        # to call Copy.
                         self._properties[property] = []
                         for item in value:
                             self._properties[property].append(item.Copy())
                     else:
                         self._properties[property] = value[:]
                 elif isinstance(value, dict):
                     self._properties[property] = value.copy()
@@ -1483,15 +1483,15 @@
         if recurse:
             for child in self._properties["children"]:
                 if child.__class__ == PBXGroup:
                     child.TakeOverOnlyChild(recurse)
 
     def SortGroup(self):
         self._properties["children"] = sorted(
-            self._properties["children"], key=cmp_to_key(lambda x, y: x.Compare(y))
+            self._properties["children"], cmp=lambda x, y: x.Compare(y)
         )
 
         # Recurse.
         for child in self._properties["children"]:
             if isinstance(child, PBXGroup):
                 child.SortGroup()
 
@@ -2128,31 +2128,29 @@
                     # BUILT_PRODUCTS_DIR, e.g.
                     # $(BUILT_PRODUCTS_DIR)/$(PLUGINS_FOLDER_PATH). Then
                     # xcode_emulation.py can export these variables with the same values
                     # as Xcode yet make & ninja files can determine the absolute path
                     # to the target. Xcode uses the dstSubfolderSpec value set here
                     # to determine the full path.
                     #
-                    # An alternative of xcode_emulation.py setting the values to
-                    # absolute paths when exporting these variables has been
-                    # ruled out because then the values would be different
-                    # depending on the build tool.
+                    # An alternative of xcode_emulation.py setting the values to absolute
+                    # paths when exporting these variables has been ruled out because
+                    # then the values would be different depending on the build tool.
                     #
                     # Another alternative is to invent new names for the variables used
                     # to match to the subfolder indices in the second table. .gyp files
                     # then will not need to prepend $(BUILT_PRODUCTS_DIR) because
                     # xcode_emulation.py can set the values of those variables to
                     # the absolute paths when exporting. This is possibly the thinking
                     # behind BUILT_FRAMEWORKS_DIR which is used in exactly this manner.
                     #
                     # Requiring prepending BUILT_PRODUCTS_DIR has been chosen because
                     # this same way could be used to specify destinations in .gyp files
                     # that pre-date this addition to GYP. However they would only work
-                    # with the Xcode generator.
-                    # The previous version of xcode_emulation.py
+                    # with the Xcode generator. The previous version of xcode_emulation.py
                     # does not export these variables. Such files will get the benefit
                     # of the Xcode UI showing the proper destination name simply by
                     # regenerating the projects with this version of GYP.
                     path_tree = path_tree_match.group(4)
                     relative_path = path_tree_match.group(6)
                     separator = "/"
 
@@ -2181,15 +2179,15 @@
                 relative_path = path
         elif path.startswith("/"):
             # Special case.  Absolute paths are in dstSubfolderSpec 0.
             subfolder = 0
             relative_path = path[1:]
         else:
             raise ValueError(
-                f"Can't use path {path} in a {self.__class__.__name__}"
+                "Can't use path %s in a %s" % (path, self.__class__.__name__)
             )
 
         self._properties["dstPath"] = relative_path
         self._properties["dstSubfolderSpec"] = subfolder
 
 
 class PBXBuildRule(XCObject):
@@ -2246,16 +2244,16 @@
             "remoteGlobalIDString": [0, XCRemoteObject, 0, 1],
             "remoteInfo": [0, str, 0, 1],
         }
     )
 
     def __repr__(self):
         props = self._properties
-        name = "{}.gyp:{}".format(props["containerPortal"].Name(), props["remoteInfo"])
-        return f"<{self.__class__.__name__} {name!r} at 0x{id(self):x}>"
+        name = "%s.gyp:%s" % (props["containerPortal"].Name(), props["remoteInfo"])
+        return "<%s %r at 0x%x>" % (self.__class__.__name__, name, id(self))
 
     def Name(self):
         # Admittedly not the best name, but it's what Xcode uses.
         return self.__class__.__name__
 
     def Hashables(self):
         # super
@@ -2284,15 +2282,15 @@
             "target": [0, None.__class__, 0, 0],
             "targetProxy": [0, PBXContainerItemProxy, 1, 1],
         }
     )
 
     def __repr__(self):
         name = self._properties.get("name") or self._properties["target"].Name()
-        return f"<{self.__class__.__name__} {name!r} at 0x{id(self):x}>"
+        return "<%s %r at 0x%x>" % (self.__class__.__name__, name, id(self))
 
     def Name(self):
         # Admittedly not the best name, but it's what Xcode uses.
         return self.__class__.__name__
 
     def Hashables(self):
         # super
@@ -2351,16 +2349,17 @@
         # super
         XCRemoteObject.__init__(self, properties, id, parent)
 
         # Set up additional defaults not expressed in the schema.  If a "name"
         # property was supplied, set "productName" if it is not present.  Also set
         # the "PRODUCT_NAME" build setting in each configuration, but only if
         # the setting is not present in any build configuration.
-        if "name" in self._properties and "productName" not in self._properties:
-            self.SetProperty("productName", self._properties["name"])
+        if "name" in self._properties:
+            if "productName" not in self._properties:
+                self.SetProperty("productName", self._properties["name"])
 
         if "productName" in self._properties:
             if "buildConfigurationList" in self._properties:
                 configs = self._properties["buildConfigurationList"]
                 if configs.HasBuildSetting("PRODUCT_NAME") == 0:
                     configs.SetBuildSetting(
                         "PRODUCT_NAME", self._properties["productName"]
@@ -2546,16 +2545,17 @@
                         force_extension = suffix[1:]
 
                 if (
                     self._properties["productType"]
                     == "com.apple.product-type-bundle.unit.test"
                     or self._properties["productType"]
                     == "com.apple.product-type-bundle.ui-testing"
-                ) and force_extension is None:
-                    force_extension = suffix[1:]
+                ):
+                    if force_extension is None:
+                        force_extension = suffix[1:]
 
                 if force_extension is not None:
                     # If it's a wrapper (bundle), set WRAPPER_EXTENSION.
                     # Extension override.
                     suffix = "." + force_extension
                     if filetype.startswith("wrapper."):
                         self.SetBuildSetting("WRAPPER_EXTENSION", force_extension)
@@ -2630,21 +2630,18 @@
         if headers_phase is None:
             headers_phase = PBXHeadersBuildPhase()
 
             # The headers phase should come before the resources, sources, and
             # frameworks phases, if any.
             insert_at = len(self._properties["buildPhases"])
             for index, phase in enumerate(self._properties["buildPhases"]):
-                if isinstance(
-                    phase,
-                    (
-                        PBXResourcesBuildPhase,
-                        PBXSourcesBuildPhase,
-                        PBXFrameworksBuildPhase,
-                    ),
+                if (
+                    isinstance(phase, PBXResourcesBuildPhase)
+                    or isinstance(phase, PBXSourcesBuildPhase)
+                    or isinstance(phase, PBXFrameworksBuildPhase)
                 ):
                     insert_at = index
                     break
 
             self._properties["buildPhases"].insert(insert_at, headers_phase)
             headers_phase.parent = self
 
@@ -2655,15 +2652,17 @@
         if resources_phase is None:
             resources_phase = PBXResourcesBuildPhase()
 
             # The resources phase should come before the sources and frameworks
             # phases, if any.
             insert_at = len(self._properties["buildPhases"])
             for index, phase in enumerate(self._properties["buildPhases"]):
-                if isinstance(phase, (PBXSourcesBuildPhase, PBXFrameworksBuildPhase)):
+                if isinstance(phase, PBXSourcesBuildPhase) or isinstance(
+                    phase, PBXFrameworksBuildPhase
+                ):
                     insert_at = index
                     break
 
             self._properties["buildPhases"].insert(insert_at, resources_phase)
             resources_phase.parent = self
 
         return resources_phase
@@ -2765,15 +2764,15 @@
         }
     )
 
     def __init__(self, properties=None, id=None, parent=None, path=None):
         self.path = path
         self._other_pbxprojects = {}
         # super
-        XCContainerPortal.__init__(self, properties, id, parent)
+        return XCContainerPortal.__init__(self, properties, id, parent)
 
     def Name(self):
         name = self.path
         if name[-10:] == ".xcodeproj":
             name = name[:-10]
         return posixpath.basename(name)
 
@@ -2890,15 +2889,15 @@
                 group.TakeOverOnlyChild(recurse)
 
     def SortGroups(self):
         # Sort the children of the mainGroup (like "Source" and "Products")
         # according to their defined order.
         self._properties["mainGroup"]._properties["children"] = sorted(
             self._properties["mainGroup"]._properties["children"],
-            key=cmp_to_key(lambda x, y: x.CompareRootGroup(y)),
+            cmp=lambda x, y: x.CompareRootGroup(y),
         )
 
         # Sort everything else by putting group before files, and going
         # alphabetically by name within sections of groups and files.  SortGroup
         # is recursive.
         for group in self._properties["mainGroup"]._properties["children"]:
             if not isinstance(group, PBXGroup):
@@ -2985,15 +2984,17 @@
             ref_dict = {"ProductGroup": product_group, "ProjectRef": project_ref}
             self._other_pbxprojects[other_pbxproject] = ref_dict
             self.AppendProperty("projectReferences", ref_dict)
 
             # Xcode seems to sort this list case-insensitively
             self._properties["projectReferences"] = sorted(
                 self._properties["projectReferences"],
-                key=lambda x: x["ProjectRef"].Name().lower()
+                cmp=lambda x, y: cmp(
+                    x["ProjectRef"].Name().lower(), y["ProjectRef"].Name().lower()
+                ),
             )
         else:
             # The link already exists.  Pull out the relevnt data.
             project_ref_dict = self._other_pbxprojects[other_pbxproject]
             product_group = project_ref_dict["ProductGroup"]
             project_ref = project_ref_dict["ProjectRef"]
 
@@ -3117,16 +3118,15 @@
                 remote_products.append(target._properties["productReference"])
 
             # Sort the PBXReferenceProxy children according to the list of remote
             # products.
             product_group = ref_dict["ProductGroup"]
             product_group._properties["children"] = sorted(
                 product_group._properties["children"],
-                key=cmp_to_key(
-                    lambda x, y, rp=remote_products: CompareProducts(x, y, rp)),
+                cmp=lambda x, y, rp=remote_products: CompareProducts(x, y, rp),
             )
 
 
 class XCProjectFile(XCObject):
     _schema = XCObject._schema.copy()
     _schema.update(
         {
@@ -3153,15 +3153,15 @@
         self._properties["objects"] = {}
         self._XCPrint(file, 0, "// !$*UTF8*$!\n")
         if self._should_print_single_line:
             self._XCPrint(file, 0, "{ ")
         else:
             self._XCPrint(file, 0, "{\n")
         for property, value in sorted(
-            self._properties.items()
+            self._properties.items(), cmp=lambda x, y: cmp(x, y)
         ):
             if property == "objects":
                 self._PrintObjects(file)
             else:
                 self._XCKVPrint(file, 1, property, value)
         self._XCPrint(file, 0, "}\n")
         del self._properties["objects"]
@@ -3181,15 +3181,15 @@
                 objects_by_class[class_name] = []
             objects_by_class[class_name].append(object)
 
         for class_name in sorted(objects_by_class):
             self._XCPrint(file, 0, "\n")
             self._XCPrint(file, 0, "/* Begin " + class_name + " section */\n")
             for object in sorted(
-                objects_by_class[class_name], key=attrgetter("id")
+                objects_by_class[class_name], cmp=lambda x, y: cmp(x.id, y.id)
             ):
                 object.Print(file)
             self._XCPrint(file, 0, "/* End " + class_name + " section */\n")
 
         if self._should_print_single_line:
             self._XCPrint(file, 0, "}; ")
         else:
```

### Comparing `gyp-next-0.15.0/pylib/gyp/xml_fix.py` & `gyp-next-0.4.0/pylib/gyp/xml_fix.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,20 +35,20 @@
         writer.write(' %s="' % a_name)
         _Replacement_write_data(writer, attrs[a_name].value, is_attrib=True)
         writer.write('"')
     if self.childNodes:
         writer.write(">%s" % newl)
         for node in self.childNodes:
             node.writexml(writer, indent + addindent, addindent, newl)
-        writer.write(f"{indent}</{self.tagName}>{newl}")
+        writer.write("%s</%s>%s" % (indent, self.tagName, newl))
     else:
         writer.write("/>%s" % newl)
 
 
-class XmlFix:
+class XmlFix(object):
     """Object to manage temporary patching of xml.dom.minidom."""
 
     def __init__(self):
         # Preserve current xml.dom.minidom functions.
         self.write_data = xml.dom.minidom._write_data
         self.writexml = xml.dom.minidom.Element.writexml
         # Inject replacement versions of a function and a method.
```

### Comparing `gyp-next-0.15.0/pylib/gyp_next.egg-info/SOURCES.txt` & `gyp-next-0.4.0/pylib/gyp_next.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-AUTHORS
-LICENSE
 README.md
-pyproject.toml
+setup.py
 pylib/gyp/MSVSNew.py
 pylib/gyp/MSVSProject.py
 pylib/gyp/MSVSSettings.py
 pylib/gyp/MSVSSettings_test.py
 pylib/gyp/MSVSToolFile.py
 pylib/gyp/MSVSUserFile.py
 pylib/gyp/MSVSUtil.py
@@ -43,9 +41,8 @@
 pylib/gyp/generator/ninja_test.py
 pylib/gyp/generator/xcode.py
 pylib/gyp/generator/xcode_test.py
 pylib/gyp_next.egg-info/PKG-INFO
 pylib/gyp_next.egg-info/SOURCES.txt
 pylib/gyp_next.egg-info/dependency_links.txt
 pylib/gyp_next.egg-info/entry_points.txt
-pylib/gyp_next.egg-info/requires.txt
 pylib/gyp_next.egg-info/top_level.txt
```

