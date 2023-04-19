# Comparing `tmp/github_poster-2.5.0.tar.gz` & `tmp/github_poster-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_poster-2.5.0.tar", last modified: Fri Apr  7 14:03:51 2023, max compression
+gzip compressed data, was "github_poster-2.5.1.tar", last modified: Wed Apr 19 01:23:59 2023, max compression
```

## Comparing `github_poster-2.5.0.tar` & `github_poster-2.5.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-07 14:03:51.405170 github_poster-2.5.0/
--rw-r--r--   0 hyi        (502) staff       (20)     1063 2022-03-17 02:50:19.000000 github_poster-2.5.0/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      439 2023-04-07 14:03:51.404900 github_poster-2.5.0/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)    24111 2023-04-07 14:00:22.000000 github_poster-2.5.0/README.md
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-07 14:03:51.339227 github_poster-2.5.0/github_poster/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       74 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)     6361 2023-03-23 07:14:27.000000 github_poster-2.5.0/github_poster/circluar_drawer.py
--rw-r--r--   0 hyi        (502) staff       (20)     6547 2023-03-23 07:14:27.000000 github_poster-2.5.0/github_poster/cli.py
--rw-r--r--   0 hyi        (502) staff       (20)     1134 2023-04-07 14:03:10.000000 github_poster-2.5.0/github_poster/config.py
--rw-r--r--   0 hyi        (502) staff       (20)     9710 2023-03-23 04:29:50.000000 github_poster-2.5.0/github_poster/drawer.py
--rw-r--r--   0 hyi        (502) staff       (20)      261 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/err.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-07 14:03:51.355601 github_poster-2.5.0/github_poster/html_parser/
--rw-r--r--   0 hyi        (502) staff       (20)      206 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/html_parser/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     1143 2023-01-09 06:11:32.000000 github_poster-2.5.0/github_poster/html_parser/github_parser.py
--rw-r--r--   0 hyi        (502) staff       (20)      256 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/html_parser/gitlab_parser.py
--rw-r--r--   0 hyi        (502) staff       (20)     2005 2022-07-12 13:26:45.000000 github_poster-2.5.0/github_poster/html_parser/jike_parse.py
--rw-r--r--   0 hyi        (502) staff       (20)      257 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/html_parser/kindle_parser.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-07 14:03:51.400518 github_poster-2.5.0/github_poster/loader/
--rw-r--r--   0 hyi        (502) staff       (20)     3482 2023-04-07 14:01:44.000000 github_poster-2.5.0/github_poster/loader/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     5187 2023-03-31 14:51:05.000000 github_poster-2.5.0/github_poster/loader/apple_health_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     7132 2023-03-23 07:14:27.000000 github_poster-2.5.0/github_poster/loader/base_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     4148 2022-11-24 13:04:14.000000 github_poster-2.5.0/github_poster/loader/bbdc_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3296 2022-10-08 00:21:43.000000 github_poster-2.5.0/github_poster/loader/bilibili_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1864 2023-04-07 14:02:07.000000 github_poster-2.5.0/github_poster/loader/chatgpt_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3287 2022-11-24 13:04:14.000000 github_poster-2.5.0/github_poster/loader/cichang_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     6322 2023-03-23 04:29:50.000000 github_poster-2.5.0/github_poster/loader/config.py
--rw-r--r--   0 hyi        (502) staff       (20)     1960 2022-07-12 13:26:45.000000 github_poster-2.5.0/github_poster/loader/covid_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1559 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/dota2_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2660 2023-01-09 10:28:31.000000 github_poster-2.5.0/github_poster/loader/duolingo_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2494 2022-11-24 13:04:14.000000 github_poster-2.5.0/github_poster/loader/forest_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2826 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/from_github_issue_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2795 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/garmin_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1547 2022-11-24 14:02:11.000000 github_poster-2.5.0/github_poster/loader/github_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3407 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/gitlab_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3166 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/gpx_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     7133 2022-11-24 13:04:14.000000 github_poster-2.5.0/github_poster/loader/jike_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1095 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/json_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1678 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/kindle_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2595 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/leetcode_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1393 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/multiple_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3095 2023-03-23 07:14:27.000000 github_poster-2.5.0/github_poster/loader/notion_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3763 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/nrc_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3321 2022-04-13 04:14:41.000000 github_poster-2.5.0/github_poster/loader/ns_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3437 2023-03-23 04:29:50.000000 github_poster-2.5.0/github_poster/loader/openlanguage_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1637 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/shanbay_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3141 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/strava_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)      965 2023-03-23 07:14:27.000000 github_poster-2.5.0/github_poster/loader/summary_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     5285 2023-03-31 14:51:00.000000 github_poster-2.5.0/github_poster/loader/todoist_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1828 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/twitter_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1807 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/wakatime_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     2134 2022-11-24 13:15:31.000000 github_poster-2.5.0/github_poster/loader/weread_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     1640 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/loader/youtube_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3849 2022-11-24 13:04:14.000000 github_poster-2.5.0/github_poster/poster.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-07 14:03:51.402300 github_poster-2.5.0/github_poster/skyline/
--rw-r--r--   0 hyi        (502) staff       (20)       74 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/skyline/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)      185 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/skyline/config.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-07 14:03:51.402886 github_poster-2.5.0/github_poster/skyline/font/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/skyline/font/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)     4008 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/skyline/skyline.py
--rw-r--r--   0 hyi        (502) staff       (20)     1674 2022-03-17 02:50:20.000000 github_poster-2.5.0/github_poster/structures.py
--rw-r--r--   0 hyi        (502) staff       (20)     2211 2023-01-09 14:20:16.000000 github_poster-2.5.0/github_poster/utils.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-07 14:03:51.352577 github_poster-2.5.0/github_poster.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      439 2023-04-07 14:03:51.000000 github_poster-2.5.0/github_poster.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     2205 2023-04-07 14:03:51.000000 github_poster-2.5.0/github_poster.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2023-04-07 14:03:51.000000 github_poster-2.5.0/github_poster.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       57 2023-04-07 14:03:51.000000 github_poster-2.5.0/github_poster.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)      243 2023-04-07 14:03:51.000000 github_poster-2.5.0/github_poster.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       20 2023-04-07 14:03:51.000000 github_poster-2.5.0/github_poster.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)       31 2022-03-17 02:50:20.000000 github_poster-2.5.0/pyproject.toml
--rw-r--r--   0 hyi        (502) staff       (20)       38 2023-04-07 14:03:51.405240 github_poster-2.5.0/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1028 2023-04-07 14:03:37.000000 github_poster-2.5.0/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-07 14:03:51.404450 github_poster-2.5.0/tests/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2022-03-17 02:50:20.000000 github_poster-2.5.0/tests/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)      732 2022-03-17 02:50:20.000000 github_poster-2.5.0/tests/test_poster_utils.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.668129 github_poster-2.5.1/
+-rw-r--r--   0 hyi        (502) staff       (20)     1063 2022-03-17 02:50:19.000000 github_poster-2.5.1/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      439 2023-04-19 01:23:59.667199 github_poster-2.5.1/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)    24221 2023-04-18 14:37:48.000000 github_poster-2.5.1/README.md
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.609786 github_poster-2.5.1/github_poster/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       74 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6361 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/circluar_drawer.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6547 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/cli.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1134 2023-04-18 13:39:47.000000 github_poster-2.5.1/github_poster/config.py
+-rw-r--r--   0 hyi        (502) staff       (20)     9710 2023-03-23 04:29:50.000000 github_poster-2.5.1/github_poster/drawer.py
+-rw-r--r--   0 hyi        (502) staff       (20)      261 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/err.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.623035 github_poster-2.5.1/github_poster/html_parser/
+-rw-r--r--   0 hyi        (502) staff       (20)      206 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/html_parser/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1143 2023-01-09 06:11:32.000000 github_poster-2.5.1/github_poster/html_parser/github_parser.py
+-rw-r--r--   0 hyi        (502) staff       (20)      256 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/html_parser/gitlab_parser.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2005 2022-07-12 13:26:45.000000 github_poster-2.5.1/github_poster/html_parser/jike_parse.py
+-rw-r--r--   0 hyi        (502) staff       (20)      257 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/html_parser/kindle_parser.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.662958 github_poster-2.5.1/github_poster/loader/
+-rw-r--r--   0 hyi        (502) staff       (20)     3482 2023-04-18 13:39:47.000000 github_poster-2.5.1/github_poster/loader/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5187 2023-03-31 14:51:05.000000 github_poster-2.5.1/github_poster/loader/apple_health_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     7132 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/loader/base_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4148 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/loader/bbdc_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3296 2022-10-08 00:21:43.000000 github_poster-2.5.1/github_poster/loader/bilibili_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2196 2023-04-18 13:39:47.000000 github_poster-2.5.1/github_poster/loader/chatgpt_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3287 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/loader/cichang_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6322 2023-03-23 04:29:50.000000 github_poster-2.5.1/github_poster/loader/config.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1960 2022-07-12 13:26:45.000000 github_poster-2.5.1/github_poster/loader/covid_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1559 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/dota2_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2470 2023-04-19 01:23:31.000000 github_poster-2.5.1/github_poster/loader/duolingo_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2494 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/loader/forest_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2826 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/from_github_issue_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2795 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/garmin_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1547 2022-11-24 14:02:11.000000 github_poster-2.5.1/github_poster/loader/github_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3407 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/gitlab_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3166 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/gpx_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     7133 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/loader/jike_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1095 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/json_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1678 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/kindle_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2595 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/leetcode_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1393 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/multiple_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3095 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/loader/notion_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3763 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/nrc_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3321 2022-04-13 04:14:41.000000 github_poster-2.5.1/github_poster/loader/ns_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3437 2023-03-23 04:29:50.000000 github_poster-2.5.1/github_poster/loader/openlanguage_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1637 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/shanbay_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3141 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/strava_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)      965 2023-03-23 07:14:27.000000 github_poster-2.5.1/github_poster/loader/summary_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5285 2023-03-31 14:51:00.000000 github_poster-2.5.1/github_poster/loader/todoist_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1828 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/twitter_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1807 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/wakatime_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2134 2022-11-24 13:15:31.000000 github_poster-2.5.1/github_poster/loader/weread_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1640 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/loader/youtube_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3849 2022-11-24 13:04:14.000000 github_poster-2.5.1/github_poster/poster.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.664339 github_poster-2.5.1/github_poster/skyline/
+-rw-r--r--   0 hyi        (502) staff       (20)       74 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/skyline/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      185 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/skyline/config.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.665020 github_poster-2.5.1/github_poster/skyline/font/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/skyline/font/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4008 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/skyline/skyline.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1674 2022-03-17 02:50:20.000000 github_poster-2.5.1/github_poster/structures.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2211 2023-01-09 14:20:16.000000 github_poster-2.5.1/github_poster/utils.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.615141 github_poster-2.5.1/github_poster.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      439 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     2205 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       57 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)      243 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       20 2023-04-19 01:23:59.000000 github_poster-2.5.1/github_poster.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       31 2022-03-17 02:50:20.000000 github_poster-2.5.1/pyproject.toml
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2023-04-19 01:23:59.668202 github_poster-2.5.1/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1028 2023-04-19 01:23:46.000000 github_poster-2.5.1/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-19 01:23:59.666681 github_poster-2.5.1/tests/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2022-03-17 02:50:20.000000 github_poster-2.5.1/tests/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      732 2022-03-17 02:50:20.000000 github_poster-2.5.1/tests/test_poster_utils.py
```

### Comparing `github_poster-2.5.0/LICENSE` & `github_poster-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/README.md` & `github_poster-2.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -192,18 +192,23 @@
 
 ### 多邻国
 
 <details>
 <summary>Make your <code>多邻国（duolingo）</code> GitHub poster</summary>
 <br>
 
+1. login duolingo in broswer
+2. console `document.cookie.match(new RegExp('(^| )jwt_token=([^;]+)'))[0].slice(11)` get duolingo_jwt
+3. 点击 profile call 接口拿到你的 duolingo_id
+
+
 ```
-python3 -m github_poster duolingo --duolingo_user_name ${user_id} --duolingo_password ${user_password} --year 2015-2021
+python3 -m github_poster duolingo --duolingo_id ${user_id} --duolingo_jwt ${duolingo_jwt} --year 2015-2021
 or
-github_poster duolingo --duolingo_user_name ${user_id} --duolingo_password ${user_password} --year 2015-2021
+github_poster duolingo --duolingo_id ${user_id} --duolingo_duolingo_jwtpassword ${duolingo_jwt} --year 2015-2021
 ```
 </details>
 
 ### 扇贝
 
 <details>
 <summary>Make your <code>扇贝（shanbay）</code> GitHub poster</summary>
@@ -662,18 +667,18 @@
 ```
 
 </details>
 
 ### ChatGPT
 
 <details>
-<summary>Make your <code>YouChatGPTTube </code> GitHub poster</summary>
+<summary>Make your <code> ChatGPT </code> GitHub poster</summary>
 <br>
 
-利用这个项目下载 ChatGPT 的[历史下载](https://github.com/abacaj/chatgpt-backup)下载 `ChatGPT` 的历史数据， 拷贝到 `IN-FOLDER` 然后运行(重命名为 chatgpt-history.json)
+将ChatGPT官方导出的历史记录中的conversations.json， 拷贝到 `IN-FOLDER` 然后运行(重命名为 chatgpt-history.json)
 
 ```
 python3 -m github_poster chatgpt 
 or
 github_poster chatgpt --me yihong0618
 ```
 </details>
```

### Comparing `github_poster-2.5.0/github_poster/circluar_drawer.py` & `github_poster-2.5.1/github_poster/circluar_drawer.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/cli.py` & `github_poster-2.5.1/github_poster/cli.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/config.py` & `github_poster-2.5.1/github_poster/config.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/drawer.py` & `github_poster-2.5.1/github_poster/drawer.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/html_parser/github_parser.py` & `github_poster-2.5.1/github_poster/html_parser/github_parser.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/html_parser/jike_parse.py` & `github_poster-2.5.1/github_poster/html_parser/jike_parse.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/__init__.py` & `github_poster-2.5.1/github_poster/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/apple_health_loader.py` & `github_poster-2.5.1/github_poster/loader/apple_health_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/base_loader.py` & `github_poster-2.5.1/github_poster/loader/base_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/bbdc_loader.py` & `github_poster-2.5.1/github_poster/loader/bbdc_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/bilibili_loader.py` & `github_poster-2.5.1/github_poster/loader/bilibili_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/chatgpt_loader.py` & `github_poster-2.5.1/github_poster/loader/json_loader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,38 @@
 import json
-import os
 from collections import defaultdict
 
-import pendulum
-
 from github_poster.loader.base_loader import BaseLoader
 
 
-class ChatGPTLoader(BaseLoader):
-    track_color = "#70A597"
+class JsonLoader(BaseLoader):
     unit = "times"
 
     def __init__(self, from_year, to_year, _type, **kwargs):
         super().__init__(from_year, to_year, _type)
         self.number_by_date_dict = defaultdict(int)
-        self.youtube_file = kwargs.get("chatgpt_history_file")
+        self.json_file = kwargs.get("json_file")
 
     @classmethod
     def add_loader_arguments(cls, parser, optional):
         parser.add_argument(
-            "--chatgpt_history_file",
-            dest="chatgpt_history_file",
+            "--json_file",
+            dest="json_file",
             type=str,
-            default=os.path.join("IN_FOLDER", "chatgpt-history.json"),
-            help="chatgpt history file path",
+            default="data.json",
+            help="json file path",
         )
 
-    def _parse_chatgpt_history(self):
-        base_file = self.youtube_file
-        data_list = []
-        with open(base_file) as f:
-            data_list = json.load(f)
-        return data_list
-
     def get_api_data(self):
-        return self._parse_chatgpt_history()
+        pass
 
     def make_track_dict(self):
-        tracks = self.get_api_data()
-        for t in tracks:
-            t = t["messages"]
-            user_ask_list = [i for i in t if i.get("role", "") == "user"]
-            for ask in user_ask_list:
-                date_time = pendulum.from_timestamp(
-                    int(ask["create_time"]), tz=self.time_zone
-                )
-                if date_time.year < self.from_year:
-                    break
-                date = date_time.to_date_string()
-                self.number_by_date_dict[date] += 1
+        with open(self.json_file, "r") as f:
+            tracks = json.load(f)
+        self.number_by_date_dict = tracks
         for _, v in self.number_by_date_dict.items():
             self.number_list.append(v)
         return tracks
 
     def get_all_track_data(self):
         self.make_track_dict()
         self.make_special_number()
```

### Comparing `github_poster-2.5.0/github_poster/loader/cichang_loader.py` & `github_poster-2.5.1/github_poster/loader/cichang_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/config.py` & `github_poster-2.5.1/github_poster/loader/config.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/covid_loader.py` & `github_poster-2.5.1/github_poster/loader/covid_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/dota2_loader.py` & `github_poster-2.5.1/github_poster/loader/dota2_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/duolingo_loader.py` & `github_poster-2.5.1/github_poster/loader/duolingo_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,50 +7,42 @@
 
 class DuolingoLoader(BaseLoader):
     unit = "XP"
     track_color = "#78C800"
 
     def __init__(self, from_year, to_year, _type, **kwargs):
         super().__init__(from_year, to_year, _type)
-        self.user_name = kwargs.get("duolingo_user_name", "")
-        self.password = kwargs.get("duolingo_password", "")
+        self.duolingo_id = kwargs.get("duolingo_user_id", "")
+        self.duolingo_jwt = kwargs.get("duolingo_jwt", "")
         self.session = requests.Session()
         self.headers = {
             "Accept": "*/*",
             "User-Agent": "request",
         }
-        # duolingo name to get the calendar
-        self.duolingo_id = ""
 
     @classmethod
     def add_loader_arguments(cls, parser, optional):
         parser.add_argument(
-            "--duolingo_user_name",
-            dest="duolingo_user_name",
+            "--duolingo_user_id",
+            dest="duolingo_user_id",
             type=str,
             help="",
             required=optional,
         )
         parser.add_argument(
-            "--duolingo_password",
-            dest="duolingo_password",
+            "--duolingo_jwt",
+            dest="duolingo_jwt",
             type=str,
-            help="",
+            help="use `document.cookie.match(new RegExp('(^| )jwt_token=([^;]+)'))[0].slice(11)` in console",
             required=optional,
         )
 
     def login(self):
-        r = self.session.post(
-            DUOLINGO_LOGIN_URL,
-            params={"login": self.user_name, "password": self.password},
-            headers=self.headers,
-        )
-        if r.status_code != 200:
-            raise Exception("Login failed")
-        self.duolingo_id = r.json()["user_id"]
+        self.headers["Authorization"] = "Bearer " + self.duolingo_jwt
+        self.duolingo_id = self.duolingo_id
 
     def get_api_data(self):
         month_list = self.make_month_list()
         for m in month_list:
             r = self.session.get(
                 DUOLINGO_CALENDAR_API.format(
                     user_id=self.duolingo_id,
```

### Comparing `github_poster-2.5.0/github_poster/loader/forest_loader.py` & `github_poster-2.5.1/github_poster/loader/forest_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/from_github_issue_loader.py` & `github_poster-2.5.1/github_poster/loader/from_github_issue_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/garmin_loader.py` & `github_poster-2.5.1/github_poster/loader/garmin_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/github_loader.py` & `github_poster-2.5.1/github_poster/loader/github_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/gitlab_loader.py` & `github_poster-2.5.1/github_poster/loader/gitlab_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/gpx_loader.py` & `github_poster-2.5.1/github_poster/loader/gpx_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/jike_loader.py` & `github_poster-2.5.1/github_poster/loader/jike_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/json_loader.py` & `github_poster-2.5.1/github_poster/loader/summary_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-import json
-from collections import defaultdict
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
 
 from github_poster.loader.base_loader import BaseLoader
 
 
-class JsonLoader(BaseLoader):
-    unit = "times"
-
+class SummaryLoader(BaseLoader):
     def __init__(self, from_year, to_year, _type, **kwargs):
         super().__init__(from_year, to_year, _type)
-        self.number_by_date_dict = defaultdict(int)
-        self.json_file = kwargs.get("json_file")
+        self.types = kwargs.get("types", "")
+        self.type_summary_dict = {}
+        self.loader_list = []
+
+    def set_loader_list(self, loader):
+        self.loader_list.append(loader)
 
     @classmethod
     def add_loader_arguments(cls, parser, optional):
         parser.add_argument(
-            "--json_file",
-            dest="json_file",
+            "--types",
+            dest="types",
             type=str,
-            default="data.json",
-            help="json file path",
+            required=True,
+            help="All types you want to generate summary, split by comma",
         )
 
+        for loader in cls.parser_loader_list:
+            loader.add_loader_arguments(parser, optional)
+
     def get_api_data(self):
         pass
 
     def make_track_dict(self):
-        with open(self.json_file, "r") as f:
-            tracks = json.load(f)
-        self.number_by_date_dict = tracks
-        for _, v in self.number_by_date_dict.items():
-            self.number_list.append(v)
-        return tracks
+        pass
 
     def get_all_track_data(self):
-        self.make_track_dict()
-        self.make_special_number()
-        return self.number_by_date_dict, self.year_list
+        pass
```

### Comparing `github_poster-2.5.0/github_poster/loader/kindle_loader.py` & `github_poster-2.5.1/github_poster/loader/kindle_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/leetcode_loader.py` & `github_poster-2.5.1/github_poster/loader/leetcode_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/multiple_loader.py` & `github_poster-2.5.1/github_poster/loader/multiple_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/notion_loader.py` & `github_poster-2.5.1/github_poster/loader/notion_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/nrc_loader.py` & `github_poster-2.5.1/github_poster/loader/nrc_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/ns_loader.py` & `github_poster-2.5.1/github_poster/loader/ns_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/openlanguage_loader.py` & `github_poster-2.5.1/github_poster/loader/openlanguage_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/shanbay_loader.py` & `github_poster-2.5.1/github_poster/loader/shanbay_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/strava_loader.py` & `github_poster-2.5.1/github_poster/loader/strava_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/todoist_loader.py` & `github_poster-2.5.1/github_poster/loader/todoist_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/twitter_loader.py` & `github_poster-2.5.1/github_poster/loader/twitter_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/wakatime_loader.py` & `github_poster-2.5.1/github_poster/loader/wakatime_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/weread_loader.py` & `github_poster-2.5.1/github_poster/loader/weread_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/loader/youtube_loader.py` & `github_poster-2.5.1/github_poster/loader/youtube_loader.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/poster.py` & `github_poster-2.5.1/github_poster/poster.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/skyline/skyline.py` & `github_poster-2.5.1/github_poster/skyline/skyline.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/structures.py` & `github_poster-2.5.1/github_poster/structures.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster/utils.py` & `github_poster-2.5.1/github_poster/utils.py`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/github_poster.egg-info/SOURCES.txt` & `github_poster-2.5.1/github_poster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `github_poster-2.5.0/setup.py` & `github_poster-2.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name="github_poster",
     author="yihong0618",
     author_email="zouzou0208@gmail.com",
     url="https://github.com/yihong0618/GitHubPoster",
     license="MIT",
-    version="2.5.0",
+    version="2.5.1",
     description="Make everything a GitHub svg poster and Skyline!",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "requests",
         "svgwrite",
         "pendulum",
```

### Comparing `github_poster-2.5.0/tests/test_poster_utils.py` & `github_poster-2.5.1/tests/test_poster_utils.py`

 * *Files identical despite different names*

