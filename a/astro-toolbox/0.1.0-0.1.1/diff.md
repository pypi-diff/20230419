# Comparing `tmp/astro-toolbox-0.1.0.tar.gz` & `tmp/astro-toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-toolbox-0.1.0.tar", last modified: Tue Apr 18 19:03:35 2023, max compression
+gzip compressed data, was "astro-toolbox-0.1.1.tar", last modified: Wed Apr 19 18:57:26 2023, max compression
```

## Comparing `astro-toolbox-0.1.0.tar` & `astro-toolbox-0.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.529279 astro-toolbox-0.1.0/
--rw-r--r--   0 romain     (501) staff       (20)    35160 2023-02-26 19:51:45.000000 astro-toolbox-0.1.0/LICENSE
--rw-r--r--   0 romain     (501) staff       (20)     4669 2023-04-18 19:03:35.529370 astro-toolbox-0.1.0/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)     3847 2023-04-18 16:51:39.000000 astro-toolbox-0.1.0/README.md
--rw-r--r--   0 romain     (501) staff       (20)     1422 2023-04-18 19:03:35.529703 astro-toolbox-0.1.0/setup.cfg
--rw-r--r--   0 romain     (501) staff       (20)       68 2023-01-06 19:50:39.000000 astro-toolbox-0.1.0/setup.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.516848 astro-toolbox-0.1.0/src/
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.519550 astro-toolbox-0.1.0/src/astro_toolbox/
--rw-r--r--   0 romain     (501) staff       (20)      968 2023-04-18 19:02:43.000000 astro-toolbox-0.1.0/src/astro_toolbox/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)       88 2023-02-07 20:30:19.000000 astro-toolbox-0.1.0/src/astro_toolbox/__main__.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.522139 astro-toolbox-0.1.0/src/astro_toolbox/angle/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.0/src/astro_toolbox/angle/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     2170 2023-03-10 13:03:07.000000 astro-toolbox-0.1.0/src/astro_toolbox/angle/degrees.py
--rw-r--r--   0 romain     (501) staff       (20)     1665 2023-03-10 13:01:21.000000 astro-toolbox-0.1.0/src/astro_toolbox/angle/dms.py
--rw-r--r--   0 romain     (501) staff       (20)     1579 2023-03-10 13:04:29.000000 astro-toolbox-0.1.0/src/astro_toolbox/angle/hms.py
--rw-r--r--   0 romain     (501) staff       (20)     2230 2023-03-10 13:06:25.000000 astro-toolbox-0.1.0/src/astro_toolbox/angle/radians.py
--rw-r--r--   0 romain     (501) staff       (20)    12587 2023-04-18 18:49:19.000000 astro-toolbox-0.1.0/src/astro_toolbox/command_line.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.522986 astro-toolbox-0.1.0/src/astro_toolbox/coordinates/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.0/src/astro_toolbox/coordinates/__init__.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.523370 astro-toolbox-0.1.0/src/astro_toolbox/coordinates/data/
--rw-r--r--   0 romain     (501) staff       (20)     2451 2023-02-02 19:46:48.000000 astro-toolbox-0.1.0/src/astro_toolbox/coordinates/data/orbital_elements.json
--rw-r--r--   0 romain     (501) staff       (20)      419 2023-04-17 18:44:34.000000 astro-toolbox-0.1.0/src/astro_toolbox/coordinates/data/sites.json
--rw-r--r--   0 romain     (501) staff       (20)     8253 2023-03-10 13:34:41.000000 astro-toolbox-0.1.0/src/astro_toolbox/coordinates/equatorial.py
--rw-r--r--   0 romain     (501) staff       (20)     3299 2023-03-10 13:34:22.000000 astro-toolbox-0.1.0/src/astro_toolbox/coordinates/horizontal.py
--rw-r--r--   0 romain     (501) staff       (20)     6648 2023-03-10 13:36:16.000000 astro-toolbox-0.1.0/src/astro_toolbox/coordinates/location.py
--rw-r--r--   0 romain     (501) staff       (20)    11831 2023-03-10 13:22:52.000000 astro-toolbox-0.1.0/src/astro_toolbox/coordinates/solar_system.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.523979 astro-toolbox-0.1.0/src/astro_toolbox/query/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-08 12:07:57.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     2415 2023-03-10 13:41:22.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/catalogs.py
--rw-r--r--   0 romain     (501) staff       (20)     3925 2023-04-17 19:20:22.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/ephemeris.py
--rw-r--r--   0 romain     (501) staff       (20)     9961 2023-04-18 18:34:45.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.527892 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/
--rw-r--r--   0 romain     (501) staff       (20)      457 2023-04-17 20:13:59.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/cloudy.png
--rw-r--r--   0 romain     (501) staff       (20)      200 2023-04-17 18:29:15.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/direction_down.png
--rw-r--r--   0 romain     (501) staff       (20)      193 2023-04-17 18:29:15.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/direction_down_left.png
--rw-r--r--   0 romain     (501) staff       (20)      220 2023-04-17 18:29:15.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/direction_down_right.png
--rw-r--r--   0 romain     (501) staff       (20)      256 2023-04-17 18:29:15.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/direction_left.png
--rw-r--r--   0 romain     (501) staff       (20)      215 2023-04-17 18:29:15.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/direction_right.png
--rw-r--r--   0 romain     (501) staff       (20)      270 2023-04-17 18:29:15.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/direction_up.png
--rw-r--r--   0 romain     (501) staff       (20)      243 2023-04-17 18:29:15.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/direction_up_left.png
--rw-r--r--   0 romain     (501) staff       (20)      228 2023-04-17 18:29:15.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/direction_up_right.png
--rw-r--r--   0 romain     (501) staff       (20)      519 2023-04-17 20:23:18.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/drizzle.png
--rw-r--r--   0 romain     (501) staff       (20)      388 2023-04-17 20:22:30.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/fog.png
--rw-r--r--   0 romain     (501) staff       (20)      470 2023-04-17 21:01:44.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/haze.png
--rw-r--r--   0 romain     (501) staff       (20)      613 2023-04-18 05:58:24.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/mainly_clear.png
--rw-r--r--   0 romain     (501) staff       (20)      329 2023-04-17 20:17:22.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/na.png
--rw-r--r--   0 romain     (501) staff       (20)      467 2023-04-17 21:07:00.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/partly_cloudy.png
--rw-r--r--   0 romain     (501) staff       (20)      555 2023-04-17 20:23:54.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/rain.png
--rw-r--r--   0 romain     (501) staff       (20)      545 2023-04-17 21:14:52.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/rain_mix.png
--rw-r--r--   0 romain     (501) staff       (20)      410 2023-04-17 20:21:39.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/sandstorm.png
--rw-r--r--   0 romain     (501) staff       (20)      525 2023-04-17 20:25:57.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/showers.png
--rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 20:24:39.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/snow.png
--rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 15:03:01.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/sunny.png
--rw-r--r--   0 romain     (501) staff       (20)      576 2023-04-17 21:16:48.000000 astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/thunderstorm.png
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.528455 astro-toolbox-0.1.0/src/astro_toolbox/scripts/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-17 20:03:46.000000 astro-toolbox-0.1.0/src/astro_toolbox/scripts/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     1780 2023-02-08 13:53:17.000000 astro-toolbox-0.1.0/src/astro_toolbox/scripts/planning.py
--rw-r--r--   0 romain     (501) staff       (20)    17118 2023-04-18 14:18:07.000000 astro-toolbox-0.1.0/src/astro_toolbox/scripts/plots.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.528792 astro-toolbox-0.1.0/src/astro_toolbox/time/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:53:46.000000 astro-toolbox-0.1.0/src/astro_toolbox/time/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     6330 2023-04-17 16:55:55.000000 astro-toolbox-0.1.0/src/astro_toolbox/time/core.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.529129 astro-toolbox-0.1.0/src/astro_toolbox/utils/
--rw-r--r--   0 romain     (501) staff       (20)      441 2023-02-08 13:53:35.000000 astro-toolbox-0.1.0/src/astro_toolbox/utils/python_functions.py
--rw-r--r--   0 romain     (501) staff       (20)      659 2023-04-17 16:11:48.000000 astro-toolbox-0.1.0/src/astro_toolbox/utils/strparser.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 19:03:35.521140 astro-toolbox-0.1.0/src/astro_toolbox.egg-info/
--rw-r--r--   0 romain     (501) staff       (20)     4669 2023-04-18 19:03:35.000000 astro-toolbox-0.1.0/src/astro_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)     2480 2023-04-18 19:03:35.000000 astro-toolbox-0.1.0/src/astro_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-04-18 19:03:35.000000 astro-toolbox-0.1.0/src/astro_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 romain     (501) staff       (20)       62 2023-04-18 19:03:35.000000 astro-toolbox-0.1.0/src/astro_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-01-18 11:00:43.000000 astro-toolbox-0.1.0/src/astro_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 romain     (501) staff       (20)      152 2023-04-18 19:03:35.000000 astro-toolbox-0.1.0/src/astro_toolbox.egg-info/requires.txt
--rw-r--r--   0 romain     (501) staff       (20)       14 2023-04-18 19:03:35.000000 astro-toolbox-0.1.0/src/astro_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.868938 astro-toolbox-0.1.1/
+-rw-r--r--   0 romain     (501) staff       (20)    35160 2023-02-26 19:51:45.000000 astro-toolbox-0.1.1/LICENSE
+-rw-r--r--   0 romain     (501) staff       (20)     4669 2023-04-19 18:57:26.869075 astro-toolbox-0.1.1/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)     3847 2023-04-18 16:51:39.000000 astro-toolbox-0.1.1/README.md
+-rw-r--r--   0 romain     (501) staff       (20)     1422 2023-04-19 18:57:26.869450 astro-toolbox-0.1.1/setup.cfg
+-rw-r--r--   0 romain     (501) staff       (20)       68 2023-01-06 19:50:39.000000 astro-toolbox-0.1.1/setup.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.854486 astro-toolbox-0.1.1/src/
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.856502 astro-toolbox-0.1.1/src/astro_toolbox/
+-rw-r--r--   0 romain     (501) staff       (20)      968 2023-04-19 18:42:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)       88 2023-02-07 20:30:19.000000 astro-toolbox-0.1.1/src/astro_toolbox/__main__.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.858699 astro-toolbox-0.1.1/src/astro_toolbox/angle/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     2170 2023-03-10 13:03:07.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/degrees.py
+-rw-r--r--   0 romain     (501) staff       (20)     1665 2023-03-10 13:01:21.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/dms.py
+-rw-r--r--   0 romain     (501) staff       (20)     1579 2023-03-10 13:04:29.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/hms.py
+-rw-r--r--   0 romain     (501) staff       (20)     2230 2023-03-10 13:06:25.000000 astro-toolbox-0.1.1/src/astro_toolbox/angle/radians.py
+-rw-r--r--   0 romain     (501) staff       (20)    12587 2023-04-18 18:49:19.000000 astro-toolbox-0.1.1/src/astro_toolbox/command_line.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.859502 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/__init__.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.859976 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/data/
+-rw-r--r--   0 romain     (501) staff       (20)     2451 2023-02-02 19:46:48.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/data/orbital_elements.json
+-rw-r--r--   0 romain     (501) staff       (20)      419 2023-04-17 18:44:34.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/data/sites.json
+-rw-r--r--   0 romain     (501) staff       (20)     8253 2023-03-10 13:34:41.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/equatorial.py
+-rw-r--r--   0 romain     (501) staff       (20)     3299 2023-03-10 13:34:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/horizontal.py
+-rw-r--r--   0 romain     (501) staff       (20)     6995 2023-04-19 18:56:14.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/location.py
+-rw-r--r--   0 romain     (501) staff       (20)    11831 2023-03-10 13:22:52.000000 astro-toolbox-0.1.1/src/astro_toolbox/coordinates/solar_system.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.860719 astro-toolbox-0.1.1/src/astro_toolbox/query/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-08 12:07:57.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     2415 2023-03-10 13:41:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/catalogs.py
+-rw-r--r--   0 romain     (501) staff       (20)     3925 2023-04-17 19:20:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/ephemeris.py
+-rw-r--r--   0 romain     (501) staff       (20)    10477 2023-04-19 18:55:51.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.867456 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/
+-rw-r--r--   0 romain     (501) staff       (20)      457 2023-04-17 20:13:59.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/cloudy.png
+-rw-r--r--   0 romain     (501) staff       (20)      200 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_down.png
+-rw-r--r--   0 romain     (501) staff       (20)      193 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_down_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      220 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_down_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      256 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      215 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      270 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_up.png
+-rw-r--r--   0 romain     (501) staff       (20)      243 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_up_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      228 2023-04-17 18:29:15.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/direction_up_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      519 2023-04-17 20:23:18.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/drizzle.png
+-rw-r--r--   0 romain     (501) staff       (20)      388 2023-04-17 20:22:30.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/fog.png
+-rw-r--r--   0 romain     (501) staff       (20)      470 2023-04-17 21:01:44.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/haze.png
+-rw-r--r--   0 romain     (501) staff       (20)      613 2023-04-18 05:58:24.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/mainly_clear.png
+-rw-r--r--   0 romain     (501) staff       (20)      329 2023-04-17 20:17:22.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/na.png
+-rw-r--r--   0 romain     (501) staff       (20)      467 2023-04-17 21:07:00.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/partly_cloudy.png
+-rw-r--r--   0 romain     (501) staff       (20)      555 2023-04-17 20:23:54.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/rain.png
+-rw-r--r--   0 romain     (501) staff       (20)      545 2023-04-17 21:14:52.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/rain_mix.png
+-rw-r--r--   0 romain     (501) staff       (20)      410 2023-04-17 20:21:39.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/sandstorm.png
+-rw-r--r--   0 romain     (501) staff       (20)      525 2023-04-17 20:25:57.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/showers.png
+-rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 20:24:39.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/snow.png
+-rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 15:03:01.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/sunny.png
+-rw-r--r--   0 romain     (501) staff       (20)      576 2023-04-17 21:16:48.000000 astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/thunderstorm.png
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.868183 astro-toolbox-0.1.1/src/astro_toolbox/scripts/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-17 20:03:46.000000 astro-toolbox-0.1.1/src/astro_toolbox/scripts/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     1780 2023-02-08 13:53:17.000000 astro-toolbox-0.1.1/src/astro_toolbox/scripts/planning.py
+-rw-r--r--   0 romain     (501) staff       (20)    17118 2023-04-18 14:18:07.000000 astro-toolbox-0.1.1/src/astro_toolbox/scripts/plots.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.868474 astro-toolbox-0.1.1/src/astro_toolbox/time/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:53:46.000000 astro-toolbox-0.1.1/src/astro_toolbox/time/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     6330 2023-04-17 16:55:55.000000 astro-toolbox-0.1.1/src/astro_toolbox/time/core.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.868808 astro-toolbox-0.1.1/src/astro_toolbox/utils/
+-rw-r--r--   0 romain     (501) staff       (20)      441 2023-02-08 13:53:35.000000 astro-toolbox-0.1.1/src/astro_toolbox/utils/python_functions.py
+-rw-r--r--   0 romain     (501) staff       (20)      659 2023-04-17 16:11:48.000000 astro-toolbox-0.1.1/src/astro_toolbox/utils/strparser.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-19 18:57:26.857816 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/
+-rw-r--r--   0 romain     (501) staff       (20)     4669 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)     2480 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 romain     (501) staff       (20)       62 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-01-18 11:00:43.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 romain     (501) staff       (20)      152 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/requires.txt
+-rw-r--r--   0 romain     (501) staff       (20)       14 2023-04-19 18:57:26.000000 astro-toolbox-0.1.1/src/astro_toolbox.egg-info/top_level.txt
```

### Comparing `astro-toolbox-0.1.0/LICENSE` & `astro-toolbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/PKG-INFO` & `astro-toolbox-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolbox for observationnal astronomy
 Home-page: https://github.com/rloustalet/astro_toolbox
 Author: Romain Loustalet Palengat
 Project-URL: Source, https://github.com/rloustalet/astro_toolbox
 Project-URL: Documentation, https://astro-toolbox.readthedocs.io/en/latest/
 Keywords: astro,toolbox,astro_toolbox,observationnal
 Platform: unix
```

### Comparing `astro-toolbox-0.1.0/README.md` & `astro-toolbox-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/setup.cfg` & `astro-toolbox-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/__init__.py` & `astro-toolbox-0.1.1/src/astro_toolbox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
     "Location",
     "Ephemeris",
     "Simbad",
     "Horizons",
     "OpenMeteo",
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/angle/degrees.py` & `astro-toolbox-0.1.1/src/astro_toolbox/angle/degrees.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/angle/dms.py` & `astro-toolbox-0.1.1/src/astro_toolbox/angle/dms.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/angle/hms.py` & `astro-toolbox-0.1.1/src/astro_toolbox/angle/hms.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/angle/radians.py` & `astro-toolbox-0.1.1/src/astro_toolbox/angle/radians.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/command_line.py` & `astro-toolbox-0.1.1/src/astro_toolbox/command_line.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/coordinates/data/orbital_elements.json` & `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/data/orbital_elements.json`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/coordinates/equatorial.py` & `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/equatorial.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/coordinates/horizontal.py` & `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/horizontal.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/coordinates/location.py` & `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,28 @@
         string
             Return a class representative string.
         """
         return (f'{self.name}: latitude: {self.latitude} '+
                 f'longitude: {self.longitude} '+
                 f'elevation = {self.elevation} m')
 
+    def compute_pressure_level(self):
+        """Pressure level computing method.
+
+        .. math:: P = 1013.25(1 - \\frac{h}{44307.694})^{5.25530}
+
+        Returns
+        -------
+        float
+            Pressure level in hPa.
+        """
+        return (1013.25 *
+                (1 - self.elevation /
+                44307.694) ** 5.25530)
+
     def save_site(self):
         """Method to save current site in sites file.
 
         Raises
         ------
         KeyError
             The first level key already exist.
```

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/coordinates/solar_system.py` & `astro-toolbox-0.1.1/src/astro_toolbox/coordinates/solar_system.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/query/catalogs.py` & `astro-toolbox-0.1.1/src/astro_toolbox/query/catalogs.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/query/ephemeris.py` & `astro-toolbox-0.1.1/src/astro_toolbox/query/ephemeris.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/query/weather.py` & `astro-toolbox-0.1.1/src/astro_toolbox/query/weather.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,34 @@
 import json
 import urllib.request as urllib
 import math
 
 from astro_toolbox.time.core import AstroDateTime
 from astro_toolbox.coordinates.location import Location
 
+OPENMETEO_LEVELS = [1000,
+                    975,
+                    950,
+                    925,
+                    900,
+                    850,
+                    800,
+                    700,
+                    600,
+                    500,
+                    400,
+                    300,
+                    250,
+                    200,
+                    150,
+                    100,
+                    70,
+                    50,
+                    30]
+
 class OpenMeteo():
     """OpenMeteo service request and parsing.
 
     Attributes
     ----------
     location : Location
             Observer location as Location class.
@@ -24,15 +44,20 @@
         ----------
         location : Location
             Observer location as Location class.
         model : str, optional
             Weather model (https://open-meteo.com/en/docs), by default 'best_match'
         """
         self.location = location
-        self.pressure_level = self.get_pressure_level()
+        pressure_level = self.location.compute_pressure_level()
+        index_pressure_level = list(abs(openmeteo_pressure_level - pressure_level)
+                                for openmeteo_pressure_level in OPENMETEO_LEVELS).index(
+                                min(list(abs(openmeteo_pressure_level - pressure_level)
+                                for openmeteo_pressure_level in OPENMETEO_LEVELS)))
+        self.pressure_level = OPENMETEO_LEVELS[index_pressure_level]
         self.model = model
         self.data = self._get_data()
 
     def __repr__(self):
         """Representative method.
 
         Returns
@@ -91,28 +116,14 @@
         """
         datetime = AstroDateTime(datetime)
         datetime_str = str(datetime)[:-5]+'00'
         if datetime_str not in self.data['hourly']['time']:
             return float('nan')
         return self.data['hourly']['time'].index(datetime_str)
 
-    def get_pressure_level(self):
-        """Pressure level computing method.
-
-        .. math:: P = 1013.25(1 - \\frac{h}{44307.694})^{5.25530}
-
-        Returns
-        -------
-        int
-            10^2 rounded pressure level in hPa.
-        """
-        return int(round((1013.25 *
-                (1 - self.location.elevation /
-                44307.694) ** 5.25530), -2))
-
     def get_temperature(self, datetime: str | tuple = None):
         """Get temperature method.
 
         Parameters
         ----------
         datetime : str | tuple, optional
             Date and Time as tuple (``YYYY,MM,DD,hh,mm,ss`` or ``YYYY-MM-DDThh:mm:ss``),
```

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/drizzle.png` & `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/drizzle.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/mainly_clear.png` & `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/mainly_clear.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/rain.png` & `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/rain.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/rain_mix.png` & `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/rain_mix.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/showers.png` & `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/showers.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/query/weather_icons/thunderstorm.png` & `astro-toolbox-0.1.1/src/astro_toolbox/query/weather_icons/thunderstorm.png`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/scripts/planning.py` & `astro-toolbox-0.1.1/src/astro_toolbox/scripts/planning.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/scripts/plots.py` & `astro-toolbox-0.1.1/src/astro_toolbox/scripts/plots.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/time/core.py` & `astro-toolbox-0.1.1/src/astro_toolbox/time/core.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox/utils/strparser.py` & `astro-toolbox-0.1.1/src/astro_toolbox/utils/strparser.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox.egg-info/PKG-INFO` & `astro-toolbox-0.1.1/src/astro_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolbox for observationnal astronomy
 Home-page: https://github.com/rloustalet/astro_toolbox
 Author: Romain Loustalet Palengat
 Project-URL: Source, https://github.com/rloustalet/astro_toolbox
 Project-URL: Documentation, https://astro-toolbox.readthedocs.io/en/latest/
 Keywords: astro,toolbox,astro_toolbox,observationnal
 Platform: unix
```

### Comparing `astro-toolbox-0.1.0/src/astro_toolbox.egg-info/SOURCES.txt` & `astro-toolbox-0.1.1/src/astro_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

