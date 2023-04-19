# Comparing `tmp/shinyswatch-0.2.0.tar.gz` & `tmp/shinyswatch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinyswatch-0.2.0.tar", last modified: Fri Apr 14 20:43:52 2023, max compression
+gzip compressed data, was "shinyswatch-0.2.1.tar", last modified: Wed Apr 19 01:10:56 2023, max compression
```

## Comparing `shinyswatch-0.2.0.tar` & `shinyswatch-0.2.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.133769 shinyswatch-0.2.0/
--rw-r--r--   0 barret     (502) staff       (20)     1067 2023-03-29 18:28:41.000000 shinyswatch-0.2.0/LICENSE
--rw-r--r--   0 barret     (502) staff       (20)      252 2023-04-12 20:21:07.000000 shinyswatch-0.2.0/MANIFEST.in
--rw-r--r--   0 barret     (502) staff       (20)     2729 2023-04-14 20:43:52.133902 shinyswatch-0.2.0/PKG-INFO
--rw-r--r--   0 barret     (502) staff       (20)     1479 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/README.md
--rw-r--r--   0 barret     (502) staff       (20)     1891 2023-04-14 20:43:52.134356 shinyswatch-0.2.0/setup.cfg
--rw-r--r--   0 barret     (502) staff       (20)       38 2023-03-23 14:55:23.000000 shinyswatch-0.2.0/setup.py
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.104700 shinyswatch-0.2.0/shinyswatch/
--rw-r--r--   0 barret     (502) staff       (20)      171 2023-04-14 20:41:18.000000 shinyswatch-0.2.0/shinyswatch/__init__.py
--rw-r--r--   0 barret     (502) staff       (20)      491 2023-04-12 20:21:07.000000 shinyswatch-0.2.0/shinyswatch/_assert.py
--rw-r--r--   0 barret     (502) staff       (20)      890 2023-04-14 18:14:54.000000 shinyswatch-0.2.0/shinyswatch/_bsw5.py
--rw-r--r--   0 barret     (502) staff       (20)     9336 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/shinyswatch/_get_theme.py
--rw-r--r--   0 barret     (502) staff       (20)     2583 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/shinyswatch/_shiny_theme.py
--rw-r--r--   0 barret     (502) staff       (20)      917 2023-04-12 20:21:07.000000 shinyswatch-0.2.0/shinyswatch/_typing_extensions.py
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.106504 shinyswatch-0.2.0/shinyswatch/bs5/
--rw-r--r--   0 barret     (502) staff       (20)    80496 2023-04-14 18:14:46.000000 shinyswatch-0.2.0/shinyswatch/bs5/bootstrap.bundle.min.js
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.101947 shinyswatch-0.2.0/shinyswatch/bsw5/
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.107313 shinyswatch-0.2.0/shinyswatch/bsw5/cerulean/
--rw-r--r--   0 barret     (502) staff       (20)   241305 2023-04-14 18:14:46.000000 shinyswatch-0.2.0/shinyswatch/bsw5/cerulean/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.108151 shinyswatch-0.2.0/shinyswatch/bsw5/cosmo/
--rw-r--r--   0 barret     (502) staff       (20)   228137 2023-04-14 18:14:47.000000 shinyswatch-0.2.0/shinyswatch/bsw5/cosmo/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.108633 shinyswatch-0.2.0/shinyswatch/bsw5/cyborg/
--rw-r--r--   0 barret     (502) staff       (20)   239795 2023-04-14 18:14:47.000000 shinyswatch-0.2.0/shinyswatch/bsw5/cyborg/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.109704 shinyswatch-0.2.0/shinyswatch/bsw5/darkly/
--rw-r--r--   0 barret     (502) staff       (20)   244211 2023-04-14 18:14:47.000000 shinyswatch-0.2.0/shinyswatch/bsw5/darkly/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.110914 shinyswatch-0.2.0/shinyswatch/bsw5/flatly/
--rw-r--r--   0 barret     (502) staff       (20)   240774 2023-04-14 18:14:48.000000 shinyswatch-0.2.0/shinyswatch/bsw5/flatly/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.112146 shinyswatch-0.2.0/shinyswatch/bsw5/journal/
--rw-r--r--   0 barret     (502) staff       (20)   238362 2023-04-14 18:14:48.000000 shinyswatch-0.2.0/shinyswatch/bsw5/journal/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.113019 shinyswatch-0.2.0/shinyswatch/bsw5/litera/
--rw-r--r--   0 barret     (502) staff       (20)   240358 2023-04-14 18:14:48.000000 shinyswatch-0.2.0/shinyswatch/bsw5/litera/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.114056 shinyswatch-0.2.0/shinyswatch/bsw5/lumen/
--rw-r--r--   0 barret     (502) staff       (20)   245474 2023-04-14 18:14:48.000000 shinyswatch-0.2.0/shinyswatch/bsw5/lumen/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.114877 shinyswatch-0.2.0/shinyswatch/bsw5/lux/
--rw-r--r--   0 barret     (502) staff       (20)   229679 2023-04-14 18:14:49.000000 shinyswatch-0.2.0/shinyswatch/bsw5/lux/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.115688 shinyswatch-0.2.0/shinyswatch/bsw5/materia/
--rw-r--r--   0 barret     (502) staff       (20)   268868 2023-04-14 18:14:49.000000 shinyswatch-0.2.0/shinyswatch/bsw5/materia/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.116608 shinyswatch-0.2.0/shinyswatch/bsw5/minty/
--rw-r--r--   0 barret     (502) staff       (20)   239411 2023-04-14 18:14:49.000000 shinyswatch-0.2.0/shinyswatch/bsw5/minty/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.117389 shinyswatch-0.2.0/shinyswatch/bsw5/morph/
--rw-r--r--   0 barret     (502) staff       (20)   264987 2023-04-14 18:14:50.000000 shinyswatch-0.2.0/shinyswatch/bsw5/morph/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.118492 shinyswatch-0.2.0/shinyswatch/bsw5/pulse/
--rw-r--r--   0 barret     (502) staff       (20)   231184 2023-04-14 18:14:50.000000 shinyswatch-0.2.0/shinyswatch/bsw5/pulse/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.120425 shinyswatch-0.2.0/shinyswatch/bsw5/quartz/
--rw-r--r--   0 barret     (502) staff       (20)   275083 2023-04-14 18:14:50.000000 shinyswatch-0.2.0/shinyswatch/bsw5/quartz/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.121416 shinyswatch-0.2.0/shinyswatch/bsw5/sandstone/
--rw-r--r--   0 barret     (502) staff       (20)   241171 2023-04-14 18:14:51.000000 shinyswatch-0.2.0/shinyswatch/bsw5/sandstone/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.122402 shinyswatch-0.2.0/shinyswatch/bsw5/simplex/
--rw-r--r--   0 barret     (502) staff       (20)   241660 2023-04-14 18:14:51.000000 shinyswatch-0.2.0/shinyswatch/bsw5/simplex/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.122935 shinyswatch-0.2.0/shinyswatch/bsw5/sketchy/
--rw-r--r--   0 barret     (502) staff       (20)   245207 2023-04-14 18:14:51.000000 shinyswatch-0.2.0/shinyswatch/bsw5/sketchy/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.124424 shinyswatch-0.2.0/shinyswatch/bsw5/slate/
--rw-r--r--   0 barret     (502) staff       (20)   253193 2023-04-14 18:14:52.000000 shinyswatch-0.2.0/shinyswatch/bsw5/slate/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.126164 shinyswatch-0.2.0/shinyswatch/bsw5/solar/
--rw-r--r--   0 barret     (502) staff       (20)   239224 2023-04-14 18:14:52.000000 shinyswatch-0.2.0/shinyswatch/bsw5/solar/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.127695 shinyswatch-0.2.0/shinyswatch/bsw5/spacelab/
--rw-r--r--   0 barret     (502) staff       (20)   242824 2023-04-14 18:14:52.000000 shinyswatch-0.2.0/shinyswatch/bsw5/spacelab/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.128676 shinyswatch-0.2.0/shinyswatch/bsw5/superhero/
--rw-r--r--   0 barret     (502) staff       (20)   239767 2023-04-14 18:14:52.000000 shinyswatch-0.2.0/shinyswatch/bsw5/superhero/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.129465 shinyswatch-0.2.0/shinyswatch/bsw5/united/
--rw-r--r--   0 barret     (502) staff       (20)   237981 2023-04-14 18:14:53.000000 shinyswatch-0.2.0/shinyswatch/bsw5/united/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.130418 shinyswatch-0.2.0/shinyswatch/bsw5/vapor/
--rw-r--r--   0 barret     (502) staff       (20)   256498 2023-04-14 18:14:53.000000 shinyswatch-0.2.0/shinyswatch/bsw5/vapor/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.131201 shinyswatch-0.2.0/shinyswatch/bsw5/yeti/
--rw-r--r--   0 barret     (502) staff       (20)   249497 2023-04-14 18:14:53.000000 shinyswatch-0.2.0/shinyswatch/bsw5/yeti/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.132006 shinyswatch-0.2.0/shinyswatch/bsw5/zephyr/
--rw-r--r--   0 barret     (502) staff       (20)   246162 2023-04-14 18:14:54.000000 shinyswatch-0.2.0/shinyswatch/bsw5/zephyr/bootswatch.min.css
--rw-r--r--   0 barret     (502) staff       (20)        0 2023-03-23 14:55:23.000000 shinyswatch-0.2.0/shinyswatch/py.typed
--rw-r--r--   0 barret     (502) staff       (20)    28215 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/shinyswatch/theme.py
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.106302 shinyswatch-0.2.0/shinyswatch.egg-info/
--rw-r--r--   0 barret     (502) staff       (20)     2729 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/PKG-INFO
--rw-r--r--   0 barret     (502) staff       (20)     1625 2023-04-14 20:43:52.000000 shinyswatch-0.2.0/shinyswatch.egg-info/SOURCES.txt
--rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/dependency_links.txt
--rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/not-zip-safe
--rw-r--r--   0 barret     (502) staff       (20)      308 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/requires.txt
--rw-r--r--   0 barret     (502) staff       (20)       12 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/top_level.txt
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.133538 shinyswatch-0.2.0/tests/
--rw-r--r--   0 barret     (502) staff       (20)     6148 2023-03-29 18:47:46.000000 shinyswatch-0.2.0/tests/.DS_Store
--rw-r--r--   0 barret     (502) staff       (20)       33 2023-03-29 18:42:55.000000 shinyswatch-0.2.0/tests/__init__.py
--rw-r--r--   0 barret     (502) staff       (20)      571 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/tests/test_themes.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.429552 shinyswatch-0.2.1/
+-rw-r--r--   0 barret     (502) staff       (20)     1067 2023-03-29 18:28:41.000000 shinyswatch-0.2.1/LICENSE
+-rw-r--r--   0 barret     (502) staff       (20)      252 2023-04-12 20:21:07.000000 shinyswatch-0.2.1/MANIFEST.in
+-rw-r--r--   0 barret     (502) staff       (20)     3513 2023-04-19 01:10:56.429679 shinyswatch-0.2.1/PKG-INFO
+-rw-r--r--   0 barret     (502) staff       (20)     2269 2023-04-19 00:42:19.000000 shinyswatch-0.2.1/README.md
+-rw-r--r--   0 barret     (502) staff       (20)     1893 2023-04-19 01:10:56.430061 shinyswatch-0.2.1/setup.cfg
+-rw-r--r--   0 barret     (502) staff       (20)       38 2023-03-23 14:55:23.000000 shinyswatch-0.2.1/setup.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.402944 shinyswatch-0.2.1/shinyswatch/
+-rw-r--r--   0 barret     (502) staff       (20)      171 2023-04-18 20:45:59.000000 shinyswatch-0.2.1/shinyswatch/__init__.py
+-rw-r--r--   0 barret     (502) staff       (20)      491 2023-04-12 20:21:07.000000 shinyswatch-0.2.1/shinyswatch/_assert.py
+-rw-r--r--   0 barret     (502) staff       (20)      890 2023-04-14 18:14:54.000000 shinyswatch-0.2.1/shinyswatch/_bsw5.py
+-rw-r--r--   0 barret     (502) staff       (20)     9336 2023-04-14 20:41:01.000000 shinyswatch-0.2.1/shinyswatch/_get_theme.py
+-rw-r--r--   0 barret     (502) staff       (20)     2583 2023-04-14 20:41:01.000000 shinyswatch-0.2.1/shinyswatch/_shiny_theme.py
+-rw-r--r--   0 barret     (502) staff       (20)      917 2023-04-12 20:21:07.000000 shinyswatch-0.2.1/shinyswatch/_typing_extensions.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.404444 shinyswatch-0.2.1/shinyswatch/bs5/
+-rw-r--r--   0 barret     (502) staff       (20)    80496 2023-04-14 18:14:46.000000 shinyswatch-0.2.1/shinyswatch/bs5/bootstrap.bundle.min.js
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.398268 shinyswatch-0.2.1/shinyswatch/bsw5/
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.405585 shinyswatch-0.2.1/shinyswatch/bsw5/cerulean/
+-rw-r--r--   0 barret     (502) staff       (20)   241305 2023-04-14 18:14:46.000000 shinyswatch-0.2.1/shinyswatch/bsw5/cerulean/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.406481 shinyswatch-0.2.1/shinyswatch/bsw5/cosmo/
+-rw-r--r--   0 barret     (502) staff       (20)   228137 2023-04-14 18:14:47.000000 shinyswatch-0.2.1/shinyswatch/bsw5/cosmo/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.406947 shinyswatch-0.2.1/shinyswatch/bsw5/cyborg/
+-rw-r--r--   0 barret     (502) staff       (20)   239795 2023-04-14 18:14:47.000000 shinyswatch-0.2.1/shinyswatch/bsw5/cyborg/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.407762 shinyswatch-0.2.1/shinyswatch/bsw5/darkly/
+-rw-r--r--   0 barret     (502) staff       (20)   244211 2023-04-14 18:14:47.000000 shinyswatch-0.2.1/shinyswatch/bsw5/darkly/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.408725 shinyswatch-0.2.1/shinyswatch/bsw5/flatly/
+-rw-r--r--   0 barret     (502) staff       (20)   240774 2023-04-14 18:14:48.000000 shinyswatch-0.2.1/shinyswatch/bsw5/flatly/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.409465 shinyswatch-0.2.1/shinyswatch/bsw5/journal/
+-rw-r--r--   0 barret     (502) staff       (20)   238362 2023-04-14 18:14:48.000000 shinyswatch-0.2.1/shinyswatch/bsw5/journal/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.410086 shinyswatch-0.2.1/shinyswatch/bsw5/litera/
+-rw-r--r--   0 barret     (502) staff       (20)   240358 2023-04-14 18:14:48.000000 shinyswatch-0.2.1/shinyswatch/bsw5/litera/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.410902 shinyswatch-0.2.1/shinyswatch/bsw5/lumen/
+-rw-r--r--   0 barret     (502) staff       (20)   245474 2023-04-14 18:14:48.000000 shinyswatch-0.2.1/shinyswatch/bsw5/lumen/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.411405 shinyswatch-0.2.1/shinyswatch/bsw5/lux/
+-rw-r--r--   0 barret     (502) staff       (20)   229679 2023-04-14 18:14:49.000000 shinyswatch-0.2.1/shinyswatch/bsw5/lux/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.412114 shinyswatch-0.2.1/shinyswatch/bsw5/materia/
+-rw-r--r--   0 barret     (502) staff       (20)   268868 2023-04-14 18:14:49.000000 shinyswatch-0.2.1/shinyswatch/bsw5/materia/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.412788 shinyswatch-0.2.1/shinyswatch/bsw5/minty/
+-rw-r--r--   0 barret     (502) staff       (20)   239411 2023-04-14 18:14:49.000000 shinyswatch-0.2.1/shinyswatch/bsw5/minty/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.413244 shinyswatch-0.2.1/shinyswatch/bsw5/morph/
+-rw-r--r--   0 barret     (502) staff       (20)   264987 2023-04-14 18:14:50.000000 shinyswatch-0.2.1/shinyswatch/bsw5/morph/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.417076 shinyswatch-0.2.1/shinyswatch/bsw5/pulse/
+-rw-r--r--   0 barret     (502) staff       (20)   231184 2023-04-14 18:14:50.000000 shinyswatch-0.2.1/shinyswatch/bsw5/pulse/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.417714 shinyswatch-0.2.1/shinyswatch/bsw5/quartz/
+-rw-r--r--   0 barret     (502) staff       (20)   275083 2023-04-14 18:14:50.000000 shinyswatch-0.2.1/shinyswatch/bsw5/quartz/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.418453 shinyswatch-0.2.1/shinyswatch/bsw5/sandstone/
+-rw-r--r--   0 barret     (502) staff       (20)   241171 2023-04-14 18:14:51.000000 shinyswatch-0.2.1/shinyswatch/bsw5/sandstone/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.419161 shinyswatch-0.2.1/shinyswatch/bsw5/simplex/
+-rw-r--r--   0 barret     (502) staff       (20)   241660 2023-04-14 18:14:51.000000 shinyswatch-0.2.1/shinyswatch/bsw5/simplex/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.419595 shinyswatch-0.2.1/shinyswatch/bsw5/sketchy/
+-rw-r--r--   0 barret     (502) staff       (20)   245207 2023-04-14 18:14:51.000000 shinyswatch-0.2.1/shinyswatch/bsw5/sketchy/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.420347 shinyswatch-0.2.1/shinyswatch/bsw5/slate/
+-rw-r--r--   0 barret     (502) staff       (20)   253193 2023-04-14 18:14:52.000000 shinyswatch-0.2.1/shinyswatch/bsw5/slate/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.421837 shinyswatch-0.2.1/shinyswatch/bsw5/solar/
+-rw-r--r--   0 barret     (502) staff       (20)   239224 2023-04-14 18:14:52.000000 shinyswatch-0.2.1/shinyswatch/bsw5/solar/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.423374 shinyswatch-0.2.1/shinyswatch/bsw5/spacelab/
+-rw-r--r--   0 barret     (502) staff       (20)   242824 2023-04-14 18:14:52.000000 shinyswatch-0.2.1/shinyswatch/bsw5/spacelab/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.424500 shinyswatch-0.2.1/shinyswatch/bsw5/superhero/
+-rw-r--r--   0 barret     (502) staff       (20)   239767 2023-04-14 18:14:52.000000 shinyswatch-0.2.1/shinyswatch/bsw5/superhero/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.425310 shinyswatch-0.2.1/shinyswatch/bsw5/united/
+-rw-r--r--   0 barret     (502) staff       (20)   237981 2023-04-14 18:14:53.000000 shinyswatch-0.2.1/shinyswatch/bsw5/united/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.426314 shinyswatch-0.2.1/shinyswatch/bsw5/vapor/
+-rw-r--r--   0 barret     (502) staff       (20)   256498 2023-04-14 18:14:53.000000 shinyswatch-0.2.1/shinyswatch/bsw5/vapor/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.427062 shinyswatch-0.2.1/shinyswatch/bsw5/yeti/
+-rw-r--r--   0 barret     (502) staff       (20)   249497 2023-04-14 18:14:53.000000 shinyswatch-0.2.1/shinyswatch/bsw5/yeti/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.427830 shinyswatch-0.2.1/shinyswatch/bsw5/zephyr/
+-rw-r--r--   0 barret     (502) staff       (20)   246162 2023-04-14 18:14:54.000000 shinyswatch-0.2.1/shinyswatch/bsw5/zephyr/bootswatch.min.css
+-rw-r--r--   0 barret     (502) staff       (20)        0 2023-03-23 14:55:23.000000 shinyswatch-0.2.1/shinyswatch/py.typed
+-rw-r--r--   0 barret     (502) staff       (20)    28215 2023-04-14 20:41:01.000000 shinyswatch-0.2.1/shinyswatch/theme.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.404159 shinyswatch-0.2.1/shinyswatch.egg-info/
+-rw-r--r--   0 barret     (502) staff       (20)     3513 2023-04-19 01:10:56.000000 shinyswatch-0.2.1/shinyswatch.egg-info/PKG-INFO
+-rw-r--r--   0 barret     (502) staff       (20)     1625 2023-04-19 01:10:56.000000 shinyswatch-0.2.1/shinyswatch.egg-info/SOURCES.txt
+-rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-19 01:10:56.000000 shinyswatch-0.2.1/shinyswatch.egg-info/dependency_links.txt
+-rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-19 01:10:56.000000 shinyswatch-0.2.1/shinyswatch.egg-info/not-zip-safe
+-rw-r--r--   0 barret     (502) staff       (20)      315 2023-04-19 01:10:56.000000 shinyswatch-0.2.1/shinyswatch.egg-info/requires.txt
+-rw-r--r--   0 barret     (502) staff       (20)       12 2023-04-19 01:10:56.000000 shinyswatch-0.2.1/shinyswatch.egg-info/top_level.txt
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-19 01:10:56.429264 shinyswatch-0.2.1/tests/
+-rw-r--r--   0 barret     (502) staff       (20)     6148 2023-03-29 18:47:46.000000 shinyswatch-0.2.1/tests/.DS_Store
+-rw-r--r--   0 barret     (502) staff       (20)       33 2023-03-29 18:42:55.000000 shinyswatch-0.2.1/tests/__init__.py
+-rw-r--r--   0 barret     (502) staff       (20)      571 2023-04-14 20:41:01.000000 shinyswatch-0.2.1/tests/test_themes.py
```

### Comparing `shinyswatch-0.2.0/LICENSE` & `shinyswatch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/PKG-INFO` & `shinyswatch-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: shinyswatch
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bootswatch + Bootstrap 5 themes for Shiny.
-Home-page: https://github.com/schloerke/py-shinyswatch
+Home-page: https://github.com/rstudio/py-shinyswatch
 Author: Barret Schloerke
 Author-email: barret@posit.co
 License: MIT
-Project-URL: Bug Tracker, https://github.com/schloerke/py-shinyswatch/issues
-Project-URL: Source Code, https://github.com/schloerke/py-shinyswatch
+Project-URL: Bug Tracker, https://github.com/rstudio/py-shinyswatch/issues
+Project-URL: Source Code, https://github.com/rstudio/py-shinyswatch
 Keywords: html
 Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -30,32 +30,59 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 # shinyswatch
 
 [Bootswatch](https://bootswatch.com/) + Bootstrap 5 themes for [Shiny](https://shiny.rstudio.com/py/).
 
+
+Here are just three of the **25 themes** in shinyswatch:
+
+| Minty                      | Sketchy                        | Superhero                          |
+|----------------------------|--------------------------------|------------------------------------|
+| ![Minty](readme_minty.png) | ![Sketchy](readme_sketchy.png) | ![Superhero](readme_superhero.png) |
+
+
 ## Installation
 
 ```sh
 pip install shinyswatch
 ```
 
 To install the latest development version from this repository:
 
 ```sh
-pip install https://github.com/schloerke/py-shinyswatch/tarball/main
+pip install https://github.com/rstudio/py-shinyswatch/tarball/main
 ```
 
 ## Usage
 
-Add your theme within your App's top level UI defintion. For example:
+To use a theme, call the theme function and add it to your App's UI definition.
+
+```python
+# Minty theme
+shinyswatch.theme.minty()
+
+# Sketchy theme
+shinyswatch.theme.sketchy()
+
+# Superhero theme
+shinyswatch.theme.superhero()
+```
+
+Example Shiny application:
+
+<table>
+    <thead><tr>
+        <th>File: <code>app.py</code></th>
+        <th>Screenshot</th>
+    </tr></thead>
+    <tbody><tr><td>
 
 ```python
-# File: app.py
 from shiny import App, Inputs, Outputs, Session, render, ui
 
 import shinyswatch
 
 app_ui = ui.page_fluid(
     # Theme code - start
     shinyswatch.theme.darkly(),
@@ -71,26 +98,36 @@
     def slider_val():
         return f"{input.num()}"
 
 
 app = App(app_ui, server)
 ```
 
-## Examples
+</td><td>
 
-There are two examples in the shinyswatch repo. You can view them online at: [shinyswatch.theme.darkly](http://rstudio.github.io/py-shinyswatch/reference/theme.darkly.html) and [get_theme](http://rstudio.github.io/py-shinyswatch/reference/get_theme.html).
+![darkly theme](readme_darkly.png)
 
-To run the demos locally, you can clone the repo and run the examples by calling:
-
-```sh
-python3 -m shiny run examples/basic-darkly/app.py
-# or
-python3 -m shiny run examples/big-sketchy/app.py
-```
+</td></tr></tbody></table>
 
 ## Development
 
 If you want to do development on shinyswatch for Python:
 
 ```sh
 pip install -e ".[dev,test]"
 ```
+
+### Examples
+
+There are three examples in the shinyswatch repo.
+
+<!-- You can view them online at: [shinyswatch.theme.darkly](http://rstudio.github.io/py-shinyswatch/reference/theme.darkly.html) and [get_theme](http://rstudio.github.io/py-shinyswatch/reference/get_theme.html). -->
+
+To run the demos locally, you can run the examples by calling:
+
+```sh
+python3 -m shiny run examples/basic-darkly/app.py
+# or
+python3 -m shiny run examples/big-sketchy/app.py
+# or
+python3 -m shiny run examples/components/app.py
+```
```

### Comparing `shinyswatch-0.2.0/README.md` & `shinyswatch-0.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,56 @@
 # shinyswatch
 
 [Bootswatch](https://bootswatch.com/) + Bootstrap 5 themes for [Shiny](https://shiny.rstudio.com/py/).
 
+
+Here are just three of the **25 themes** in shinyswatch:
+
+| Minty                      | Sketchy                        | Superhero                          |
+|----------------------------|--------------------------------|------------------------------------|
+| ![Minty](readme_minty.png) | ![Sketchy](readme_sketchy.png) | ![Superhero](readme_superhero.png) |
+
+
 ## Installation
 
 ```sh
 pip install shinyswatch
 ```
 
 To install the latest development version from this repository:
 
 ```sh
-pip install https://github.com/schloerke/py-shinyswatch/tarball/main
+pip install https://github.com/rstudio/py-shinyswatch/tarball/main
 ```
 
 ## Usage
 
-Add your theme within your App's top level UI defintion. For example:
+To use a theme, call the theme function and add it to your App's UI definition.
+
+```python
+# Minty theme
+shinyswatch.theme.minty()
+
+# Sketchy theme
+shinyswatch.theme.sketchy()
+
+# Superhero theme
+shinyswatch.theme.superhero()
+```
+
+Example Shiny application:
+
+<table>
+    <thead><tr>
+        <th>File: <code>app.py</code></th>
+        <th>Screenshot</th>
+    </tr></thead>
+    <tbody><tr><td>
 
 ```python
-# File: app.py
 from shiny import App, Inputs, Outputs, Session, render, ui
 
 import shinyswatch
 
 app_ui = ui.page_fluid(
     # Theme code - start
     shinyswatch.theme.darkly(),
@@ -39,26 +66,36 @@
     def slider_val():
         return f"{input.num()}"
 
 
 app = App(app_ui, server)
 ```
 
-## Examples
+</td><td>
 
-There are two examples in the shinyswatch repo. You can view them online at: [shinyswatch.theme.darkly](http://rstudio.github.io/py-shinyswatch/reference/theme.darkly.html) and [get_theme](http://rstudio.github.io/py-shinyswatch/reference/get_theme.html).
+![darkly theme](readme_darkly.png)
 
-To run the demos locally, you can clone the repo and run the examples by calling:
-
-```sh
-python3 -m shiny run examples/basic-darkly/app.py
-# or
-python3 -m shiny run examples/big-sketchy/app.py
-```
+</td></tr></tbody></table>
 
 ## Development
 
 If you want to do development on shinyswatch for Python:
 
 ```sh
 pip install -e ".[dev,test]"
 ```
+
+### Examples
+
+There are three examples in the shinyswatch repo.
+
+<!-- You can view them online at: [shinyswatch.theme.darkly](http://rstudio.github.io/py-shinyswatch/reference/theme.darkly.html) and [get_theme](http://rstudio.github.io/py-shinyswatch/reference/get_theme.html). -->
+
+To run the demos locally, you can run the examples by calling:
+
+```sh
+python3 -m shiny run examples/basic-darkly/app.py
+# or
+python3 -m shiny run examples/big-sketchy/app.py
+# or
+python3 -m shiny run examples/components/app.py
+```
```

### Comparing `shinyswatch-0.2.0/setup.cfg` & `shinyswatch-0.2.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = shinyswatch
 version = attr: shinyswatch.__version__
 author = Barret Schloerke
 author_email = barret@posit.co
-url = https://github.com/schloerke/py-shinyswatch
+url = https://github.com/rstudio/py-shinyswatch
 description = Bootswatch + Bootstrap 5 themes for Shiny.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = html
 license = MIT
 license_file = LICENSE
 platforms = any
@@ -22,16 +22,16 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Text Processing :: Markup :: HTML
 project_urls = 
-	Bug Tracker = https://github.com/schloerke/py-shinyswatch/issues
-	Source Code = https://github.com/schloerke/py-shinyswatch
+	Bug Tracker = https://github.com/rstudio/py-shinyswatch/issues
+	Source Code = https://github.com/rstudio/py-shinyswatch
 
 [options]
 python_requires = >=3.7
 packages = find:
 test_suite = tests
 include_package_data = True
 setup_requires = 
@@ -53,14 +53,15 @@
 	black>=23.1.0
 	flake8==5.0.4;python_version<="3.7"
 	flake8>=6.0.0;python_version>"3.7"
 	isort>=5.11.2
 	pyright>=1.1.301
 	pre-commit>=2.15.0
 	wheel
+	pandas
 docs = 
 	shinylive
 
 [options.packages.find]
 include = shinyswatch
 
 [options.package_data]
```

### Comparing `shinyswatch-0.2.0/shinyswatch/_bsw5.py` & `shinyswatch-0.2.1/shinyswatch/_bsw5.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/_get_theme.py` & `shinyswatch-0.2.1/shinyswatch/_get_theme.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/_shiny_theme.py` & `shinyswatch-0.2.1/shinyswatch/_shiny_theme.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/_typing_extensions.py` & `shinyswatch-0.2.1/shinyswatch/_typing_extensions.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bs5/bootstrap.bundle.min.js` & `shinyswatch-0.2.1/shinyswatch/bs5/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/cerulean/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/cerulean/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/cosmo/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/cosmo/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/cyborg/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/cyborg/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/darkly/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/darkly/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/flatly/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/flatly/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/journal/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/journal/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/litera/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/litera/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/lumen/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/lumen/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/lux/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/lux/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/materia/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/materia/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/minty/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/minty/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/morph/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/morph/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/pulse/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/pulse/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/quartz/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/quartz/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/sandstone/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/sandstone/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/simplex/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/simplex/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/sketchy/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/sketchy/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/slate/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/slate/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/solar/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/solar/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/spacelab/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/spacelab/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/superhero/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/superhero/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/united/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/united/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/vapor/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/vapor/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/yeti/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/yeti/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/bsw5/zephyr/bootswatch.min.css` & `shinyswatch-0.2.1/shinyswatch/bsw5/zephyr/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch/theme.py` & `shinyswatch-0.2.1/shinyswatch/theme.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/shinyswatch.egg-info/PKG-INFO` & `shinyswatch-0.2.1/shinyswatch.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: shinyswatch
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bootswatch + Bootstrap 5 themes for Shiny.
-Home-page: https://github.com/schloerke/py-shinyswatch
+Home-page: https://github.com/rstudio/py-shinyswatch
 Author: Barret Schloerke
 Author-email: barret@posit.co
 License: MIT
-Project-URL: Bug Tracker, https://github.com/schloerke/py-shinyswatch/issues
-Project-URL: Source Code, https://github.com/schloerke/py-shinyswatch
+Project-URL: Bug Tracker, https://github.com/rstudio/py-shinyswatch/issues
+Project-URL: Source Code, https://github.com/rstudio/py-shinyswatch
 Keywords: html
 Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -30,32 +30,59 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 # shinyswatch
 
 [Bootswatch](https://bootswatch.com/) + Bootstrap 5 themes for [Shiny](https://shiny.rstudio.com/py/).
 
+
+Here are just three of the **25 themes** in shinyswatch:
+
+| Minty                      | Sketchy                        | Superhero                          |
+|----------------------------|--------------------------------|------------------------------------|
+| ![Minty](readme_minty.png) | ![Sketchy](readme_sketchy.png) | ![Superhero](readme_superhero.png) |
+
+
 ## Installation
 
 ```sh
 pip install shinyswatch
 ```
 
 To install the latest development version from this repository:
 
 ```sh
-pip install https://github.com/schloerke/py-shinyswatch/tarball/main
+pip install https://github.com/rstudio/py-shinyswatch/tarball/main
 ```
 
 ## Usage
 
-Add your theme within your App's top level UI defintion. For example:
+To use a theme, call the theme function and add it to your App's UI definition.
+
+```python
+# Minty theme
+shinyswatch.theme.minty()
+
+# Sketchy theme
+shinyswatch.theme.sketchy()
+
+# Superhero theme
+shinyswatch.theme.superhero()
+```
+
+Example Shiny application:
+
+<table>
+    <thead><tr>
+        <th>File: <code>app.py</code></th>
+        <th>Screenshot</th>
+    </tr></thead>
+    <tbody><tr><td>
 
 ```python
-# File: app.py
 from shiny import App, Inputs, Outputs, Session, render, ui
 
 import shinyswatch
 
 app_ui = ui.page_fluid(
     # Theme code - start
     shinyswatch.theme.darkly(),
@@ -71,26 +98,36 @@
     def slider_val():
         return f"{input.num()}"
 
 
 app = App(app_ui, server)
 ```
 
-## Examples
+</td><td>
 
-There are two examples in the shinyswatch repo. You can view them online at: [shinyswatch.theme.darkly](http://rstudio.github.io/py-shinyswatch/reference/theme.darkly.html) and [get_theme](http://rstudio.github.io/py-shinyswatch/reference/get_theme.html).
+![darkly theme](readme_darkly.png)
 
-To run the demos locally, you can clone the repo and run the examples by calling:
-
-```sh
-python3 -m shiny run examples/basic-darkly/app.py
-# or
-python3 -m shiny run examples/big-sketchy/app.py
-```
+</td></tr></tbody></table>
 
 ## Development
 
 If you want to do development on shinyswatch for Python:
 
 ```sh
 pip install -e ".[dev,test]"
 ```
+
+### Examples
+
+There are three examples in the shinyswatch repo.
+
+<!-- You can view them online at: [shinyswatch.theme.darkly](http://rstudio.github.io/py-shinyswatch/reference/theme.darkly.html) and [get_theme](http://rstudio.github.io/py-shinyswatch/reference/get_theme.html). -->
+
+To run the demos locally, you can run the examples by calling:
+
+```sh
+python3 -m shiny run examples/basic-darkly/app.py
+# or
+python3 -m shiny run examples/big-sketchy/app.py
+# or
+python3 -m shiny run examples/components/app.py
+```
```

### Comparing `shinyswatch-0.2.0/shinyswatch.egg-info/SOURCES.txt` & `shinyswatch-0.2.1/shinyswatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/tests/.DS_Store` & `shinyswatch-0.2.1/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.2.0/tests/test_themes.py` & `shinyswatch-0.2.1/tests/test_themes.py`

 * *Files identical despite different names*

